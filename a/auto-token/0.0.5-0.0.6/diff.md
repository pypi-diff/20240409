# Comparing `tmp/auto_token-0.0.5-py3-none-any.whl.zip` & `tmp/auto_token-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5760 bytes, number of entries: 11
--rw-r--r--  2.0 unx      535 b- defN 16-Jan-01 00:00 auto_token-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 auto_token-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 16-Jan-01 00:00 auto_token-0.0.5.dist-info/entry_points.txt
+Zip file size: 5710 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      535 b- defN 16-Jan-01 00:00 auto_token-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 auto_token-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 16-Jan-01 00:00 auto_token-0.0.6.dist-info/entry_points.txt
 -rw-r--r--  2.0 unx      117 b- defN 16-Jan-01 00:00 auto_token/__init__.py
--rw-r--r--  2.0 unx     5311 b- defN 16-Jan-01 00:00 auto_token/__main__.py
+-rw-r--r--  2.0 unx     5428 b- defN 16-Jan-01 00:00 auto_token/__main__.py
 -rw-r--r--  2.0 unx       21 b- defN 16-Jan-01 00:00 auto_token/__version__.py
 -rw-r--r--  2.0 unx       66 b- defN 16-Jan-01 00:00 auto_token/model/__init__.py
 -rw-r--r--  2.0 unx      328 b- defN 16-Jan-01 00:00 auto_token/model/config.py
 -rw-r--r--  2.0 unx      800 b- defN 16-Jan-01 00:00 auto_token/model/token.py
--rw-r--r--  2.0 unx     3902 b- defN 16-Jan-01 00:00 auto_token/utils.py
-?rw-------  2.0 unx      871 b- defN 16-Jan-01 00:00 auto_token-0.0.5.dist-info/RECORD
-11 files, 12097 bytes uncompressed, 4282 bytes compressed:  64.6%
+-rw-r--r--  2.0 unx     3690 b- defN 16-Jan-01 00:00 auto_token/utils.py
+?rw-------  2.0 unx      871 b- defN 16-Jan-01 00:00 auto_token-0.0.6.dist-info/RECORD
+11 files, 12002 bytes uncompressed, 4232 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: auto_token-0.0.5.dist-info/METADATA
+Filename: auto_token-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: auto_token-0.0.5.dist-info/WHEEL
+Filename: auto_token-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: auto_token-0.0.5.dist-info/entry_points.txt
+Filename: auto_token-0.0.6.dist-info/entry_points.txt
 Comment: 
 
 Filename: auto_token/__init__.py
 Comment: 
 
 Filename: auto_token/__main__.py
 Comment: 
@@ -24,11 +24,11 @@
 
 Filename: auto_token/model/token.py
 Comment: 
 
 Filename: auto_token/utils.py
 Comment: 
 
-Filename: auto_token-0.0.5.dist-info/RECORD
+Filename: auto_token-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## auto_token/__main__.py

