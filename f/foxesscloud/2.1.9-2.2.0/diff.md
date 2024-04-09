# Comparing `tmp/foxesscloud-2.1.9.tar.gz` & `tmp/foxesscloud-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-xf0ec4om\foxesscloud-2.1.9.tar", last modified: Mon Apr  1 18:01:15 2024, max compression
+gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-an7s2f9q\foxesscloud-2.2.0.tar", last modified: Tue Apr  9 15:32:39 2024, max compression
```

## Comparing `foxesscloud-2.1.9.tar` & `foxesscloud-2.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/
--rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.1.9/LICENCE
--rw-rw-rw-   0        0        0    39241 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/PKG-INFO
--rw-rw-rw-   0        0        0    38686 2024-04-01 17:58:50.000000 foxesscloud-2.1.9/README.md
--rw-rw-rw-   0        0        0      635 2024-04-01 13:28:21.000000 foxesscloud-2.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud/
--rw-rw-rw-   0        0        0   174889 2024-04-01 17:51:43.000000 foxesscloud-2.1.9/src/foxesscloud/foxesscloud.py
--rw-rw-rw-   0        0        0   169176 2024-04-01 17:51:43.000000 foxesscloud-2.1.9/src/foxesscloud/openapi.py
-drwxrwxrwx   0        0        0        0 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud.egg-info/
--rw-rw-rw-   0        0        0    39241 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/
+-rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.0/LICENCE
+-rw-rw-rw-   0        0        0    39156 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    38601 2024-04-09 15:25:31.000000 foxesscloud-2.2.0/README.md
+-rw-rw-rw-   0        0        0      635 2024-04-09 15:23:57.000000 foxesscloud-2.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud/
+-rw-rw-rw-   0        0        0   175090 2024-04-09 15:25:23.000000 foxesscloud-2.2.0/src/foxesscloud/foxesscloud.py
+-rw-rw-rw-   0        0        0   169383 2024-04-09 15:28:42.000000 foxesscloud-2.2.0/src/foxesscloud/openapi.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud.egg-info/
+-rw-rw-rw-   0        0        0    39156 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud.egg-info/top_level.txt
```

### Comparing `foxesscloud-2.1.9/LICENCE` & `foxesscloud-2.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `foxesscloud-2.1.9/PKG-INFO` & `foxesscloud-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.1.9
+Version: 2.2.0
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -115,15 +115,14 @@
 
 ## Inverter Settings
 You can change inverter settings using:
 
 ```
 f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2)
-f.set_work_mode(mode)
 f.set_group(start, end, mode, min_soc, fdsoc, fdpwr)
 f.get_flag()
 f.set_schedule(enable, groups, template)
 ```
 
 set_min() applies new SoC settings to the inverter. The parameters update battery_settings:
 + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15%
@@ -133,16 +132,14 @@
 + ch1: enable charge from grid for period 1 (True or False)
 + st1: the start time for period 1
 + en1: the end time for period 1
 + ch2: enable charge from grid for period 2 (True or False)
 + st2: the start time for period 2
 + en2: the end time for period 2
 
-set_work_mode(mode) takes a work mode as a parameter and sets the inverter to this work mode. Valid work modes are held in work_modes. The new mode is stored in work_mode.
-
 set_flag() returns the current settings for strategy periods: 'supported' and 'enable'
 
 set_group() returns a time segment structure that can be used to build a list of time segments for set_schedule()
 + start, end, mode: required parameters
 + min_soc: optional, default is 10
 + fdsoc: optional, default is 10. Used when setting a period with ForceDischarge mode
 + fdpwr: optional, default is 0. Used when setting a period with ForceDischarge mode
@@ -369,14 +366,15 @@
 special_contingency: 30       # contingency for special days when consumption might be higher
 special_days: ['12-25', '12-26', '01-01']
 full_charge: None             # day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue' etc
 derate_temp: 21               # battery temperature in C when derating charge current is applied
 derate_step: 5                # step size for derating e.g. 21, 16, 11
 derating: [24, 15, 10, 2]     # derated charge current for each temperature step e.g. 21C, 16C, 11C, 6C
 force: 1                      # 1 = disable strategy periods when setting charge. 0 = fail if strategy period has been set.
+data_wrap: 6                  # data items to show per line
 ```
 These values are stored / available in f.charge_config.
 
 The default battery open circuit voltage curve versus SoC from 0% to 100% is:
 ```
 lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50]
 ```
@@ -667,14 +665,18 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
+2.20.<br>
+Added 'data_wrap' to charge_config.
+
+
 2.1.9<br>
 Update get_history() to use GMT or BST when plotting instead of mixed time zones.
 Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode.
 Better reporting of reason for http error code.
 Template code for get_named_settings() added - not functional in this version due to Open API limitations.
 Update set_pvoutput() to allow push=2.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.1.9 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.0 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -65,52 +65,49 @@
 'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The result
 also updates f.battery. get_settings() will return the battery settings and is
 equivalent to get_charge() and get_min(). The results are stored in
 f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge
 from grid and the charge times. get_schedule() returns the current work mode /
 soc schedule settings. The result is stored in f.schedule. ## Inverter Settings
 You can change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
