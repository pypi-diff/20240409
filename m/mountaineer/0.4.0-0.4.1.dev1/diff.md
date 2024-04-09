# Comparing `tmp/mountaineer-0.4.0.tar.gz` & `tmp/mountaineer-0.4.1.dev1.tar.gz`

## Comparing `mountaineer-0.4.0.tar` & `mountaineer-0.4.1.dev1.tar`

### file list

```diff
@@ -1,259 +1,259 @@
--rw-r--r--   0     1001      127      269 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src_go/Cargo.toml
--rw-r--r--   0     1001      127     1995 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src_go/build.rs
--rw-r--r--   0     1001      127     5657 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src_go/go/js_build.go
--rw-r--r--   0     1001      127      168 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src_go/go.mod
--rw-r--r--   0     1001      127      376 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src_go/go.sum
--rw-r--r--   0     1001      127     5750 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src_go/src/lib.rs
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 mountaineer-0.4.0/Cargo.toml
--rw-r--r--   0     1001      127      133 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.git-blame-ignore-revs
--rw-r--r--   0     1001      127      138 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.gitattributes
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.github/README_SCRIPTS.md
--rw-r--r--   0     1001      127    14036 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.github/poetry.lock
--rw-r--r--   0     1001      127      767 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.github/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.github/scripts/__init__.py
--rw-r--r--   0     1001      127     3032 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.github/scripts/__tests__/test_update_version.py
--rw-r--r--   0     1001      127     2181 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.github/scripts/check_dependencies.py
--rw-r--r--   0     1001      127     3382 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.github/scripts/update_version.py
--rw-r--r--   0     1001      127     1321 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.github/workflows/publish_docs.yml
--rw-r--r--   0     1001      127    19767 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.github/workflows/test.yml
--rw-r--r--   0     1001      127      504 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.github/workflows/validate.yml
--rw-r--r--   0     1001      127     3404 2024-04-07 01:32:53.000000 mountaineer-0.4.0/.gitignore
--rw-r--r--   0     1001      127     1750 2024-04-07 01:32:53.000000 mountaineer-0.4.0/Dockerfile
--rw-r--r--   0     1001      127     1079 2024-04-07 01:32:53.000000 mountaineer-0.4.0/LICENSE
--rw-r--r--   0     1001      127     4976 2024-04-07 01:32:53.000000 mountaineer-0.4.0/Makefile
--rw-r--r--   0     1001      127    14891 2024-04-07 01:32:53.000000 mountaineer-0.4.0/README.md
--rw-r--r--   0     1001      127      105 2024-04-07 01:32:53.000000 mountaineer-0.4.0/benchmarking/README.md
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/benchmarking/benchmarking/__init__.py
--rw-r--r--   0     1001      127      425 2024-04-07 01:32:53.000000 mountaineer-0.4.0/benchmarking/benchmarking/simple_render.py
--rw-r--r--   0     1001      127   127093 2024-04-07 01:32:53.000000 mountaineer-0.4.0/benchmarking/poetry.lock
--rw-r--r--   0     1001      127      291 2024-04-07 01:32:53.000000 mountaineer-0.4.0/benchmarking/pyproject.toml
--rw-r--r--   0     1001      127      850 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/README.md
--rw-r--r--   0     1001      127        1 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/__init__.py
--rw-r--r--   0     1001      127      775 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/app.py
--rw-r--r--   0     1001      127      489 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/cli.py
--rw-r--r--   0     1001      127      111 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/config.py
--rw-r--r--   0     1001      127        1 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/controllers/__init__.py
--rw-r--r--   0     1001      127     1433 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/controllers/complex.py
--rw-r--r--   0     1001      127      581 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/controllers/detail.py
--rw-r--r--   0     1001      127     1658 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/controllers/home.py
--rw-r--r--   0     1001      127      559 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/controllers/stream.py
--rw-r--r--   0     1001      127       77 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/main.py
--rw-r--r--   0     1001      127      208 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/views/__init__.py
--rw-r--r--   0     1001      127     2261 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/views/app/complex/page.tsx
--rw-r--r--   0     1001      127      453 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/views/app/detail/page.tsx
--rw-r--r--   0     1001      127     2822 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/views/app/home/page.tsx
--rw-r--r--   0     1001      127       59 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/views/app/main.css
--rw-r--r--   0     1001      127      708 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/views/app/stream/page.tsx
--rw-r--r--   0     1001      127   125408 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/views/package-lock.json
--rw-r--r--   0     1001      127      453 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/views/postcss.config.js
--rw-r--r--   0     1001      127      161 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/ci_webapp/views/tailwind.config.js
--rw-r--r--   0     1001      127   107805 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/poetry.lock
--rw-r--r--   0     1001      127      724 2024-04-07 01:32:53.000000 mountaineer-0.4.0/ci_webapp/pyproject.toml
--rw-r--r--   0     1001      127     1593 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/README.md
--rw-r--r--   0     1001      127        1 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
--rw-r--r--   0     1001      127     1055 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
--rw-r--r--   0     1001      127     7904 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
--rw-r--r--   0     1001      127      292 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
--rw-r--r--   0     1001      127      816 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
--rw-r--r--   0     1001      127     4277 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/builder.py
--rw-r--r--   0     1001      127     4656 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/cli.py
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
--rw-r--r--   0     1001      127     1383 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/environments/base.py
--rw-r--r--   0     1001      127     4591 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
--rw-r--r--   0     1001      127     1832 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/environments/venv.py
--rw-r--r--   0     1001      127     1336 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/external.py
--rw-r--r--   0     1001      127     1925 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/generation.py
--rw-r--r--   0     1001      127      327 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/io.py
--rw-r--r--   0     1001      127       30 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
--rw-r--r--   0     1001      127      212 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
--rw-r--r--   0     1001      127      190 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
--rw-r--r--   0     1001      127      137 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
--rw-r--r--   0     1001      127      109 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
--rw-r--r--   0     1001      127      170 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/.env
--rw-r--r--   0     1001      127     3373 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
--rw-r--r--   0     1001      127      645 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
--rw-r--r--   0     1001      127       17 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
--rw-r--r--   0     1001      127      767 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
--rw-r--r--   0     1001      127      947 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
--rw-r--r--   0     1001      127      282 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
--rw-r--r--   0     1001      127      227 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
--rw-r--r--   0     1001      127     1702 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
--rw-r--r--   0     1001      127     1124 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
--rw-r--r--   0     1001      127       84 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
--rw-r--r--   0     1001      127      157 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
--rw-r--r--   0     1001      127     1219 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
--rw-r--r--   0     1001      127      995 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
--rw-r--r--   0     1001      127       95 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
--rw-r--r--   0     1001      127      524 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
--rw-r--r--   0     1001      127      117 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
--rw-r--r--   0     1001      127      195 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
--rw-r--r--   0     1001      127      332 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
--rw-r--r--   0     1001      127     1493 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
--rw-r--r--   0     1001      127    61104 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/poetry.lock
--rw-r--r--   0     1001      127     1214 2024-04-07 01:32:53.000000 mountaineer-0.4.0/create_mountaineer_app/pyproject.toml
--rw-r--r--   0     1001      127       30 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/.zed/settings.json
--rw-r--r--   0     1001      127      107 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/README.md
--rw-r--r--   0     1001      127       15 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/CNAME
--rw-r--r--   0     1001      127      310 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/actions.md
--rw-r--r--   0     1001      127      454 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/api_exception.md
--rw-r--r--   0     1001      127       99 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/app-controller.md
--rw-r--r--   0     1001      127      281 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/build_plugins/base.md
--rw-r--r--   0     1001      127       57 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/build_plugins/javascript.md
--rw-r--r--   0     1001      127       62 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/build_plugins/postcss.md
--rw-r--r--   0     1001      127      411 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/cli.md
--rw-r--r--   0     1001      127      376 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/config.md
--rw-r--r--   0     1001      127       61 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/controller.md
--rw-r--r--   0     1001      127       67 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/core_dependencies.md
--rw-r--r--   0     1001      127       66 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/database/config.md
--rw-r--r--   0     1001      127       71 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/database/dependencies.md
--rw-r--r--   0     1001      127       80 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/logging.md
--rw-r--r--   0     1001      127      479 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/render.md
--rw-r--r--   0     1001      127      365 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/ssr.md
--rw-r--r--   0     1001      127      299 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/api/watch_server.md
--rw-r--r--   0     1001      127     9375 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/client_actions.md
--rw-r--r--   0     1001      127      753 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/cma.md
--rw-r--r--   0     1001      127     3021 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/database.md
--rw-r--r--   0     1001      127     4677 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/deploy.md
--rw-r--r--   0     1001      127     7698 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/error_handling.md
--rw-r--r--   0     1001      127     1081 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/index.md
--rw-r--r--   0     1001      127     1541 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/internal/core_library.md
--rw-r--r--   0     1001      127     2156 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/links.md
--rw-r--r--   0     1001      127   365251 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/media/final_todo_list.png
--rw-r--r--   0     1001      127   148261 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/media/ide_typehints.png
--rw-r--r--   0     1001      127   545494 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/media/network_debug.png
--rw-r--r--   0     1001      127   346903 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/media/server_side_rendering.png
--rw-r--r--   0     1001      127     2263 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/metadata.md
--rw-r--r--   0     1001      127     2347 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/postcss.md
--rw-r--r--   0     1001      127    12265 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/quickstart.md
--rw-r--r--   0     1001      127     4875 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/static_analysis.md
--rw-r--r--   0     1001      127     2490 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/structure.md
--rw-r--r--   0     1001      127     1219 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/stylesheets/extra.css
--rw-r--r--   0     1001      127     4080 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/docs/views.md
--rw-r--r--   0     1001      127     1823 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/mkdocs.yml
--rw-r--r--   0     1001      127      109 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/overrides/partials/footer.html
--rw-r--r--   0     1001      127   156250 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/poetry.lock
--rw-r--r--   0     1001      127      479 2024-04-07 01:32:53.000000 mountaineer-0.4.0/docs_website/pyproject.toml
--rw-r--r--   0     1001      127   675789 2024-04-07 01:32:53.000000 mountaineer-0.4.0/media/header.png
--rw-r--r--   0     1001      127      954 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/actions/__init__.py
--rw-r--r--   0     1001      127     7884 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/actions/test_fields.py
--rw-r--r--   0     1001      127     9707 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/actions/test_passthrough.py
--rw-r--r--   0     1001      127     9074 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/actions/test_sideeffect.py
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/client_builder/__init__.py
--rw-r--r--   0     1001      127    12565 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/client_builder/test_build_actions.py
--rw-r--r--   0     1001      127     3474 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/client_builder/test_build_links.py
--rw-r--r--   0     1001      127     8065 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/client_builder/test_build_schemas.py
--rw-r--r--   0     1001      127     5001 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/client_builder/test_builder.py
--rw-r--r--   0     1001      127     4153 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/client_builder/test_typescript.py
--rw-r--r--   0     1001      127      319 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/common.py
--rw-r--r--   0     1001      127      497 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/conftest.py
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/database/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/database/dependencies/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/database/dependencies/conftest.py
--rw-r--r--   0     1001      127      801 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/database/dependencies/test_core.py
--rw-r--r--   0     1001      127      627 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/database/test_config.py
--rw-r--r--   0     1001      127      616 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/database/test_sqlmodel.py
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/dependencies/__init__.py
--rw-r--r--   0     1001      127     2567 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/dependencies/test_base.py
--rw-r--r--   0     1001      127      211 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/fixtures/__init__.py
--rw-r--r--   0     1001      127   571338 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
--rw-r--r--   0     1001      127  1638568 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
--rw-r--r--   0     1001      127   575422 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/js_compiler/__init__.py
--rw-r--r--   0     1001      127     9973 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/js_compiler/test_javascript.py
--rw-r--r--   0     1001      127      808 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/js_compiler/test_postcss.py
--rw-r--r--   0     1001      127     2823 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/js_compiler/test_source_maps.py
--rw-r--r--   0     1001      127     1236 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_annotation_helpers.py
--rw-r--r--   0     1001      127     8602 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_app.py
--rw-r--r--   0     1001      127      734 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_cache.py
--rw-r--r--   0     1001      127     5281 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_cli.py
--rw-r--r--   0     1001      127      494 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_config.py
--rw-r--r--   0     1001      127     6571 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_controller.py
--rw-r--r--   0     1001      127     3239 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_cropper.py
--rw-r--r--   0     1001      127     1227 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_exceptions.py
--rw-r--r--   0     1001      127     1924 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_logging.py
--rw-r--r--   0     1001      127     8419 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_paths.py
--rw-r--r--   0     1001      127     2565 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_ssr.py
--rw-r--r--   0     1001      127     3177 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/__tests__/test_watch.py
--rw-r--r--   0     1001      127      397 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/actions/__init__.py
--rw-r--r--   0     1001      127    12321 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/actions/fields.py
--rw-r--r--   0     1001      127     6835 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/actions/passthrough.py
--rw-r--r--   0     1001      127    11635 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/actions/sideeffect.py
--rw-r--r--   0     1001      127     4352 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/annotation_helpers.py
--rw-r--r--   0     1001      127    18916 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/app.py
--rw-r--r--   0     1001      127     3216 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/cache.py
--rw-r--r--   0     1001      127    18059 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/cli.py
--rw-r--r--   0     1001      127    10826 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/client_builder/build_actions.py
--rw-r--r--   0     1001      127     3958 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/client_builder/build_links.py
--rw-r--r--   0     1001      127     9737 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/client_builder/build_schemas.py
--rw-r--r--   0     1001      127    28180 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/client_builder/builder.py
--rw-r--r--   0     1001      127     9899 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/client_builder/openapi.py
--rw-r--r--   0     1001      127     3317 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/client_builder/typescript.py
--rw-r--r--   0     1001      127     2424 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/config.py
--rw-r--r--   0     1001      127       40 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/constants.py
--rw-r--r--   0     1001      127    14854 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/controller.py
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/controllers/__init__.py
--rw-r--r--   0     1001      127     1216 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/controllers/exception_controller.py
--rw-r--r--   0     1001      127    10359 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/cropper.py
--rw-r--r--   0     1001      127      327 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/database/__init__.py
--rw-r--r--   0     1001      127     1866 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/database/cli.py
--rw-r--r--   0     1001      127     1822 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/database/config.py
--rw-r--r--   0     1001      127      133 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/database/dependencies/__init__.py
--rw-r--r--   0     1001      127     3188 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/database/dependencies/core.py
--rw-r--r--   0     1001      127     7969 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/database/sqlmodel.py
--rw-r--r--   0     1001      127     8737 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/database/validator.py
--rw-r--r--   0     1001      127      251 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/dependencies/__init__.py
--rw-r--r--   0     1001      127     5122 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/dependencies/base.py
--rw-r--r--   0     1001      127      116 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/dependencies/core/__init__.py
--rw-r--r--   0     1001      127     1069 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/dependencies/core/core.py
--rw-r--r--   0     1001      127     3317 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/exceptions.py
--rw-r--r--   0     1001      127     1188 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/io.py
--rw-r--r--   0     1001      127        1 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/js_compiler/__init__.py
--rw-r--r--   0     1001      127     1731 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/js_compiler/base.py
--rw-r--r--   0     1001      127      199 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/js_compiler/exceptions.py
--rw-r--r--   0     1001      127    15443 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/js_compiler/javascript.py
--rw-r--r--   0     1001      127     4163 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/js_compiler/postcss.py
--rw-r--r--   0     1001      127     5614 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/js_compiler/source_maps.py
--rw-r--r--   0     1001      127     2039 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/logging.py
--rw-r--r--   0     1001      127    12599 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/paths.py
--rw-r--r--   0     1001      127        0 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/py.typed
--rw-r--r--   0     1001      127     5816 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/render.py
--rw-r--r--   0     1001      127     3228 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/ssr.py
--rw-r--r--   0     1001      127      210 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/static/__init__.py
--rw-r--r--   0     1001      127     6299 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/static/api.ts
--rw-r--r--   0     1001      127     3976 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/static/live_reload.ts
--rw-r--r--   0     1001      127      323 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/static/ssr_polyfills.js
--rw-r--r--   0     1001      127     7261 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/test_utilities.py
--rw-r--r--   0     1001      127      213 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/views/__init__.py
--rw-r--r--   0     1001      127      432 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/views/core/exception/page.tsx
--rw-r--r--   0     1001      127      178 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/views/core/layout.tsx
--rw-r--r--   0     1001      127       59 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/views/core/main.css
--rw-r--r--   0     1001      127     1478 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/views/package-lock.json
--rw-r--r--   0     1001      127      257 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/views/postcss.config.js
--rw-r--r--   0     1001      127      162 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/views/tailwind.config.js
--rw-r--r--   0     1001      127     8378 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/watch.py
--rw-r--r--   0     1001      127     3087 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/watch_server.py
--rw-r--r--   0     1001      127      866 2024-04-07 01:32:53.000000 mountaineer-0.4.0/mountaineer/webservice.py
--rw-r--r--   0     1001      127   124933 2024-04-07 01:32:53.000000 mountaineer-0.4.0/poetry.lock
--rw-r--r--   0     1001      127   453080 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/benches/fixtures/complex_sourcemap_mapping.txt
--rw-r--r--   0     1001      127   575422 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/benches/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127      322 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/benches/fixtures/ssr_polyfill_archive.js
--rw-r--r--   0     1001      127      899 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/benches/lexers_benchmark.rs
--rw-r--r--   0     1001      127     1089 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/benches/source_map_benchmark.rs
--rw-r--r--   0     1001      127     1595 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/benches/ssr_benchmark.rs
--rw-r--r--   0     1001      127      499 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/errors.rs
--rw-r--r--   0     1001      127     4648 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/lexers.rs
--rw-r--r--   0     1001      127     8366 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/lib.rs
--rw-r--r--   0     1001      127      680 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/logging.rs
--rw-r--r--   0     1001      127    17549 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/source_map.rs
--rw-r--r--   0     1001      127    15113 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/ssr.rs
--rw-r--r--   0     1001      127     3998 2024-04-07 01:32:53.000000 mountaineer-0.4.0/src/timeout.rs
--rw-r--r--   0     1001      127    32088 2024-04-07 01:33:15.000000 mountaineer-0.4.0/Cargo.lock
--rw-r--r--   0     1001      127     1602 2024-04-07 01:33:10.000000 mountaineer-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    15349 1970-01-01 00:00:00.000000 mountaineer-0.4.0/PKG-INFO
+-rw-r--r--   0     1001      127      269 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src_go/Cargo.toml
+-rw-r--r--   0     1001      127     1995 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src_go/build.rs
+-rw-r--r--   0     1001      127     5657 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src_go/go/js_build.go
+-rw-r--r--   0     1001      127      168 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src_go/go.mod
+-rw-r--r--   0     1001      127      376 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src_go/go.sum
+-rw-r--r--   0     1001      127     5750 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src_go/src/lib.rs
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.4.1.dev1/Cargo.toml
+-rw-r--r--   0     1001      127      133 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.git-blame-ignore-revs
+-rw-r--r--   0     1001      127      138 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.gitattributes
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.github/README_SCRIPTS.md
+-rw-r--r--   0     1001      127    14036 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.github/poetry.lock
+-rw-r--r--   0     1001      127      767 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.github/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.github/scripts/__init__.py
+-rw-r--r--   0     1001      127     3032 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.github/scripts/__tests__/test_update_version.py
+-rw-r--r--   0     1001      127     2181 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.github/scripts/check_dependencies.py
+-rw-r--r--   0     1001      127     3382 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.github/scripts/update_version.py
+-rw-r--r--   0     1001      127     1321 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.github/workflows/publish_docs.yml
+-rw-r--r--   0     1001      127    19767 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      504 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.github/workflows/validate.yml
+-rw-r--r--   0     1001      127     3404 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/.gitignore
+-rw-r--r--   0     1001      127     1750 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/Dockerfile
+-rw-r--r--   0     1001      127     1079 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/LICENSE
+-rw-r--r--   0     1001      127     4976 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/Makefile
+-rw-r--r--   0     1001      127    14891 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/README.md
+-rw-r--r--   0     1001      127      105 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/benchmarking/README.md
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/benchmarking/benchmarking/__init__.py
+-rw-r--r--   0     1001      127      425 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/benchmarking/benchmarking/simple_render.py
+-rw-r--r--   0     1001      127   127093 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/benchmarking/poetry.lock
+-rw-r--r--   0     1001      127      291 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/benchmarking/pyproject.toml
+-rw-r--r--   0     1001      127      850 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/README.md
+-rw-r--r--   0     1001      127        1 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/__init__.py
+-rw-r--r--   0     1001      127      775 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/app.py
+-rw-r--r--   0     1001      127      489 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/cli.py
+-rw-r--r--   0     1001      127      111 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/config.py
+-rw-r--r--   0     1001      127        1 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/controllers/__init__.py
+-rw-r--r--   0     1001      127     1433 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/controllers/complex.py
+-rw-r--r--   0     1001      127      581 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/controllers/detail.py
+-rw-r--r--   0     1001      127     1658 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/controllers/home.py
+-rw-r--r--   0     1001      127      559 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/controllers/stream.py
+-rw-r--r--   0     1001      127       77 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/main.py
+-rw-r--r--   0     1001      127      208 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/__init__.py
+-rw-r--r--   0     1001      127     2261 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/app/complex/page.tsx
+-rw-r--r--   0     1001      127      453 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127     2822 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       59 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/app/main.css
+-rw-r--r--   0     1001      127      708 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/app/stream/page.tsx
+-rw-r--r--   0     1001      127   125408 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/package-lock.json
+-rw-r--r--   0     1001      127      453 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/postcss.config.js
+-rw-r--r--   0     1001      127      161 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/tailwind.config.js
+-rw-r--r--   0     1001      127   107805 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/poetry.lock
+-rw-r--r--   0     1001      127      724 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/ci_webapp/pyproject.toml
+-rw-r--r--   0     1001      127     1593 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/README.md
+-rw-r--r--   0     1001      127        1 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
+-rw-r--r--   0     1001      127     1055 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
+-rw-r--r--   0     1001      127     7904 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
+-rw-r--r--   0     1001      127      292 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      816 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
+-rw-r--r--   0     1001      127     4277 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/builder.py
+-rw-r--r--   0     1001      127     4656 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/cli.py
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
+-rw-r--r--   0     1001      127     1383 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/environments/base.py
+-rw-r--r--   0     1001      127     4591 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
+-rw-r--r--   0     1001      127     1832 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/environments/venv.py
+-rw-r--r--   0     1001      127     1336 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/external.py
+-rw-r--r--   0     1001      127     1925 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/generation.py
+-rw-r--r--   0     1001      127      327 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/io.py
+-rw-r--r--   0     1001      127       30 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
+-rw-r--r--   0     1001      127      212 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
+-rw-r--r--   0     1001      127      190 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
+-rw-r--r--   0     1001      127      137 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
+-rw-r--r--   0     1001      127      109 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
+-rw-r--r--   0     1001      127      170 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.env
+-rw-r--r--   0     1001      127     3373 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
+-rw-r--r--   0     1001      127      645 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
+-rw-r--r--   0     1001      127       17 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
+-rw-r--r--   0     1001      127      767 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
+-rw-r--r--   0     1001      127      947 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
+-rw-r--r--   0     1001      127      282 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
+-rw-r--r--   0     1001      127      227 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
+-rw-r--r--   0     1001      127     1702 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
+-rw-r--r--   0     1001      127     1124 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
+-rw-r--r--   0     1001      127       84 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
+-rw-r--r--   0     1001      127      157 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
+-rw-r--r--   0     1001      127     1219 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127      995 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       95 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
+-rw-r--r--   0     1001      127      524 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
+-rw-r--r--   0     1001      127      117 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
+-rw-r--r--   0     1001      127      195 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
+-rw-r--r--   0     1001      127      332 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
+-rw-r--r--   0     1001      127     1493 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
+-rw-r--r--   0     1001      127    61104 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/poetry.lock
+-rw-r--r--   0     1001      127     1214 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/create_mountaineer_app/pyproject.toml
+-rw-r--r--   0     1001      127       30 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/.zed/settings.json
+-rw-r--r--   0     1001      127      107 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/README.md
+-rw-r--r--   0     1001      127       15 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/CNAME
+-rw-r--r--   0     1001      127      310 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/actions.md
+-rw-r--r--   0     1001      127      454 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/api_exception.md
+-rw-r--r--   0     1001      127       99 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/app-controller.md
+-rw-r--r--   0     1001      127      281 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/build_plugins/base.md
+-rw-r--r--   0     1001      127       57 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/build_plugins/javascript.md
+-rw-r--r--   0     1001      127       62 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/build_plugins/postcss.md
+-rw-r--r--   0     1001      127      411 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/cli.md
+-rw-r--r--   0     1001      127      376 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/config.md
+-rw-r--r--   0     1001      127       61 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/controller.md
+-rw-r--r--   0     1001      127       67 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/core_dependencies.md
+-rw-r--r--   0     1001      127       66 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/database/config.md
+-rw-r--r--   0     1001      127       71 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/database/dependencies.md
+-rw-r--r--   0     1001      127       80 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/logging.md
+-rw-r--r--   0     1001      127      479 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/render.md
+-rw-r--r--   0     1001      127      365 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/ssr.md
+-rw-r--r--   0     1001      127      299 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/api/watch_server.md
+-rw-r--r--   0     1001      127     9375 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/client_actions.md
+-rw-r--r--   0     1001      127      753 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/cma.md
+-rw-r--r--   0     1001      127     3021 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/database.md
+-rw-r--r--   0     1001      127     4677 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/deploy.md
+-rw-r--r--   0     1001      127     7698 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/error_handling.md
+-rw-r--r--   0     1001      127     1081 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/index.md
+-rw-r--r--   0     1001      127     1541 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/internal/core_library.md
+-rw-r--r--   0     1001      127     2156 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/links.md
+-rw-r--r--   0     1001      127   365251 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/media/final_todo_list.png
+-rw-r--r--   0     1001      127   148261 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/media/ide_typehints.png
+-rw-r--r--   0     1001      127   545494 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/media/network_debug.png
+-rw-r--r--   0     1001      127   346903 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/media/server_side_rendering.png
+-rw-r--r--   0     1001      127     2263 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/metadata.md
+-rw-r--r--   0     1001      127     2347 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/postcss.md
+-rw-r--r--   0     1001      127    12265 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/quickstart.md
+-rw-r--r--   0     1001      127     4875 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/static_analysis.md
+-rw-r--r--   0     1001      127     2490 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/structure.md
+-rw-r--r--   0     1001      127     1219 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127     4080 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/docs/views.md
+-rw-r--r--   0     1001      127     1823 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/mkdocs.yml
+-rw-r--r--   0     1001      127      109 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/overrides/partials/footer.html
+-rw-r--r--   0     1001      127   156250 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/poetry.lock
+-rw-r--r--   0     1001      127      479 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/docs_website/pyproject.toml
+-rw-r--r--   0     1001      127   675789 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/media/header.png
+-rw-r--r--   0     1001      127      954 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/actions/__init__.py
+-rw-r--r--   0     1001      127     7884 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/actions/test_fields.py
+-rw-r--r--   0     1001      127     9707 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/actions/test_passthrough.py
+-rw-r--r--   0     1001      127     9074 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/actions/test_sideeffect.py
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/client_builder/__init__.py
+-rw-r--r--   0     1001      127    12565 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/client_builder/test_build_actions.py
+-rw-r--r--   0     1001      127     3474 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/client_builder/test_build_links.py
+-rw-r--r--   0     1001      127     9485 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/client_builder/test_build_schemas.py
+-rw-r--r--   0     1001      127     5001 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/client_builder/test_builder.py
+-rw-r--r--   0     1001      127     4153 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/client_builder/test_typescript.py
+-rw-r--r--   0     1001      127      319 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/common.py
+-rw-r--r--   0     1001      127      497 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/conftest.py
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/database/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/database/dependencies/conftest.py
+-rw-r--r--   0     1001      127      801 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/database/dependencies/test_core.py
+-rw-r--r--   0     1001      127      627 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/database/test_config.py
+-rw-r--r--   0     1001      127      616 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/database/test_sqlmodel.py
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/dependencies/__init__.py
+-rw-r--r--   0     1001      127     2567 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/dependencies/test_base.py
+-rw-r--r--   0     1001      127      211 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/fixtures/__init__.py
+-rw-r--r--   0     1001      127   571338 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127  1638568 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
+-rw-r--r--   0     1001      127   575422 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     9973 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/js_compiler/test_javascript.py
+-rw-r--r--   0     1001      127      808 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/js_compiler/test_postcss.py
+-rw-r--r--   0     1001      127     2823 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/js_compiler/test_source_maps.py
+-rw-r--r--   0     1001      127     1236 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_annotation_helpers.py
+-rw-r--r--   0     1001      127     8602 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_app.py
+-rw-r--r--   0     1001      127      734 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_cache.py
+-rw-r--r--   0     1001      127     5281 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      494 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_config.py
+-rw-r--r--   0     1001      127     6571 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_controller.py
+-rw-r--r--   0     1001      127     3239 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_cropper.py
+-rw-r--r--   0     1001      127     1227 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_exceptions.py
+-rw-r--r--   0     1001      127     1924 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_logging.py
+-rw-r--r--   0     1001      127     8419 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_paths.py
+-rw-r--r--   0     1001      127     2565 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_ssr.py
+-rw-r--r--   0     1001      127     3177 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/__tests__/test_watch.py
+-rw-r--r--   0     1001      127      397 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/actions/__init__.py
+-rw-r--r--   0     1001      127    12321 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/actions/fields.py
+-rw-r--r--   0     1001      127     6835 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/actions/passthrough.py
+-rw-r--r--   0     1001      127    11635 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/actions/sideeffect.py
+-rw-r--r--   0     1001      127     4352 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/annotation_helpers.py
+-rw-r--r--   0     1001      127    18916 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/app.py
+-rw-r--r--   0     1001      127     3216 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/cache.py
+-rw-r--r--   0     1001      127    18059 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/cli.py
+-rw-r--r--   0     1001      127    10826 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/client_builder/build_actions.py
+-rw-r--r--   0     1001      127     3958 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/client_builder/build_links.py
+-rw-r--r--   0     1001      127    10693 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/client_builder/build_schemas.py
+-rw-r--r--   0     1001      127    28180 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/client_builder/builder.py
+-rw-r--r--   0     1001      127    11312 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/client_builder/openapi.py
+-rw-r--r--   0     1001      127     3253 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/client_builder/typescript.py
+-rw-r--r--   0     1001      127     2424 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/config.py
+-rw-r--r--   0     1001      127       40 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/constants.py
+-rw-r--r--   0     1001      127    14854 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/controller.py
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/controllers/__init__.py
+-rw-r--r--   0     1001      127     1216 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/controllers/exception_controller.py
+-rw-r--r--   0     1001      127    10359 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/cropper.py
+-rw-r--r--   0     1001      127      327 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/database/__init__.py
+-rw-r--r--   0     1001      127     1866 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/database/cli.py
+-rw-r--r--   0     1001      127     1822 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/database/config.py
+-rw-r--r--   0     1001      127      133 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127     3188 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/database/dependencies/core.py
+-rw-r--r--   0     1001      127     7969 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/database/sqlmodel.py
+-rw-r--r--   0     1001      127     8737 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/database/validator.py
+-rw-r--r--   0     1001      127      251 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/dependencies/__init__.py
+-rw-r--r--   0     1001      127     5122 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/dependencies/base.py
+-rw-r--r--   0     1001      127      116 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/dependencies/core/__init__.py
+-rw-r--r--   0     1001      127     1069 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/dependencies/core/core.py
+-rw-r--r--   0     1001      127     3317 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/exceptions.py
+-rw-r--r--   0     1001      127     1188 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/io.py
+-rw-r--r--   0     1001      127        1 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     1731 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/js_compiler/base.py
+-rw-r--r--   0     1001      127      199 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/js_compiler/exceptions.py
+-rw-r--r--   0     1001      127    15443 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/js_compiler/javascript.py
+-rw-r--r--   0     1001      127     4163 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/js_compiler/postcss.py
+-rw-r--r--   0     1001      127     5614 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/js_compiler/source_maps.py
+-rw-r--r--   0     1001      127     2039 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/logging.py
+-rw-r--r--   0     1001      127    12599 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/paths.py
+-rw-r--r--   0     1001      127        0 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/py.typed
+-rw-r--r--   0     1001      127     5816 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/render.py
+-rw-r--r--   0     1001      127     3228 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/ssr.py
+-rw-r--r--   0     1001      127      210 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/static/__init__.py
+-rw-r--r--   0     1001      127     6299 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/static/api.ts
+-rw-r--r--   0     1001      127     3976 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/static/live_reload.ts
+-rw-r--r--   0     1001      127      323 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/static/ssr_polyfills.js
+-rw-r--r--   0     1001      127     7261 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/test_utilities.py
+-rw-r--r--   0     1001      127      213 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/views/__init__.py
+-rw-r--r--   0     1001      127      432 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/views/core/exception/page.tsx
+-rw-r--r--   0     1001      127      178 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/views/core/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/views/core/main.css
+-rw-r--r--   0     1001      127     1478 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/views/package-lock.json
+-rw-r--r--   0     1001      127      257 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/views/postcss.config.js
+-rw-r--r--   0     1001      127      162 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/views/tailwind.config.js
+-rw-r--r--   0     1001      127     8378 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/watch.py
+-rw-r--r--   0     1001      127     3087 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/watch_server.py
+-rw-r--r--   0     1001      127      866 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/mountaineer/webservice.py
+-rw-r--r--   0     1001      127   124933 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/poetry.lock
+-rw-r--r--   0     1001      127   453080 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/benches/fixtures/complex_sourcemap_mapping.txt
+-rw-r--r--   0     1001      127   575422 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/benches/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127      322 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/benches/fixtures/ssr_polyfill_archive.js
+-rw-r--r--   0     1001      127      899 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/benches/lexers_benchmark.rs
+-rw-r--r--   0     1001      127     1089 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/benches/source_map_benchmark.rs
+-rw-r--r--   0     1001      127     1595 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/benches/ssr_benchmark.rs
+-rw-r--r--   0     1001      127      499 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/errors.rs
+-rw-r--r--   0     1001      127     4648 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/lexers.rs
+-rw-r--r--   0     1001      127     8366 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/lib.rs
+-rw-r--r--   0     1001      127      680 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/logging.rs
+-rw-r--r--   0     1001      127    17549 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/source_map.rs
+-rw-r--r--   0     1001      127    15113 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/ssr.rs
+-rw-r--r--   0     1001      127     3998 2024-04-09 14:17:20.000000 mountaineer-0.4.1.dev1/src/timeout.rs
+-rw-r--r--   0     1001      127    32093 2024-04-09 14:17:38.000000 mountaineer-0.4.1.dev1/Cargo.lock
+-rw-r--r--   0     1001      127     1607 2024-04-09 14:17:34.000000 mountaineer-0.4.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0    15354 1970-01-01 00:00:00.000000 mountaineer-0.4.1.dev1/PKG-INFO
```