```diff
@@ -45,24 +45,24 @@
             logger.error("You can't operate on base token.")
             raise typer.Exit(1)
 
         config = get_config(config_path, config_logger=config_logger)
         token = get_token(name, config)
 
         if token is None:
-            logger.error(f"Token {name} not exists, please add it first.")
+            logger.error("Token {:} not exists, please add it first.".format(name))
             raise typer.Exit(1)
 
         func(token)
 
-        token_path = Path(config.token_dir).expanduser() / f"{token.name}.toml"
+        token_path = Path(config.token_dir).expanduser() / "{:}.toml".format(token.name)
 
         if not token_path.exists():
             logger.warning(
-                f"Token {name} exists, but token file not found, which may be created manually. Please check."
+                "Token {:} exists, but token file not found, which may be created manually. Please check.".format(name)
             )
 
         with open(token_path, mode="w") as f:
             toml.dump(token.model_dump(mode="json"), f)
 
     wrapper.__name__ = func.__name__
     return wrapper
@@ -73,21 +73,21 @@
     name = "base"
     config_logger = log_level is None
     if not config_logger:
         init_logger(log_level)
     config = get_config(config_path, config_logger=config_logger)
 
     if name in config.tokens:
-        logger.warning("Base already exists, will overwrite it. (Ctrl+C to exit)")
+        logger.warning("{:} already exists, will overwrite it. (Ctrl+C to exit)".format(name))
 
     token_dir = Path(config.token_dir).expanduser()
     token = Token(
         name=name, envs={Env(name="AUTO_TOKEN_ENV_DIR", type=EnvType.env, value=config.env_dir.expanduser().as_posix())}
     )
-    with open(token_dir / f"{name}.toml", mode="w") as f:
+    with open(token_dir / "{:}.toml".format(name), mode="w") as f:
         toml.dump(token.model_dump(mode="json"), f)
 
 
 @app.command("list")
 def list_token(config_path: Path = Path("~/.config/auto-token/config.toml"), log_level: str = typer.Option(None)):
     config_logger = log_level is None
     if not config_logger:
@@ -110,40 +110,40 @@
 ):
     config_logger = log_level is None
     if not config_logger:
         init_logger(log_level)
     config = get_config(config_path, config_logger=config_logger)
 
     if name in config.tokens:
-        logger.warning(f"Token {name} already exists, will overwrite it. (Ctrl+C to exit)")
+        logger.warning("Token {:} already exists, will overwrite it. (Ctrl+C to exit)".format(name))
 
     token_dir = Path(config.token_dir).expanduser()
     token = create_token(name)
-    with open(token_dir / f"{name}.toml", mode="w") as f:
+    with open(token_dir / "{:}.toml".format(name), mode="w") as f:
         toml.dump(token.model_dump(mode="json"), f)
 
 
 @app.command()
 @update_token_command()
 def enable(
     token: Token,
 ):
     if token.active:
-        logger.warning(f"Token {token.name} already enabled.")
+        logger.warning("Token {:} already enabled.".format(token.name))
     else:
         token.active = True
 
 
 @app.command()
 @update_token_command()
 def disable(
     token: Token,
 ):
     if not token.active:
-        logger.warning(f"Token {token.name} already disabled.")
+        logger.warning("Token {:} already disabled.".format(token.name))
     else:
         token.active = False
 
 
 @app.command()
 @update_token_command()
 def rename(
@@ -157,25 +157,25 @@
 def shellenv(config_path: Path = Path("~/.config/auto-token/config.toml")):
     logger.remove()
     config = get_config(config_path, config_logger=False)
 
     for token in config.tokens:
         if token.active:
             for env in token.envs:
-                print(f"export {env.name}={env.value}")
+                print("export {:}={:}".format(env.name, env.value))
 
 
 @app.command()
 def dumpenv(config_path: Path = Path("~/.config/auto-token/config.toml")):
     logger.remove()
     config = get_config(config_path, config_logger=False)
     env_dir = config.env_dir.expanduser()
     env_dir.expanduser().mkdir(parents=True, exist_ok=True)
 
     for token in config.tokens:
-        with open(env_dir / f"{token.name}.env", "w") as f:
+        with open(env_dir / "{:}.env".format(token.name), "w") as f:
             for env in token.envs:
-                f.write(f"{env.name}={env.value}\n")
+                f.write("{:}={:}\n".format(env.name, env.value))
 
 
 if __name__ == "__main__":
     app()
```

## auto_token/__version__.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.5'
+__version__ = '0.0.6'
```

## auto_token/utils.py

```diff
@@ -15,19 +15,19 @@
 from .model import Config, Env, EnvType, Token
 
 
 def prompt_env(env_name: str, description: str | None = None, use_env: bool | None = None) -> Env:
     value = os.environ.get(env_name, None)
     if value is not None:
         if use_env is None:
-            use_env = typer.confirm(f"Wheather to use {env_name} in env?", default=True)
+            use_env = typer.confirm("Wheather to use {:} in env?".format(env_name), default=True)
         if use_env:
             return Env(name=env_name, type=EnvType.env, value=value)
     if description is None:
-        description = f"Please input env {env_name} value"
+        description = "Please input env {:} value".format(env_name)
     value = typer.prompt(description)
     return Env(name=env_name, type=EnvType.env, value=value)
 
 
 def init_logger(log_level: str):
     handler = RichHandler(console=Console(style=Style()), highlighter=NullHighlighter(), markup=True)
     logger.remove()
@@ -35,50 +35,44 @@
 
 
 def get_config(config_path: Path | str = "~/.config/auto-token/config.toml", config_logger: bool = True) -> Config:
     config_path = Path(config_path).expanduser()
     if not config_path.exists():
         if config_logger:
             init_logger("INFO")
-        create_config = typer.confirm(
-            f"Config file not found at {config_path}. Do you want to create it?", default=True
-        )
         config = Config()