-f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_work_mode(mode) f.set_group
-(start, end, mode, min_soc, fdsoc, fdpwr) f.get_flag() f.set_schedule(enable,
-groups, template) ``` set_min() applies new SoC settings to the inverter. The
-parameters update battery_settings: + minSocOnGrid: min Soc on Grid setting
-e.g. 15 = 15% + minSoc: min Soc setting e.g. 10 = 10% set_charge() takes the
-charge times from the battery_settings and applies these to the inverter. The
-parameters are optional and will update battery_settings. You should specify
-all 3 parameter for a time period: + ch1: enable charge from grid for period 1
-(True or False) + st1: the start time for period 1 + en1: the end time for
-period 1 + ch2: enable charge from grid for period 2 (True or False) + st2: the
-start time for period 2 + en2: the end time for period 2 set_work_mode(mode)
-takes a work mode as a parameter and sets the inverter to this work mode. Valid
-work modes are held in work_modes. The new mode is stored in work_mode.
-set_flag() returns the current settings for strategy periods: 'supported' and
-'enable' set_group() returns a time segment structure that can be used to build
-a list of time segments for set_schedule() + start, end, mode: required
-parameters + min_soc: optional, default is 10 + fdsoc: optional, default is 10.
-Used when setting a period with ForceDischarge mode + fdpwr: optional, default
-is 0. Used when setting a period with ForceDischarge mode + enable: sets
-whether this time segment is enable (1) or disabled (0). The default is
-enabled. set_schedule() configures a list of scheduled work mode / soc changes
-with enable=1. If called with enable=0, any existing schedules are disabled. To
-enable a schedule, you must provide a list of time segments + enable: 1 to
-enable schedules, 0 to disable schedules. The default is 1. + groups: a time
-segment or list of time segments created using f.set_group(). ## Real Time Data
-Real time data reports the latest values for inverter variables, collected
-every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars() f.get_real(v) ```
-f.invert_ct2 determines how the meterPower2 data is handled. When invert_ct2 =
-0, meterPower2 produces +ve power values during secondary generation. If
-meterPower2 produces -ve power values during secondary generation, setting
-invert_ct2 = 1 will flip the values so they are +ve when generating. The
-default setting is 1 (invert). f.get_vars() returns the list of variables that
-can be queried. This also stores the information: + f.var_table: a table,
-indexed by variable that contains information such as the name and unit. ++
-f.var_list: a list of all the variables that are available There are also pre-
-defined lists: + power_vars lists the main power variables provided by the
-inverter + battery_vars lists the main variables relevant to the battery / BMS
-f.get_real returns the latest values for a list of variables. + v is a
+f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_group(start, end, mode,
+min_soc, fdsoc, fdpwr) f.get_flag() f.set_schedule(enable, groups, template)
+``` set_min() applies new SoC settings to the inverter. The parameters update
+battery_settings: + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% +
+minSoc: min Soc setting e.g. 10 = 10% set_charge() takes the charge times from
+the battery_settings and applies these to the inverter. The parameters are
+optional and will update battery_settings. You should specify all 3 parameter
+for a time period: + ch1: enable charge from grid for period 1 (True or False)
++ st1: the start time for period 1 + en1: the end time for period 1 + ch2:
+enable charge from grid for period 2 (True or False) + st2: the start time for
+period 2 + en2: the end time for period 2 set_flag() returns the current
+settings for strategy periods: 'supported' and 'enable' set_group() returns a
+time segment structure that can be used to build a list of time segments for
+set_schedule() + start, end, mode: required parameters + min_soc: optional,
+default is 10 + fdsoc: optional, default is 10. Used when setting a period with
+ForceDischarge mode + fdpwr: optional, default is 0. Used when setting a period
+with ForceDischarge mode + enable: sets whether this time segment is enable (1)
+or disabled (0). The default is enabled. set_schedule() configures a list of
+scheduled work mode / soc changes with enable=1. If called with enable=0, any
+existing schedules are disabled. To enable a schedule, you must provide a list
+of time segments + enable: 1 to enable schedules, 0 to disable schedules. The
+default is 1. + groups: a time segment or list of time segments created using
+f.set_group(). ## Real Time Data Real time data reports the latest values for
+inverter variables, collected every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars
+() f.get_real(v) ``` f.invert_ct2 determines how the meterPower2 data is
+handled. When invert_ct2 = 0, meterPower2 produces +ve power values during
+secondary generation. If meterPower2 produces -ve power values during secondary
+generation, setting invert_ct2 = 1 will flip the values so they are +ve when
+generating. The default setting is 1 (invert). f.get_vars() returns the list of
+variables that can be queried. This also stores the information: + f.var_table:
+a table, indexed by variable that contains information such as the name and
+unit. ++ f.var_list: a list of all the variables that are available There are
+also pre-defined lists: + power_vars lists the main power variables provided by
+the inverter + battery_vars lists the main variables relevant to the battery /
+BMS f.get_real returns the latest values for a list of variables. + v is a
 variable, or list of variables. The default is to return the latest value for
 all available variables ## History Data History data reports inverter
 variables, collected every 5 minutes, on a given date / time and period: ```
 f.get_history(time_span, d, v, summary, save, load, plot) ``` + time_span
 determines the period covered by the data, for example, 'hour', 'day' or
 'week'. The default is 'hour' + d is a date and time in the format 'YYYY-MM-DD
 HH:MM:SS'. The default is today's date and time. d may also be a list of dates
@@ -275,54 +272,54 @@
 None special_contingency: 30 # contingency for special days when consumption
 might be higher special_days: ['12-25', '12-26', '01-01'] full_charge: None #
 day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue'
 etc derate_temp: 21 # battery temperature in C when derating charge current is
 applied derate_step: 5 # step size for derating e.g. 21, 16, 11 derating: [24,
 15, 10, 2] # derated charge current for each temperature step e.g. 21C, 16C,
 11C, 6C force: 1 # 1 = disable strategy periods when setting charge. 0 = fail