### Comparing `mountaineer-0.4.0/src_go/build.rs` & `mountaineer-0.4.1.dev1/src_go/build.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src_go/go/js_build.go` & `mountaineer-0.4.1.dev1/src_go/go/js_build.go`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src_go/src/lib.rs` & `mountaineer-0.4.1.dev1/src_go/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/Cargo.toml` & `mountaineer-0.4.1.dev1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [[bench]]
 path = "src/benches/lexers_benchmark.rs"
 name = "lexers_benchmark"
 harness = false
 
 [package]
 name = "mountaineer"
-version = "0.4.0"
+version = "0.4.1-dev1"
 edition = "2021"
 
 [dependencies]
 v8 = "0.89.0"
 deno_core_icudata = "0.73.0"
 lazy_static = "1.4.0"
 serde_json = "1.0"
```

### Comparing `mountaineer-0.4.0/.github/poetry.lock` & `mountaineer-0.4.1.dev1/.github/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/.github/pyproject.toml` & `mountaineer-0.4.1.dev1/.github/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/.github/scripts/__tests__/test_update_version.py` & `mountaineer-0.4.1.dev1/.github/scripts/__tests__/test_update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/.github/scripts/check_dependencies.py` & `mountaineer-0.4.1.dev1/.github/scripts/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/.github/scripts/update_version.py` & `mountaineer-0.4.1.dev1/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/.github/workflows/publish_docs.yml` & `mountaineer-0.4.1.dev1/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/.github/workflows/test.yml` & `mountaineer-0.4.1.dev1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/.gitignore` & `mountaineer-0.4.1.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/Dockerfile` & `mountaineer-0.4.1.dev1/Dockerfile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/LICENSE` & `mountaineer-0.4.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/Makefile` & `mountaineer-0.4.1.dev1/Makefile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/README.md` & `mountaineer-0.4.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/benchmarking/poetry.lock` & `mountaineer-0.4.1.dev1/benchmarking/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/README.md` & `mountaineer-0.4.1.dev1/ci_webapp/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/ci_webapp/app.py` & `mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/ci_webapp/controllers/complex.py` & `mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/controllers/complex.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/ci_webapp/controllers/detail.py` & `mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/ci_webapp/controllers/home.py` & `mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/ci_webapp/controllers/stream.py` & `mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/controllers/stream.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/ci_webapp/views/app/complex/page.tsx` & `mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/app/complex/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/ci_webapp/views/app/home/page.tsx` & `mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/ci_webapp/views/app/stream/page.tsx` & `mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/app/stream/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/ci_webapp/views/package-lock.json` & `mountaineer-0.4.1.dev1/ci_webapp/ci_webapp/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/poetry.lock` & `mountaineer-0.4.1.dev1/ci_webapp/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/ci_webapp/pyproject.toml` & `mountaineer-0.4.1.dev1/ci_webapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/README.md` & `mountaineer-0.4.1.dev1/create_mountaineer_app/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/__tests__/common.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/common.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/builder.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/cli.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/environments/base.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/environments/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/environments/poetry.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/environments/venv.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/environments/venv.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/external.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/external.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/generation.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/README.md` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml` & `mountaineer-0.4.1.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/poetry.lock` & `mountaineer-0.4.1.dev1/create_mountaineer_app/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/create_mountaineer_app/pyproject.toml` & `mountaineer-0.4.1.dev1/create_mountaineer_app/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/client_actions.md` & `mountaineer-0.4.1.dev1/docs_website/docs/client_actions.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/cma.md` & `mountaineer-0.4.1.dev1/docs_website/docs/cma.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/database.md` & `mountaineer-0.4.1.dev1/docs_website/docs/database.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/deploy.md` & `mountaineer-0.4.1.dev1/docs_website/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/error_handling.md` & `mountaineer-0.4.1.dev1/docs_website/docs/error_handling.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/index.md` & `mountaineer-0.4.1.dev1/docs_website/docs/index.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/internal/core_library.md` & `mountaineer-0.4.1.dev1/docs_website/docs/internal/core_library.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/links.md` & `mountaineer-0.4.1.dev1/docs_website/docs/links.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/media/final_todo_list.png` & `mountaineer-0.4.1.dev1/docs_website/docs/media/final_todo_list.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/media/ide_typehints.png` & `mountaineer-0.4.1.dev1/docs_website/docs/media/ide_typehints.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/media/network_debug.png` & `mountaineer-0.4.1.dev1/docs_website/docs/media/network_debug.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/media/server_side_rendering.png` & `mountaineer-0.4.1.dev1/docs_website/docs/media/server_side_rendering.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/metadata.md` & `mountaineer-0.4.1.dev1/docs_website/docs/metadata.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/postcss.md` & `mountaineer-0.4.1.dev1/docs_website/docs/postcss.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/quickstart.md` & `mountaineer-0.4.1.dev1/docs_website/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/static_analysis.md` & `mountaineer-0.4.1.dev1/docs_website/docs/static_analysis.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/structure.md` & `mountaineer-0.4.1.dev1/docs_website/docs/structure.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/stylesheets/extra.css` & `mountaineer-0.4.1.dev1/docs_website/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/docs/views.md` & `mountaineer-0.4.1.dev1/docs_website/docs/views.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/mkdocs.yml` & `mountaineer-0.4.1.dev1/docs_website/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/docs_website/poetry.lock` & `mountaineer-0.4.1.dev1/docs_website/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/media/header.png` & `mountaineer-0.4.1.dev1/media/header.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__init__.py` & `mountaineer-0.4.1.dev1/mountaineer/__init__.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/actions/test_fields.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/actions/test_fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/actions/test_passthrough.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/actions/test_passthrough.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/actions/test_sideeffect.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/actions/test_sideeffect.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/client_builder/test_build_actions.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/client_builder/test_build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/client_builder/test_build_links.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/client_builder/test_build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/client_builder/test_build_schemas.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/client_builder/test_build_schemas.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from enum import Enum, IntEnum, StrEnum
 from json import dumps as json_dumps
-from typing import Generic, TypeVar
+from typing import Any, Generic, Literal, TypeVar
 
 import pytest
 from pydantic import BaseModel, Field, create_model
 
 from mountaineer.client_builder.build_schemas import (
     OpenAPISchema,
     OpenAPIToTypescriptSchemaConverter,
 )
 from mountaineer.client_builder.openapi import OpenAPIProperty, OpenAPISchemaType
+from mountaineer.logging import LOGGER
 
 T = TypeVar("T")
 
 
 class SubModel1(BaseModel):
     sub_a: str
 
@@ -107,28 +108,53 @@
         (dict[str, SubModel1], ["value: Record<string, SubModel1>"]),
         (dict[str, int], ["value: Record<string, number>"]),
         (dict[str, dict[str, str]], ["value: Record<string, Record<string, string>>"]),
         ("SubModel1", ["value: SubModel1"]),
         (MyStrEnum, ["value: MyStrEnum"]),
         (MyIntEnum, ["value: MyIntEnum"]),
         (MyEnum, ["value: MyEnum"]),
+        (str | None, ["value: null | string"]),
+        (list[str] | None, ["value: Array<string> | null"]),
+        (list[str | int] | None, ["value: Array<number | string> | null"]),
+        (list | None, ["value: Array<any> | null"]),
+        (
+            dict[str, str | None | int | float],
+            ["value: Record<string, null | number | string>"],
+        ),
+        (list[str | None] | None, ["value: Array<null | string> | null"]),
+        (tuple[str, str], ["value: [string, string]"]),
+        (tuple[str, int | None], ["value: [string, null | number]"]),
+        (list[tuple[str, int] | str], ["value: Array<[string, number] | string>"]),
+        (Literal["my_value"], ["value: 'my_value'"]),
+        (Literal["my_value"] | Literal[True], ["value: 'my_value' | true"]),  # type: ignore
+        (bool, ["value: boolean"]),
+        (float, ["value: number"]),
+        (Any, ["value: any"]),
+        # We don't consider types that would encompass other types, so right now
+        # we just parse separately
+        (Any | None, ["value: any | null"]),  # type: ignore
+        # OpenAPI doesn't support bytes, so it casts them as strings
+        (bytes, ["value: string"]),
+        # OpenAPI doesn't support sets, so it casts them as arrays
+        (set[str], ["value: Array<string>"]),
     ],
 )
 def test_python_to_typescript_types(
     python_type: type, expected_typescript_types: list[str]
 ):
     """
     Test type resolution when attached to a given model's field
     """
     # Create a model schema automatically with the passed in typing
     fake_model = create_model(
         "FakeModel",
         value=(python_type, Field()),
     )
 
+    LOGGER.debug(f"Raw schema: {fake_model.model_json_schema()}")
     schema = OpenAPISchema(**fake_model.model_json_schema())
 
     converter = OpenAPIToTypescriptSchemaConverter()
     interface_definition = converter.convert_schema_to_interface(
         schema,
         base=schema,
         defaults_are_required=False,
```

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/client_builder/test_builder.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/client_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/client_builder/test_typescript.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/client_builder/test_typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/database/dependencies/test_core.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/database/dependencies/test_core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/database/test_config.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/database/test_config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/database/test_sqlmodel.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/database/test_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/dependencies/test_base.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/dependencies/test_base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/fixtures/home_controller_source_map.js.map` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/fixtures/home_controller_source_map.js.map`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/js_compiler/test_javascript.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/js_compiler/test_javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/js_compiler/test_postcss.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/js_compiler/test_postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/js_compiler/test_source_maps.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/js_compiler/test_source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/test_annotation_helpers.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/test_annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/test_app.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/test_app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/test_cache.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/test_cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/test_cli.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/test_cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/test_controller.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/test_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/test_cropper.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/test_cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/test_exceptions.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/test_logging.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/test_logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/test_paths.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/test_paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/test_ssr.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/test_ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/__tests__/test_watch.py` & `mountaineer-0.4.1.dev1/mountaineer/__tests__/test_watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/actions/fields.py` & `mountaineer-0.4.1.dev1/mountaineer/actions/fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/actions/passthrough.py` & `mountaineer-0.4.1.dev1/mountaineer/actions/passthrough.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/actions/sideeffect.py` & `mountaineer-0.4.1.dev1/mountaineer/actions/sideeffect.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/annotation_helpers.py` & `mountaineer-0.4.1.dev1/mountaineer/annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/app.py` & `mountaineer-0.4.1.dev1/mountaineer/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/cache.py` & `mountaineer-0.4.1.dev1/mountaineer/cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/cli.py` & `mountaineer-0.4.1.dev1/mountaineer/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/client_builder/build_actions.py` & `mountaineer-0.4.1.dev1/mountaineer/client_builder/build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/client_builder/build_links.py` & `mountaineer-0.4.1.dev1/mountaineer/client_builder/build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/client_builder/build_schemas.py` & `mountaineer-0.4.1.dev1/mountaineer/client_builder/build_schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from typing import Any, Dict, Iterator, Type, get_args, get_origin
 
 from inflection import camelize
 from pydantic import BaseModel, create_model
 
 from mountaineer.annotation_helpers import get_value_by_alias, yield_all_subtypes
 from mountaineer.client_builder.openapi import (
+    EmptyAPIProperty,
     OpenAPIProperty,
     OpenAPISchema,
     OpenAPISchemaType,
 )
 from mountaineer.client_builder.typescript import (
     TSLiteral,
     map_openapi_type_to_ts,
     python_payload_to_typescript,
 )