-        if create_config:
-            config_path.parent.mkdir(parents=True, exist_ok=True)
-            with open(config_path, mode="w") as f:
-                toml.dump(config.model_dump(mode="json"), f)
-            logger.info(f"Use default config and create config file at [bold purple]{config_path}[/].")
-        else:
-            logger.info("No config file found, use default config.")
+        config_path.parent.mkdir(parents=True, exist_ok=True)
+        with open(config_path, mode="w") as f:
+            toml.dump(config.model_dump(mode="json"), f)
+        logger.info("Use default config and create config file at [bold purple]{:}[/].".format(config_path))
     else:
         with open(config_path) as f:
             config = Config.model_validate(toml.load(f))
         if config_logger:
             init_logger(config.log_level)
-        logger.info(f"Loaded config from [bold purple]{config_path}[/].")
+        logger.info("Loaded config from [bold purple]{:}[/].".format(config_path))
 
     tokens_path = Path(config.token_dir).expanduser()
     tokens_path.mkdir(parents=True, exist_ok=True)
     for token_path in tokens_path.iterdir():
         with open(token_path) as f:
             raw_dict = toml.load(f)
             raw_dict["name"] = token_path.stem
             token = Token.model_validate(raw_dict)
             if token in config.tokens:
-                logger.warning(f"Token {token.name} already loaded from {token_path}, which will be ignored.")
+                logger.warning("Token {:} already loaded from {:}, which will be ignored.".format(token.name, token_path))
             config.tokens.add(token)
 
     return config
 
 
 def create_token(name: str) -> Token:
     token = Token(name=name, envs=set())
     while True:
-        env_name = typer.prompt(f"Please input env name for {name} (empty to exit)", default="", show_default=False)
+        env_name = typer.prompt("Please input env name for {:} (empty to exit)".format(name), default="", show_default=False)
         if env_name == "":
             break
         env = prompt_env(env_name)
         token.envs.add(env)
     return token
```

## Comparing `auto_token-0.0.5.dist-info/METADATA` & `auto_token-0.0.6.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-token
-Version: 0.0.5
+Version: 0.0.6
 Summary: auto manage token
 Author-Email: Zhan Rongrui <2742392377@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: rich>=13.7.0
 Requires-Dist: typer[all]>=0.9.0
```

## Comparing `auto_token-0.0.5.dist-info/RECORD` & `auto_token-0.0.6.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-auto_token-0.0.5.dist-info/METADATA,sha256=ZCiaItxoZzoFB8uq8kcCFwvUdG-4c_y8azKf-Jqieq0,535
-auto_token-0.0.5.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
-auto_token-0.0.5.dist-info/entry_points.txt,sha256=WC2M5yCpGnwoLGfqjAYo7Qtx3CxCe6VkLaYgwybprlE,56
+auto_token-0.0.6.dist-info/METADATA,sha256=0ml1TI1j165WiU0yTNlvIcMU5gdCcSlfd1RK5aei9ss,535
+auto_token-0.0.6.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
+auto_token-0.0.6.dist-info/entry_points.txt,sha256=WC2M5yCpGnwoLGfqjAYo7Qtx3CxCe6VkLaYgwybprlE,56
 auto_token/__init__.py,sha256=5DA3WWm7v_Vb_9VINbbqGHCTWAzREKYltmnXivDY9pg,117
-auto_token/__main__.py,sha256=PPDoyEx_iBmAE2xF6v4DEuCJrZ7vmOppZXXVwuxDoAU,5311
-auto_token/__version__.py,sha256=0Uc3zDF9XadX9j08cOIZbGoZsI0JPHTxemWum3gkos4,21
+auto_token/__main__.py,sha256=UASfKJsbVwHV5EiKiJgtPPLr3LvgGvjtB-3PxMNnejs,5428
+auto_token/__version__.py,sha256=UwR0idQSHgdEemLAk-o2bPOXYWCj-lyyQzAPFRLbziA,21
 auto_token/model/__init__.py,sha256=EM-fQYR_vguOORLrgBDSf60p1eCkw0z940QRADmWBfM,66
 auto_token/model/config.py,sha256=-4dcm3G5EBgY0C1XJKju4CZEJSyeiiHDZeqBzvwQXBU,328
 auto_token/model/token.py,sha256=r_-FAPHAh7txyfTrsUwbXucYMvPyL7D4QBcPTFI4Fuc,800
-auto_token/utils.py,sha256=Ohis7QKHGlAPkbYzw00OAxm6XfU7pUSrIYowUx8NUHA,3902
-auto_token-0.0.5.dist-info/RECORD,,
+auto_token/utils.py,sha256=yQcmu_JiGQ08_vdloI5BKRr9OKXXlHB42arPeZRLHtU,3690
+auto_token-0.0.6.dist-info/RECORD,,
```