-if strategy period has been set. ``` These values are stored / available in
-f.charge_config. The default battery open circuit voltage curve versus SoC from
-0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60,
-52.70, 52.80, 52.9, 53.1, 53.50] ``` This example shows the results reported by
-charge needed: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery Info Provides
-detailed information on the current state of the batteries: ``` f.battery_info
-(count, plot, log) f.battery_monitor(interval, run, log, save, count) ```
-battery_info() prints information on the battery and cells: + count: optional
-over-ride. The default is based on rounding the battery voltage divided by 53 +
-plot: 1 plot the cell voltages for each battery, 0 don't plot. The default is 1
-+ log: see below. Default is 0 battery_monitor() runs battery_info() in log
-mode on a schedule to provide information on the battery status over a period
-of time: + interval: the time in minutes between log entries. The default is 30
-minutes + run: the number of log entries to create. The default is 48 i.e.
-every 30 minues for 24 hours in total + log: 0 = display, 1 = log battery info,
-2 = add cell volts, 3 = add cell temps. The default is 1 + save: name of a CSV
-file to write log data to + count: optional over-ride for the number of
-batteries This is an example of the output from battery_info(): ![image](https:
-//github.com/TonyM1958/FoxESS-Cloud/assets/63789168/a8eb52b6-ce3f-4b58-bb76-
-5483d5e40fa7) ## Date Ranges ``` f.date_list(s, e, limit, span, today) ```
-Returns a list of dates in the format 'YYYY-MM-DD'. This function will not
-return dates in the future. The last date will be yesterday or today (if today
-is True). All parameters are optional: + s: start date + e: end date + limit:
-maximum number of days. The default is 200 + span: the range of dates. One of
-'day', 'week', 'month' or 'year', '2days' or 'weekday' + today: 1 allows today
-to be included, 2 allows future dates to be included. Default is 0, date list
-will stop at yesterday You can use 'span' as follows: + 'day' provides a single
-day + 'week' will provide the dates of 7 consequetive days + 'month' will
-provide the dates of the days up to the same date in the preceeding (or
-follwing) month + '2days' will provide the dates of yesterday and today +
-'weekday' will provide the dates of the same day of the week, going backwards
-(or forwards) up to 7 weeks ``` f.british_summer_time(d) # 1 if d is in Britsh
-Summer Time, 0 if not ``` ## Time Periods Times and time period settings are
-held as decimal hours. Functions for working with time strings with the format
-'HH:MM:SS' and decimal hours include: ``` f.time_hours(t, d=None) # convert
-time to decimal hours. t is a time string ('HH:MM' or 'HH:MM:SS'), d is
-optional and is the default time if s is None f.hours_time(h, mm=True,
-ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm = include
-minutes, ss = include seconds, day = include /n for day when hours > 24
+if strategy period has been set. data_wrap: 6 # data items to show per line ```
+These values are stored / available in f.charge_config. The default battery
+open circuit voltage curve versus SoC from 0% to 100% is: ``` lifepo4_curve =
+[51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ```
+This example shows the results reported by charge needed: ![image](https://
+github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-
+20d806b1e7e8) ## Battery Info Provides detailed information on the current
+state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
+(interval, run, log, save, count) ``` battery_info() prints information on the
+battery and cells: + count: optional over-ride. The default is based on
+rounding the battery voltage divided by 53 + plot: 1 plot the cell voltages for
+each battery, 0 don't plot. The default is 1 + log: see below. Default is 0
+battery_monitor() runs battery_info() in log mode on a schedule to provide
+information on the battery status over a period of time: + interval: the time
+in minutes between log entries. The default is 30 minutes + run: the number of
+log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
+total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
+cell temps. The default is 1 + save: name of a CSV file to write log data to +
+count: optional over-ride for the number of batteries This is an example of the
+output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
+assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
+f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
+'YYYY-MM-DD'. This function will not return dates in the future. The last date
+will be yesterday or today (if today is True). All parameters are optional: +
+s: start date + e: end date + limit: maximum number of days. The default is 200
++ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+'weekday' + today: 1 allows today to be included, 2 allows future dates to be
+included. Default is 0, date list will stop at yesterday You can use 'span' as
+follows: + 'day' provides a single day + 'week' will provide the dates of 7
+consequetive days + 'month' will provide the dates of the days up to the same
+date in the preceeding (or follwing) month + '2days' will provide the dates of
+yesterday and today + 'weekday' will provide the dates of the same day of the
+week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
+# 1 if d is in Britsh Summer Time, 0 if not ``` ## Time Periods Times and time
+period settings are held as decimal hours. Functions for working with time
+strings with the format 'HH:MM:SS' and decimal hours include: ``` f.time_hours
+(t, d=None) # convert time to decimal hours. t is a time string ('HH:MM' or
+'HH:MM:SS'), d is optional and is the default time if s is None f.hours_time(h,
+mm=True, ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm =
+include minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
@@ -459,15 +456,16 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.1.9
+(verbose) # Version Info 2.20.
+Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.1.9/README.md` & `foxesscloud-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,14 @@
 
 ## Inverter Settings
 You can change inverter settings using:
 
 ```
 f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2)
-f.set_work_mode(mode)
 f.set_group(start, end, mode, min_soc, fdsoc, fdpwr)
 f.get_flag()
 f.set_schedule(enable, groups, template)
 ```
 
 set_min() applies new SoC settings to the inverter. The parameters update battery_settings:
 + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15%
@@ -119,16 +118,14 @@
 + ch1: enable charge from grid for period 1 (True or False)
 + st1: the start time for period 1
 + en1: the end time for period 1
 + ch2: enable charge from grid for period 2 (True or False)
 + st2: the start time for period 2
 + en2: the end time for period 2
 
-set_work_mode(mode) takes a work mode as a parameter and sets the inverter to this work mode. Valid work modes are held in work_modes. The new mode is stored in work_mode.
-
 set_flag() returns the current settings for strategy periods: 'supported' and 'enable'
 
 set_group() returns a time segment structure that can be used to build a list of time segments for set_schedule()
 + start, end, mode: required parameters
 + min_soc: optional, default is 10
 + fdsoc: optional, default is 10. Used when setting a period with ForceDischarge mode
 + fdpwr: optional, default is 0. Used when setting a period with ForceDischarge mode
@@ -355,14 +352,15 @@
 special_contingency: 30       # contingency for special days when consumption might be higher
 special_days: ['12-25', '12-26', '01-01']
 full_charge: None             # day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue' etc
 derate_temp: 21               # battery temperature in C when derating charge current is applied
 derate_step: 5                # step size for derating e.g. 21, 16, 11
 derating: [24, 15, 10, 2]     # derated charge current for each temperature step e.g. 21C, 16C, 11C, 6C
 force: 1                      # 1 = disable strategy periods when setting charge. 0 = fail if strategy period has been set.
+data_wrap: 6                  # data items to show per line
 ```
 These values are stored / available in f.charge_config.
 
 The default battery open circuit voltage curve versus SoC from 0% to 100% is:
 ```
 lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50]
 ```
@@ -653,14 +651,18 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
+2.20.<br>
+Added 'data_wrap' to charge_config.
+
+
 2.1.9<br>
 Update get_history() to use GMT or BST when plotting instead of mixed time zones.
 Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode.
 Better reporting of reason for http error code.
 Template code for get_named_settings() added - not functional in this version due to Open API limitations.
 Update set_pvoutput() to allow push=2.
```

#### html2text {}

```diff
@@ -58,52 +58,49 @@
 'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The result
 also updates f.battery. get_settings() will return the battery settings and is
 equivalent to get_charge() and get_min(). The results are stored in
 f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge
 from grid and the charge times. get_schedule() returns the current work mode /
 soc schedule settings. The result is stored in f.schedule. ## Inverter Settings
 You can change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