+from mountaineer.logging import LOGGER
 
 
 class OpenAPIToTypescriptSchemaConverter:
     """
     Transform a pydantic.BaseModel into a TypeScript interface, by using
     OpenAPI as an intermediate layer. This also allows client callers to support
     generating interfaces from other OpenAPI-compliant schemas.
@@ -77,15 +79,20 @@
         """
         Return all unique models that are used in the given OpenAPI schema. This allows clients
         to build up all of the dependencies that the core model needs.
 
         :param base: The core OpenAPI Schema
         """
 
-        def walk_models(property: OpenAPIProperty) -> Iterator[OpenAPIProperty]:
+        def walk_models(
+            property: OpenAPIProperty | EmptyAPIProperty,
+        ) -> Iterator[OpenAPIProperty]:
+            if isinstance(property, EmptyAPIProperty):
+                return
+
             if (
                 property.variable_type == OpenAPISchemaType.OBJECT
                 or property.enum is not None
             ):
                 yield property
             if property.ref is not None:
                 yield from walk_models(self.resolve_ref(property.ref, base))
@@ -148,49 +155,65 @@
         base: BaseModel,
         defaults_are_required: bool,
         all_fields_required: bool,
     ):
         fields = []
 
         # We have to support arrays with one and multiple values
-        def walk_array_types(prop: OpenAPIProperty) -> Iterator[str]:
-            if prop.ref:
+        def walk_array_types(prop: OpenAPIProperty | EmptyAPIProperty) -> Iterator[str]:
+            if isinstance(prop, EmptyAPIProperty):
+                yield "any"
+                return
+
+            if prop.variable_type == OpenAPISchemaType.ARRAY:
+                # Special case for arrays where we shouldn't use the Array syntax
+                if prop.prefixItems:
+                    tuple_values = [
+                        " | ".join(sorted(set(walk_array_types(item))))
+                        for item in prop.prefixItems
+                    ]
+                    yield f"[{', '.join(tuple_values)}]"
+                    return
+
+                array_types: list[str] = (
+                    sorted(set(walk_array_types(prop.items))) if prop.items else ["any"]
+                )
+                yield f"Array<{' | '.join(array_types)}>"
+            elif prop.ref:
                 yield self.get_typescript_interface_name(
                     self.resolve_ref(prop.ref, base=base)
                 )
             elif prop.items:
                 yield from walk_array_types(prop.items)
             elif prop.anyOf:
                 for sub_prop in prop.anyOf:
                     yield from walk_array_types(sub_prop)
             elif prop.additionalProperties:
                 # OpenAPI doesn't specify the type of the keys since JSON forces them to be strings
                 # By the time we get to this function we should have called validate_typescript_candidate
-                sub_types = " | ".join(walk_array_types(prop.additionalProperties))
+                sub_types = " | ".join(
+                    sorted(set(walk_array_types(prop.additionalProperties)))
+                )
                 yield f"Record<{map_openapi_type_to_ts(OpenAPISchemaType.STRING)}, {sub_types}>"
             elif prop.variable_type:
                 yield map_openapi_type_to_ts(prop.variable_type)
+            elif prop.const:
+                yield python_payload_to_typescript(prop.const)
+            else:
+                LOGGER.warning(f"Unknown property type: {prop}")
 
         for prop_name, prop_details in model.properties.items():
             is_required = (
                 (prop_name in model.required)
                 or (defaults_are_required and prop_details.default is not None)
                 or all_fields_required
             )
 
-            ts_type = (
-                map_openapi_type_to_ts(prop_details.variable_type)
-                if prop_details.variable_type
-                else None
-            )
-
-            annotation_str = " | ".join(set(walk_array_types(prop_details)))
-            ts_type = (
-                ts_type.format(types=annotation_str) if ts_type else annotation_str
-            )
+            # Sort types for determinism in tests and built code
+            ts_type = " | ".join(sorted(set(walk_array_types(prop_details))))
 
             if prop_details.description:
                 fields.append("  /**")
                 fields.append(f"   * {prop_details.description}")
                 fields.append("   */")
 
             fields.append(f"  {prop_name}{'?' if not is_required else ''}: {ts_type};")
```

### Comparing `mountaineer-0.4.0/mountaineer/client_builder/builder.py` & `mountaineer-0.4.1.dev1/mountaineer/client_builder/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/client_builder/openapi.py` & `mountaineer-0.4.1.dev1/mountaineer/client_builder/openapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from enum import StrEnum
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
-from pydantic import BaseModel, Field, model_validator
+from pydantic import BaseModel, ConfigDict, Field, model_validator
 
 #
 # Enum definitions
 #
 
 
 class OpenAPISchemaType(StrEnum):
@@ -14,14 +14,16 @@
     STRING = "string"
     INTEGER = "integer"
     FLOAT = "float"
     BOOLEAN = "boolean"
     ARRAY = "array"
     # Typically used to indicate an optional type within an anyOf statement
     NULL = "null"
+    # Used in some cases when endpoints can accept multiple number types (like integers and floats)
+    NUMBER = "number"
 
 
 class ParameterLocationType(StrEnum):
     # https://swagger.io/specification: Parameter Object
     PATH = "path"
     QUERY = "query"
 
@@ -39,53 +41,85 @@
 
 
 #
 # Nested schemas inside OpenAPI definitions
 #
 
 
+class EmptyAPIProperty(BaseModel):
+    # Ensure our model has exactly zero items for it to be
+    # an empty dict
+    #
+    # Sometimes this is used explicitly as an "any", sometimes it is derived
+    # that any is the only value that can match the type constraints
+    # and it's inserted by our OpenAPI generator automatically
+    #
+    # It can also optionally have a "title" and description in case it was
+    # defined explicitly
+    title: str | None = None
+    description: str | None = None
+    default: Any | None = None
+
+    model_config = ConfigDict(extra="forbid")
+
+
 class OpenAPIProperty(BaseModel):
     """
     A property is the core wrapper for OpenAPI model objects. It allows users to recursively
     define data structures based on their type. Each property can have a list of subproperties, alongside
     the constraints of how they're used (ie. required attributes, union of attributes, etc).
 
     """
 
     title: str | None = None
     description: str | None = None
-    properties: dict[str, "OpenAPIProperty"] = {}
-    additionalProperties: Optional["OpenAPIProperty"] = None
+    properties: dict[str, Union["OpenAPIProperty", EmptyAPIProperty]] = {}
+    additionalProperties: Union["OpenAPIProperty", EmptyAPIProperty, None] = None
     required: list[str] = []
 
     # Just specified on the leaf object
     format: str | None = None
 
     # Self-contained type: object, int, etc
     variable_type: OpenAPISchemaType | None = Field(alias="type", default=None)
     # Reference to another type
     ref: str | None = Field(alias="$ref", default=None)
     # Array of another type
-    items: Optional["OpenAPIProperty"] = None
+    items: Union["OpenAPIProperty", EmptyAPIProperty, None] = None
     # Enum type
     enum: list[Any] | None = None
+    # Literal objects that require a static value
+    const: Any | None = None
 
     default: Any | None = None
 
     # Pointer to multiple possible subtypes
-    anyOf: list["OpenAPIProperty"] = []
+    anyOf: list[Union["OpenAPIProperty", EmptyAPIProperty]] = []
+
+    # Supported by OpenAPI 3.1+, allows for definition of arrays that only accept
+    # certain quantity of item/type combinations (like a tuple)
+    prefixItems: list[Union["OpenAPIProperty", EmptyAPIProperty]] = []
 
     model_config = {"populate_by_name": True}
 
     # Validator to ensure that one of the optional values is set
     @model_validator(mode="after")
     def check_provided_value(self: "OpenAPIProperty") -> "OpenAPIProperty":
-        if not any([self.variable_type, self.ref, self.items, self.anyOf, self.enum]):
+        if not any(
+            [
+                self.variable_type,
+                self.ref,
+                self.items,
+                self.anyOf,
+                self.enum,
+                self.const,
+            ]
+        ):
             raise ValueError(
-                "One of variable_type, $ref, anyOf, enum, or items must be set"
+                "One of variable_type, $ref, anyOf, enum, const, or items must be set"
             )
         return self
 
     @classmethod
     def from_meta(
         cls,
         title: str | None = None,
@@ -93,14 +127,15 @@
         properties: dict[str, "OpenAPIProperty"] = {},
         additional_properties: Optional["OpenAPIProperty"] = None,
         required: list[str] = [],
         format: str | None = None,
         variable_type: OpenAPISchemaType | None = None,
         ref: str | None = None,
         items: Optional["OpenAPIProperty"] = None,
+        const: Any | None = None,
         enum: list[Any] | None = None,
         anyOf: list["OpenAPIProperty"] = [],
     ) -> "OpenAPIProperty":
         return cls.model_validate(
             {
                 "title": title,
                 "description": description,
@@ -108,14 +143,15 @@
                 "additionalProperties": additional_properties,
                 "required": required,
                 "format": format,
                 "type": variable_type,
                 "$ref": ref,
                 "items": items,
                 "enum": enum,
+                "const": const,
                 "anyOf": anyOf,
             }
         )
 
     def __hash__(self):
         # Normally we would make use of a frozen BaseClass to enable hashing, but since
         # dictionaries are included in the payload here an easier way is just to convert
@@ -284,20 +320,23 @@
 
 
 #
 # Helper methods
 #
 
 
-def get_types_from_parameters(schema: OpenAPIProperty):
+def get_types_from_parameters(schema: OpenAPIProperty | EmptyAPIProperty):
     """
     Handle potentially complex types from the parameter schema, like the case
     of optional fields.
 
     """
+    if isinstance(schema, EmptyAPIProperty):
+        return "any"
+
     # Recursively gather all of the types that might be nested
     if schema.variable_type:
         yield schema.variable_type
 
     for property in schema.properties.values():
         yield from get_types_from_parameters(property)
```

### Comparing `mountaineer-0.4.0/mountaineer/client_builder/typescript.py` & `mountaineer-0.4.1.dev1/mountaineer/client_builder/typescript.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,14 @@
 def map_openapi_type_to_ts(openapi_type: OpenAPISchemaType):
     mapping = {
         "string": "string",
         "integer": "number",
         "number": "number",
         "boolean": "boolean",
         "null": "null",
-        "array": "Array<{types}>",
-        "object": "{types}",
     }
     return mapping[openapi_type]
 
 
 def get_typehint_for_parameter(parameter: URLParameterDefinition):
     """
     Get the typehint for a parameter, which may be a single type or a union of types.