-f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_work_mode(mode) f.set_group
-(start, end, mode, min_soc, fdsoc, fdpwr) f.get_flag() f.set_schedule(enable,
-groups, template) ``` set_min() applies new SoC settings to the inverter. The
-parameters update battery_settings: + minSocOnGrid: min Soc on Grid setting
-e.g. 15 = 15% + minSoc: min Soc setting e.g. 10 = 10% set_charge() takes the
-charge times from the battery_settings and applies these to the inverter. The
-parameters are optional and will update battery_settings. You should specify
-all 3 parameter for a time period: + ch1: enable charge from grid for period 1
-(True or False) + st1: the start time for period 1 + en1: the end time for
-period 1 + ch2: enable charge from grid for period 2 (True or False) + st2: the
-start time for period 2 + en2: the end time for period 2 set_work_mode(mode)
-takes a work mode as a parameter and sets the inverter to this work mode. Valid
-work modes are held in work_modes. The new mode is stored in work_mode.
-set_flag() returns the current settings for strategy periods: 'supported' and
-'enable' set_group() returns a time segment structure that can be used to build
-a list of time segments for set_schedule() + start, end, mode: required
-parameters + min_soc: optional, default is 10 + fdsoc: optional, default is 10.
-Used when setting a period with ForceDischarge mode + fdpwr: optional, default
-is 0. Used when setting a period with ForceDischarge mode + enable: sets
-whether this time segment is enable (1) or disabled (0). The default is
-enabled. set_schedule() configures a list of scheduled work mode / soc changes
-with enable=1. If called with enable=0, any existing schedules are disabled. To
-enable a schedule, you must provide a list of time segments + enable: 1 to
-enable schedules, 0 to disable schedules. The default is 1. + groups: a time
-segment or list of time segments created using f.set_group(). ## Real Time Data
-Real time data reports the latest values for inverter variables, collected
-every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars() f.get_real(v) ```
-f.invert_ct2 determines how the meterPower2 data is handled. When invert_ct2 =
-0, meterPower2 produces +ve power values during secondary generation. If
-meterPower2 produces -ve power values during secondary generation, setting
-invert_ct2 = 1 will flip the values so they are +ve when generating. The
-default setting is 1 (invert). f.get_vars() returns the list of variables that
-can be queried. This also stores the information: + f.var_table: a table,
-indexed by variable that contains information such as the name and unit. ++
-f.var_list: a list of all the variables that are available There are also pre-
-defined lists: + power_vars lists the main power variables provided by the
-inverter + battery_vars lists the main variables relevant to the battery / BMS
-f.get_real returns the latest values for a list of variables. + v is a
+f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_group(start, end, mode,
+min_soc, fdsoc, fdpwr) f.get_flag() f.set_schedule(enable, groups, template)
+``` set_min() applies new SoC settings to the inverter. The parameters update
+battery_settings: + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% +
+minSoc: min Soc setting e.g. 10 = 10% set_charge() takes the charge times from
+the battery_settings and applies these to the inverter. The parameters are
+optional and will update battery_settings. You should specify all 3 parameter
+for a time period: + ch1: enable charge from grid for period 1 (True or False)
++ st1: the start time for period 1 + en1: the end time for period 1 + ch2:
+enable charge from grid for period 2 (True or False) + st2: the start time for
+period 2 + en2: the end time for period 2 set_flag() returns the current
+settings for strategy periods: 'supported' and 'enable' set_group() returns a
+time segment structure that can be used to build a list of time segments for
+set_schedule() + start, end, mode: required parameters + min_soc: optional,
+default is 10 + fdsoc: optional, default is 10. Used when setting a period with
+ForceDischarge mode + fdpwr: optional, default is 0. Used when setting a period
+with ForceDischarge mode + enable: sets whether this time segment is enable (1)
+or disabled (0). The default is enabled. set_schedule() configures a list of
+scheduled work mode / soc changes with enable=1. If called with enable=0, any
+existing schedules are disabled. To enable a schedule, you must provide a list
+of time segments + enable: 1 to enable schedules, 0 to disable schedules. The
+default is 1. + groups: a time segment or list of time segments created using
+f.set_group(). ## Real Time Data Real time data reports the latest values for
+inverter variables, collected every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars
+() f.get_real(v) ``` f.invert_ct2 determines how the meterPower2 data is
+handled. When invert_ct2 = 0, meterPower2 produces +ve power values during
+secondary generation. If meterPower2 produces -ve power values during secondary
+generation, setting invert_ct2 = 1 will flip the values so they are +ve when
+generating. The default setting is 1 (invert). f.get_vars() returns the list of
+variables that can be queried. This also stores the information: + f.var_table:
+a table, indexed by variable that contains information such as the name and
+unit. ++ f.var_list: a list of all the variables that are available There are
+also pre-defined lists: + power_vars lists the main power variables provided by
+the inverter + battery_vars lists the main variables relevant to the battery /
+BMS f.get_real returns the latest values for a list of variables. + v is a
 variable, or list of variables. The default is to return the latest value for
 all available variables ## History Data History data reports inverter
 variables, collected every 5 minutes, on a given date / time and period: ```
 f.get_history(time_span, d, v, summary, save, load, plot) ``` + time_span
 determines the period covered by the data, for example, 'hour', 'day' or
 'week'. The default is 'hour' + d is a date and time in the format 'YYYY-MM-DD
 HH:MM:SS'. The default is today's date and time. d may also be a list of dates
@@ -268,54 +265,54 @@
 None special_contingency: 30 # contingency for special days when consumption
 might be higher special_days: ['12-25', '12-26', '01-01'] full_charge: None #
 day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue'
 etc derate_temp: 21 # battery temperature in C when derating charge current is
 applied derate_step: 5 # step size for derating e.g. 21, 16, 11 derating: [24,
 15, 10, 2] # derated charge current for each temperature step e.g. 21C, 16C,
 11C, 6C force: 1 # 1 = disable strategy periods when setting charge. 0 = fail
-if strategy period has been set. ``` These values are stored / available in
-f.charge_config. The default battery open circuit voltage curve versus SoC from
-0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60,
-52.70, 52.80, 52.9, 53.1, 53.50] ``` This example shows the results reported by
-charge needed: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery Info Provides
-detailed information on the current state of the batteries: ``` f.battery_info
-(count, plot, log) f.battery_monitor(interval, run, log, save, count) ```
-battery_info() prints information on the battery and cells: + count: optional
-over-ride. The default is based on rounding the battery voltage divided by 53 +
-plot: 1 plot the cell voltages for each battery, 0 don't plot. The default is 1
-+ log: see below. Default is 0 battery_monitor() runs battery_info() in log
-mode on a schedule to provide information on the battery status over a period
-of time: + interval: the time in minutes between log entries. The default is 30
-minutes + run: the number of log entries to create. The default is 48 i.e.
-every 30 minues for 24 hours in total + log: 0 = display, 1 = log battery info,
-2 = add cell volts, 3 = add cell temps. The default is 1 + save: name of a CSV
-file to write log data to + count: optional over-ride for the number of
-batteries This is an example of the output from battery_info(): ![image](https:
-//github.com/TonyM1958/FoxESS-Cloud/assets/63789168/a8eb52b6-ce3f-4b58-bb76-
-5483d5e40fa7) ## Date Ranges ``` f.date_list(s, e, limit, span, today) ```
-Returns a list of dates in the format 'YYYY-MM-DD'. This function will not
-return dates in the future. The last date will be yesterday or today (if today
-is True). All parameters are optional: + s: start date + e: end date + limit:
-maximum number of days. The default is 200 + span: the range of dates. One of
-'day', 'week', 'month' or 'year', '2days' or 'weekday' + today: 1 allows today
-to be included, 2 allows future dates to be included. Default is 0, date list
-will stop at yesterday You can use 'span' as follows: + 'day' provides a single
-day + 'week' will provide the dates of 7 consequetive days + 'month' will
-provide the dates of the days up to the same date in the preceeding (or
-follwing) month + '2days' will provide the dates of yesterday and today +
-'weekday' will provide the dates of the same day of the week, going backwards
-(or forwards) up to 7 weeks ``` f.british_summer_time(d) # 1 if d is in Britsh
-Summer Time, 0 if not ``` ## Time Periods Times and time period settings are
-held as decimal hours. Functions for working with time strings with the format
-'HH:MM:SS' and decimal hours include: ``` f.time_hours(t, d=None) # convert
-time to decimal hours. t is a time string ('HH:MM' or 'HH:MM:SS'), d is
-optional and is the default time if s is None f.hours_time(h, mm=True,
-ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm = include
-minutes, ss = include seconds, day = include /n for day when hours > 24
+if strategy period has been set. data_wrap: 6 # data items to show per line ```
+These values are stored / available in f.charge_config. The default battery
+open circuit voltage curve versus SoC from 0% to 100% is: ``` lifepo4_curve =
+[51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ```
+This example shows the results reported by charge needed: ![image](https://
+github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-
+20d806b1e7e8) ## Battery Info Provides detailed information on the current
+state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
+(interval, run, log, save, count) ``` battery_info() prints information on the
+battery and cells: + count: optional over-ride. The default is based on
+rounding the battery voltage divided by 53 + plot: 1 plot the cell voltages for
+each battery, 0 don't plot. The default is 1 + log: see below. Default is 0
+battery_monitor() runs battery_info() in log mode on a schedule to provide
+information on the battery status over a period of time: + interval: the time
+in minutes between log entries. The default is 30 minutes + run: the number of
+log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
+total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
+cell temps. The default is 1 + save: name of a CSV file to write log data to +
+count: optional over-ride for the number of batteries This is an example of the
+output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
+assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
+f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
+'YYYY-MM-DD'. This function will not return dates in the future. The last date
+will be yesterday or today (if today is True). All parameters are optional: +
+s: start date + e: end date + limit: maximum number of days. The default is 200
++ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+'weekday' + today: 1 allows today to be included, 2 allows future dates to be
+included. Default is 0, date list will stop at yesterday You can use 'span' as
+follows: + 'day' provides a single day + 'week' will provide the dates of 7
+consequetive days + 'month' will provide the dates of the days up to the same
+date in the preceeding (or follwing) month + '2days' will provide the dates of
+yesterday and today + 'weekday' will provide the dates of the same day of the
+week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
+# 1 if d is in Britsh Summer Time, 0 if not ``` ## Time Periods Times and time
+period settings are held as decimal hours. Functions for working with time
+strings with the format 'HH:MM:SS' and decimal hours include: ``` f.time_hours
+(t, d=None) # convert time to decimal hours. t is a time string ('HH:MM' or
+'HH:MM:SS'), d is optional and is the default time if s is None f.hours_time(h,
+mm=True, ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm =
+include minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
@@ -452,15 +449,16 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.1.9
+(verbose) # Version Info 2.20.
+Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.1.9/pyproject.toml` & `foxesscloud-2.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "foxesscloud"
-version = "2.1.9"
+version = "2.2.0"
 authors = [
   {name="Tony Matthews", email="tony@quasair.co.uk"},
 ]
 description = "library for accessing Fox ESS cloud data using Open API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `foxesscloud-2.1.9/src/foxesscloud/foxesscloud.py` & `foxesscloud-2.2.0/src/foxesscloud/foxesscloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud
-Updated:  01 April 2024
+Updated:  09 April 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud web site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2023
 ##################################################################################################
 
-version = "1.3.1"
+version = "1.3.2"
 print(f"FoxESS-Cloud version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -1338,15 +1338,15 @@
         hour = 0
         if energy:
             kwh = 0.0       # kwh total
             kwh_off = 0.0   # kwh during off peak time (02:00-05:00)
             kwh_peak = 0.0  # kwh during peak time (16:00-19:00)
             kwh_neg = 0.0
             if len(var['data']) > 1:
-                sample_time = round(60 * sample_rounding * (time_hours(var['data'][-1]['time'][11:19]) - time_hours(var['data'][0]['time'][11:19])) / (len(var['data']) - 1), 0) / sample_rounding
+                sample_time = round(60 * sample_rounding * (time_hours(var['data'][-1]['time'][11:]) - time_hours(var['data'][0]['time'][11:])) / (len(var['data']) - 1), 0) / sample_rounding
             else:
                 sample_time = 5.0
             if debug_setting > 1:
                 output(f"{var['variable']}: samples = {len(var['data'])}, sample_time = {sample_time} minutes")
         sum = 0.0
         count = 0
         max = None
@@ -1769,15 +1769,16 @@
 def split_hours(h):
     if h is None:
         return (None, None)
     hours = int(h % 24)
     minutes = int (h % 1 * 60 + 0.5)
     return (hours, minutes)
 
-# convert time string HH:MM:SS to decimal hours
+# convert time string HH:MM:SS to decimal hours (range 0 to 24)
+# If BST time zone is included, convert to GMT (range -1 to 23)
 def time_hours(t, d = None):
     if t is None:
         t = d
     if type(t) is float:
         return t
     if type(t) is int:
         return float(t)
@@ -2344,15 +2345,16 @@
     'timed_mode': 0,                  # 1 = apply timed work mode, 0 = None
     'special_contingency': 33,        # contingency for special days when consumption might be higher
     'special_days': ['12-25', '12-26', '01-01'],
     'full_charge': None,              # day of month (1-28) to do full charge, or 'daily' or 'Mon', 'Tue' etc
     'derate_temp': 22,                # battery temperature where cold derating starts to be applied
     'derate_step': 5,                 # scale for derating factors in C
     'derating': [24, 15, 10, 2],      # max charge current e.g. 5C step = 22C, 17C, 12C, 7C
-    'force': 1                        # 0 = don't over-ride schedule, 1 = disable schedule
+    'force': 1,                       # 0 = don't over-ride schedule, 1 = disable schedule
+    'data_wrap': 6                    # data to show per line
 }
 
 # app key for charge_needed (used to send output via pushover)
 charge_needed_app_key = "awcr5gro2v13oher3v1qu6hwnovp28"
 
 # work out the charge times to set using the parameters:
 #  forecast: the kWh expected tomorrow. If none, forecast data is loaded from solcast etc