```

### Comparing `mountaineer-0.4.0/mountaineer/config.py` & `mountaineer-0.4.1.dev1/mountaineer/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/controller.py` & `mountaineer-0.4.1.dev1/mountaineer/controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/controllers/exception_controller.py` & `mountaineer-0.4.1.dev1/mountaineer/controllers/exception_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/cropper.py` & `mountaineer-0.4.1.dev1/mountaineer/cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/database/cli.py` & `mountaineer-0.4.1.dev1/mountaineer/database/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/database/config.py` & `mountaineer-0.4.1.dev1/mountaineer/database/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/database/dependencies/core.py` & `mountaineer-0.4.1.dev1/mountaineer/database/dependencies/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/database/sqlmodel.py` & `mountaineer-0.4.1.dev1/mountaineer/database/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/database/validator.py` & `mountaineer-0.4.1.dev1/mountaineer/database/validator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/dependencies/base.py` & `mountaineer-0.4.1.dev1/mountaineer/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/dependencies/core/core.py` & `mountaineer-0.4.1.dev1/mountaineer/dependencies/core/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/exceptions.py` & `mountaineer-0.4.1.dev1/mountaineer/exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/io.py` & `mountaineer-0.4.1.dev1/mountaineer/io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/js_compiler/base.py` & `mountaineer-0.4.1.dev1/mountaineer/js_compiler/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/js_compiler/javascript.py` & `mountaineer-0.4.1.dev1/mountaineer/js_compiler/javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/js_compiler/postcss.py` & `mountaineer-0.4.1.dev1/mountaineer/js_compiler/postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/js_compiler/source_maps.py` & `mountaineer-0.4.1.dev1/mountaineer/js_compiler/source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/logging.py` & `mountaineer-0.4.1.dev1/mountaineer/logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/paths.py` & `mountaineer-0.4.1.dev1/mountaineer/paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/render.py` & `mountaineer-0.4.1.dev1/mountaineer/render.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/ssr.py` & `mountaineer-0.4.1.dev1/mountaineer/ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/static/api.ts` & `mountaineer-0.4.1.dev1/mountaineer/static/api.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/static/live_reload.ts` & `mountaineer-0.4.1.dev1/mountaineer/static/live_reload.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/test_utilities.py` & `mountaineer-0.4.1.dev1/mountaineer/test_utilities.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/views/package-lock.json` & `mountaineer-0.4.1.dev1/mountaineer/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/watch.py` & `mountaineer-0.4.1.dev1/mountaineer/watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/watch_server.py` & `mountaineer-0.4.1.dev1/mountaineer/watch_server.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/mountaineer/webservice.py` & `mountaineer-0.4.1.dev1/mountaineer/webservice.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/poetry.lock` & `mountaineer-0.4.1.dev1/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src/benches/fixtures/complex_sourcemap_mapping.txt` & `mountaineer-0.4.1.dev1/src/benches/fixtures/complex_sourcemap_mapping.txt`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src/benches/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.4.1.dev1/src/benches/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src/benches/lexers_benchmark.rs` & `mountaineer-0.4.1.dev1/src/benches/lexers_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src/benches/source_map_benchmark.rs` & `mountaineer-0.4.1.dev1/src/benches/source_map_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src/benches/ssr_benchmark.rs` & `mountaineer-0.4.1.dev1/src/benches/ssr_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src/lexers.rs` & `mountaineer-0.4.1.dev1/src/lexers.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src/lib.rs` & `mountaineer-0.4.1.dev1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src/logging.rs` & `mountaineer-0.4.1.dev1/src/logging.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src/source_map.rs` & `mountaineer-0.4.1.dev1/src/source_map.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src/ssr.rs` & `mountaineer-0.4.1.dev1/src/ssr.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/src/timeout.rs` & `mountaineer-0.4.1.dev1/src/timeout.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.0/Cargo.lock` & `mountaineer-0.4.1.dev1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mountaineer"
-version = "0.4.0"
+version = "0.4.1-dev1"
 dependencies = [
  "criterion",
  "deno_core_icudata",
  "env_logger",
  "lazy_static",
  "libc",
  "log",
```

### Comparing `mountaineer-0.4.0/pyproject.toml` & `mountaineer-0.4.1.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "mountaineer"
 dependencies = [ "pydantic", "fastapi", "inflection", "click", "tqdm", "uvicorn[standard]", "packaging", "watchdog", "pydantic-settings", "sqlmodel", "asyncpg", "sqlalchemy[asyncio]",]
 exclude = [ "fixtures", "ci_webapp", "create_mountaineer_app", "media", "docs_website", "benchmarking",]
 
 [tool.poetry]
 name = "mountaineer"
-version = "0.4.0"
+version = "0.4.1.dev1"
 description = ""
 authors = [ "Pierce Freeman <pierce@freeman.vc>",]
 readme = "README.md"
 
 [tool.mypy]
 warn_return_any = true
 warn_unused_configs = true
```

### Comparing `mountaineer-0.4.0/PKG-INFO` & `mountaineer-0.4.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mountaineer
-Version: 0.4.0
+Version: 0.4.1.dev1
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: inflection
 Requires-Dist: click
 Requires-Dist: tqdm
 Requires-Dist: uvicorn[standard]
 Requires-Dist: packaging
```