@@ -2843,19 +2845,20 @@
             output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed[i]:6.3f}, {bat_timed[i]:6.3f}")
         if kwh_needed > 0 and show_data > 3:
             output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh (before charging)")
             for i in range(0, run_time):
                 h = base_hour + i
                 output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed_old[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed_old[i]:6.3f}, {bat_timed_old[i]:6.3f}")
     if show_data > 0:
+        data_wrap = charge_config['data_wrap']
         s = f"\nBattery Energy kWh:\n" if show_data == 2 else f"\nBattery SoC %:\n"
-        s += " " * (18 if show_data == 2 else 17) * (base_hour % 6)
+        s += " " * (18 if show_data == 2 else 17) * (base_hour % data_wrap)
         h = base_hour
         for r in bat_timed:
-            s += "\n" if h > hour_now and h % 6 == 0 else ""
+            s += "\n" if h > hour_now and h % data_wrap == 0 else ""
             s += f"  {hours_time(h - (hour_adjustment if h >= change_hour else 0), day=True)}"
             s += f" = {r:5.2f}," if show_data == 2 else f" = {r / capacity * 100:3.0f}%,"
             h += 1
         output(s[:-1])
     if show_plot > 0:
         print()
         plt.figure(figsize=(figure_width, figure_width/2))
```

### Comparing `foxesscloud-2.1.9/src/foxesscloud/openapi.py` & `foxesscloud-2.2.0/src/foxesscloud/openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud using Open API
-Updated:  01 April 2024
+Updated:  09 April 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud api site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2024
 ##################################################################################################
 
-version = "2.1.9"
+version = "2.2.0"
 print(f"FoxESS-Cloud Open API version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -1242,15 +1242,15 @@
         hour = 0
         if energy:
             kwh = 0.0       # kwh total
             kwh_off = 0.0   # kwh during off peak time (02:00-05:00)
             kwh_peak = 0.0  # kwh during peak time (16:00-19:00)
             kwh_neg = 0.0
             if len(var['data']) > 1:
-                sample_time = round(60 * sample_rounding * (time_hours(var['data'][-1]['time'][11:19]) - time_hours(var['data'][0]['time'][11:19])) / (len(var['data']) - 1), 0) / sample_rounding
+                sample_time = round(60 * sample_rounding * (time_hours(var['data'][-1]['time'][11:]) - time_hours(var['data'][0]['time'][11:])) / (len(var['data']) - 1), 0) / sample_rounding
             else:
                 sample_time = 5.0
             if debug_setting > 1:
                 output(f"{var['variable']}: samples = {len(var['data'])}, sample_time = {sample_time} minutes")
         sum = 0.0
         count = 0
         max = None
@@ -1642,15 +1642,16 @@
 def split_hours(h):
     if h is None:
         return (None, None)
     hours = int(h % 24)
     minutes = int (h % 1 * 60 + 0.5)
     return (hours, minutes)
 
-# convert time string HH:MM:SS to decimal hours
+# convert time string HH:MM:SS to decimal hours (range 0 to 24)
+# If BST time zone is included, convert to GMT (range -1 to 23)
 def time_hours(t, d = None):
     if t is None:
         t = d
     if type(t) is float:
         return t
     if type(t) is int:
         return float(t)
@@ -2217,15 +2218,16 @@
     'timed_mode': 0,                  # 1 = apply timed work mode, 0 = None
     'special_contingency': 33,        # contingency for special days when consumption might be higher
     'special_days': ['12-25', '12-26', '01-01'],
     'full_charge': None,              # day of month (1-28) to do full charge, or 'daily' or 'Mon', 'Tue' etc
     'derate_temp': 22,                # battery temperature where cold derating starts to be applied
     'derate_step': 5,                 # scale for derating factors in C
     'derating': [24, 15, 10, 2],      # max charge current e.g. 5C step = 22C, 17C, 12C, 7C
-    'force': 1                        # 0 = don't over-ride schedule, 1 = disable schedule
+    'force': 1,                       # 0 = don't over-ride schedule, 1 = disable schedule
+    'data_wrap': 6                    # data items to show per line
 }
 
 # app key for charge_needed (used to send output via pushover)
 charge_needed_app_key = "awcr5gro2v13oher3v1qu6hwnovp28"
 
 # work out the charge times to set using the parameters:
 #  forecast: the kWh expected tomorrow. If none, forecast data is loaded from solcast etc
@@ -2713,19 +2715,20 @@
             output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed[i]:6.3f}, {bat_timed[i]:6.3f}")
         if kwh_needed > 0 and show_data > 3:
             output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh (before charging)")
             for i in range(0, run_time):
                 h = base_hour + i
                 output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed_old[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed_old[i]:6.3f}, {bat_timed_old[i]:6.3f}")
     if show_data > 0:
+        data_wrap = charge_config['data_wrap']
         s = f"\nBattery Energy kWh:\n" if show_data == 2 else f"\nBattery SoC %:\n"
-        s += " " * (18 if show_data == 2 else 17) * (base_hour % 6)
+        s += " " * (18 if show_data == 2 else 17) * (base_hour % data_wrap)
         h = base_hour
         for r in bat_timed:
-            s += "\n" if h > hour_now and h % 6 == 0 else ""
+            s += "\n" if h > hour_now and h % data_wrap == 0 else ""
             s += f"  {hours_time(h - (hour_adjustment if h >= change_hour else 0), day=True)}"
             s += f" = {r:5.2f}," if show_data == 2 else f" = {r / capacity * 100:3.0f}%,"
             h += 1
         output(s[:-1])
     if show_plot > 0:
         print()
         plt.figure(figsize=(figure_width, figure_width/2))
```

### Comparing `foxesscloud-2.1.9/src/foxesscloud.egg-info/PKG-INFO` & `foxesscloud-2.2.0/src/foxesscloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.1.9
+Version: 2.2.0
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -115,15 +115,14 @@
 
 ## Inverter Settings
 You can change inverter settings using:
 
 ```
 f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2)
-f.set_work_mode(mode)
 f.set_group(start, end, mode, min_soc, fdsoc, fdpwr)
 f.get_flag()
 f.set_schedule(enable, groups, template)
 ```
 
 set_min() applies new SoC settings to the inverter. The parameters update battery_settings:
 + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15%
@@ -133,16 +132,14 @@
 + ch1: enable charge from grid for period 1 (True or False)
 + st1: the start time for period 1
 + en1: the end time for period 1
 + ch2: enable charge from grid for period 2 (True or False)
 + st2: the start time for period 2
 + en2: the end time for period 2
 
-set_work_mode(mode) takes a work mode as a parameter and sets the inverter to this work mode. Valid work modes are held in work_modes. The new mode is stored in work_mode.
-
 set_flag() returns the current settings for strategy periods: 'supported' and 'enable'
 
 set_group() returns a time segment structure that can be used to build a list of time segments for set_schedule()
 + start, end, mode: required parameters
 + min_soc: optional, default is 10
 + fdsoc: optional, default is 10. Used when setting a period with ForceDischarge mode
 + fdpwr: optional, default is 0. Used when setting a period with ForceDischarge mode
@@ -369,14 +366,15 @@
 special_contingency: 30       # contingency for special days when consumption might be higher
 special_days: ['12-25', '12-26', '01-01']
 full_charge: None             # day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue' etc
 derate_temp: 21               # battery temperature in C when derating charge current is applied
 derate_step: 5                # step size for derating e.g. 21, 16, 11
 derating: [24, 15, 10, 2]     # derated charge current for each temperature step e.g. 21C, 16C, 11C, 6C
 force: 1                      # 1 = disable strategy periods when setting charge. 0 = fail if strategy period has been set.
+data_wrap: 6                  # data items to show per line
 ```
 These values are stored / available in f.charge_config.
 
 The default battery open circuit voltage curve versus SoC from 0% to 100% is:
 ```
 lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50]
 ```
@@ -667,14 +665,18 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
+2.20.<br>
+Added 'data_wrap' to charge_config.
+
+
 2.1.9<br>
 Update get_history() to use GMT or BST when plotting instead of mixed time zones.
 Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode.
 Better reporting of reason for http error code.
 Template code for get_named_settings() added - not functional in this version due to Open API limitations.
 Update set_pvoutput() to allow push=2.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.1.9 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.0 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -65,52 +65,49 @@
 'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The result
 also updates f.battery. get_settings() will return the battery settings and is
 equivalent to get_charge() and get_min(). The results are stored in
 f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge
 from grid and the charge times. get_schedule() returns the current work mode /
 soc schedule settings. The result is stored in f.schedule. ## Inverter Settings
 You can change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
-f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_work_mode(mode) f.set_group
-(start, end, mode, min_soc, fdsoc, fdpwr) f.get_flag() f.set_schedule(enable,
-groups, template) ``` set_min() applies new SoC settings to the inverter. The
-parameters update battery_settings: + minSocOnGrid: min Soc on Grid setting
-e.g. 15 = 15% + minSoc: min Soc setting e.g. 10 = 10% set_charge() takes the
-charge times from the battery_settings and applies these to the inverter. The
-parameters are optional and will update battery_settings. You should specify
-all 3 parameter for a time period: + ch1: enable charge from grid for period 1
-(True or False) + st1: the start time for period 1 + en1: the end time for
-period 1 + ch2: enable charge from grid for period 2 (True or False) + st2: the
-start time for period 2 + en2: the end time for period 2 set_work_mode(mode)
-takes a work mode as a parameter and sets the inverter to this work mode. Valid
-work modes are held in work_modes. The new mode is stored in work_mode.
-set_flag() returns the current settings for strategy periods: 'supported' and
-'enable' set_group() returns a time segment structure that can be used to build
-a list of time segments for set_schedule() + start, end, mode: required
-parameters + min_soc: optional, default is 10 + fdsoc: optional, default is 10.
-Used when setting a period with ForceDischarge mode + fdpwr: optional, default
-is 0. Used when setting a period with ForceDischarge mode + enable: sets
-whether this time segment is enable (1) or disabled (0). The default is
-enabled. set_schedule() configures a list of scheduled work mode / soc changes
-with enable=1. If called with enable=0, any existing schedules are disabled. To
-enable a schedule, you must provide a list of time segments + enable: 1 to
-enable schedules, 0 to disable schedules. The default is 1. + groups: a time
-segment or list of time segments created using f.set_group(). ## Real Time Data
-Real time data reports the latest values for inverter variables, collected
-every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars() f.get_real(v) ```
-f.invert_ct2 determines how the meterPower2 data is handled. When invert_ct2 =
-0, meterPower2 produces +ve power values during secondary generation. If
-meterPower2 produces -ve power values during secondary generation, setting
-invert_ct2 = 1 will flip the values so they are +ve when generating. The
-default setting is 1 (invert). f.get_vars() returns the list of variables that
-can be queried. This also stores the information: + f.var_table: a table,
-indexed by variable that contains information such as the name and unit. ++
-f.var_list: a list of all the variables that are available There are also pre-
-defined lists: + power_vars lists the main power variables provided by the
-inverter + battery_vars lists the main variables relevant to the battery / BMS
-f.get_real returns the latest values for a list of variables. + v is a
+f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_group(start, end, mode,
+min_soc, fdsoc, fdpwr) f.get_flag() f.set_schedule(enable, groups, template)
+``` set_min() applies new SoC settings to the inverter. The parameters update
+battery_settings: + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% +
+minSoc: min Soc setting e.g. 10 = 10% set_charge() takes the charge times from
+the battery_settings and applies these to the inverter. The parameters are
+optional and will update battery_settings. You should specify all 3 parameter
+for a time period: + ch1: enable charge from grid for period 1 (True or False)
++ st1: the start time for period 1 + en1: the end time for period 1 + ch2:
+enable charge from grid for period 2 (True or False) + st2: the start time for
+period 2 + en2: the end time for period 2 set_flag() returns the current
+settings for strategy periods: 'supported' and 'enable' set_group() returns a
+time segment structure that can be used to build a list of time segments for
+set_schedule() + start, end, mode: required parameters + min_soc: optional,
+default is 10 + fdsoc: optional, default is 10. Used when setting a period with
+ForceDischarge mode + fdpwr: optional, default is 0. Used when setting a period
+with ForceDischarge mode + enable: sets whether this time segment is enable (1)
+or disabled (0). The default is enabled. set_schedule() configures a list of
+scheduled work mode / soc changes with enable=1. If called with enable=0, any
+existing schedules are disabled. To enable a schedule, you must provide a list
+of time segments + enable: 1 to enable schedules, 0 to disable schedules. The
+default is 1. + groups: a time segment or list of time segments created using
+f.set_group(). ## Real Time Data Real time data reports the latest values for
+inverter variables, collected every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars
+() f.get_real(v) ``` f.invert_ct2 determines how the meterPower2 data is
+handled. When invert_ct2 = 0, meterPower2 produces +ve power values during
+secondary generation. If meterPower2 produces -ve power values during secondary
+generation, setting invert_ct2 = 1 will flip the values so they are +ve when
+generating. The default setting is 1 (invert). f.get_vars() returns the list of
+variables that can be queried. This also stores the information: + f.var_table:
+a table, indexed by variable that contains information such as the name and
+unit. ++ f.var_list: a list of all the variables that are available There are
+also pre-defined lists: + power_vars lists the main power variables provided by
+the inverter + battery_vars lists the main variables relevant to the battery /
+BMS f.get_real returns the latest values for a list of variables. + v is a
 variable, or list of variables. The default is to return the latest value for
 all available variables ## History Data History data reports inverter
 variables, collected every 5 minutes, on a given date / time and period: ```
 f.get_history(time_span, d, v, summary, save, load, plot) ``` + time_span
 determines the period covered by the data, for example, 'hour', 'day' or
 'week'. The default is 'hour' + d is a date and time in the format 'YYYY-MM-DD
 HH:MM:SS'. The default is today's date and time. d may also be a list of dates
@@ -275,54 +272,54 @@
 None special_contingency: 30 # contingency for special days when consumption
 might be higher special_days: ['12-25', '12-26', '01-01'] full_charge: None #
 day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue'
 etc derate_temp: 21 # battery temperature in C when derating charge current is
 applied derate_step: 5 # step size for derating e.g. 21, 16, 11 derating: [24,
 15, 10, 2] # derated charge current for each temperature step e.g. 21C, 16C,
 11C, 6C force: 1 # 1 = disable strategy periods when setting charge. 0 = fail
-if strategy period has been set. ``` These values are stored / available in
-f.charge_config. The default battery open circuit voltage curve versus SoC from
-0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60,
-52.70, 52.80, 52.9, 53.1, 53.50] ``` This example shows the results reported by
-charge needed: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery Info Provides
-detailed information on the current state of the batteries: ``` f.battery_info
-(count, plot, log) f.battery_monitor(interval, run, log, save, count) ```
-battery_info() prints information on the battery and cells: + count: optional
-over-ride. The default is based on rounding the battery voltage divided by 53 +
-plot: 1 plot the cell voltages for each battery, 0 don't plot. The default is 1
-+ log: see below. Default is 0 battery_monitor() runs battery_info() in log
-mode on a schedule to provide information on the battery status over a period
-of time: + interval: the time in minutes between log entries. The default is 30
-minutes + run: the number of log entries to create. The default is 48 i.e.
-every 30 minues for 24 hours in total + log: 0 = display, 1 = log battery info,
-2 = add cell volts, 3 = add cell temps. The default is 1 + save: name of a CSV
-file to write log data to + count: optional over-ride for the number of
-batteries This is an example of the output from battery_info(): ![image](https:
-//github.com/TonyM1958/FoxESS-Cloud/assets/63789168/a8eb52b6-ce3f-4b58-bb76-
-5483d5e40fa7) ## Date Ranges ``` f.date_list(s, e, limit, span, today) ```
-Returns a list of dates in the format 'YYYY-MM-DD'. This function will not
-return dates in the future. The last date will be yesterday or today (if today
-is True). All parameters are optional: + s: start date + e: end date + limit:
-maximum number of days. The default is 200 + span: the range of dates. One of
-'day', 'week', 'month' or 'year', '2days' or 'weekday' + today: 1 allows today
-to be included, 2 allows future dates to be included. Default is 0, date list
-will stop at yesterday You can use 'span' as follows: + 'day' provides a single
-day + 'week' will provide the dates of 7 consequetive days + 'month' will
-provide the dates of the days up to the same date in the preceeding (or
-follwing) month + '2days' will provide the dates of yesterday and today +
-'weekday' will provide the dates of the same day of the week, going backwards
-(or forwards) up to 7 weeks ``` f.british_summer_time(d) # 1 if d is in Britsh
-Summer Time, 0 if not ``` ## Time Periods Times and time period settings are
-held as decimal hours. Functions for working with time strings with the format
-'HH:MM:SS' and decimal hours include: ``` f.time_hours(t, d=None) # convert
-time to decimal hours. t is a time string ('HH:MM' or 'HH:MM:SS'), d is
-optional and is the default time if s is None f.hours_time(h, mm=True,
-ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm = include
-minutes, ss = include seconds, day = include /n for day when hours > 24
+if strategy period has been set. data_wrap: 6 # data items to show per line ```
+These values are stored / available in f.charge_config. The default battery
+open circuit voltage curve versus SoC from 0% to 100% is: ``` lifepo4_curve =
+[51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ```
+This example shows the results reported by charge needed: ![image](https://
+github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-
+20d806b1e7e8) ## Battery Info Provides detailed information on the current
+state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
+(interval, run, log, save, count) ``` battery_info() prints information on the
+battery and cells: + count: optional over-ride. The default is based on
+rounding the battery voltage divided by 53 + plot: 1 plot the cell voltages for
+each battery, 0 don't plot. The default is 1 + log: see below. Default is 0
+battery_monitor() runs battery_info() in log mode on a schedule to provide
+information on the battery status over a period of time: + interval: the time
+in minutes between log entries. The default is 30 minutes + run: the number of
+log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
+total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
+cell temps. The default is 1 + save: name of a CSV file to write log data to +
+count: optional over-ride for the number of batteries This is an example of the
+output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
+assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
+f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
+'YYYY-MM-DD'. This function will not return dates in the future. The last date
+will be yesterday or today (if today is True). All parameters are optional: +
+s: start date + e: end date + limit: maximum number of days. The default is 200
++ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+'weekday' + today: 1 allows today to be included, 2 allows future dates to be
+included. Default is 0, date list will stop at yesterday You can use 'span' as
+follows: + 'day' provides a single day + 'week' will provide the dates of 7
+consequetive days + 'month' will provide the dates of the days up to the same
+date in the preceeding (or follwing) month + '2days' will provide the dates of
+yesterday and today + 'weekday' will provide the dates of the same day of the
+week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
+# 1 if d is in Britsh Summer Time, 0 if not ``` ## Time Periods Times and time
+period settings are held as decimal hours. Functions for working with time
+strings with the format 'HH:MM:SS' and decimal hours include: ``` f.time_hours
+(t, d=None) # convert time to decimal hours. t is a time string ('HH:MM' or
+'HH:MM:SS'), d is optional and is the default time if s is None f.hours_time(h,
+mm=True, ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm =
+include minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
@@ -459,15 +456,16 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.1.9
+(verbose) # Version Info 2.20.
+Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

