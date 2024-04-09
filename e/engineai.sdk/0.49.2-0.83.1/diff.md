# Comparing `tmp/engineai_sdk-0.49.2.tar.gz` & `tmp/engineai_sdk-0.83.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engineai_sdk-0.49.2.tar", max compression
+gzip compressed data, was "engineai_sdk-0.83.1.tar", max compression
```

## Comparing `engineai_sdk-0.49.2.tar` & `engineai_sdk-0.83.1.tar`

### file list

```diff
@@ -1,360 +1,380 @@
--rw-r--r--   0        0        0     1065 2023-12-06 19:18:25.466520 engineai_sdk-0.49.2/LICENSE
--rw-r--r--   0        0        0      251 2024-04-08 13:34:03.261810 engineai_sdk-0.49.2/engineai/sdk/__init__.py
--rw-r--r--   0        0        0       28 2023-12-06 19:18:25.476299 engineai_sdk-0.49.2/engineai/sdk/cli/__init__.py
--rw-r--r--   0        0        0     4158 2024-04-08 13:34:03.262197 engineai_sdk-0.49.2/engineai/sdk/cli/console.py
--rw-r--r--   0        0        0     5125 2024-04-08 13:34:03.262480 engineai_sdk-0.49.2/engineai/sdk/cli/generator.py
--rw-r--r--   0        0        0       42 2023-12-06 19:18:25.477097 engineai_sdk-0.49.2/engineai/sdk/cli/template/content/.env.sample
--rw-r--r--   0        0        0      911 2023-12-06 19:18:25.477321 engineai_sdk-0.49.2/engineai/sdk/cli/template/content/main.py
--rw-r--r--   0        0        0     2676 2023-12-06 19:18:25.477589 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/AAPL_dividends.csv
--rw-r--r--   0        0        0      593 2023-12-06 19:18:25.477770 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/AAPL_earnings.csv
--rw-r--r--   0        0        0   152608 2023-12-06 19:18:25.479154 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/AAPL_history.csv
--rw-r--r--   0        0        0     7518 2023-12-06 19:18:25.479488 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/AAPL_info.json
--rw-r--r--   0        0        0     7217 2023-12-06 19:18:25.479720 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/AMZN_info.json
--rw-r--r--   0        0        0   139522 2023-12-06 19:18:25.480516 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/GSPC.csv
--rw-r--r--   0        0        0   135696 2023-12-06 19:18:25.481404 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/IXIC.csv
--rw-r--r--   0        0        0     8115 2023-12-06 19:18:25.481697 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JNJ_dividends.csv
--rw-r--r--   0        0        0      581 2023-12-06 19:18:25.481907 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JNJ_earnings.csv
--rw-r--r--   0        0        0   152152 2023-12-06 19:18:25.483165 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JNJ_history.csv
--rw-r--r--   0        0        0     8122 2023-12-06 19:18:25.483491 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JNJ_info.json
--rw-r--r--   0        0        0     5125 2023-12-06 19:18:25.483699 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JPM_dividends.csv
--rw-r--r--   0        0        0      571 2023-12-06 19:18:25.483890 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JPM_earnings.csv
--rw-r--r--   0        0        0   151607 2023-12-06 19:18:25.485276 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JPM_history.csv
--rw-r--r--   0        0        0     8080 2023-12-06 19:18:25.485809 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JPM_info.json
--rw-r--r--   0        0        0     2425 2023-12-06 19:18:25.486347 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/MSFT_dividends.csv
--rw-r--r--   0        0        0      623 2023-12-06 19:18:25.486658 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/MSFT_earnings.csv
--rw-r--r--   0        0        0   152489 2023-12-06 19:18:25.488040 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/MSFT_history.csv
--rw-r--r--   0        0        0     8221 2023-12-06 19:18:25.488460 engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/MSFT_info.json
--rw-r--r--   0        0        0     6718 2024-04-08 13:34:03.263579 engineai_sdk-0.49.2/engineai/sdk/cli/utils.py
--rw-r--r--   0        0        0       38 2023-12-06 19:18:25.489024 engineai_sdk-0.49.2/engineai/sdk/dashboard/__init__.py
--rw-r--r--   0        0        0      211 2024-04-08 13:34:03.263891 engineai_sdk-0.49.2/engineai/sdk/dashboard/abstract/__init__.py
--rw-r--r--   0        0        0      198 2024-04-08 13:34:03.264176 engineai_sdk-0.49.2/engineai/sdk/dashboard/abstract/interface.py
--rw-r--r--   0        0        0     2181 2023-12-06 19:18:25.489681 engineai_sdk-0.49.2/engineai/sdk/dashboard/abstract/layout.py
--rw-r--r--   0        0        0      207 2023-12-06 19:18:25.489902 engineai_sdk-0.49.2/engineai/sdk/dashboard/abstract/selectable_widgets.py
--rw-r--r--   0        0        0      537 2024-04-08 13:34:03.264700 engineai_sdk-0.49.2/engineai/sdk/dashboard/abstract/typing.py
--rw-r--r--   0        0        0     2570 2024-04-08 13:34:03.264955 engineai_sdk-0.49.2/engineai/sdk/dashboard/abstract/widget_dependencies.py
--rw-r--r--   0        0        0      942 2024-04-08 13:34:03.265227 engineai_sdk-0.49.2/engineai/sdk/dashboard/base.py
--rw-r--r--   0        0        0       96 2023-12-06 19:18:25.490733 engineai_sdk-0.49.2/engineai/sdk/dashboard/clients/__init__.py
--rw-r--r--   0        0        0     8784 2024-04-08 13:34:03.265594 engineai_sdk-0.49.2/engineai/sdk/dashboard/clients/api.py
--rw-r--r--   0        0        0     1451 2023-12-06 19:18:25.491144 engineai_sdk-0.49.2/engineai/sdk/dashboard/clients/exceptions.py
--rw-r--r--   0        0        0      515 2023-12-06 19:18:25.491316 engineai_sdk-0.49.2/engineai/sdk/dashboard/config.py
--rw-r--r--   0        0        0      202 2024-04-08 13:34:03.266224 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/__init__.py
--rw-r--r--   0        0        0    10995 2024-04-08 13:34:03.266631 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/dashboard.py
--rw-r--r--   0        0        0      140 2023-12-06 19:18:25.491988 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/enums.py
--rw-r--r--   0        0        0     5256 2024-04-08 13:34:03.266919 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/exceptions.py
--rw-r--r--   0        0        0     3125 2024-04-08 13:34:03.267072 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/exit_handler.py
--rw-r--r--   0        0        0     8149 2024-04-08 13:34:03.267278 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/graph.py
--rw-r--r--   0        0        0       41 2023-12-06 19:18:25.492813 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/page/__init__.py
--rw-r--r--   0        0        0     1645 2024-04-08 13:34:03.268099 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/page/dependency.py
--rw-r--r--   0        0        0     4846 2024-04-08 13:34:03.268504 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/page/page.py
--rw-r--r--   0        0        0     1882 2024-04-08 13:34:03.268797 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/page/root.py
--rw-r--r--   0        0        0     2326 2024-04-08 13:34:03.269072 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/page/route.py
--rw-r--r--   0        0        0      345 2023-12-06 19:18:25.493791 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/typings.py
--rw-r--r--   0        0        0       33 2023-12-06 19:18:25.494059 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/version/__init__.py
--rw-r--r--   0        0        0     5060 2024-04-08 13:34:03.269668 engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/version/version.py
--rw-r--r--   0        0        0      139 2024-04-08 13:34:03.270233 engineai_sdk-0.49.2/engineai/sdk/dashboard/data/__init__.py
--rw-r--r--   0        0        0     9951 2024-04-08 13:34:03.270841 engineai_sdk-0.49.2/engineai/sdk/dashboard/data/decorator.py
--rw-r--r--   0        0        0     4641 2024-04-08 13:34:03.271985 engineai_sdk-0.49.2/engineai/sdk/dashboard/data/exceptions.py
--rw-r--r--   0        0        0     2444 2024-04-08 13:34:03.272137 engineai_sdk-0.49.2/engineai/sdk/dashboard/data/file_keys_handler.py
--rw-r--r--   0        0        0     1306 2023-12-06 19:18:25.495673 engineai_sdk-0.49.2/engineai/sdk/dashboard/data/manager/interface.py
--rw-r--r--   0        0        0     8347 2024-04-08 13:34:03.273084 engineai_sdk-0.49.2/engineai/sdk/dashboard/data/manager/manager.py
--rw-r--r--   0        0        0      284 2024-04-08 13:34:03.273590 engineai_sdk-0.49.2/engineai/sdk/dashboard/dependencies/__init__.py
--rw-r--r--   0        0        0     2605 2024-04-08 13:34:03.274173 engineai_sdk-0.49.2/engineai/sdk/dashboard/dependencies/datastore.py
--rw-r--r--   0        0        0     2908 2024-04-08 13:34:03.274648 engineai_sdk-0.49.2/engineai/sdk/dashboard/dependencies/route.py
--rw-r--r--   0        0        0     1502 2024-04-08 13:34:03.275351 engineai_sdk-0.49.2/engineai/sdk/dashboard/dependencies/widget.py
--rw-r--r--   0        0        0      369 2023-12-06 19:18:25.497337 engineai_sdk-0.49.2/engineai/sdk/dashboard/enum/__init__.py
--rw-r--r--   0        0        0      934 2023-12-06 19:18:25.497535 engineai_sdk-0.49.2/engineai/sdk/dashboard/enum/align.py
--rw-r--r--   0        0        0      705 2023-12-06 19:18:25.497705 engineai_sdk-0.49.2/engineai/sdk/dashboard/enum/legend_position.py
--rw-r--r--   0        0        0     5156 2023-12-06 19:18:25.497890 engineai_sdk-0.49.2/engineai/sdk/dashboard/exceptions.py
--rw-r--r--   0        0        0      569 2023-12-06 19:18:25.498155 engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/__init__.py
--rw-r--r--   0        0        0     3688 2023-12-06 19:18:25.498369 engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/axis.py
--rw-r--r--   0        0        0     1817 2023-12-06 19:18:25.498560 engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/datetime.py
--rw-r--r--   0        0        0      661 2023-12-06 19:18:25.498736 engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/exceptions.py
--rw-r--r--   0        0        0     1259 2023-12-06 19:18:25.498911 engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/mapper.py
--rw-r--r--   0        0        0     5108 2023-12-06 19:18:25.499125 engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/number.py
--rw-r--r--   0        0        0     1272 2023-12-06 19:18:25.499319 engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/text.py
--rw-r--r--   0        0        0      331 2023-12-06 19:18:25.499487 engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/typing.py
--rw-r--r--   0        0        0      985 2023-12-06 19:18:25.499663 engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/validator.py
--rw-r--r--   0        0        0      869 2024-04-08 13:34:03.275811 engineai_sdk-0.49.2/engineai/sdk/dashboard/interface.py
--rw-r--r--   0        0        0      825 2023-12-06 19:18:25.500094 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/__init__.py
--rw-r--r--   0        0        0      417 2023-12-06 19:18:25.500274 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/build_item.py
--rw-r--r--   0        0        0       28 2023-12-06 19:18:25.500552 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/card/__init__.py
--rw-r--r--   0        0        0     5431 2024-04-08 13:34:03.277231 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/card/card.py
--rw-r--r--   0        0        0     2936 2024-04-08 13:34:03.278166 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/card/chip.py
--rw-r--r--   0        0        0     1611 2024-04-08 13:34:03.279008 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/card/header.py
--rw-r--r--   0        0        0       55 2023-12-06 19:18:25.501755 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/collapsible/__init__.py
--rw-r--r--   0        0        0     3186 2024-04-08 13:34:03.279870 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/collapsible/chip.py
--rw-r--r--   0        0        0     1955 2024-04-08 13:34:03.280707 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/collapsible/header.py
--rw-r--r--   0        0        0     6294 2024-04-08 13:34:03.281184 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/collapsible/section.py
--rw-r--r--   0        0        0     5754 2024-04-08 13:34:03.281651 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/column.py
--rw-r--r--   0        0        0     4838 2024-04-08 13:34:03.282363 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/components/chip.py
--rw-r--r--   0        0        0     2036 2024-04-08 13:34:03.282812 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/components/header.py
--rw-r--r--   0        0        0     2358 2024-04-08 13:34:03.283930 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/components/label.py
--rw-r--r--   0        0        0     4695 2023-12-06 19:18:25.504100 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/exceptions.py
--rw-r--r--   0        0        0       31 2023-12-06 19:18:25.504550 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/fluid_row/__init__.py
--rw-r--r--   0        0        0     5658 2023-12-06 19:18:25.504784 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py
--rw-r--r--   0        0        0     1697 2023-12-06 19:18:25.505004 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/fluid_row/items_build.py
--rw-r--r--   0        0        0     7079 2024-04-08 13:34:03.284531 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/grid.py
--rw-r--r--   0        0        0    10269 2024-04-08 13:34:03.285029 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/row.py
--rw-r--r--   0        0        0       36 2023-12-06 19:18:25.505728 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/selectable/__init__.py
--rw-r--r--   0        0        0     7552 2024-04-08 13:34:03.285772 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/selectable/base.py
--rw-r--r--   0        0        0     2171 2023-12-06 19:18:25.506158 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/selectable/exceptions.py
--rw-r--r--   0        0        0     3944 2024-04-08 13:34:03.286506 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/selectable/tab.py
--rw-r--r--   0        0        0      410 2023-12-06 19:18:25.506561 engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/typings.py
--rw-r--r--   0        0        0      182 2024-04-08 13:34:03.287416 engineai_sdk-0.49.2/engineai/sdk/dashboard/links/__init__.py
--rw-r--r--   0        0        0     6016 2023-12-06 19:18:25.507070 engineai_sdk-0.49.2/engineai/sdk/dashboard/links/abstract.py
--rw-r--r--   0        0        0     2065 2024-04-08 13:34:03.288695 engineai_sdk-0.49.2/engineai/sdk/dashboard/links/route_link.py
--rw-r--r--   0        0        0     2576 2023-12-06 19:18:25.507719 engineai_sdk-0.49.2/engineai/sdk/dashboard/links/template_string_link.py
--rw-r--r--   0        0        0      202 2023-12-06 19:18:25.507896 engineai_sdk-0.49.2/engineai/sdk/dashboard/links/typing.py
--rw-r--r--   0        0        0      934 2023-12-06 19:18:25.508074 engineai_sdk-0.49.2/engineai/sdk/dashboard/links/widget_dependency.py
--rw-r--r--   0        0        0     2942 2024-04-08 13:34:03.289254 engineai_sdk-0.49.2/engineai/sdk/dashboard/links/widget_field.py
--rw-r--r--   0        0        0        0 2023-12-06 19:18:25.508379 engineai_sdk-0.49.2/engineai/sdk/dashboard/py.typed
--rw-r--r--   0        0        0     2020 2023-12-06 19:18:25.508592 engineai_sdk-0.49.2/engineai/sdk/dashboard/selected.py
--rw-r--r--   0        0        0      100 2023-12-06 19:18:25.508886 engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/__init__.py
--rw-r--r--   0        0        0      744 2023-12-06 19:18:25.509184 engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/__init__.py
--rw-r--r--   0        0        0     3094 2024-04-08 13:34:03.290132 engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/default_specs.py
--rw-r--r--   0        0        0     6474 2024-04-08 13:34:03.291108 engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/discrete_map.py
--rw-r--r--   0        0        0     1663 2024-04-08 13:34:03.291635 engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/divergent.py
--rw-r--r--   0        0        0     3547 2024-04-08 13:34:03.292436 engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/gradient.py
--rw-r--r--   0        0        0     4687 2024-04-08 13:34:03.292939 engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/palette.py
--rw-r--r--   0        0        0      802 2024-04-08 13:34:03.293350 engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/single.py
--rw-r--r--   0        0        0      946 2023-12-06 19:18:25.510558 engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/spec.py
--rw-r--r--   0        0        0      277 2023-12-06 19:18:25.510727 engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/typing.py
--rw-r--r--   0        0        0     3436 2023-12-06 19:18:25.510926 engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/icons.py
--rw-r--r--   0        0        0     8298 2023-12-06 19:18:25.511135 engineai_sdk-0.49.2/engineai/sdk/dashboard/templated_string.py
--rw-r--r--   0        0        0     2561 2024-04-08 13:34:03.293751 engineai_sdk-0.49.2/engineai/sdk/dashboard/utils.py
--rw-r--r--   0        0        0       25 2023-12-06 19:18:25.511578 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/__init__.py
--rw-r--r--   0        0        0     8665 2024-04-08 13:34:03.295530 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/base.py
--rw-r--r--   0        0        0     2647 2023-12-06 19:18:25.512102 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/__init__.py
--rw-r--r--   0        0        0       44 2023-12-06 19:18:25.512361 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/axis/__init__.py
--rw-r--r--   0        0        0     3538 2024-04-08 13:34:03.296414 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/axis/base.py
--rw-r--r--   0        0        0      365 2023-12-06 19:18:25.512826 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/axis/typing.py
--rw-r--r--   0        0        0     2121 2024-04-08 13:34:03.296989 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py
--rw-r--r--   0        0        0     5209 2024-04-08 13:34:03.297709 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py
--rw-r--r--   0        0        0     4333 2024-04-08 13:34:03.298513 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/cartesian.py
--rw-r--r--   0        0        0     4453 2024-04-08 13:34:03.299052 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/chart.py
--rw-r--r--   0        0        0     1468 2023-12-06 19:18:25.514009 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/exceptions.py
--rw-r--r--   0        0        0      960 2024-04-08 13:34:03.300106 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/legend.py
--rw-r--r--   0        0        0       45 2023-12-06 19:18:25.514515 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/__init__.py
--rw-r--r--   0        0        0     2613 2024-04-08 13:34:03.302378 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/area.py
--rw-r--r--   0        0        0     3996 2024-04-08 13:34:03.303090 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py
--rw-r--r--   0        0        0     7228 2024-04-08 13:34:03.306649 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/base.py
--rw-r--r--   0        0        0     5275 2024-04-08 13:34:03.307321 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py
--rw-r--r--   0        0        0     2633 2024-04-08 13:34:03.309715 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/column.py
--rw-r--r--   0        0        0     2613 2024-04-08 13:34:03.310324 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/line.py
--rw-r--r--   0        0        0     2652 2024-04-08 13:34:03.310685 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py
--rw-r--r--   0        0        0      573 2023-12-06 19:18:25.516213 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/typing.py
--rw-r--r--   0        0        0     4957 2023-12-06 19:18:25.516485 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/chart_utils.py
--rw-r--r--   0        0        0       39 2023-12-06 19:18:25.516772 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/__init__.py
--rw-r--r--   0        0        0       87 2023-12-06 19:18:25.517138 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/actions/links/__init__.py
--rw-r--r--   0        0        0     2602 2024-04-08 13:34:03.311384 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/actions/links/base.py
--rw-r--r--   0        0        0     1475 2023-12-06 19:18:25.517521 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py
--rw-r--r--   0        0        0     1883 2024-04-08 13:34:03.311805 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py
--rw-r--r--   0        0        0       47 2023-12-06 19:18:25.518036 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/__init__.py
--rw-r--r--   0        0        0       56 2023-12-06 19:18:25.518306 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/__init__.py
--rw-r--r--   0        0        0      416 2023-12-06 19:18:25.518574 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/__init__.py
--rw-r--r--   0        0        0      965 2024-04-08 13:34:03.312916 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py
--rw-r--r--   0        0        0     1479 2024-04-08 13:34:03.313546 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py
--rw-r--r--   0        0        0     1479 2024-04-08 13:34:03.316155 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py
--rw-r--r--   0        0        0     1117 2023-12-06 19:18:25.520136 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py
--rw-r--r--   0        0        0     2629 2024-04-08 13:34:03.316710 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py
--rw-r--r--   0        0        0      338 2023-12-06 19:18:25.520558 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/typing.py
--rw-r--r--   0        0        0      151 2023-12-06 19:18:25.520732 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/consts.py
--rw-r--r--   0        0        0     7162 2023-12-06 19:18:25.520935 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/exceptions.py
--rw-r--r--   0        0        0       25 2023-12-06 19:18:25.521204 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/series/__init__.py
--rw-r--r--   0        0        0     2787 2023-12-06 19:18:25.521387 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/series/base.py
--rw-r--r--   0        0        0       23 2023-12-06 19:18:25.521635 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/__init__.py
--rw-r--r--   0        0        0      955 2023-12-06 19:18:25.521852 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py
--rw-r--r--   0        0        0     2138 2023-12-06 19:18:25.522041 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py
--rw-r--r--   0        0        0      806 2023-12-06 19:18:25.522220 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py
--rw-r--r--   0        0        0      314 2023-12-06 19:18:25.522394 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/typing.py
--rw-r--r--   0        0        0      696 2023-12-06 19:18:25.522740 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py
--rw-r--r--   0        0        0     1312 2024-04-08 13:34:03.317997 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/area.py
--rw-r--r--   0        0        0     1346 2024-04-08 13:34:03.318562 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py
--rw-r--r--   0        0        0     4041 2023-12-06 19:18:25.523553 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/base.py
--rw-r--r--   0        0        0     3351 2024-04-08 13:34:03.319170 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py
--rw-r--r--   0        0        0     2949 2024-04-08 13:34:03.320091 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py
--rw-r--r--   0        0        0     1307 2024-04-08 13:34:03.320838 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/column.py
--rw-r--r--   0        0        0     1047 2023-12-06 19:18:25.524366 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py
--rw-r--r--   0        0        0     1315 2024-04-08 13:34:03.321818 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py
--rw-r--r--   0        0        0     3443 2024-04-08 13:34:03.322286 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/line.py
--rw-r--r--   0        0        0     1282 2024-04-08 13:34:03.322667 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/point.py
--rw-r--r--   0        0        0     1292 2024-04-08 13:34:03.323490 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py
--rw-r--r--   0        0        0      802 2023-12-06 19:18:25.525336 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py
--rw-r--r--   0        0        0      282 2023-12-06 19:18:25.525569 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/toolbar.py
--rw-r--r--   0        0        0      319 2023-12-06 19:18:25.525896 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/__init__.py
--rw-r--r--   0        0        0     3619 2024-04-08 13:34:03.324573 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py
--rw-r--r--   0        0        0     1265 2024-04-08 13:34:03.325048 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py
--rw-r--r--   0        0        0     1425 2024-04-08 13:34:03.325449 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py
--rw-r--r--   0        0        0      617 2023-12-06 19:18:25.526762 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py
--rw-r--r--   0        0        0     1102 2023-12-06 19:18:25.526949 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py
--rw-r--r--   0        0        0     1308 2024-04-08 13:34:03.326207 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py
--rw-r--r--   0        0        0     1380 2024-04-08 13:34:03.326729 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py
--rw-r--r--   0        0        0      647 2023-12-06 19:18:25.527476 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/typing.py
--rw-r--r--   0        0        0       29 2023-12-06 19:18:25.527736 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/__init__.py
--rw-r--r--   0        0        0     1192 2023-12-06 19:18:25.528025 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py
--rw-r--r--   0        0        0     4730 2024-04-08 13:34:03.327504 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/base.py
--rw-r--r--   0        0        0       35 2023-12-06 19:18:25.528484 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/__init__.py
--rw-r--r--   0        0        0      228 2023-12-06 19:18:25.528736 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/area.py
--rw-r--r--   0        0        0      236 2023-12-06 19:18:25.528930 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/column.py
--rw-r--r--   0        0        0      228 2023-12-06 19:18:25.529139 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/line.py
--rw-r--r--   0        0        0     1184 2023-12-06 19:18:25.529376 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py
--rw-r--r--   0        0        0      379 2023-12-06 19:18:25.529636 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/typing.py
--rw-r--r--   0        0        0      974 2023-12-06 19:18:25.529858 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py
--rw-r--r--   0        0        0       36 2023-12-06 19:18:25.530205 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/__init__.py
--rw-r--r--   0        0        0     1424 2024-04-08 13:34:03.328206 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py
--rw-r--r--   0        0        0      875 2024-04-08 13:34:03.328967 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py
--rw-r--r--   0        0        0      866 2024-04-08 13:34:03.329682 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py
--rw-r--r--   0        0        0      879 2024-04-08 13:34:03.330151 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py
--rw-r--r--   0        0        0     1236 2024-04-08 13:34:03.330556 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py
--rw-r--r--   0        0        0      339 2023-12-06 19:18:25.531514 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/typing.py
--rw-r--r--   0        0        0       34 2023-12-06 19:18:25.531816 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/text/__init__.py
--rw-r--r--   0        0        0      852 2024-04-08 13:34:03.331004 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py
--rw-r--r--   0        0        0     1361 2024-04-08 13:34:03.331566 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py
--rw-r--r--   0        0        0      916 2024-04-08 13:34:03.331924 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py
--rw-r--r--   0        0        0      876 2024-04-08 13:34:03.332281 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py
--rw-r--r--   0        0        0      331 2023-12-06 19:18:25.532812 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/text/typing.py
--rw-r--r--   0        0        0     1313 2023-12-06 19:18:25.533108 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py
--rw-r--r--   0        0        0     2014 2023-12-06 19:18:25.533299 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py
--rw-r--r--   0        0        0     2003 2023-12-06 19:18:25.533507 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py
--rw-r--r--   0        0        0      136 2023-12-06 19:18:25.533794 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/content/__init__.py
--rw-r--r--   0        0        0     2805 2024-04-08 13:34:03.332948 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/content/content.py
--rw-r--r--   0        0        0     1265 2023-12-06 19:18:25.534195 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/content/exceptions.py
--rw-r--r--   0        0        0      613 2023-12-06 19:18:25.534377 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/content/item.py
--rw-r--r--   0        0        0     1404 2024-04-08 13:34:03.333401 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/content/markdown.py
--rw-r--r--   0        0        0     3756 2023-12-06 19:18:25.534812 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/exceptions.py
--rw-r--r--   0        0        0      350 2023-12-06 19:18:25.535169 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/__init__.py
--rw-r--r--   0        0        0      768 2023-12-06 19:18:25.535530 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/enums.py
--rw-r--r--   0        0        0      980 2023-12-06 19:18:25.536037 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/exceptions.py
--rw-r--r--   0        0        0       25 2023-12-06 19:18:25.536563 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/geo/__init__.py
--rw-r--r--   0        0        0     7497 2024-04-08 13:34:03.334470 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/geo/base.py
--rw-r--r--   0        0        0     4002 2024-04-08 13:34:03.334954 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/geo/geo.py
--rw-r--r--   0        0        0      946 2024-04-08 13:34:03.335345 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/legend.py
--rw-r--r--   0        0        0       42 2023-12-06 19:18:25.537462 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/series/__init__.py
--rw-r--r--   0        0        0     4854 2024-04-08 13:34:03.335872 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/series/numeric.py
--rw-r--r--   0        0        0      625 2023-12-06 19:18:25.537878 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/series/series.py
--rw-r--r--   0        0        0     2757 2024-04-08 13:34:03.336758 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/series/styling.py
--rw-r--r--   0        0        0     1419 2024-04-08 13:34:03.337318 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pandas_utils.py
--rw-r--r--   0        0        0      672 2023-12-06 19:18:25.538666 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/__init__.py
--rw-r--r--   0        0        0     2563 2024-04-08 13:34:03.338266 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/chart.py
--rw-r--r--   0        0        0      852 2023-12-06 19:18:25.539041 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/exceptions.py
--rw-r--r--   0        0        0      743 2023-12-06 19:18:25.539250 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/legend.py
--rw-r--r--   0        0        0     6613 2024-04-08 13:34:03.338793 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/pie.py
--rw-r--r--   0        0        0       35 2023-12-06 19:18:25.539759 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/series/__init__.py
--rw-r--r--   0        0        0     6016 2024-04-08 13:34:03.339907 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/series/base.py
--rw-r--r--   0        0        0     3173 2024-04-08 13:34:03.341206 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/series/country.py
--rw-r--r--   0        0        0     3523 2024-04-08 13:34:03.341874 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/series/series.py
--rw-r--r--   0        0        0     3055 2024-04-08 13:34:03.342332 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/series/styling.py
--rw-r--r--   0        0        0      165 2023-12-06 19:18:25.540775 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/series/typings.py
--rw-r--r--   0        0        0     2863 2024-04-08 13:34:03.342718 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/tooltip.py
--rw-r--r--   0        0        0      391 2023-12-06 19:18:25.541255 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/__init__.py
--rw-r--r--   0        0        0     3415 2023-12-06 19:18:25.541430 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/exceptions.py
--rw-r--r--   0        0        0       28 2023-12-06 19:18:25.541674 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/__init__.py
--rw-r--r--   0        0        0     2793 2023-12-06 19:18:25.541895 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/base.py
--rw-r--r--   0        0        0      900 2023-12-06 19:18:25.542078 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/build_result.py
--rw-r--r--   0        0        0     3346 2023-12-06 19:18:25.542288 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/number.py
--rw-r--r--   0        0        0       21 2023-12-06 19:18:25.542540 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/styling/__init__.py
--rw-r--r--   0        0        0     3252 2023-12-06 19:18:25.542703 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py
--rw-r--r--   0        0        0     1420 2023-12-06 19:18:25.542896 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/styling/number.py
--rw-r--r--   0        0        0     1611 2023-12-06 19:18:25.543072 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/styling/text.py
--rw-r--r--   0        0        0     2305 2023-12-06 19:18:25.543227 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/text.py
--rw-r--r--   0        0        0      280 2023-12-06 19:18:25.543426 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/typing.py
--rw-r--r--   0        0        0     7905 2024-04-08 13:34:03.343260 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/search.py
--rw-r--r--   0        0        0       79 2023-12-06 19:18:25.543917 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/select/__init__.py
--rw-r--r--   0        0        0     2135 2023-12-06 19:18:25.544119 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/select/exceptions.py
--rw-r--r--   0        0        0     1783 2023-12-06 19:18:25.544293 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/select/group.py
--rw-r--r--   0        0        0     6261 2024-04-08 13:34:03.344111 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/select/select.py
--rw-r--r--   0        0        0     2453 2023-12-06 19:18:25.544779 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/__init__.py
--rw-r--r--   0        0        0       50 2023-12-06 19:18:25.545080 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/__init__.py
--rw-r--r--   0        0        0       26 2023-12-06 19:18:25.545373 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/__init__.py
--rw-r--r--   0        0        0     6119 2024-04-08 13:34:03.346700 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/base.py
--rw-r--r--   0        0        0     6055 2024-04-08 13:34:03.348319 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/category.py
--rw-r--r--   0        0        0       46 2023-12-06 19:18:25.546142 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/__init__.py
--rw-r--r--   0        0        0     5488 2024-04-08 13:34:03.350942 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py
--rw-r--r--   0        0        0     7027 2023-12-06 19:18:25.546570 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py
--rw-r--r--   0        0        0     5515 2024-04-08 13:34:03.351685 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py
--rw-r--r--   0        0        0     5520 2024-04-08 13:34:03.352213 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py
--rw-r--r--   0        0        0     5184 2024-04-08 13:34:03.354102 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py
--rw-r--r--   0        0        0     4939 2024-04-08 13:34:03.354598 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/country.py
--rw-r--r--   0        0        0     5698 2024-04-08 13:34:03.355466 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py
--rw-r--r--   0        0        0     4011 2023-12-06 19:18:25.547767 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py
--rw-r--r--   0        0        0     5942 2024-04-08 13:34:03.356065 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/number.py
--rw-r--r--   0        0        0     5446 2024-04-08 13:34:03.357116 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/range.py
--rw-r--r--   0        0        0     5251 2024-04-08 13:34:03.357888 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/text.py
--rw-r--r--   0        0        0     3699 2024-04-08 13:34:03.359074 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py
--rw-r--r--   0        0        0       49 2023-12-06 19:18:25.548938 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-08 13:34:03.362308 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/area.py
--rw-r--r--   0        0        0     1538 2024-04-08 13:34:03.362987 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py
--rw-r--r--   0        0        0     5242 2024-04-08 13:34:03.365602 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/base.py
--rw-r--r--   0        0        0     1418 2024-04-08 13:34:03.366977 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py
--rw-r--r--   0        0        0     2328 2024-04-08 13:34:03.369675 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py
--rw-r--r--   0        0        0     1020 2024-04-08 13:34:03.370118 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/column.py
--rw-r--r--   0        0        0     1199 2024-04-08 13:34:03.370512 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py
--rw-r--r--   0        0        0     1176 2024-04-08 13:34:03.370934 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py
--rw-r--r--   0        0        0     1537 2023-12-06 19:18:25.550983 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py
--rw-r--r--   0        0        0     1272 2024-04-08 13:34:03.371400 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/font.py
--rw-r--r--   0        0        0     1119 2024-04-08 13:34:03.371772 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py
--rw-r--r--   0        0        0     1008 2024-04-08 13:34:03.372121 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/line.py
--rw-r--r--   0        0        0     1377 2024-04-08 13:34:03.372486 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/range.py
--rw-r--r--   0        0        0     2602 2024-04-08 13:34:03.372845 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py
--rw-r--r--   0        0        0     1585 2024-04-08 13:34:03.373186 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py
--rw-r--r--   0        0        0     1779 2023-12-06 19:18:25.552392 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py
--rw-r--r--   0        0        0      473 2023-12-06 19:18:25.552577 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/enums.py
--rw-r--r--   0        0        0     5437 2024-04-08 13:34:03.373647 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/exceptions.py
--rw-r--r--   0        0        0     1721 2024-04-08 13:34:03.374091 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/group.py
--rw-r--r--   0        0        0     8996 2024-04-08 13:34:03.374485 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/header.py
--rw-r--r--   0        0        0     2560 2024-04-08 13:34:03.375217 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/initial_state.py
--rw-r--r--   0        0        0     1889 2024-04-08 13:34:03.375669 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/styling.py
--rw-r--r--   0        0        0    15889 2024-04-08 13:34:03.377440 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/table.py
--rw-r--r--   0        0        0     3155 2023-12-06 19:18:25.554676 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/__init__.py
--rw-r--r--   0        0        0       45 2023-12-06 19:18:25.554962 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/__init__.py
--rw-r--r--   0        0        0     1695 2024-04-08 13:34:03.378176 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/base.py
--rw-r--r--   0        0        0      221 2023-12-06 19:18:25.555357 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/x_axis.py
--rw-r--r--   0        0        0       35 2023-12-06 19:18:25.555627 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/__init__.py
--rw-r--r--   0        0        0     4955 2024-04-08 13:34:03.378849 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py
--rw-r--r--   0        0        0      902 2023-12-06 19:18:25.556005 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py
--rw-r--r--   0        0        0     3109 2024-04-08 13:34:03.379237 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py
--rw-r--r--   0        0        0     4225 2024-04-08 13:34:03.379710 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py
--rw-r--r--   0        0        0     8767 2024-04-08 13:34:03.380139 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/chart.py
--rw-r--r--   0        0        0      513 2023-12-06 19:18:25.556957 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/consts.py
--rw-r--r--   0        0        0     1436 2023-12-06 19:18:25.557151 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/enums.py
--rw-r--r--   0        0        0    12557 2024-04-08 13:34:03.381479 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/exceptions.py
--rw-r--r--   0        0        0     1099 2024-04-08 13:34:03.381893 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/legend.py
--rw-r--r--   0        0        0     3065 2024-04-08 13:34:03.382288 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/navigator.py
--rw-r--r--   0        0        0       56 2023-12-06 19:18:25.558035 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/__init__.py
--rw-r--r--   0        0        0     2529 2024-04-08 13:34:03.382765 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py
--rw-r--r--   0        0        0     1051 2023-12-06 19:18:25.558460 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py
--rw-r--r--   0        0        0     5252 2024-04-08 13:34:03.383282 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py
--rw-r--r--   0        0        0     1196 2023-12-06 19:18:25.558907 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py
--rw-r--r--   0        0        0       46 2023-12-06 19:18:25.559162 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/__init__.py
--rw-r--r--   0        0        0     3300 2024-04-08 13:34:03.384079 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/area.py
--rw-r--r--   0        0        0     4388 2024-04-08 13:34:03.384499 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py
--rw-r--r--   0        0        0     8190 2024-04-08 13:34:03.384961 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/base.py
--rw-r--r--   0        0        0     5749 2024-04-08 13:34:03.385372 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py
--rw-r--r--   0        0        0     3322 2024-04-08 13:34:03.385899 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/column.py
--rw-r--r--   0        0        0     4334 2024-04-08 13:34:03.386294 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py
--rw-r--r--   0        0        0     3279 2024-04-08 13:34:03.386640 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/line.py
--rw-r--r--   0        0        0     3289 2024-04-08 13:34:03.387265 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/point.py
--rw-r--r--   0        0        0     3318 2024-04-08 13:34:03.387609 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py
--rw-r--r--   0        0        0      618 2023-12-06 19:18:25.561259 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/typing.py
--rw-r--r--   0        0        0    22466 2024-04-08 13:34:03.389271 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/timeseries.py
--rw-r--r--   0        0        0     1693 2024-04-08 13:34:03.389853 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/transform.py
--rw-r--r--   0        0        0       87 2023-12-06 19:18:25.561968 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/toggle/__init__.py
--rw-r--r--   0        0        0      543 2023-12-06 19:18:25.562137 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/toggle/exceptions.py
--rw-r--r--   0        0        0     4854 2024-04-08 13:34:03.390453 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/toggle/toggle.py
--rw-r--r--   0        0        0     2755 2023-12-06 19:18:25.562535 engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/utils.py
--rw-r--r--   0        0        0       33 2023-12-06 19:18:25.562797 engineai_sdk-0.49.2/engineai/sdk/internal/__init__.py
--rw-r--r--   0        0        0     1050 2024-04-08 13:34:03.390910 engineai_sdk-0.49.2/engineai/sdk/internal/authentication/auth0.py
--rw-r--r--   0        0        0     5939 2024-04-08 13:34:03.391285 engineai_sdk-0.49.2/engineai/sdk/internal/authentication/utils.py
--rw-r--r--   0        0        0      432 2023-12-06 19:18:25.563520 engineai_sdk-0.49.2/engineai/sdk/internal/graphql_dataclasses/__init__.py
--rw-r--r--   0        0        0      348 2023-12-06 19:18:25.563765 engineai_sdk-0.49.2/engineai/sdk/internal/graphql_dataclasses/exceptions.py
--rw-r--r--   0        0        0        0 2023-12-06 19:18:25.563861 engineai_sdk-0.49.2/engineai/sdk/internal/graphql_dataclasses/py.typed
--rw-r--r--   0        0        0     3169 2023-12-06 19:18:25.564074 engineai_sdk-0.49.2/engineai/sdk/internal/graphql_dataclasses/schema.py
--rw-r--r--   0        0        0     6996 2023-12-06 19:18:25.564272 engineai_sdk-0.49.2/engineai/sdk/internal/graphql_dataclasses/types.py
--rw-r--r--   0        0        0      108 2024-04-08 13:34:03.391606 engineai_sdk-0.49.2/engineai/sdk/internal/rubik/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 13:34:03.391696 engineai_sdk-0.49.2/engineai/sdk/internal/rubik/py.typed
--rw-r--r--   0        0        0    14330 2024-04-08 13:34:03.392307 engineai_sdk-0.49.2/engineai/sdk/internal/rubik/rubik.py
--rw-r--r--   0        0        0      207 2024-04-08 13:34:03.392849 engineai_sdk-0.49.2/engineai/sdk/internal/rubik/serialization/__init__.py
--rw-r--r--   0        0        0     6859 2024-04-08 13:34:03.393649 engineai_sdk-0.49.2/engineai/sdk/internal/rubik/serialization/dataframe.py
--rw-r--r--   0        0        0     3021 2024-04-08 13:34:03.393957 engineai_sdk-0.49.2/engineai/sdk/internal/rubik/serialization/json.py
--rw-r--r--   0        0        0     2050 2024-04-08 13:34:03.395049 engineai_sdk-0.49.2/pyproject.toml
--rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 engineai_sdk-0.49.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/LICENSE
+-rw-r--r--   0        0        0      987 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/README.md
+-rw-r--r--   0        0        0      435 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2541 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/commands/app.py
+-rw-r--r--   0        0        0    14446 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/commands/dashboard.py
+-rw-r--r--   0        0        0     1379 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/console.py
+-rw-r--r--   0        0        0     5489 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/generator.py
+-rw-r--r--   0        0        0       42 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/template/content/.env.sample
+-rw-r--r--   0        0        0      911 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/template/content/main.py
+-rw-r--r--   0        0        0     2676 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_dividends.csv
+-rw-r--r--   0        0        0      593 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_earnings.csv
+-rw-r--r--   0        0        0   152608 2024-04-09 13:47:43.227949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_history.csv
+-rw-r--r--   0        0        0     7518 2024-04-09 13:47:43.227949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_info.json
+-rw-r--r--   0        0        0     7217 2024-04-09 13:47:43.227949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AMZN_info.json
+-rw-r--r--   0        0        0   139522 2024-04-09 13:47:43.227949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/GSPC.csv
+-rw-r--r--   0        0        0   135696 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/IXIC.csv
+-rw-r--r--   0        0        0     8115 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_dividends.csv
+-rw-r--r--   0        0        0      581 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_earnings.csv
+-rw-r--r--   0        0        0   152152 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_history.csv
+-rw-r--r--   0        0        0     8122 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_info.json
+-rw-r--r--   0        0        0     5125 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_dividends.csv
+-rw-r--r--   0        0        0      571 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_earnings.csv
+-rw-r--r--   0        0        0   151607 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_history.csv
+-rw-r--r--   0        0        0     8080 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_info.json
+-rw-r--r--   0        0        0     2425 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_dividends.csv
+-rw-r--r--   0        0        0      623 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_earnings.csv
+-rw-r--r--   0        0        0   152489 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_history.csv
+-rw-r--r--   0        0        0     8221 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_info.json
+-rw-r--r--   0        0        0    10363 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/utils.py
+-rw-r--r--   0        0        0       38 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/__init__.py
+-rw-r--r--   0        0        0      121 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/__init__.py
+-rw-r--r--   0        0        0     2181 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/layout.py
+-rw-r--r--   0        0        0      207 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/selectable_widgets.py
+-rw-r--r--   0        0        0      570 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/typing.py
+-rw-r--r--   0        0        0     1600 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/base.py
+-rw-r--r--   0        0        0       96 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/__init__.py
+-rw-r--r--   0        0        0     3574 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/activate_dashboard.py
+-rw-r--r--   0        0        0     7670 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/api.py
+-rw-r--r--   0        0        0     1451 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/exceptions.py
+-rw-r--r--   0        0        0      217 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/__init__.py
+-rw-r--r--   0        0        0      472 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/py.typed
+-rw-r--r--   0        0        0      207 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/serialization/__init__.py
+-rw-r--r--   0        0        0     6861 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py
+-rw-r--r--   0        0        0     3134 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/serialization/json.py
+-rw-r--r--   0        0        0     4618 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/storage.py
+-rw-r--r--   0        0        0      515 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/config.py
+-rw-r--r--   0        0        0      310 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/__init__.py
+-rw-r--r--   0        0        0    13152 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/dashboard.py
+-rw-r--r--   0        0        0      140 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/enums.py
+-rw-r--r--   0        0        0     4691 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/exceptions.py
+-rw-r--r--   0        0        0       27 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/__init__.py
+-rw-r--r--   0        0        0     2417 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/executor_config.py
+-rw-r--r--   0        0        0     8389 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/instance.py
+-rw-r--r--   0        0        0     1231 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/node.py
+-rw-r--r--   0        0        0     2586 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/utils.py
+-rw-r--r--   0        0        0       41 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/__init__.py
+-rw-r--r--   0        0        0     1431 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/dependency.py
+-rw-r--r--   0        0        0     5634 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/page.py
+-rw-r--r--   0        0        0     1909 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/root.py
+-rw-r--r--   0        0        0     2932 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/route.py
+-rw-r--r--   0        0        0      345 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/typings.py
+-rw-r--r--   0        0        0       33 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/version/__init__.py
+-rw-r--r--   0        0        0     5105 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/version/version.py
+-rw-r--r--   0        0        0      185 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/__init__.py
+-rw-r--r--   0        0        0    12893 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/decorator.py
+-rw-r--r--   0        0        0     1822 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/duplicated.py
+-rw-r--r--   0        0        0     1047 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/enums.py
+-rw-r--r--   0        0        0     4676 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/exceptions.py
+-rw-r--r--   0        0        0     1996 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/http.py
+-rw-r--r--   0        0        0     3616 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/io_handler.py
+-rw-r--r--   0        0        0     1306 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/manager/interface.py
+-rw-r--r--   0        0        0     9994 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/manager/manager.py
+-rw-r--r--   0        0        0     2892 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/decorator.py
+-rw-r--r--   0        0        0      441 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/__init__.py
+-rw-r--r--   0        0        0     3521 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/datastore.py
+-rw-r--r--   0        0        0      141 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/http/__init__.py
+-rw-r--r--   0        0        0      966 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/http/header.py
+-rw-r--r--   0        0        0     2555 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/http/http.py
+-rw-r--r--   0        0        0     2026 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/route.py
+-rw-r--r--   0        0        0     2518 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/widget.py
+-rw-r--r--   0        0        0      369 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/enum/__init__.py
+-rw-r--r--   0        0        0      934 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/enum/align.py
+-rw-r--r--   0        0        0      705 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/enum/legend_position.py
+-rw-r--r--   0        0        0     5156 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/exceptions.py
+-rw-r--r--   0        0        0      569 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/__init__.py
+-rw-r--r--   0        0        0     3688 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/axis.py
+-rw-r--r--   0        0        0     1817 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/datetime.py
+-rw-r--r--   0        0        0      661 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/exceptions.py
+-rw-r--r--   0        0        0     1259 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/mapper.py
+-rw-r--r--   0        0        0     5108 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/number.py
+-rw-r--r--   0        0        0     1272 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/text.py
+-rw-r--r--   0        0        0      331 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/typing.py
+-rw-r--r--   0        0        0      985 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/validator.py
+-rw-r--r--   0        0        0     1056 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/interface.py
+-rw-r--r--   0        0        0      825 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/__init__.py
+-rw-r--r--   0        0        0      417 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/build_item.py
+-rw-r--r--   0        0        0       28 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/__init__.py
+-rw-r--r--   0        0        0     5748 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/card.py
+-rw-r--r--   0        0        0     2770 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/chip.py
+-rw-r--r--   0        0        0     1533 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/header.py
+-rw-r--r--   0        0        0       55 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/__init__.py
+-rw-r--r--   0        0        0     2949 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/chip.py
+-rw-r--r--   0        0        0     1806 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/header.py
+-rw-r--r--   0        0        0     6529 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/section.py
+-rw-r--r--   0        0        0     5782 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/column.py
+-rw-r--r--   0        0        0     2679 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/chip.py
+-rw-r--r--   0        0        0     2165 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/header.py
+-rw-r--r--   0        0        0     2385 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/label.py
+-rw-r--r--   0        0        0     4695 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/exceptions.py
+-rw-r--r--   0        0        0       31 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/fluid_row/__init__.py
+-rw-r--r--   0        0        0     5658 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py
+-rw-r--r--   0        0        0     1697 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/fluid_row/items_build.py
+-rw-r--r--   0        0        0     7107 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/grid.py
+-rw-r--r--   0        0        0    10297 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/row.py
+-rw-r--r--   0        0        0       36 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/__init__.py
+-rw-r--r--   0        0        0     7582 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/base.py
+-rw-r--r--   0        0        0     2171 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/exceptions.py
+-rw-r--r--   0        0        0     4295 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/tab.py
+-rw-r--r--   0        0        0      410 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/typings.py
+-rw-r--r--   0        0        0      244 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/__init__.py
+-rw-r--r--   0        0        0     6016 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/abstract.py
+-rw-r--r--   0        0        0     2201 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/route_link.py
+-rw-r--r--   0        0        0     2576 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/template_string_link.py
+-rw-r--r--   0        0        0      202 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/typing.py
+-rw-r--r--   0        0        0     1427 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/url.py
+-rw-r--r--   0        0        0      934 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/widget_dependency.py
+-rw-r--r--   0        0        0     3039 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/widget_field.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/py.typed
+-rw-r--r--   0        0        0     2020 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/selected.py
+-rw-r--r--   0        0        0      100 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/__init__.py
+-rw-r--r--   0        0        0     5773 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/default_specs.py
+-rw-r--r--   0        0        0     6505 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/discrete_map.py
+-rw-r--r--   0        0        0     1690 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/divergent.py
+-rw-r--r--   0        0        0     3576 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/gradient.py
+-rw-r--r--   0        0        0     5791 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/palette.py
+-rw-r--r--   0        0        0      829 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/single.py
+-rw-r--r--   0        0        0      946 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/spec.py
+-rw-r--r--   0        0        0      277 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/typing.py
+-rw-r--r--   0        0        0     3436 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/icons.py
+-rw-r--r--   0        0        0     8298 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/templated_string.py
+-rw-r--r--   0        0        0     3514 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/utils.py
+-rw-r--r--   0        0        0       25 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/__init__.py
+-rw-r--r--   0        0        0     8515 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/base.py
+-rw-r--r--   0        0        0     2647 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/__init__.py
+-rw-r--r--   0        0        0     3566 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/base.py
+-rw-r--r--   0        0        0      365 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/typing.py
+-rw-r--r--   0        0        0     2149 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py
+-rw-r--r--   0        0        0     5237 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py
+-rw-r--r--   0        0        0     4417 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/cartesian.py
+-rw-r--r--   0        0        0     4481 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/chart.py
+-rw-r--r--   0        0        0     1468 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/exceptions.py
+-rw-r--r--   0        0        0      987 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/legend.py
+-rw-r--r--   0        0        0       45 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/__init__.py
+-rw-r--r--   0        0        0     2640 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/area.py
+-rw-r--r--   0        0        0     4026 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py
+-rw-r--r--   0        0        0     7256 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/base.py
+-rw-r--r--   0        0        0     5303 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py
+-rw-r--r--   0        0        0     2660 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/column.py
+-rw-r--r--   0        0        0     2640 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/line.py
+-rw-r--r--   0        0        0     2679 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py
+-rw-r--r--   0        0        0      573 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/typing.py
+-rw-r--r--   0        0        0     4957 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/chart_utils.py
+-rw-r--r--   0        0        0       39 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/__init__.py
+-rw-r--r--   0        0        0     2630 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/base.py
+-rw-r--r--   0        0        0     1475 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py
+-rw-r--r--   0        0        0     1910 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py
+-rw-r--r--   0        0        0       47 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/__init__.py
+-rw-r--r--   0        0        0       56 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/__init__.py
+-rw-r--r--   0        0        0      416 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/__init__.py
+-rw-r--r--   0        0        0      992 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py
+-rw-r--r--   0        0        0     1506 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py
+-rw-r--r--   0        0        0     1506 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py
+-rw-r--r--   0        0        0     1117 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py
+-rw-r--r--   0        0        0     2656 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py
+-rw-r--r--   0        0        0      338 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/typing.py
+-rw-r--r--   0        0        0      151 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/consts.py
+-rw-r--r--   0        0        0     7162 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/exceptions.py
+-rw-r--r--   0        0        0       25 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/__init__.py
+-rw-r--r--   0        0        0     2787 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/base.py
+-rw-r--r--   0        0        0       23 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/__init__.py
+-rw-r--r--   0        0        0      955 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py
+-rw-r--r--   0        0        0     2138 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py
+-rw-r--r--   0        0        0      806 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py
+-rw-r--r--   0        0        0      314 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/typing.py
+-rw-r--r--   0        0        0      696 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py
+-rw-r--r--   0        0        0     1339 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/area.py
+-rw-r--r--   0        0        0     1373 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py
+-rw-r--r--   0        0        0     4041 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/base.py
+-rw-r--r--   0        0        0     3379 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py
+-rw-r--r--   0        0        0     2977 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py
+-rw-r--r--   0        0        0     1334 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/column.py
+-rw-r--r--   0        0        0     1047 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py
+-rw-r--r--   0        0        0     1342 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py
+-rw-r--r--   0        0        0     3471 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/line.py
+-rw-r--r--   0        0        0     1309 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/point.py
+-rw-r--r--   0        0        0     1319 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py
+-rw-r--r--   0        0        0      802 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py
+-rw-r--r--   0        0        0      282 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/toolbar.py
+-rw-r--r--   0        0        0      319 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/__init__.py
+-rw-r--r--   0        0        0     3647 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py
+-rw-r--r--   0        0        0     1292 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py
+-rw-r--r--   0        0        0     1452 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py
+-rw-r--r--   0        0        0      617 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py
+-rw-r--r--   0        0        0     1102 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py
+-rw-r--r--   0        0        0     1335 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py
+-rw-r--r--   0        0        0     1407 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py
+-rw-r--r--   0        0        0      647 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/typing.py
+-rw-r--r--   0        0        0       29 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/__init__.py
+-rw-r--r--   0        0        0     1192 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py
+-rw-r--r--   0        0        0     4758 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/base.py
+-rw-r--r--   0        0        0       35 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/__init__.py
+-rw-r--r--   0        0        0      228 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/area.py
+-rw-r--r--   0        0        0      236 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/column.py
+-rw-r--r--   0        0        0      228 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/line.py
+-rw-r--r--   0        0        0     1184 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py
+-rw-r--r--   0        0        0      379 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/typing.py
+-rw-r--r--   0        0        0      974 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py
+-rw-r--r--   0        0        0       36 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/__init__.py
+-rw-r--r--   0        0        0     1451 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py
+-rw-r--r--   0        0        0      902 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py
+-rw-r--r--   0        0        0      893 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py
+-rw-r--r--   0        0        0      906 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py
+-rw-r--r--   0        0        0     1263 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py
+-rw-r--r--   0        0        0      339 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/typing.py
+-rw-r--r--   0        0        0       34 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/__init__.py
+-rw-r--r--   0        0        0      879 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py
+-rw-r--r--   0        0        0     1388 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py
+-rw-r--r--   0        0        0      943 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py
+-rw-r--r--   0        0        0      903 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py
+-rw-r--r--   0        0        0      331 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/typing.py
+-rw-r--r--   0        0        0     1313 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py
+-rw-r--r--   0        0        0     2014 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py
+-rw-r--r--   0        0        0     2003 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py
+-rw-r--r--   0        0        0      136 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/__init__.py
+-rw-r--r--   0        0        0     2890 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/content.py
+-rw-r--r--   0        0        0     1265 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/exceptions.py
+-rw-r--r--   0        0        0      613 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/item.py
+-rw-r--r--   0        0        0     1431 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/markdown.py
+-rw-r--r--   0        0        0     3756 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/exceptions.py
+-rw-r--r--   0        0        0      350 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/__init__.py
+-rw-r--r--   0        0        0      768 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/enums.py
+-rw-r--r--   0        0        0      980 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/exceptions.py
+-rw-r--r--   0        0        0       25 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/geo/__init__.py
+-rw-r--r--   0        0        0     7581 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/geo/base.py
+-rw-r--r--   0        0        0     4086 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/geo/geo.py
+-rw-r--r--   0        0        0      973 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/legend.py
+-rw-r--r--   0        0        0       42 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/__init__.py
+-rw-r--r--   0        0        0     4882 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/numeric.py
+-rw-r--r--   0        0        0      625 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/series.py
+-rw-r--r--   0        0        0     2785 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/styling.py
+-rw-r--r--   0        0        0     2113 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pandas_utils.py
+-rw-r--r--   0        0        0      672 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/__init__.py
+-rw-r--r--   0        0        0     1952 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/chart.py
+-rw-r--r--   0        0        0      852 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/exceptions.py
+-rw-r--r--   0        0        0      743 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/legend.py
+-rw-r--r--   0        0        0     6161 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/pie.py
+-rw-r--r--   0        0        0       35 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/__init__.py
+-rw-r--r--   0        0        0     6044 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/base.py
+-rw-r--r--   0        0        0     3201 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/country.py
+-rw-r--r--   0        0        0     2932 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/series.py
+-rw-r--r--   0        0        0     3082 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/styling.py
+-rw-r--r--   0        0        0      165 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/typings.py
+-rw-r--r--   0        0        0     2405 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/tooltip.py
+-rw-r--r--   0        0        0      391 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/__init__.py
+-rw-r--r--   0        0        0     3415 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/exceptions.py
+-rw-r--r--   0        0        0       28 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/__init__.py
+-rw-r--r--   0        0        0     2793 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/base.py
+-rw-r--r--   0        0        0      900 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/build_result.py
+-rw-r--r--   0        0        0     3346 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/number.py
+-rw-r--r--   0        0        0       21 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/__init__.py
+-rw-r--r--   0        0        0     3252 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py
+-rw-r--r--   0        0        0     1420 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/number.py
+-rw-r--r--   0        0        0     1611 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/text.py
+-rw-r--r--   0        0        0     2305 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/text.py
+-rw-r--r--   0        0        0      280 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/typing.py
+-rw-r--r--   0        0        0     7989 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/search.py
+-rw-r--r--   0        0        0       79 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/exceptions.py
+-rw-r--r--   0        0        0     1783 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/group.py
+-rw-r--r--   0        0        0     6345 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/select.py
+-rw-r--r--   0        0        0     2453 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/__init__.py
+-rw-r--r--   0        0        0       26 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/__init__.py
+-rw-r--r--   0        0        0     6147 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/base.py
+-rw-r--r--   0        0        0     6083 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/category.py
+-rw-r--r--   0        0        0       46 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/__init__.py
+-rw-r--r--   0        0        0     5516 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py
+-rw-r--r--   0        0        0     6726 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py
+-rw-r--r--   0        0        0     5543 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py
+-rw-r--r--   0        0        0     5548 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py
+-rw-r--r--   0        0        0     5211 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py
+-rw-r--r--   0        0        0     4967 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/country.py
+-rw-r--r--   0        0        0     5726 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py
+-rw-r--r--   0        0        0     4011 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py
+-rw-r--r--   0        0        0     5970 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/number.py
+-rw-r--r--   0        0        0     5474 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/range.py
+-rw-r--r--   0        0        0     5277 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/text.py
+-rw-r--r--   0        0        0     3727 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py
+-rw-r--r--   0        0        0       49 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/area.py
+-rw-r--r--   0        0        0     1565 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py
+-rw-r--r--   0        0        0     5055 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/base.py
+-rw-r--r--   0        0        0     1445 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py
+-rw-r--r--   0        0        0     2355 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py
+-rw-r--r--   0        0        0     1047 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/column.py
+-rw-r--r--   0        0        0     1226 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py
+-rw-r--r--   0        0        0     1203 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py
+-rw-r--r--   0        0        0     1537 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py
+-rw-r--r--   0        0        0     1299 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/font.py
+-rw-r--r--   0        0        0     1146 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py
+-rw-r--r--   0        0        0     1035 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/line.py
+-rw-r--r--   0        0        0     1404 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/range.py
+-rw-r--r--   0        0        0     2629 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py
+-rw-r--r--   0        0        0     1612 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py
+-rw-r--r--   0        0        0     1779 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py
+-rw-r--r--   0        0        0      473 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/enums.py
+-rw-r--r--   0        0        0     5447 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/exceptions.py
+-rw-r--r--   0        0        0     1749 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/group.py
+-rw-r--r--   0        0        0     9024 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/header.py
+-rw-r--r--   0        0        0     2587 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/initial_state.py
+-rw-r--r--   0        0        0     1916 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/styling.py
+-rw-r--r--   0        0        0    17137 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/table.py
+-rw-r--r--   0        0        0     3155 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/__init__.py
+-rw-r--r--   0        0        0     1722 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/base.py
+-rw-r--r--   0        0        0      221 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/x_axis.py
+-rw-r--r--   0        0        0       35 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/__init__.py
+-rw-r--r--   0        0        0     4983 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py
+-rw-r--r--   0        0        0      902 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py
+-rw-r--r--   0        0        0     3137 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py
+-rw-r--r--   0        0        0     4253 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py
+-rw-r--r--   0        0        0     8795 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/chart.py
+-rw-r--r--   0        0        0      513 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/consts.py
+-rw-r--r--   0        0        0     1436 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/enums.py
+-rw-r--r--   0        0        0    12101 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/exceptions.py
+-rw-r--r--   0        0        0     1126 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/legend.py
+-rw-r--r--   0        0        0     3093 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/navigator.py
+-rw-r--r--   0        0        0       56 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/__init__.py
+-rw-r--r--   0        0        0     2557 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py
+-rw-r--r--   0        0        0     1051 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py
+-rw-r--r--   0        0        0     5279 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py
+-rw-r--r--   0        0        0     1196 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py
+-rw-r--r--   0        0        0       46 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/__init__.py
+-rw-r--r--   0        0        0     3328 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/area.py
+-rw-r--r--   0        0        0     4520 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py
+-rw-r--r--   0        0        0     7615 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/base.py
+-rw-r--r--   0        0        0     5777 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py
+-rw-r--r--   0        0        0     3350 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/column.py
+-rw-r--r--   0        0        0     4362 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py
+-rw-r--r--   0        0        0     3307 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/line.py
+-rw-r--r--   0        0        0     3317 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/point.py
+-rw-r--r--   0        0        0     3346 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py
+-rw-r--r--   0        0        0      618 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/typing.py
+-rw-r--r--   0        0        0    22602 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/timeseries.py
+-rw-r--r--   0        0        0     1720 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/transform.py
+-rw-r--r--   0        0        0       87 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/toggle/__init__.py
+-rw-r--r--   0        0        0      543 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/toggle/exceptions.py
+-rw-r--r--   0        0        0     4938 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/toggle/toggle.py
+-rw-r--r--   0        0        0     2755 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/utils.py
+-rw-r--r--   0        0        0       33 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/__init__.py
+-rw-r--r--   0        0        0     1336 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/authentication/auth0.py
+-rw-r--r--   0        0        0     5852 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/authentication/utils.py
+-rw-r--r--   0        0        0       92 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/clients/__init__.py
+-rw-r--r--   0        0        0     5003 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/clients/api.py
+-rw-r--r--   0        0        0     1195 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/clients/exceptions.py
+-rw-r--r--   0        0        0      482 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/exceptions.py
+-rw-r--r--   0        0        0      432 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/py.typed
+-rw-r--r--   0        0        0     3169 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/schema.py
+-rw-r--r--   0        0        0     6996 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/types.py
+-rw-r--r--   0        0        0      319 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/url_config.py
+-rw-r--r--   0        0        0     2049 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/pyproject.toml
+-rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 engineai_sdk-0.83.1/PKG-INFO
```

### Comparing `engineai_sdk-0.49.2/LICENSE` & `engineai_sdk-0.83.1/LICENSE`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/generator.py` & `engineai_sdk-0.83.1/engineai/sdk/cli/generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,54 +10,61 @@
 
 
 class _TemplateGenerator:
     PLACEHOLDER_SLUG = "@dashboard_slug@"
     DIRECTORY_NAME = "content"
     MAIN_FILE = "main%s.py"
 
-    def __init__(self, dashboard_slug: str, tutorial: bool = False) -> None:
-        self.__tutorial = tutorial
+    def __init__(self, dashboard_slug: str, tutorial_data: bool = False) -> None:
+        self.__tutorial_data = tutorial_data
         self._dashboard_slug = dashboard_slug
         self.empty = True
+        self.__is_new_project = False
 
     @property
     def _template_path(self) -> Path:
         return Path(f"{Path(__file__).parent.absolute()}/template")
 
     @property
     def _tutorial_path(self) -> Path:
         return Path(f"{Path(__file__).parent.absolute()}/tutorial_data")
 
     @property
     def _project_path(self) -> Path:
         return Path(Path(os.getcwd()) / f"{self._dashboard_slug}")
 
+    @property
+    def is_new_project(self) -> bool:
+        return self.__is_new_project
+
     def run(self) -> None:
         os.chdir(os.getcwd())
         self.__validate_project()
         self.__add_project()
 
     def __validate_project(self) -> None:
         """Validate current project."""
         if (
-            not self.__tutorial
+            not self.__tutorial_data
             and os.path.exists(self._dashboard_slug)
-            or self.__tutorial
+            or self.__tutorial_data
             and os.path.exists(self._project_path / "data")
         ):
             raise ProjectAlreadyExistsError()
 
     def __add_project(self):
         if not os.path.exists(self._project_path):
             self.__copy_paths()
             self.__update_dashboard_slug()
 
             self.__move_files()
             self.__create_dot_env()
 
+            self.__is_new_project = True
+
         self.__copy_tutorial_files()
 
     def __copy_paths(self) -> None:
         shutil.copytree(
             self._template_path / self.DIRECTORY_NAME,
             Path(os.getcwd()) / self.DIRECTORY_NAME,
         )
@@ -116,29 +123,34 @@
     def __create_dot_env(self) -> None:
         if not os.path.exists(f"{self._dashboard_slug}/.env"):
             os.rename(
                 f"{self._dashboard_slug}/.env.sample", f"{self._dashboard_slug}/.env"
             )
 
     def __copy_tutorial_files(self):
-        if self.__tutorial and not os.path.exists(self._project_path / "data"):
+        if self.__tutorial_data and not os.path.exists(self._project_path / "data"):
             shutil.copytree(
                 self._tutorial_path,
                 self._project_path / "data",
             )
 
 
-def generate_template(dashboard_slug: str, tutorial: bool) -> None:
+def generate_template(dashboard_slug: str, tutorial_data: bool) -> bool:
     """Interface to generate a template for a new dashboard.
 
     Args:
         dashboard_slug (str): Dashboard slug.
-        tutorial (bool): If True, generate a template for a tutorial.
+        tutorial_data (bool): If True, will generate example data.
+
+    Returns:
+        True if it is a new project, False otherwise.
     """
-    _TemplateGenerator(dashboard_slug, tutorial).run()
+    template_generator = _TemplateGenerator(dashboard_slug, tutorial_data)
+    template_generator.run()
+    return template_generator.is_new_project
 
 
 def remove_temporary_files():
     """Method that removes the temporary files created by the cookiecutter."""
     if os.path.isdir(main_folder := os.path.join(os.getcwd(), "content")):
         shutil.rmtree(main_folder)
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/template/content/main.py` & `engineai_sdk-0.83.1/engineai/sdk/cli/template/content/main.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/AAPL_dividends.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_dividends.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/AAPL_earnings.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_earnings.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/AAPL_history.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_history.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/AAPL_info.json` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_info.json`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/AMZN_info.json` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AMZN_info.json`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/GSPC.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/GSPC.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/IXIC.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/IXIC.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JNJ_dividends.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_dividends.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JNJ_earnings.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_earnings.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JNJ_history.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_history.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JNJ_info.json` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_info.json`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JPM_dividends.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_dividends.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JPM_earnings.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_earnings.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JPM_history.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_history.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/JPM_info.json` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_info.json`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/MSFT_dividends.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_dividends.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/MSFT_earnings.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_earnings.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/MSFT_history.csv` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_history.csv`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/tutorial_data/MSFT_info.json` & `engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_info.json`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/cli/utils.py` & `engineai_sdk-0.83.1/engineai/sdk/internal/authentication/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,143 +1,126 @@
 """Auxiliary console methods."""
 import datetime as dt
 import json
 import os
-import runpy
 import sys
 import webbrowser
 from pathlib import Path
 from time import sleep
 from typing import Any
 from typing import Dict
 from typing import Optional
-from typing import Tuple
 from urllib.parse import urlparse
 
 import click
 import dotenv
 import requests
 
 from engineai.sdk.dashboard.config import DASHBOARD_API_URL
-from engineai.sdk.internal.authentication.auth0 import AUTH_CONFIG
 
+from .auth0 import AUTH_CONFIG
+from .auth0 import DEFAULT_URL
 
-def add_token_into_env_file(url: str) -> None:
-    """Method that adds environment variables into the .env file."""
-    if not os.path.isfile(".env"):
-        Path(".env").touch(exist_ok=True)
 
-    dotenv_file = dotenv.find_dotenv(raise_error_if_not_found=True, usecwd=True)
-    dotenv.load_dotenv(dotenv_file, override=True)
-    dotenv.set_key(dotenv_file, "DASHBOARD_API_URL", url)
+class MalformedURLError(Exception):
+    """Exception raised when the URL is malformed."""
+
+
+class URLNotSupportedError(Exception):
+    """Exception raised when the URL is not supported."""
+
+
+def get_auth_config(url) -> Dict[str, str]:
+    """Method that gets the auth config."""
+    return AUTH_CONFIG.get(urlparse(url).netloc, {})
+
 
+def get_url(url: Optional[str] = None) -> str:
+    """Method that validates the URL."""
+    final_url = _get_url_from_variables(url)
 
-def run_env(file_path: Path, skip_data: bool, skip_browser: bool) -> None:
-    """Adds the root directory into the context and runs the python file."""
-    dirpath = os.path.dirname(os.path.abspath(file_path))
-
-    sys.path.insert(0, dirpath)
-    os.environ["SKIP_DATA"] = str(skip_data)
-    os.environ["SKIP_OPEN_DASHBOARD"] = str(skip_browser)
-
-    if file_path.exists():
-        runpy.run_path(
-            file_path.as_posix(),
-            run_name=file_path.as_posix().split("/")[-1].split(".")[0],
+    if not urlparse(final_url).netloc:
+        raise MalformedURLError(
+            f"URL ({final_url}) is malformed. "
+            f"Please use the default url {DEFAULT_URL} or insert a valid one."
         )
-        sys.stdout.write("\nPublishing Dashboard...\n")
-    else:
+    if not bool(get_auth_config(final_url)):
+        raise URLNotSupportedError(
+            f"URL ({final_url}) is not supported. "
+            f"Please use the default url {DEFAULT_URL} or insert a valid one."
+        )
+    return final_url
+
+
+def _get_url_from_variables(url: Optional[str]) -> str:
+    if DASHBOARD_API_URL and url:
         sys.stdout.write(
-            "By default we use `main.py` to publish but was not found in the current "
-            "directory. Please make sure you are in the right directory or use "
-            "`--filename` argument to indicate the new position or filename."
+            f"Using DASHBOARD_API_URL environment variable: "
+            f"{DASHBOARD_API_URL} (ignoring 'url' argument).\n"
         )
 
-    os.environ.pop("SKIP_DATA")
-    os.environ.pop("SKIP_OPEN_DASHBOARD")
-    sys.path.remove(dirpath)
+    return DASHBOARD_API_URL or url or DEFAULT_URL
+
+
+def add_url_into_env_file(url: str) -> None:
+    """Method that adds DASHBOARD_API_URL environment variables into the .env file."""
+    if not os.path.isfile(".env"):
+        Path(".env").touch(exist_ok=True)
+
+    dotenv_file = dotenv.find_dotenv(raise_error_if_not_found=True, usecwd=True)
+    dotenv.load_dotenv(dotenv_file, override=True)
+    dotenv.set_key(dotenv_file, "DASHBOARD_API_URL", url)
+    dotenv.load_dotenv(dotenv_file, override=True)
+    os.environ["DASHBOARD_API_URL"] = url
 
 
 def authenticate(
-    url: Optional[str] = None,
-    force_auth: bool = False,
-    force_token: bool = False,
-) -> Tuple[str, str]:
-    """Method that authenticates to the API to get the necessary publish tokens."""
-    final_url = url or DASHBOARD_API_URL or ""
-    if force_auth:
-        final_url = final_url if final_url != "" else f"https://{list(AUTH_CONFIG)[-1]}"
-    parsed_url = urlparse(final_url)
-    if not parsed_url.netloc:
-        raise ValueError(
-            f"URL ({final_url}) is malformed. Please use the default or insert a "
-            "valid one."
-        )
-    auth_config: Dict[str, str] = AUTH_CONFIG.get(str(parsed_url.netloc), {})
-
-    if not bool(auth_config):
-        raise ValueError(
-            f"URL ({final_url}) is not supported. Please use the default or insert a "
-            "valid one."
-        )
-
-    token = _handle_cli_auth(auth_config, force_token)
-    return final_url, token
-
-
-def _handle_cli_auth(
-    auth_config: Dict[str, str],
-    force_token: bool,
+    url: str,
+    force_authentication: bool = False,
 ) -> str:
-    token_file = _get_token_file_full_path(auth_config)
-    if force_token:
+    """Method that authenticates to the API to get the necessary publish tokens."""
+    auth_config = get_auth_config(url)
+    token_file = _get_token_file_full_path()
+
+    if force_authentication or not _is_current_token_valid(token_file):
         return _get_token(token_file, auth_config, _get_device_auth_code(auth_config))
-    if (
+    else:
+        return str(json.loads(token_file.read_text(encoding="utf-8"))["access_token"])
+
+
+def _is_current_token_valid(token_file) -> bool:
+    return (
         token_file.exists()
         and json.loads(token_file.read_text(encoding="utf-8"))["expires_at"]
         > dt.datetime.now().timestamp()
-    ):
-        token = str(json.loads(token_file.read_text(encoding="utf-8"))["access_token"])
-    else:
-        token = _get_token(token_file, auth_config, _get_device_auth_code(auth_config))
-
-    return token
+    )
 
 
-def _get_token_file_full_path(auth_config: Dict[str, str]) -> Path:
-    return Path(os.path.join(_get_token_directory(), _get_token_filename(auth_config)))
+def _get_token_file_full_path() -> Path:
+    return Path(os.path.join(_get_token_directory(), ".engineai_sdk"))
 
 
 def _get_token_directory() -> str:
     path: str = os.path.expanduser("~")
     path = os.path.join(path, ".engineai")
 
     if not os.path.isdir(path):
         os.mkdir(path)
 
     return path
 
 
-def _get_token_filename(auth_config: Dict[str, str]) -> str:
-    filename = ".engineai_sdk"
-
-    if not auth_config["audience"].endswith("com"):
-        filename = f"{filename}_{auth_config['audience'].split('.')[-1]}"
-
-    return filename
-
-
 def _get_token(
     token_file: Path, auth_config: Dict[str, str], device_info: Dict[str, str]
 ) -> str:
     client_id = auth_config["client_id"]
     device_code_expires_at = dt.datetime.now() + dt.timedelta(
         seconds=float(device_info["expires_in"])
     )
-    click.echo("Waiting for browser authentication ", nl=False)
+    click.echo("Waiting for browser confirmation", nl=False)
     while dt.datetime.now() < device_code_expires_at:
         click.echo(".", nl=False)
         sleep(int(device_info["interval"]))
 
         response = requests.post(
             auth_config["token_url"],
             json={
@@ -192,18 +175,15 @@
         click.echo(
             f"Unexpected status code (status_code={response.status_code}) "
             f"for url: {auth_config['device_code_url']}. "
             f"Response text: {response.text}"
         )
         raise click.Abort
     device_info = response.json()
-
     click.echo(
-        "A web browser has been opened at "
-        f"{device_info['verification_uri_complete']}. "
-        "Please continue the login in the web browser. If the web browser fails to "
-        "open please copy paste the respective url manually. Return here once "
-        "you've logged in."
+        f"Validate the following code in the browser: {device_info['user_code']}\n\n"
+        f"Opening URL at {device_info['verification_uri_complete']} "
+        "(copy if it does not open automatically)\n"
     )
     webbrowser.open(device_info["verification_uri_complete"])
 
     return device_info
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/abstract/layout.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/layout.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/abstract/typing.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/typing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Typing for the dashboard SDK."""
 from typing import Any
 from typing import Dict
 from typing import TypedDict
 
 from typing_extensions import NotRequired
 
-from engineai.sdk.internal.rubik import Rubik
+from engineai.sdk.dashboard.clients.storage import StorageConfig
 
 from .selectable_widgets import AbstractSelectWidget
 
 
 class PrepareParams(TypedDict):
     """Parameters for kwargs in prepare method."""
 
     # General
     dashboard_slug: str
+    storage_type: NotRequired[Any]
     page: NotRequired[Any]
-    storage: NotRequired[Rubik]
+    storage: NotRequired[StorageConfig]
     selectable_widgets: NotRequired[Dict[str, AbstractSelectWidget]]
-    write: NotRequired[bool]
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/abstract/widget_dependencies.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-"""Abstract Widget Dependency."""
+"""Spec for defining dependencies with a widget."""
 from typing import Any
 from typing import Generator
 from typing import Optional
 from typing import Tuple
 
+from engineai.sdk.dashboard.base import DependencyInterface
 from engineai.sdk.dashboard.utils import generate_input
 
-from .interface import DependencyInterface
 
-
-class AbstractWidgetDependency(DependencyInterface):
+class WidgetSelectDependency(DependencyInterface):
     """Specs base for defining the Widget Dependency."""
 
     API_DEPENDENCY_INPUT: Optional[str] = None
+    _INPUT_KEY = "widget"
 
-    def __init__(self, *, dependency_id: str, widget_id: str, path: str):
+    def __init__(self, *, dependency_id: str, widget_id: str, path: str = "selected"):
         """Creates dependency with a widget.
 
         Args:
-            dependency_id (str): id of dependency (to be used in other dependencies)
-            widget_id (str): id of widget to associate dependency with
-            path (str): path for state exposed by widget
+            dependency_id: id of dependency (to be used in other dependencies)
+            widget_id: id of widget to associate dependency with
+            path: path for state exposed by widget
         """
         super().__init__()
         self.__dependency_id = dependency_id
         self.__widget_id = widget_id
         self.__path = path
 
     def __iter__(self) -> Generator[Tuple[str, str], None, None]:
@@ -69,15 +69,12 @@
     def build(self) -> Any:
         """Builds spec for dashboard API.
 
         Returns:
             Any: Input object for Dashboard API
         """
         return generate_input(
-            self.api_dependency_input,
-            widget=generate_input(
-                "WidgetDependencyInput",
-                widgetId=self.__widget_id,
-                path=self.__path,
-                name=self.__dependency_id,
-            ),
+            "WidgetDependencyInput",
+            widgetId=self.__widget_id,
+            path=self.__path,
+            name=self.__dependency_id,
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/clients/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/config.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/config.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/dashboard.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/dashboard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,95 @@
 """Spec for a Dashboard."""
+import enum
 import logging
 import os
 import re
 import sys
-import warnings
-from dataclasses import dataclass
+import webbrowser
 from datetime import datetime
+from pathlib import Path
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 from typing import cast
-from warnings import filterwarnings
+from urllib.parse import urlparse
 
-from beartype import beartype
-from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
 from environs import Env
 
+from engineai.sdk.dashboard.clients.activate_dashboard import ActivateDashboard
+from engineai.sdk.dashboard.clients.storage import StorageConfig
 from engineai.sdk.dashboard.dashboard.typings import DashboardContent
+from engineai.sdk.dashboard.data import StorageType
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
-from engineai.sdk.internal.rubik import Rubik
+from engineai.sdk.internal.url_config import PLATFORM_URL
 
 from ..abstract.typing import PrepareParams
 from ..clients import DashboardAPI
+from ..clients.api import DashboardResponse
 from ..clients.exceptions import APIServerError
 from .enums import DashboardStatus
-from .exceptions import DashboardCreateRunError
 from .exceptions import DashboardDuplicatedPathsError
 from .exceptions import DashboardEmptyContentError
 from .exceptions import DashboardInvalidSlugError
 from .exceptions import DashboardNoDashboardFoundError
 from .exceptions import DashboardSkipDataCannotCreateRunError
-from .exit_handler import ExitHandler
-from .graph import Graph
+from .graph.instance import Graph
 from .page.page import Page
 from .version.version import DashboardVersion
 
-filterwarnings("ignore", category=BeartypeDecorHintPep585DeprecationWarning)
-
-logging.getLogger("azure").setLevel(logging.WARNING)
 logger = logging.getLogger(__name__)
 
 
 env = Env()
 
 
-@dataclass
-class APIResponse:
-    """API response."""
-
-    url: str
-    has_connection_string: bool
-    version: str
-    run: str
+class PublishMode(enum.Enum):
+    """Dashboard Publish Mode.
+
+    Attributes:
+        DEFAULT: Default publish mode. The dashboard does not create new
+            runs and automatically activates the published version.
+        DEV: Development publish mode. The dashboard creates new
+            runs and automatically activates the published version/run.
+        DRAFT: Draft publish mode. The dashboard creates new
+            runs but does not activate the published version/run.
+        LIVE: Live publish mode. The dashboard creates new
+            runs and automatically activates only the published run.
+
+    **Version**: Set using the Dashboard *version* argument.
+
+    **Run**: Automatically set based on the published date.
+    """
+
+    DEFAULT = "default"
+    DEV = "dev"
+    DRAFT = "draft"
+    LIVE = "live"
 
 
 class Dashboard:
     """Dashboard class."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         slug: str = "new_dashboard",
         content: Union[List[Page], DashboardContent],
         app_id: Optional[str] = None,
         name: Optional[str] = None,
         description: Optional[str] = None,
         last_available_data: Optional[Union[datetime, List[str]]] = None,
         status: Optional[DashboardStatus] = None,
         version: Optional[str] = None,
-        create_run: bool = False,
         skip_data: bool = False,
-        activate: bool = True,
-        auto_upgrade: Optional[bool] = None,
+        storage_type: StorageType = StorageType.BLOB,
+        publish_mode: PublishMode = PublishMode.DEFAULT,
     ):
         """Construct for Dashboard class.
 
         Args:
             slug: unique identifier for dashboard.
             content: Dashboard content.
             app_id: App id where the dashboard will be published.
@@ -88,72 +100,65 @@
             description: Dashboard description. Markdown compliant
                 string.
             last_available_data: Last available
                 data for dashboard.
             status: Dashboard status.
             version: Dashboard version. By default, is None, can also be set
                 using environment variable DASHBOARD_VERSION.
-            create_run: create run for dashboard. If true the API will create a run,
-                if false the API will pick the active run, if there isn't one it will
-                be created as none.
             skip_data: skip data processing. If True the publish process will
                 only update the dashboard layout, if False the publish process will
                 update the data and the layout.
-            activate: flag to activate the dashboard after a successful publish.
-            auto_upgrade: auto upgrade dashboard version. If true the API will
-                automatically upgrade the dashboard version to the published version.
+            publish_mode: dashboard publish mode.
+            storage_type: flag to set the storage type for the dashboard.
         """
-        self.__api_client = DashboardAPI()
+        self._api_client = DashboardAPI()
         self.__slug: str = self._set_slug(slug)
         self.__name: str = name or slug.replace("_", " ").title()
         self.__pages = self.__generate_content(content=content)
         self.__skip_data = skip_data or env.bool("SKIP_DATA", False)
-        self.__container_name: str
-        self._set_activate(activate=activate, auto_upgrade=auto_upgrade)
+        self.__publish_mode = publish_mode
+        self.__set_publish_mode()
+        _reset_data_writes()
+        self.__storage_type = storage_type
 
-        if self.__skip_data and create_run:
+        if self.__skip_data and self.__create_run:
             raise DashboardSkipDataCannotCreateRunError()
 
-        if create_run and version is None:
-            raise DashboardCreateRunError()
-
-        self.__version = (
-            DashboardVersion(
-                slug=self.__slug,
-                last_available_data=last_available_data,
-                status=status,
-                version=version,
-                create_run=create_run,
-            )
-            if version
-            else None
+        self.__version: DashboardVersion = DashboardVersion(
+            slug=self.__slug,
+            last_available_data=last_available_data,
+            status=status,
+            version=version,
+            create_run=self.__create_run,
         )
 
         self.__description = description
-        self.__rubik: Optional[Rubik] = None
-        self.__api_connection_string: Optional[str] = None
+        self.__storage_config: Optional[StorageConfig] = None
         self.__skip_open_dashboard = env.bool("SKIP_OPEN_DASHBOARD", True)
         self.__app_id = self._set_app_id(app_id)
         self.__publish()
 
-    def _set_activate(
-        self,
-        activate: bool,
-        auto_upgrade: Optional[bool] = None,
-    ) -> None:
-        if auto_upgrade is not None:
-            warnings.warn(
-                "Dashboard `auto_upgrade`flag is deprecated and it will be removed "
-                "in the next major version. Please use `activate` instead.",
-                DeprecationWarning,
-            )
-
-        self.__activate = (
-            auto_upgrade if auto_upgrade is not None and auto_upgrade else activate
-        )
+    def __set_publish_mode(self) -> None:
+        """Set activate flag."""
+        if self.__publish_mode == PublishMode.DEFAULT:
+            self.__create_run = False
+            self.__activate_version = True
+            self.__activate_run = True
+        elif self.__publish_mode == PublishMode.DEV:
+            self.__create_run = True
+            self.__activate_version = True
+            self.__activate_run = True
+        elif self.__publish_mode == PublishMode.DRAFT:
+            self.__create_run = True
+            self.__activate_version = False
+            self.__activate_run = False
+        else:
+            self.__create_run = True
+            self.__activate_version = False
+            self.__activate_run = True
 
     @staticmethod
     def _set_slug(slug: str) -> str:
         """Set a new dashboard slug."""
         pattern = re.compile("^[a-z0-9-_]+$")
 
         if pattern.search(slug) is None or slug[-1] == "_":
@@ -181,133 +186,173 @@
         else:
             return [Page(name=self.__name, content=cast(DashboardContent, content))]
 
     def __publish(self) -> None:
         self.__validate_dashboard_exists()
         self.__prepare()
         self.__validate_pages()
+        self.__publish_dashboard()
 
-        sys.stdout.write("\nBuilding and sending layout to the API...⏳")
+    def __publish_dashboard(self) -> None:
+        dashboard_response = self._publish_in_api()
+        if dashboard_response is not None:
+            sys.stdout.write("Uploading Data.\n")
+            self.__store_data(dashboard_response=dashboard_response)
+            self.__activate_dashboard(
+                dashboard_response=dashboard_response,
+            )
 
-        self.__set_exit_handler(self.__set_api_variables())
+            self.__finish_publish(dashboard_response=dashboard_response)
 
-    def __set_api_variables(self) -> APIResponse:
-        data, has_connection_string = self.__api_client.add_dashboard(
-            dashboard=self.__build()
+    def __finish_publish(
+        self,
+        dashboard_response: DashboardResponse,
+    ) -> None:
+        """Notify the user when the run ends."""
+        full_url = self.__get_publish_url(dashboard_response=dashboard_response)
+        sys.stdout.write("\n\nDashboard Successfully Published 🚀\n")
+        sys.stdout.write(f"URL: {full_url}\n\n")
+        self.__show_activate_command(dashboard_response=dashboard_response)
+        if not self.__skip_open_dashboard:
+            sys.stdout.write("Opening Dashboard in browser.....\n")
+            webbrowser.open(full_url)
+
+    def __get_publish_url(self, dashboard_response: DashboardResponse) -> str:
+        platform_url = PLATFORM_URL.get(urlparse(self._api_client.url).netloc)
+        url = (
+            f"{platform_url}{dashboard_response.url_path}"
+            if self._api_client.url is not None
+            else None
         )
-        version = data["version"]
-        run = data["run"]
 
-        if has_connection_string:
-            self.__api_connection_string = data["storage"]["blob"]["connectionString"]
-            self.__container_name = (
-                data["storage"]["blob"]["containerName"]
-                + "/"
-                + data["storage"]["blob"]["path"]
+        return (
+            url
+            if self.__publish_mode in [PublishMode.DEFAULT, PublishMode.DEV]
+            else (
+                f"{url}?"
+                f"dashboard-version={dashboard_response.version}&"
+                f"dashboard-version-run={dashboard_response.run}"
             )
-            sys.stdout.write("\nLayout sent successfully ✅\n")
-
-        return APIResponse(
-            url=data["url"],
-            has_connection_string=has_connection_string,
-            version=version,
-            run=run,
         )
 
-    def __set_exit_handler(self, api_response: APIResponse) -> None:
-        with ExitHandler(
-            url=self.__api_client.url,
-            name=self.__name,
-            url_path=api_response.url,
-            skip_open_dashboard=self.__skip_open_dashboard,
-            activate=self.__activate,
-        ):
-            self.__store_data(api_response.has_connection_string)
-            self.__activate_dashboard(
-                version=api_response.version,
-                run=api_response.run,
+    def __show_activate_command(
+        self,
+        dashboard_response: DashboardResponse,
+    ) -> None:
+        """Show the command to activate the dashboard."""
+        if self.__publish_mode in [PublishMode.LIVE, PublishMode.DRAFT]:
+            sys.stdout.write(
+                "Dashboard published without activation. "
+                "To activate please run this command:\n"
+                f"engineai dashboard -s {dashboard_response.dashboard_slug} "
+                f"activate -v {dashboard_response.version} "
+                f"-r {dashboard_response.run}\n\n"
             )
 
+    def _publish_in_api(self) -> Optional[DashboardResponse]:
+        return self._api_client.publish_dashboard(dashboard=self._build().to_dict())
+
     def __validate_pages(self) -> None:
         paths = set()
         for page in self.__pages:
             if page.path not in paths:
                 paths.add(page.path)
             else:
                 raise DashboardDuplicatedPathsError(page.path)
             page.validate()
 
     def __validate_dashboard_exists(self) -> None:
         if self.__skip_data:
             try:
-                self.__api_client.get_dashboard(
+                self._api_client.get_dashboard(
                     dashboard_slug=self.__slug.replace("_", "-"),
                     app_id=self.__app_id,
-                    version=None if self.__version is None else self.__version.version,
+                    version=self.__version.version,
                 )
             except APIServerError as e:
                 raise DashboardNoDashboardFoundError(
                     slug=self.__slug,
                     app_id=self.__app_id,
-                    version=None if self.__version is None else self.__version.version,
+                    version=self.__version.version,
                 ) from e
 
     def __prepare(self) -> None:
         kwargs: PrepareParams = {
             "dashboard_slug": self.__slug,
+            "storage_type": self.__storage_type,
         }
         if self.__version:
             self.__version.prepare(**kwargs)
         for page in self.__pages:
             page.prepare(**kwargs)
 
-    def key_value_storage(self) -> Rubik:
+    def __key_value_config(
+        self, dashboard_response: DashboardResponse
+    ) -> StorageConfig:
         """Returns Dashboard default storage."""
-        if self.__rubik is None:
-            self.__rubik = self.__create_storage_instance()
-        return self.__rubik
-
-    def __create_storage_instance(self) -> Rubik:
-        return Rubik(
-            base_path=self.__container_name,
-            protocol="abfs",
-            storage_options={
-                "connection_string": self.__api_connection_string,
-                "create": False,
+        if self.__storage_config is None:
+            self.__storage_config = self.__create_storage_config(dashboard_response)
+        return self.__storage_config
+
+    def __create_storage_config(
+        self, dashboard_response: DashboardResponse
+    ) -> StorageConfig:
+        url = (
+            self._api_client.url
+            if not self._api_client.url.endswith("/")
+            else self._api_client.url[:-1]
+        )
+
+        return StorageConfig(
+            base_path=f"{url}/data-proxy/"
+            f"app/{dashboard_response.app_id}/"
+            f"dashboard/{dashboard_response.dashboard_slug}/"
+            f"version/{dashboard_response.version}/"
+            f"run/{dashboard_response.run}"
+            f"/datastore/",
+            headers={
+                "Authorization": f"Bearer {self._api_client.token}",
+                "Content-Type": "application/json",
             },
         )
 
-    def __store_data(self, has_connection_string: bool) -> None:
-        if has_connection_string and not self.__skip_data:
+    def __store_data(self, dashboard_response: DashboardResponse) -> None:
+        if not self.__skip_data:
             kwargs: PrepareParams = {
                 "dashboard_slug": self.__slug,
+                "storage": self.__key_value_config(dashboard_response),
+                "storage_type": self.__storage_type,
             }
-            if has_connection_string:
-                kwargs.update({"storage": self.key_value_storage()})
             widgets = []
             routes = []
             for page in self.__pages:
                 routes.append(page.route)
                 widgets.append(page.widgets)
-            sys.stdout.write("\nPreparing to store data..⏳\n")
             Graph(widgets=widgets, routes=routes, **kwargs)
 
-    def __activate_dashboard(self, version: str, run: str) -> None:
-        if self.__activate:
-            self.__api_client.activate_dashboard(
-                dashboard_slug=self.__slug.replace("_", "-"),
-                version=version,
-                run=run,
+    def __activate_dashboard(self, dashboard_response: DashboardResponse) -> None:
+        self._api_client.activate_dashboard(
+            activate_dashboard=ActivateDashboard(
+                dashboard_id=dashboard_response.dashboard_id,
+                version=dashboard_response.version,
+                activate_version=self.__activate_version,
+                run=dashboard_response.run,
+                activate_run=self.__activate_run,
             )
+        )
 
-    def __build(self) -> Any:
+    def _build(self) -> Any:
         """Builds spec for dashboard API."""
         return generate_input(
             "DashboardInput",
             name=self.__name,
             slug=self.__slug.replace("_", "-"),
             description=self.__description,
             version=self.__version.build() if self.__version else None,
-            activate=False,
             pages=[page.build() for page in self.__pages],
             appId=self.__app_id,
         )
+
+
+def _reset_data_writes() -> None:
+    if Path(".storage.txt").exists():
+        Path(".storage.txt").unlink()
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,29 +97,15 @@
 class DashboardSkipDataCannotCreateRunError(EngineAIDashboardError):
     """Exception raised when cannot create run and skip data at the same time."""
 
     def __init__(self, *args: object) -> None:
         """Construct for DashboardSkipDataCannotCreateRunError class."""
         super().__init__(*args)
         self.error_strings.append(
-            "Cannot use skip_data flag when trying to publish a Dashboard with"
-            "create_run active. The create run feature needs to publish new data"
-            "for each run, so the data processing is mandatory."
-        )
-
-
-class DashboardCreateRunError(EngineAIDashboardError):
-    """Exception raised when create_run active and no version."""
-
-    def __init__(self, *args: object) -> None:
-        """Construct for DashboardCreateRunError class."""
-        super().__init__(*args)
-        self.error_strings.append(
-            "Cannot use create_run flag when trying to publish a "
-            "Dashboard setting the version."
+            "To use skip_data flag, you should set the publish mode to DEFAULT."
         )
 
 
 class DashboardDuplicatedPathsError(EngineAIDashboardError):
     """Exception raised when dashboard pages have the same path."""
 
     def __init__(self, duplicated_path: str, *args: object) -> None:
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/exit_handler.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/chip.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,76 @@
-"""Class that manages the Dashboard status updates."""
-import atexit
-import sys
-import webbrowser
+"""Spec for the layout chip component."""
+
 from typing import Any
-from typing import Callable
-from typing import Dict
+from typing import List
 from typing import Optional
-from urllib.parse import urljoin
+from typing import Union
 
-from ..utils import notify
+from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.base import DependencyInterface
+from engineai.sdk.dashboard.decorator import type_check
+from engineai.sdk.dashboard.layout.components.label import build_context_label
+from engineai.sdk.dashboard.links.typing import GenericLink
+from engineai.sdk.dashboard.templated_string import TemplatedStringItem
+from engineai.sdk.dashboard.templated_string import build_templated_strings
+from engineai.sdk.dashboard.utils import generate_input
 
-PLATFORM_URL: Dict[str, str] = {
-    "https://api.engineai.dev": "https://platform.engineai.dev",
-    "https://api.engineai.review": "https://platform.engineai.review",
-    "https://api.engineai.com": "https://platform.engineai.com",
-}
 
+class BaseChip(AbstractFactory):
+    """Spec for the layout chip component.
 
-class ExitHandler:
-    """Class that manages the at exit handlers."""
+    This component is used in Card and CollapsibleSection components.
+    """
 
+    @type_check
     def __init__(
         self,
-        url_path: str,
-        name: str,
-        url: Optional[str],
-        datastores_publishing: bool = False,
-        skip_open_dashboard: bool = True,
-        activate: bool = True,
+        *,
+        label: Union[str, GenericLink],
+        tooltip_text: Optional[List[TemplatedStringItem]] = None,
+        separator: str = "-",
+        prefix: str = "",
+        suffix: str = "",
     ) -> None:
-        """Constructor for exit handlers Class.
+        """Constructor for BaseChip.
 
         Args:
-            url_path: dashboard slug.
-            name: dashboard name.
-            url: dashboard url.
-            datastores_publishing: flag to show the datastores publishing.
-            skip_open_dashboard: flag to skip the open dashboard.
-            activate: flag to activate the dashboard.
+            label: Header label value. Can assume a static label or a single
+                GenericLink.
+            tooltip_text: informational pop up text. Each element of list is displayed
+                as a separate paragraph. Can only use this option if the `label` is
+                set.
+            separator: label separator in case of a List of WidgetLinks
+            prefix: prefix value to use in before each label.
+            suffix: suffix value to use in after each label.
         """
-        self.__url = self.__set_url(url_path, url)
-        self.__dashboard_name = name
-        self.__datastores_publishing = datastores_publishing
-        self.__skip_open_dashboard = skip_open_dashboard
-        self.__activate = activate
-
-    def __set_url(self, url_path: str, url: Optional[str]) -> Optional[str]:
-        """Set the url of the dashboard."""
-        return f"{PLATFORM_URL.get(url)}{url_path}" if url is not None else None
-
-    def __enter__(self) -> "ExitHandler":
-        if self.__datastores_publishing:
-            sys.stdout.write("\nUploading Datastores into Blob..⏳\n")
-        return self
-
-    def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
-        if exc_value is None:
-            register_at_end(
-                show_published_url,
-                self.__url,
-                self.__skip_open_dashboard,
-                self.__activate,
-            )
-        else:
-            atexit.unregister(show_published_url)
-        register_at_end(notify, self.__dashboard_name, self.__url, exc_value)
-
-
-def show_published_url(
-    dashboard_url: Optional[str], skip_open_dashboard: bool, activate: bool
-) -> None:
-    """Notify the user when the run ends."""
-    if (
-        dashboard_url is not None
-        and urljoin(dashboard_url, "/")[:-1] in PLATFORM_URL.values()
-    ):
-        if activate:
-            sys.stdout.write(
-                f"\n✅ Dashboard Successfully Published at: {dashboard_url} ✅\n"
-            )
-            if not skip_open_dashboard:
-                webbrowser.open(dashboard_url)
-        else:
-            sys.stdout.write("\nDashboard Successfully Published but not active.\n")
-
+        super().__init__()
+        self.__tooltip_text = tooltip_text or []
+        self.__label = label
+        self.__separator = separator
+        self.__prefix = prefix
+        self.__suffix = suffix
+
+    @property
+    def dependencies(self) -> List[DependencyInterface]:
+        """Method to generate the dependencies list from the elements of this class."""
+        return [self.__label.dependency] if not isinstance(self.__label, str) else []
 
-def register_at_end(func: Callable[..., Any], *args: object) -> None:
-    """Method that resets the at exit functions.
+    def build(self) -> Any:
+        """Builds spec for dashboard API.
 
-    Args:
-        func (Callable[..., Any]): function that will be updated at exit.
-    """
-    atexit.unregister(func)
-    atexit.register(func, *args)
+        Returns:
+            Input object for Dashboard API
+        """
+        return generate_input(
+            "DashboardGridCardHeaderContextInput",
+            label=build_context_label(
+                label=self.__label,
+                separator=self.__separator,
+                prefix=self.__prefix,
+                suffix=self.__suffix,
+            ),
+            tooltipText=[
+                build_templated_strings(items=tooltip)
+                for tooltip in self.__tooltip_text
+            ],
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/graph.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/instance.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,237 +1,249 @@
 """Specs for Dependencies Graph."""
+import atexit
 import concurrent.futures
-import contextvars
-from threading import Thread
-from typing import Any
+import itertools
+import logging
+import os
+import shutil
 from typing import Dict
 from typing import Iterable
 from typing import List
-from typing import Optional
 from typing import Set
 from typing import Tuple
 from typing import Union
-from typing import cast
 
 import networkx as nx
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.config import TOTAL_WORKERS
+from engineai.sdk.dashboard.data import DataSource
 from engineai.sdk.dashboard.interface import WidgetInterface as Widget
-from engineai.sdk.dashboard.utils import generate_progressbar
+from engineai.sdk.dashboard.links.typing import GenericLink
+from engineai.sdk.dashboard.utils import ProgressBar
 
-from ..abstract.typing import PrepareParams
-from ..data.file_keys_handler import DataKeysReader
-from .page.route import Route
+from ...abstract.typing import PrepareParams
+from ..page.route import Route
+from .executor_config import ThreadExecutor
+from .node import Node
+from .utils import group_data
+from .utils import process_dependencies
+from .utils import store_data_source
 
+logger = logging.getLogger(__name__)
 
-class _ThreadExecutor(concurrent.futures.ThreadPoolExecutor):
-    """Custom ThreadPoolExecutor class that has an exceptions handler."""
 
-    def __init__(self, max_workers: Optional[int] = None):
-        """Initializes a new ThreadPoolExecutor instance.
+class Graph:
+    """Dependencies graph that will be used to manage the store process."""
 
-        Args:
-            max_workers: The maximum number of threads that can be used to
-                execute the given calls.
-        """
-        self.parent_ctx = contextvars.copy_context()
+    def __init__(
+        self,
+        widgets: List[List[Widget]],
+        routes: List[Union[Route, None]],
+        **kwargs: Unpack[PrepareParams],
+    ) -> None:
+        """Constructor for dependencies graph."""
+        self.__instance: nx.Graph = nx.DiGraph()
+        self.__add_nodes(data=group_data(widgets), routes=routes)
+        self.__store_data(**kwargs)
 
-        super().__init__(
-            initializer=self._set_context,
-            max_workers=max_workers,
-            thread_name_prefix="dashboard-factory",
-        )
+    def __add_nodes(
+        self, data: Dict[str, Set[Node]], routes: List[Union[Route, None]]
+    ) -> None:
+        self.__add_route_nodes(routes)
+        self.__add_data_nodes(data)
+        self.__get_metadata()
+
+    def __add_route_nodes(self, routes: List[Union[Route, None]]) -> None:
+        for route in set(filter(lambda x: x is not None, routes)):
+            for data_source in route.data:
+                self.__instance.add_node(
+                    data_source.base_path,
+                    nodes={
+                        (
+                            node := Node(
+                                data_source.base_path,
+                                data_source,
+                            )
+                        )
+                    },
+                    metadata=node.links,
+                    fields=set(),
+                )
 
-    def _set_context(self) -> None:
-        for var, value in self.parent_ctx.items():
-            var.set(value)
+    def __add_data_nodes(self, data: Dict[str, Set[Node]]) -> None:
+        for base_path, nodes in data.items():
+            node = next(iter(nodes))
+            self.__instance.add_node(
+                base_path,
+                nodes=nodes,
+                metadata=set(itertools.chain(*[n.links for n in nodes])),
+                fields=set(),
+            )
+            for element in nodes:
+                self.__add_edges(
+                    element.data_source.args,
+                    base_path,
+                    node.data_source,
+                )
+                self.__add_edges(
+                    element.data_source.component.widget_fields,
+                    base_path,
+                    node.data_source,
+                )
 
-    def custom_shutdown(
+    def __add_edges(
         self,
+        dependencies: Iterable[GenericLink],
+        base_path: str,
+        data_source: DataSource,
     ) -> None:
-        cast(Set[Thread], self._threads).clear()
-
+        for dependency in dependencies:
+            for dep_data_source in dependency.link_component.data:
+                self.__add_data_source_edge(base_path, data_source, dep_data_source)
 
-class Node:
-    """Specs for dependency node."""
+    def __add_data_source_edge(
+        self,
+        base_path: str,
+        data_source: DataSource,
+        dep_data_source: DataSource,
+    ) -> None:
+        self.__exists_in_graph(Node(dep_data_source.base_path, dep_data_source))
+        self.__exists_in_graph(Node(base_path, data_source))
+        self.__instance.add_edge(dep_data_source.base_path, base_path)
+
+    def __exists_in_graph(self, node: Node) -> None:
+        if node.name not in self.__instance.nodes:
+            self.__instance.add_node(
+                node.name, nodes={node}, metadata=node.links, fields=set()
+            )
+        else:
+            self.__instance.nodes[node.name]["nodes"].add(node)
+            self.__instance.nodes[node.name]["metadata"].union(node.links)
 
-    def __init__(self, name: str, component: Union[Widget, Route]) -> None:
-        """Node constructor."""
-        self.name = name
-        self.component = component
-        self.args = {repr(dep) for dep in ([d.args for d in self.component.data])}
+    def __get_metadata(self) -> None:
+        """Gets metadata for each node."""
+        instance_copy = self.__instance.copy()
+        for node in nx.topological_sort(self.__instance):
+            current_node = next(iter(self.__instance.nodes[node]["nodes"]))
+            for successor in self.__instance.successors(node):
+                for link in self.__instance.nodes[successor]["metadata"]:
+                    if current_node.data_source == next(iter(link.link_component.data)):
+                        instance_copy.nodes[node]["fields"].add(link.field)
+        self.__instance = instance_copy
 
-        self.kwargs = {repr(d.kwargs) for d in self.component.data}
+    def __store_data(self, **kwargs: Unpack[PrepareParams]) -> None:
+        """Stores items data."""
+        futures: Dict[str, concurrent.futures.Future] = {}
+        completed: Set[str] = set()
+        instance_copy = self.__instance.copy()
 
-    def __str__(self) -> str:
-        return (
-            f"{self.name}{tuple(self.args) if self.args else ''}"
-            f"{tuple(self.kwargs) if self.kwargs else ''}"
-        )
+        pbar = ProgressBar(len(self.__instance), length=20)
 
-    def __repr__(self) -> str:
-        return (
-            f"{self.name}{tuple(self.args) if self.args else ''}"
-            f"{tuple(self.kwargs) if self.kwargs else ''}"
-        )
+        with ThreadExecutor(max_workers=TOTAL_WORKERS) as executor:
+            while len(completed) != len(self.__instance):
+                if executor.cancelled:
+                    raise executor.cancelled
+                blocked: List[str] = []
+                for node in nx.topological_sort(instance_copy):
+                    if executor.cancelled:
+                        break
+                    pred = self.__instance.predecessors(node)
+                    dependencies, blocked = process_dependencies(
+                        node, pred, blocked, futures
+                    )
 
-    def __hash__(self) -> int:
-        return hash(f"{self.name}_{''.join(self.args)}_{''.join(self.kwargs)}")
+                    if node in blocked:
+                        continue
 
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, Node):
-            return (
-                self.name == other.name
-                and self.args == other.args
-                and self.kwargs == other.kwargs
-            )
-        else:
-            return False
+                    _, not_done = concurrent.futures.wait(
+                        dependencies,
+                        return_when=concurrent.futures.FIRST_COMPLETED,
+                    )
 
+                    if len(not_done) > 0:
+                        blocked.append(node)
+                        continue
+
+                    if executor.cancelled:
+                        break
+
+                    (
+                        completed,
+                        futures,
+                    ) = self.__handle_next_running_node(
+                        node,
+                        completed,
+                        futures,
+                        executor,
+                        pbar,
+                        **kwargs,
+                    )
 
-class Graph:
-    """Dependencies graph that will be used to manage the store process."""
+                instance_copy.remove_nodes_from(completed)
 
-    def __init__(
+    def __handle_next_running_node(
         self,
-        widgets: List[List[Widget]],
-        routes: List[Union[Route, None]],
+        node: str,
+        completed: Set[str],
+        futures: Dict[str, concurrent.futures.Future],
+        executor: ThreadExecutor,
+        pbar: ProgressBar,
         **kwargs: Unpack[PrepareParams],
-    ) -> None:
-        """Constructor for dependencies graph."""
-        self.__instance: nx.DiGraph = nx.DiGraph()
-        self.__add_nodes(widgets=self.__filter_widgets(widgets), routes=routes)
-        self.__start_store_data(**kwargs)
-
-    def __start_store_data(self, **kwargs: Unpack[PrepareParams]) -> None:
-        DataKeysReader.delete()
-        self.__store_data(**kwargs)
-
-    def __filter_widgets(self, widgets: List[List[Widget]]) -> List[Widget]:
-        filter_set = set()
-        result = []
-        for elements in widgets:
-            for widget in elements:
-                key = self.__generate_key(widget)
-                if key not in filter_set:
-                    filter_set.add(key)
-                    result.append(widget)
-        return result
-
-    def __generate_key(self, widget: Widget) -> Optional[str]:
-        data = widget.data
-
-        # return none if is json data
-        if data is None:
-            return None
-
-        base_path = "@".join({d.base_path for d in data})
+    ) -> Tuple[Set[str], Dict[str, concurrent.futures.Future]]:
+        if futures.get(node, None) is None:
+            completed.add(node)
+            future = self.__create_future(
+                executor=executor,
+                node=node,
+                pbar=pbar,
+                **kwargs,
+            )
+            futures[node] = future
 
-        args = (repr(dep) for d in data for dep in d.args)
+        return completed, futures
 
-        kwargs = {repr(d.kwargs) for d in data}
+    def __create_future(
+        self,
+        executor: ThreadExecutor,
+        node: str,
+        pbar: ProgressBar,
+        **kwargs: Unpack[PrepareParams],
+    ) -> concurrent.futures.Future:
+        nodes = self.__instance.nodes[node]["nodes"]
 
-        return f"{base_path}_{args}_{kwargs}"
+        data_sources, write_keys = self.__prepare_future_info(nodes)
 
-    def __add_nodes(
-        self, widgets: List[Widget], routes: List[Union[Route, None]]
-    ) -> None:
-        for route in routes:
-            if route is not None:
-                for element in route.data:
-                    self.__instance.add_node(
-                        Node(
-                            element.base_path,  # type: ignore
-                            route,
-                        )
-                    )
+        future = executor.submit(
+            store_data_source,
+            data_sources=data_sources,
+            storage_config=kwargs["storage"],
+            write_keys=write_keys,
+            metadata=self.__instance.nodes[node]["fields"],
+            storage_type=kwargs["storage_type"],
+        )
+        future.add_done_callback(lambda _: pbar.update())
+        return future
 
-        for element in widgets:
-            data = element.data
-            if data is None:
-                continue
-            base_path = "@".join({d.base_path for d in data})
-            self.__instance.add_node(Node(base_path, element))
-            self.__add_edges(next(iter(data)).args, base_path, element)
-            self.__add_edges(element.widget_fields, base_path, element)
+    def __prepare_future_info(
+        self, nodes: Set[Node]
+    ) -> Tuple[Union[DataSource, Set[DataSource]], bool]:
+        data_sources = (
+            next(iter(nodes)).data_source
+            if len(nodes) == 1
+            else {n.data_source for n in nodes}
+        )
 
-    def __add_edges(
-        self, iterable: Iterable[Any], base_path: str, element: Widget
-    ) -> None:
-        for dep in iterable:
-            for d in dep.link_component.data:
-                self.__instance.add_edge(
-                    Node(d.base_path, dep.link_component),
-                    Node(base_path, element),
-                )
+        graph_key = next(iter(nodes)).name
 
-    def __store_data(self, **kwargs: Unpack[PrepareParams]) -> None:
-        """Stores items data."""
-        futures: Dict[Node, Any] = {}
-        completed: List[Node] = []
-        instance_copy = self.__instance.copy()
-        with _ThreadExecutor(max_workers=TOTAL_WORKERS) as executor:
-            with generate_progressbar(
-                total=len(self.__instance), additional=True
-            ) as pbar:
-                while len(completed) != len(self.__instance):
-                    blocked: List[Node] = []
-                    for node in nx.topological_sort(instance_copy):
-                        pred = self.__instance.predecessors(node)
-                        dependencies, blocked = self.__process_dependencies(
-                            node, pred, blocked, futures
-                        )
+        write_keys = len(self.__instance.out_edges(graph_key)) > 0
 
-                        if node in blocked:
-                            continue
+        return data_sources, write_keys
 
-                        done, not_done = concurrent.futures.wait(
-                            dependencies,
-                            return_when=concurrent.futures.FIRST_COMPLETED,
-                        )
 
-                        self.__handle_exceptions(executor, done)
+def close() -> None:
+    """Close filesystem."""
+    if os.path.exists("graph"):
+        shutil.rmtree("graph")
 
-                        if len(not_done) > 0:
-                            blocked.append(node)
-                            continue
-
-                        completed.append(node)
-                        kwargs.update(
-                            {"write": len(self.__instance.out_edges(node)) > 0}
-                        )
-                        future = executor.submit(node.component.store_data, **kwargs)
-                        future.add_done_callback(lambda _: pbar.update(1))
-                        future.add_done_callback(lambda _: pbar.refresh(nolock=True))
-                        futures[node] = future
-                    instance_copy.remove_nodes_from(completed)
-                self.__handle_exceptions(
-                    executor, concurrent.futures.as_completed(futures.values())
-                )
-                pbar.set_description_str(
-                    "✅ All data stored..✅ ",
-                )
 
-    def __process_dependencies(
-        self,
-        node: Node,
-        pred: Any,
-        blocked: List[Node],
-        futures: Dict[Node, Any],
-    ) -> Tuple[List[Any], List[Node]]:
-        dependencies: List[Any] = []
-        for dependency in pred:
-            if dependency in blocked:
-                blocked.append(node)
-                break
-            dependencies.append(futures[dependency])
-        return dependencies, blocked
-
-    def __handle_exceptions(self, executor: _ThreadExecutor, tasks: Any) -> None:
-        for task in tasks:
-            if task.exception() is not None:
-                try:
-                    task.result()
-                except BaseException as e:
-                    executor.custom_shutdown()
-                    raise e
+atexit.register(close)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/page/dependency.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/dependency.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,56 @@
 """Specs for Dashboard Route Datastore Dependency."""
 
 from typing import Any
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class RouteDatastoreDependency(AbstractFactory):
     """Specs for Dashboard Route Datastore Dependency."""
 
-    @beartype
+    _INPUT_KEY: str = "urlQuery"
+
+    @type_check
     def __init__(
         self,
         *,
         dependency_id: str,
-        path: str,
         query_parameter: str,
     ) -> None:
-        """Construct for DashboardRouteDatastoreDependency class.
+        """Construct for RouteDatastoreDependency class.
 
         Args:
-            dependency_id (str): Dependency ID.
-            path (str): Datastore path.
-            query_parameter (str): query parameter to select the series.
+            dependency_id: Dependency ID.
+            path: Datastore path.
+            query_parameter: query parameter to select the series.
         """
         self.__dependency_id = dependency_id
         self.__query_parameter = query_parameter
-        self.__path = path
-        self.__dashboard_slug: str = ""
 
-    def prepare(self, dashboard_slug: str) -> None:
-        """Prepare route."""
-        self.__dashboard_slug = dashboard_slug
+    @property
+    def input_key(self) -> str:
+        """Input Key."""
+        return self._INPUT_KEY
 
     @property
-    def store_id(self) -> str:
-        """Returns store_id associated with dependency.
+    def dependency_id(self) -> str:
+        """Returns dependency id.
 
         Returns:
-            str: store id
+            str: dependency
         """
-        return self.__dashboard_slug.replace("_", "-")
+        return self.__dependency_id
 
     def build(self) -> Any:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
         return generate_input(
-            "DashboardPageUrlQueryApiDependencyInput",
+            "UrlQueryDependencyInput",
             name=self.__dependency_id,
-            storeId=self.store_id,
-            seriesIdPrefix=self.__path,
-            seriesIdQueryKey=self.__query_parameter,
+            query=self.__query_parameter,
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/page/page.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/page.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 """DashboardPage spec."""
 from typing import Any
 from typing import Final
 from typing import List
 from typing import Optional
+from typing import Union
 
-from beartype import beartype
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.abstract.layout import AbstractLayoutItem
 from engineai.sdk.dashboard.abstract.selectable_widgets import AbstractSelectWidget
 from engineai.sdk.dashboard.abstract.typing import PrepareParams
 from engineai.sdk.dashboard.dashboard.exceptions import (
     DashboardDuplicatedWidgetIdsError,
 )
 from engineai.sdk.dashboard.dashboard.typings import DashboardContent
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.interface import CollapsibleInterface
 from engineai.sdk.dashboard.interface import WidgetInterface as Widget
 from engineai.sdk.dashboard.layout.card.card import Card
 from engineai.sdk.dashboard.layout.grid import Grid
 from engineai.sdk.dashboard.layout.selectable.base import SelectableSection
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 
+from ...base import DependencyInterface
+from ...links import RouteLink
+from .dependency import RouteDatastoreDependency
 from .root import RootGrid
 from .route import Route
 
 ROW_HEIGHT_PIXELS: Final[int] = 100
 
 
 class Page:
     """Dashboard Page spec."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         name: TemplatedStringItem,
         content: DashboardContent,
         route: Optional[Route] = None,
         path: str = "/",
     ):
         """Page class constructor.
 
         Args:
             name: Dashboard name to be displayed. Defaults to slug
                 title case.
             content: Dashboard content.
-            control_bar: Control bar spec.
             route: Specs for Page routing.
             path: page endpoint path.
         """
         self.__name = name
         self.__generate_content(content)
         self.__path = path
         self.__dashboard_slug = ""
@@ -100,15 +103,15 @@
             w.widget_id: w for w in self._items() if isinstance(w, AbstractSelectWidget)
         }
         kwargs["page"] = self
         self.__grid.prepare_heights()
         self.__grid.prepare(**kwargs)
 
         if self.__route is not None:
-            self.__route.prepare(self.__dashboard_slug)
+            self.__route.prepare(**kwargs)
 
     def validate(self) -> None:
         """Validates layout spec."""
         dashboard_widget_ids = [
             w.widget_id for w in self._items() if isinstance(w, Widget)
         ]
 
@@ -126,20 +129,40 @@
             "grid": generate_input(
                 "DashboardPageContentGridInput",
                 rowHeightPixels=ROW_HEIGHT_PIXELS,
                 rootGrid=self.__grid.build(),
             )
         }
 
+    def __build_dependencies(self) -> Any:
+        dependencies = set()
+        if self.__route is not None:
+            for dependency in self.__route.dependency:
+                dependencies.add(dependency)
+
+        if not isinstance(self.__name, (str, RouteLink)):
+            dependencies.add(self.__name.dependency)
+
+        return [self.__build_dependency(dependency) for dependency in dependencies]
+
+    @staticmethod
+    def __build_dependency(
+        dependency: Union[RouteDatastoreDependency, DependencyInterface]
+    ) -> Any:
+        return generate_input(
+            "DashboardPageDependencyUnionInput",
+            **{dependency.input_key: dependency.build()},
+        )
+
     def build(self) -> Any:
         """Builds spec for Dashboard Page."""
         return generate_input(
             "DashboardPageInput",
             path=self.__path,
             name=build_templated_strings(items=self.__name),
             content=self._build_content(),
             selectable=False,
             searchable=False,
             controlBar=None,
             entities=[],
-            **self.__route.build() if self.__route is not None else {},
+            dependencies=self.__build_dependencies(),
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/page/root.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/root.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Spec for a root grid in a dashboard."""
 
 from typing import Any
 from typing import List
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.interface import CollapsibleInterface as CollapsibleSection
 from engineai.sdk.dashboard.layout import FluidRow
 from engineai.sdk.dashboard.layout import Grid
 from engineai.sdk.dashboard.layout import Row
 from engineai.sdk.dashboard.layout.typings import LayoutItem
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class RootGrid(Grid):
     """Spec for a root grid in a dashboard."""
 
-    @beartype
+    @type_check
     def __init__(
         self, *items: Union[LayoutItem, Row, FluidRow, CollapsibleSection]
     ) -> None:
         """Construct dashboard grid.
 
         Args:
             items: items to add to grid. Can be widgets, rows or
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/page/route.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/route.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,83 @@
 """Specs for dashboard Route."""
 from typing import Any
-from typing import Mapping
+from typing import List
+from typing import Union
 
 import pandas as pd
-from beartype import beartype
+from typing_extensions import Unpack
 
+from engineai.sdk.dashboard.abstract.typing import PrepareParams
 from engineai.sdk.dashboard.dashboard.page.dependency import RouteDatastoreDependency
 from engineai.sdk.dashboard.data.manager.manager import DependencyManager
 from engineai.sdk.dashboard.data.manager.manager import RouteDataType
+from engineai.sdk.dashboard.decorator import type_check
+from engineai.sdk.dashboard.interface import DependencyInterface
 from engineai.sdk.dashboard.interface import RouteInterface
 from engineai.sdk.dashboard.links import RouteLink
 from engineai.sdk.dashboard.selected import Selected
 
 
 class _Selected(Selected["Route", RouteLink, "Route"]):
     """Route Selected property configuration."""
 
 
 class Route(DependencyManager, RouteInterface):
     """Specs for dashboard Route."""
 
     _DEPENDENCY_ID = "__ROUTE__"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         data: RouteDataType,
         *,
         query_parameter: str,
     ) -> None:
         """Constructor for dashboard Route.
 
         Args:
-            data (RouteDataType): data for the widget. Can be a
+            data: data for the widget. Can be a
                 pandas dataframe or Storage object if the data is to be retrieved
                 from a storage.
-            query_parameter (str): parameter that will be used to apply url queries.
+            query_parameter: parameter that will be used to apply url queries.
         """
         super().__init__(data=data, base_path="route")
         self.__query_parameter = query_parameter
         self.__dependency: RouteDatastoreDependency = RouteDatastoreDependency(
             query_parameter=query_parameter,
-            path=self._data.base_path + self._data.separator,
-            dependency_id=self.dependency_id,
+            dependency_id=f"{self.dependency_id}{query_parameter}",
         )
         self.selected = _Selected(component=self)
+        self._route_data_dependency: DependencyInterface
 
     @property
     def data_id(self) -> str:
         """Returns data id."""
         return "route"
 
     @property
     def query_parameter(self) -> str:
         """Query parameter."""
         return self.__query_parameter
 
-    def prepare(self, dashboard_slug: str) -> None:
+    def prepare(self, **kwargs: Unpack[PrepareParams]) -> None:
         """Prepare page routing."""
-        self.__dependency.prepare(dashboard_slug=dashboard_slug)
+        self._prepare_dependencies(**kwargs)
+        # Will always be one dependency
+        if not hasattr(self, "_route_data_dependency"):
+            self._route_data_dependency = next(iter(self.dependencies))
+            self._route_data_dependency.prepare(
+                route_dependency_id=self.__dependency.dependency_id
+            )
 
     def validate(self, data: pd.DataFrame, **_: Any) -> None:
         """Page routing has no validations to do."""
 
-    def build(self) -> Mapping[str, Any]:
-        """Builds spec for dashboard API.
-
-        Returns:
-            Input object for Dashboard API
-        """
-        return {"dependency": self.__dependency.build()}
+    @property
+    def dependency(self) -> List[Union[RouteDatastoreDependency, DependencyInterface]]:
+        """Returns dependency."""
+        return [self.__dependency, self._route_data_dependency]
+
+    def build(self) -> Any:
+        """Build Item."""
+        # TODO Need to validate if we can remove this method.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/dashboard/version/version.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/version/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class DashboardVersion(AbstractFactory):
     """Spec for Dashboard version."""
 
     def __init__(
         self,
         slug: str,
-        version: str,
+        version: Optional[str],
         last_available_data: Optional[Union[datetime, List[str]]] = None,
         status: Optional[DashboardStatus] = None,
         create_run: bool = False,
     ) -> None:
         """Construct DashboardVersion Class.
 
         Args:
@@ -46,15 +46,15 @@
             status: optional field that is used to tag
                 the dashboard status.
             create_run: create run for dashboard. If true the API will create a run,
                 if false the API will pick the active run, if there isn't one it will
                 be created as none.
         """
         self.__slug = slug
-        self.__version = self.__set_version(version)
+        self.__version = self.__set_version(version) if version is not None else "none"
         self.__last_available_data = last_available_data
         self.__status = status
         self.__create_run = create_run
 
     @property
     def version(self) -> str:
         """Returns the version of the dashboard."""
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/data/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 """Dashboard Data Error."""
 from typing import List
 from typing import Optional
 
+from engineai.sdk.dashboard.data.manager.interface import StaticDataType
 from engineai.sdk.dashboard.exceptions import EngineAIDashboardError
 from engineai.sdk.dashboard.utils import is_uuid
 
 
 class DataValidationError(EngineAIDashboardError):
     """Dashboard Widget Data Error."""
 
     def __init__(
         self,
+        data: StaticDataType,
         data_id: str,
         class_name: str,
         options: Optional[List[str]],
         error_string: str,
         function_name: Optional[str],
         *args: object,
     ) -> None:
         """Constructor for Dashboard Widget Data Error.
 
         Args:
-            data_id (str): id for component (widget or route).
-            class_name (str): widget type.
-            options (Optional[List[str]]): options for widget.
-            error_string (str): error string.
-            function_name (str): function name.
+            data: data to be validated.
+            data_id: id for component (widget or route).
+            class_name: widget type.
+            options: options for widget.
+            error_string: error string.
+            function_name: function name.
         """
         super().__init__(
-            data_id, class_name, options, error_string, function_name, *args
+            data, data_id, class_name, options, error_string, function_name, *args
         )
         if not is_uuid(data_id):
             message = f"{class_name} with {data_id=}."
         else:
             message = (
                 f"{class_name} error (to track which widget raised "
                 "an error set the widget_id "
@@ -59,20 +62,20 @@
         function_name: Optional[str],
         function_arguments: Optional[List[str]],
         *args: object,
     ) -> None:
         """Constructor for DataProcessError.
 
         Args:
-            data_id (str): id for component.
-            class_name (str): widget type.
-            options (Optional[List[str]]): options for widget.
-            error_string (str): error string.
-            function_name (str): function name.
-            function_arguments (Optional[List[str]]): function arguments.
+            data_id: id for component.
+            class_name: widget type.
+            options: options for widget.
+            error_string: error string.
+            function_name: function name.
+            function_arguments: function arguments.
         """
         super().__init__(
             data_id,
             class_name,
             options,
             error_string,
             function_name,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/data/manager/interface.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/manager/interface.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/data/manager/manager.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/manager/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,38 +2,42 @@
 import re
 from copy import copy
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
+from typing import Type
 from typing import Union
 from typing import cast
 
 import pandas as pd
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.abstract.selectable_widgets import AbstractSelectWidget
 from engineai.sdk.dashboard.abstract.typing import PrepareParams
 from engineai.sdk.dashboard.dependencies import WidgetSelectDependency
 from engineai.sdk.dashboard.links import RouteLink
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.widgets.exceptions import WidgetTemplateStringWidgetNotFound
 
-from ...abstract.interface import DependencyInterface
+from ...base import DependencyInterface
 from ...dependencies.datastore import DashboardStorage
+from ...utils import generate_input
 from ..decorator import DataSource
 from ..decorator import OperationItem
+from ..enums import StorageType
+from ..http import Http
 from .interface import DependencyManagerInterface
 from .interface import StaticDataType
 
-WidgetDataType = Union[DataSource, StaticDataType]
+WidgetDataType = Union[DataSource, StaticDataType, Http]
 
-RouteDataType = Union[DataSource, pd.DataFrame]
+RouteDataType = Union[DataSource, pd.DataFrame, Http]
 
 
 class DependencyManager(AbstractFactoryLinkItemsHandler, DependencyManagerInterface):
     """Class to manage component's data and dependencies."""
 
     def __init__(
         self,
@@ -42,27 +46,38 @@
     ) -> None:
         """Constructor to manage components data.
 
         Args:
             data: data for the widget.
                 Can be a pandas dataframe or a dictionary depending on the widget type,
                 or Storage object if the data is to be retrieved from a storage.
-            base_path: data base path.
+            base_path: data storage base path.
         """
         super().__init__()
         self.__dependencies: Set[DependencyInterface] = set()
         self._data = self.__set_data(data=data, base_path=base_path)
 
+    @property
+    def dependencies(self) -> Set[DependencyInterface]:
+        """Returns dependencies of widget.
+
+        Returns:
+            Set[DependencyInterface]: dependencies of widget
+        """
+        return self.__dependencies
+
     def __set_data(
         self,
-        data: Optional[Union[WidgetDataType, RouteDataType]],
+        data: Optional[Union[WidgetDataType, RouteDataType, Http]],
         base_path: Optional[str] = None,
-    ) -> Optional[DataSource]:
+    ) -> Optional[Union[DataSource, Http]]:
         if data is None:
             return None
+        if isinstance(data, Http):
+            return data
         data = (
             data
             if isinstance(data, DataSource)
             else DataSource(data, base_path=base_path)
         )
         data.component = self
         return data
@@ -76,48 +91,66 @@
         """
         return self.get_data_sources()
 
     def _prepare_dependencies(self, **kwargs: Unpack[PrepareParams]) -> None:
         """Prepares dependencies for widget."""
         page_id = re.sub(r"\W+", "", kwargs["page"].path)
         self.__set_internal_data_field()
-        self.__set_template_links_widgets(
-            **kwargs,
-        )
-        self.__set_storage()
+        self.__set_template_links_widgets(**kwargs)
+        self.__set_storage(**kwargs)
         self.__prepare_template_dependencies()
         self.__prepare_route_dependencies()
         self.__prepare_widget_fields()
         self.__prepare_widget_dependencies(page_id)
+        self.__prepare_http_dependencies()
 
-    def store_data(self, **kwargs: Unpack[PrepareParams]) -> None:
-        """Stores data in widget.
-
-        Args:
-            kwargs (dict): keyword arguments
-        """
+    def store_data(
+        self, write: bool, metadata: Set[str], **kwargs: Unpack[PrepareParams]
+    ) -> None:
+        """Stores data in widget."""
         for data_source in self.get_data_sources():
+            data_source.storage_type = kwargs.get("storage_type", None)
             data_source(
-                storage=kwargs["storage"],
-                write_keys=kwargs["write"],
+                storage_config=kwargs["storage"],
+                write_keys=write,
+                metadata=metadata,
             )
 
     def build_datastore_dependencies(self) -> List[Any]:
         """Build datastore dependencies."""
-        return [dependency.build() for dependency in self.__dependencies]
+        return [
+            self.__build_dependency(dependency) for dependency in self.__dependencies
+        ]
+
+    @staticmethod
+    def __build_dependency(dependency: DependencyInterface) -> Any:
+        return generate_input(
+            "WidgetOwnedDependencyUnionInput",
+            **{dependency.input_key: dependency.build()},
+        )
 
     def __prepare_widget_dependencies(self, page_id: str) -> None:
         for dependency in self.__dependencies:
             if (
                 isinstance(dependency, WidgetSelectDependency)
                 and page_id
                 and not dependency.widget_id.endswith(page_id)
             ):
                 dependency.widget_id = f"{dependency.widget_id}_{page_id}"
 
+    def __prepare_http_dependencies(self) -> None:
+        if isinstance(self._data, Http):
+            http_dependency = self._data.dependency
+            http_dependency.dependency_id = self.dependency_id
+            self.__dependencies.add(http_dependency)
+            if http_dependency.operations is not None:
+                self.__add_operations_dependencies(
+                    operations=http_dependency.operations,
+                )
+
     def __prepare_widget_fields(self) -> None:
         for widget_field in self.get_widget_fields():
             dependency = widget_field.link_component.select_dependency()
             self.__dependencies.add(cast(WidgetSelectDependency, dependency))
 
     def __prepare_template_dependencies(self) -> None:
         for template_link in self.get_template_links():
@@ -164,30 +197,39 @@
                 template_link.component = cast(
                     AbstractSelectWidget,
                     selectable_widgets.get(template_link.widget_id),
                 )
             elif template_link.is_route_link():
                 template_link.component = kwargs["page"].route
 
-    def __set_storage(self) -> None:
+    def __set_storage(self, **kwargs: PrepareParams) -> None:
         """Sets the data storage based on widget dependency id(s)."""
         for data_source in self.get_data_sources():
+            data_source.storage_type = kwargs.get("storage_type", None)
             self.__add_link_dependencies(data_source=data_source)
-            self.__dependencies.add(
-                DashboardStorage(
-                    dependency_id=data_source.component.dependency_id,
-                    series_id=self.__generate_series_id(data_source),
-                    operations=data_source.operations,
-                )
-            )
+            dependency: DashboardStorage = self.__set_dependency(data_source)
+
+            self.__dependencies.add(dependency)
+
             if data_source.operations is not None:
                 self.__add_operations_dependencies(
                     operations=data_source.operations,
                 )
 
+    def __set_dependency(self, data_source: DataSource) -> DashboardStorage:
+        _storage_type: Type[DashboardStorage] = StorageType.get_storage_class(
+            data_source.storage_type.value
+        )
+        dependency = _storage_type(
+            dependency_id=data_source.component.dependency_id,
+            series_id=self.__generate_series_id(data_source),
+            operations=data_source.operations,
+        )
+        return dependency
+
     @staticmethod
     def __generate_series_id(data_source: DataSource) -> str:
         if len(data_source.args) > 0:
             store_id_templates: List[str] = [str(link) for link in data_source.args]
 
             series_id = (
                 store_id_templates[0]
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/dependencies/datastore.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/http/http.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,79 @@
-"""Spec for defining a dependency with a widget."""
-
+"""Spec for defining dependencies with a widget."""
 from typing import Any
-from typing import Generator
 from typing import List
 from typing import Optional
-from typing import Tuple
 
-from engineai.sdk.dashboard.abstract.interface import DependencyInterface
+from engineai.sdk.dashboard.base import DependencyInterface
 from engineai.sdk.dashboard.interface import OperationInterface as OperationItem
+from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 
+from .header import HttpHeader
+
 
-class DashboardStorage(DependencyInterface):
-    """Spec for defining a dependency with a datastore."""
+class HttpDependency(DependencyInterface):
+    """Specs base for defining the Widget Dependency."""
+
+    _INPUT_KEY = "http"
 
     def __init__(
         self,
         *,
-        dependency_id: str,
-        series_id: str,
+        path: TemplatedStringItem,
+        host: str,
+        headers: Optional[List[HttpHeader]] = None,
         operations: Optional[List[OperationItem]] = None,
     ):
-        """Creates dependency with a series in a datastore.
+        """Creates dependency with a widget.
 
         Args:
-            dependency_id: id of dependency (to be used in other dependencies)
-            series_id: id of series in datastore.
-                Defaults to empty string.
-            operations: list of operations to be applied to data.
+            path: path to the data.
+            host: host of the data.
+            headers: headers for the request.
+            operations: operations to be performed on the data.
+
+        Note: Only `application/json` are supported for `Content-Type` header.
         """
         super().__init__()
-        self.__dependency_id = dependency_id
-        self.__series_id = series_id
-        self.__operations = operations or []
-
-    def __iter__(self) -> Generator[Tuple[str, str], None, None]:
-        yield "dependency_id", self.__dependency_id
-        yield "series_id", self.__series_id
-
-    def __hash__(self) -> int:
-        return hash(f"{self.__dependency_id}_{self.__series_id}")
-
-    def __eq__(self, other: Any) -> bool:
-        return (
-            isinstance(other, type(self))
-            and self.__series_id == other.series_id
-            and self.__dependency_id == other.dependency_id
-        )
+        self.__path = path
+        self.__host = host
+        self.__headers = headers
+        self.__operations = operations
+        self.__dependency_id = ""
 
     @property
     def dependency_id(self) -> str:
-        """Returns dependency id.
-
-        Returns:
-            str: dependency
-        """
+        """Return Dependency ID."""
+        if self.__dependency_id == "":
+            raise NotImplementedError("Dependency ID not set.")
         return self.__dependency_id
 
-    @property
-    def series_id(self) -> str:
-        """Returns series id.
+    @dependency_id.setter
+    def dependency_id(self, dependency_id: str) -> None:
+        """Set Dependency ID."""
+        self.__dependency_id = dependency_id
 
-        Returns:
-            str: series id
-        """
-        return self.__series_id
+    @property
+    def operations(self) -> Optional[List[OperationItem]]:
+        """Returns operations to be performed on the data."""
+        return self.__operations
 
     def build(self) -> Any:
         """Builds spec for dashboard API.
 
         Returns:
             Any: Input object for Dashboard API
         """
         return generate_input(
-            "WidgetOwnedDependencyUnionInput",
-            dashboardSelfBlobStore=generate_input(
-                "DashboardStoreSelfBlobDependencyInput",
-                fileName=build_templated_strings(items=self.__series_id),
-                name=self.__dependency_id,
-                operations=[operation.build() for operation in self.__operations],
-            ),
+            "HttpDependencyInput",
+            name=self.dependency_id,
+            path=build_templated_strings(items=self.__path),
+            host=self.__host,
+            headers=[header.build() for header in self.__headers]
+            if self.__headers is not None
+            else None,
+            operations=[operation.build() for operation in self.__operations]
+            if self.__operations is not None
+            else None,
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/dependencies/route.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/route.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """Spec for defining a dependency with a widget."""
 
 from typing import Any
 from typing import Generator
 from typing import Optional
 from typing import Tuple
 
-from engineai.sdk.dashboard.abstract.interface import DependencyInterface
+from engineai.sdk.dashboard.base import DependencyInterface
 from engineai.sdk.dashboard.utils import generate_input
 
 
-class BaseRouteDependency(DependencyInterface):
+class RouteDependency(DependencyInterface):
     """Spec for defining a dependency with a datastore."""
 
     API_DEPENDENCY_INPUT: Optional[str] = None
+    _INPUT_KEY = "dashboardPage"
 
     def __init__(self, *, dependency_id: str, field: str):
         """Creates dependency with a series in a datastore.
 
         Args:
             dependency_id (str): id of dependency (to be used in other dependencies)
             field (str): field ID inside the datastore.
         """
         self.__dependency_id = dependency_id
         self.__field_id = field
-        self.__path: str = ""
 
     def __iter__(self) -> Generator[Tuple[str, str], None, None]:
         yield "field_id", self.__field_id
 
     def __hash__(self) -> int:
         return hash(self.__dependency_id)
 
@@ -42,24 +42,14 @@
         if self.API_DEPENDENCY_INPUT is None:
             raise NotImplementedError(
                 f"Class {self.__class__.__name__}.API_DEPENDENCY_INPUT not defined."
             )
         return self.API_DEPENDENCY_INPUT
 
     @property
-    def path(self) -> str:
-        """Get Datastore Path."""
-        return self.__path
-
-    @path.setter
-    def path(self, path: str) -> None:
-        """Set Datastore Path."""
-        self.__path = path
-
-    @property
     def dependency_id(self) -> str:
         """Get Dependency ID."""
         return self.__dependency_id
 
     @property
     def field_id(self) -> str:
         """Get Field ID."""
@@ -68,31 +58,10 @@
     def build(self) -> Any:
         """Builds spec for dashboard API.
 
         Returns:
             Any: Input object for Dashboard API
         """
         return generate_input(
-            self.api_dependency_input,
-            dashboardPage=generate_input(
-                "DashboardPageVariableDependencyInput",
-                name=self.__dependency_id,
-            ),
+            "DashboardPageVariableDependencyInput",
+            name=self.__dependency_id,
         )
-
-
-class RouteDependency(BaseRouteDependency):
-    """Spec for defining a dependency with a datastore."""
-
-    API_DEPENDENCY_INPUT = "WidgetOwnedDependencyUnionInput"
-
-
-class CardRouteDependency(BaseRouteDependency):
-    """Spec for defining a dependency with a datastore."""
-
-    API_DEPENDENCY_INPUT = "DashboardGridCardDependencyUnionInput"
-
-
-class CollapsibleSectionRouteDependency(CardRouteDependency):
-    """Spec for defining a dependency with a datastore."""
-
-    API_DEPENDENCY_INPUT = "DashboardCollapsibleCardDependencyUnionInput"
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/enum/align.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/enum/align.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/enum/legend_position.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/enum/legend_position.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/__init__.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/axis.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/axis.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/datetime.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/datetime.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/mapper.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/mapper.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/number.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/number.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/text.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/text.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/formatting/validator.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/validator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/__init__.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/card/card.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/card.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """Spec for a Card in a dashboard  grid layout."""
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.abstract.layout import AbstractLayoutItem
 from engineai.sdk.dashboard.abstract.typing import PrepareParams
-from engineai.sdk.dashboard.dependencies.route import CardRouteDependency
-from engineai.sdk.dashboard.dependencies.widget import CardSelectDependency
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.interface import CardInterface
 from engineai.sdk.dashboard.interface import WidgetInterface as Widget
 from engineai.sdk.dashboard.layout.build_item import build_item
 from engineai.sdk.dashboard.layout.exceptions import ElementHeightNotDefinedError
 from engineai.sdk.dashboard.layout.typings import LayoutItem
+from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
 
+from ...base import DependencyInterface
 from .header import CardHeader
 
 
 class Card(CardInterface):
     """Spec for a Card in a dashboard layout."""
 
     _INPUT_KEY = "card"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         content: Union[LayoutItem, List[LayoutItem]],
-        header: Optional[Union[str, CardHeader]] = None,
+        header: Optional[Union[TemplatedStringItem, CardHeader]] = None,
     ) -> None:
         """Construct Card in dashboard layout.
 
         Args:
             content: content within the Card. One of Widget, Card, Grid,
                 SelectableSection.
             header: Header card spec. Defaults to None, i.e. a card without title.
@@ -103,28 +103,23 @@
         """Returns if the Item has custom heights in its inner components."""
         return (
             False
             if isinstance(self.__content, Widget)
             else self.__content.has_custom_heights
         )
 
-    @property
-    def dependencies(
-        self,
-    ) -> List[Union[CardSelectDependency, CardRouteDependency]]:
-        """Returns the Card underlying item."""
-        return self.__header.dependencies
-
-    def _set_header(self, header: Optional[Union[str, CardHeader]]) -> CardHeader:
+    def _set_header(
+        self, header: Optional[Union[TemplatedStringItem, CardHeader]]
+    ) -> CardHeader:
         if header is None:
             return CardHeader()
-        elif isinstance(header, str):
-            return CardHeader(title=header)
-        else:
+        elif isinstance(header, CardHeader):
             return header
+        else:
+            return CardHeader(title=header)
 
     def items(self) -> List[AbstractLayoutItem]:
         """Returns list of grid items that need to be inserted individually."""
         return self.__content.items()
 
     def prepare(self, **kwargs: Unpack[PrepareParams]) -> None:
         """Prepare card.
@@ -137,19 +132,33 @@
     def prepare_heights(self, row_height: Optional[Union[float, int]] = None) -> None:
         """Prepare Selectable Layout heights."""
         if not isinstance(self.__content, Widget):
             self.__content.prepare_heights(row_height=row_height)
 
         self.__height = row_height or self.__content.height
 
+    def __build_dependencies(self) -> List[Any]:
+        """Build dependencies for Card."""
+        dependencies = []
+        for dependency in self.__header.dependencies:
+            dependencies.append(self.__build_dependency(dependency))
+        return dependencies
+
+    @staticmethod
+    def __build_dependency(dependency: DependencyInterface) -> Any:
+        return generate_input(
+            "DashboardGridCardDependencyUnionInput",
+            **{dependency.input_key: dependency.build()},
+        )
+
     def build(self) -> Any:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
         return generate_input(
             "DashboardGridCardInput",
             item=build_item(self.__content),
             header=self.__header.build(),
-            dependencies=[dependency.build() for dependency in self.dependencies],
+            dependencies=self.__build_dependencies(),
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/card/header.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/header.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """Spec for the layout Card Header."""
 
 from typing import Optional
 
-from beartype import beartype
-
-from engineai.sdk.dashboard.dependencies.route import CardRouteDependency
-from engineai.sdk.dashboard.dependencies.widget import CardSelectDependency
+from engineai.sdk.dashboard.decorator import type_check
+from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..components.header import BaseHeader
 from .chip import CardChip
 
 
-class CardHeader(BaseHeader[CardSelectDependency, CardRouteDependency]):
+class CardHeader(BaseHeader):
     """Spec for the layout Card Header."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *chips: CardChip,
-        title: Optional[str] = None,
+        title: Optional[TemplatedStringItem] = None,
     ):
         """Construct Header in card layout.
 
         Args:
             chips: chips to be added to the card header.
             title: Card title.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/collapsible/chip.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/chip.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 """Spec for the layout Collapsible Section Header context."""
 
 from typing import List
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
-from engineai.sdk.dashboard.dependencies.route import CollapsibleSectionRouteDependency
-from engineai.sdk.dashboard.dependencies.widget import (
-    CollapsibleSectionSelectDependency,
-)
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..components.chip import BaseChip
 
 
-class CollapsibleSectionChip(
-    BaseChip[CollapsibleSectionSelectDependency, CollapsibleSectionRouteDependency]
-):
+class CollapsibleSectionChip(BaseChip):
     """Spec for the layout Collapsible Section Header context."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         label: Union[str, GenericLink],
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         prefix: str = "",
         suffix: str = "",
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/collapsible/header.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/header.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 """Spec for the layout Collapsible Section Header."""
 
 from typing import Optional
 
-from beartype import beartype
-
-from engineai.sdk.dashboard.dependencies.route import CollapsibleSectionRouteDependency
-from engineai.sdk.dashboard.dependencies.widget import (
-    CollapsibleSectionSelectDependency,
-)
+from engineai.sdk.dashboard.decorator import type_check
+from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..components.header import BaseHeader
 from .chip import CollapsibleSectionChip
 
 
-class CollapsibleSectionHeader(
-    BaseHeader[CollapsibleSectionSelectDependency, CollapsibleSectionRouteDependency]
-):
+class CollapsibleSectionHeader(BaseHeader):
     """Spec for the layout Collapsible Section Header."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *chips: CollapsibleSectionChip,
-        title: Optional[str] = None,
+        title: Optional[TemplatedStringItem] = None,
     ):
         """Construct Header for Collapsible Section layout.
 
         Args:
             chips: chips to be added to the collapsible section header.
             title: Collapsible Section title.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/collapsible/section.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/section.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 """Spec for a Collapsible Section in a dashboard grid layout."""
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.abstract.layout import AbstractLayoutItem
 from engineai.sdk.dashboard.abstract.typing import PrepareParams
-from engineai.sdk.dashboard.dependencies.route import CollapsibleSectionRouteDependency
-from engineai.sdk.dashboard.dependencies.widget import (
-    CollapsibleSectionSelectDependency,
-)
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.interface import CollapsibleInterface
 from engineai.sdk.dashboard.interface import WidgetInterface as Widget
 from engineai.sdk.dashboard.layout.build_item import build_item
 from engineai.sdk.dashboard.layout.exceptions import ElementHeightNotDefinedError
 from engineai.sdk.dashboard.layout.grid import Grid
 from engineai.sdk.dashboard.layout.typings import LayoutItem
+from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
 
+from ...base import DependencyInterface
 from .header import CollapsibleSectionHeader
 
 
 class CollapsibleSection(CollapsibleInterface):
     """Spec for a Collapsible Section in a dashboard layout."""
 
     _INPUT_KEY = "collapsible"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         content: Union[LayoutItem, List[LayoutItem]],
-        header: Optional[Union[str, CollapsibleSectionHeader]] = None,
+        header: Optional[Union[TemplatedStringItem, CollapsibleSectionHeader]] = None,
         expanded: bool = True,
     ) -> None:
         """Construct Collapsible Section in dashboard layout.
 
         CollapsibleSection is only supported in the root level in each Page.
 
         Args:
@@ -121,32 +119,23 @@
         """Returns if the Item has custom heights in its inner components."""
         return (
             False
             if isinstance(self.__content, Widget)
             else self.__content.has_custom_heights
         )
 
-    @property
-    def dependencies(
-        self,
-    ) -> List[
-        Union[CollapsibleSectionSelectDependency, CollapsibleSectionRouteDependency]
-    ]:
-        """Returns the Section underlying item."""
-        return self.__header.dependencies
-
     def _set_header(
-        self, header: Optional[Union[str, CollapsibleSectionHeader]]
+        self, header: Optional[Union[TemplatedStringItem, CollapsibleSectionHeader]]
     ) -> CollapsibleSectionHeader:
         if header is None:
             return CollapsibleSectionHeader()
-        elif isinstance(header, str):
-            return CollapsibleSectionHeader(title=header)
-        else:
+        elif isinstance(header, CollapsibleSectionHeader):
             return header
+        else:
+            return CollapsibleSectionHeader(title=header)
 
     def items(self) -> List[AbstractLayoutItem]:
         """Returns list of grid items that need to be inserted individually."""
         return self.__content.items()
 
     def prepare(self, **kwargs: Unpack[PrepareParams]) -> None:
         """Prepare Section.
@@ -159,21 +148,35 @@
     def prepare_heights(self, row_height: Optional[Union[float, int]] = None) -> None:
         """Prepare Selectable Layout heights."""
         if not isinstance(self.__content, Widget):
             self.__content.prepare_heights(row_height=row_height)
 
         self.__height = row_height or self.__content.height
 
+    def __build_dependencies(self) -> List[Any]:
+        """Build dependencies for Card."""
+        dependencies = []
+        for dependency in self.__header.dependencies:
+            dependencies.append(self.__build_dependency(dependency))
+        return dependencies
+
+    @staticmethod
+    def __build_dependency(dependency: DependencyInterface) -> Any:
+        return generate_input(
+            "DashboardGridCardDependencyUnionInput",
+            **{dependency.input_key: dependency.build()},
+        )
+
     def build(self) -> Any:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
         return generate_input(
             "DashboardCollapsibleCardInput",
             item=build_item(self.__content),
             height=self.height,
             header=self.__header.build(),
             expanded=self.__expanded,
-            dependencies=[dependency.build() for dependency in self.dependencies],
+            dependencies=self.__build_dependencies(),
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/column.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Spec for a column in a dashboard vertical grid layout."""
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.layout.build_item import build_item
 from engineai.sdk.dashboard.layout.typings import LayoutItem
 
 from ..abstract.layout import AbstractLayoutItem
 from ..abstract.typing import PrepareParams
 from ..utils import generate_input
 from ..widgets.base import Widget
@@ -20,15 +20,15 @@
 from .exceptions import ColumnWrongWidthSizeError
 from .exceptions import ElementHeightNotDefinedError
 
 
 class Column(AbstractFactory):
     """Spec for a column in a dashboard vertical grid layout."""
 
-    @beartype
+    @type_check
     def __init__(self, *, content: LayoutItem, width: Optional[int] = None):
         """Construct column in dashboard vertical grid layout.
 
         Args:
             content: Content that is going to be added inside the column.
             width: Sets the column width, value between 3 and 12. If value is None
                 the width will be set automatically based on the number of columns
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/components/header.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/header.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 """Spec for the layout Header component."""
 
 from typing import Any
-from typing import Generic
 from typing import List
 from typing import Optional
-from typing import Union
-
-from beartype import beartype
 
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.base import DependencyInterface
+from engineai.sdk.dashboard.decorator import type_check
+from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 
 from .chip import BaseChip
-from .chip import RouteDependencyType
-from .chip import SelectDependencyType
 
 
-class BaseHeader(AbstractFactory, Generic[SelectDependencyType, RouteDependencyType]):
+class BaseHeader(AbstractFactory):
     """Spec for the layout Header component.
 
     This component is used in Card and CollapsibleSection components.
     """
 
-    @beartype
+    @type_check
     def __init__(
         self,
-        *chips: BaseChip[SelectDependencyType, RouteDependencyType],
-        title: Optional[str] = None,
+        *chips: BaseChip,
+        title: Optional[TemplatedStringItem] = None,
     ):
         """Construct Header in layout.
 
         Args:
             chips: chips to be added to the header.
             title: Component title.
         """
@@ -42,23 +39,25 @@
     def has_title(self) -> bool:
         """Method to validate if header has title."""
         return self.__title is not None
 
     @property
     def dependencies(
         self,
-    ) -> List[Union[SelectDependencyType, RouteDependencyType]]:
-        """Method to generate the dependencies list from the elements of the class.
-
-        Returns:
-            List[CardSelectDependency]: List of dependencies.
-        """
+    ) -> List[DependencyInterface]:
+        """Method to generate the dependencies list from the elements of the class."""
         dependencies_list = []
         for chip in self.__chips:
             dependencies_list.extend(chip.dependencies)
+
+        if self.__title is not None and not isinstance(self.__title, str):
+            if isinstance(self.__title, list):
+                dependencies_list.extend([title.dependency for title in self.__title])
+            else:
+                dependencies_list.extend([self.__title.dependency])
         return dependencies_list
 
     def build(self) -> Any:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/components/label.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/label.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Spec Card Context Labels."""
 
 import warnings
 from typing import Any
 from typing import Iterable
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import RouteLink
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.widget_dependency import WidgetDependencyValue
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 
 
-@beartype
+@type_check
 def build_context_label(
     *,
     label: TemplatedStringItem,
     separator: str = "-",
     prefix: str = "",
     suffix: str = "",
 ) -> Any:
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/fluid_row/items_build.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/fluid_row/items_build.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/grid.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Spec for a grid in a dashboard vertical grid layout."""
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
 from typing_extensions import Unpack
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.layout.typings import LayoutItem
 
 from ..abstract.layout import AbstractLayoutItem
 from ..abstract.typing import PrepareParams
 from ..interface import GridInterface
 from ..utils import generate_input
 from .exceptions import ElementHeightNotDefinedError
@@ -20,15 +20,15 @@
 
 
 class Grid(GridInterface):
     """Spec for a grid in a dashboard vertical grid layout."""
 
     _INPUT_KEY = "grid"
 
-    @beartype
+    @type_check
     def __init__(self, *items: Union[LayoutItem, Row, FluidRow]) -> None:
         """Construct dashboard grid.
 
         Args:
             items: items to add to grid. Can be widgets, rows or
                 selectable sections (e.g tabs).
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/row.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Spec for a row in a dashboard vertical grid layout."""
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 
 from ..abstract.layout import AbstractLayoutItem
 from ..abstract.typing import PrepareParams
 from ..utils import generate_input
 from .column import Column
 from .exceptions import ElementHeightNotDefinedError
 from .exceptions import RowColumnsAutoWidthError
@@ -25,15 +25,15 @@
 from .exceptions import RowsHeightsSetMultipleLevelsError
 from .typings import LayoutItem
 
 
 class Row(AbstractFactory):
     """Spec for a row in a dashboard vertical grid layout."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *items: Union[LayoutItem, Column],
         height: Optional[Union[float, int]] = None,
     ) -> None:
         """Construct row in dashboard vertical grid layout.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/selectable/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from abc import abstractmethod
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Union
 
-from beartype import beartype
 from typing_extensions import Unpack
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.interface import SelectableInterface
 from engineai.sdk.dashboard.interface import WidgetInterface as Widget
 from engineai.sdk.dashboard.layout.typings import LayoutItem
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ...abstract.layout import AbstractLayoutItem
 from ...abstract.typing import PrepareParams
@@ -25,15 +25,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class SelectableItem(AbstractLayoutItem):
     """Spec for item for a selectable section in a dashboard vertical grid layout."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         label: TemplatedStringItem,
         content: Union[LayoutItem, List[LayoutItem]],
         default_selected: bool = False,
     ) -> None:
@@ -127,15 +127,15 @@
 
 class SelectableSection(SelectableInterface):
     """Spec for section in a dashboard vertical grid layout."""
 
     _API_TYPE: Optional[str] = None
     _HEIGHT_TITLE = 0.48
 
-    @beartype
+    @type_check
     def __init__(
         self,
     ) -> None:
         """Construct Selectable Section for dashboard vertical grid layout."""
         super().__init__()
         self._items: List[SelectableItem] = []
         self.__item_labels: Set[TemplatedStringItem] = set()
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/selectable/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/layout/selectable/tab.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/tab.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 """Specs for Tab and TabSection."""
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.layout.build_item import build_item
 from engineai.sdk.dashboard.layout.typings import LayoutItem
 from engineai.sdk.dashboard.links.widget_field import WidgetField
 from engineai.sdk.dashboard.styling.icons import Icons
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
+from engineai.sdk.dashboard.utils import is_valid_url
 
 from .base import SelectableItem
 from .base import SelectableSection
 
 
 class Tab(SelectableItem):
     """Specs for tab in a tab section."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         label: TemplatedStringItem,
         content: Union[LayoutItem, List[LayoutItem]],
-        icon: Optional[Union[Icons, WidgetField]] = None,
+        icon: Optional[Union[Icons, WidgetField, str]] = None,
         default_selected: bool = False,
     ):
         """Construct tab for tab section dashboard vertical grid layout.
 
         Args:
             label: label to be displayed in tab.
             content: item to be added in tab.
             icon: tab icon.
             default_selected: set tab as default selected.
         """
         super().__init__(
             label=label, content=content, default_selected=default_selected
         )
+        self.validate_icon(icon)
         self.__icon = icon
 
+    def validate_icon(self, icon: Optional[Union[Icons, WidgetField, str]]) -> None:
+        """Check if the icon is valid."""
+        if icon is not None:
+            if isinstance(icon, str):
+                is_valid_url(icon)
+
     def build(self) -> Any:
         """Method implemented by all factories to generate Input spec."""
         return generate_input(
             "DashboardGridTabSectionOptionInput",
             label=build_templated_strings(items=self.label),
             item=build_item(self.item),
             icon=build_templated_strings(
@@ -63,15 +70,15 @@
 
 class TabSection(SelectableSection):
     """Spec for tab section in the layout."""
 
     _API_TYPE = "tabSection"
     _INPUT_KEY = "tabSection"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *tabs: Tab,
     ):
         """Construct for TabSection class.
 
         Args:
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/links/abstract.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/links/abstract.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/links/route_link.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/links/route_link.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Specs for DashboardRouteLink."""
 from typing import Any
 from typing import Generator
 from typing import Optional
 from typing import Tuple
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractLink
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.dependencies import RouteDependency
 from engineai.sdk.dashboard.interface import RouteInterface as Route
 
 
 class RouteLink(AbstractLink):
     """Establish a link to the route and the widget or layout item."""
 
     __dependency: Optional[RouteDependency] = None
 
-    @beartype
+    @type_check
     def __init__(self, route: Route, field: str):
         """Construct for DashboardRouteLink class."""
         self.__field = field
         self.__route = route
 
     def __eq__(self, other: Any) -> bool:
         """Return True if other is equal to self."""
@@ -30,14 +29,17 @@
 
     def __iter__(self) -> Generator[Tuple[str, str], None, None]:
         yield "field", self.__field
 
     def __hash__(self) -> int:
         return hash(tuple(self))
 
+    def __repr__(self) -> str:
+        return f"R_{next(iter(self.__route.data)).base_path}:{self.__field}"
+
     @property
     def field(self) -> str:
         """Returns id of field to be used from selectable widget.
 
         Returns:
             str: field id from selectable widget
         """
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/links/template_string_link.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/links/template_string_link.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/links/widget_dependency.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/links/widget_dependency.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/links/widget_field.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/links/widget_field.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 """Specs for WidgetField."""
 from typing import Any
 from typing import Generator
 from typing import Tuple
 
 import pandas as pd
-from beartype import beartype
 
 from engineai.sdk.dashboard.abstract.selectable_widgets import AbstractSelectWidget
-from engineai.sdk.dashboard.abstract.widget_dependencies import AbstractWidgetDependency
 from engineai.sdk.dashboard.base import AbstractLink
+from engineai.sdk.dashboard.decorator import type_check
+from engineai.sdk.dashboard.dependencies import WidgetSelectDependency
 
 
 class WidgetField(AbstractLink):
     """Establish a link to a selectable widget.
 
     Used in indirect dependencies and text fields that are linked to a other widgets.
     """
 
-    @beartype
+    @type_check
     def __init__(self, *, widget: AbstractSelectWidget, field: str):
         """Construct link to a selectable widget.
 
         Args:
             widget (SelectableWidget): selectable widget to establish link
             field (str): field from selectable widget
         """
         self.__widget = widget
         self.__field = field
 
     def __repr__(self) -> str:
-        return f"{next(iter(self.__widget.data)).base_path}:{self.__field}"
+        ds = self.__widget.data
+
+        if len(ds) > 0:
+            return f"WF_{next(iter(ds)).base_path}:{self.__field}"
+
+        return f"WF_http:{self.__field}"
 
     @property
     def item_id(self) -> str:
         """Returns Item Id."""
         return f"WF_{self.__widget.widget_id}_{self.__field}"
 
     def __iter__(self) -> Generator[Tuple[str, str], None, None]:
@@ -48,15 +53,15 @@
 
     def validate(self, storage: Any, data: pd.DataFrame, data_column_name: str) -> None:
         """Validates if field used in link is exposed by widget.
 
         For instance if field is an id of one of the columns in a table
 
         Args:
-            storage (Any): Rubik storage,
+            storage (Any): storage spec.
             data (DataFrame): pandas DataFrame where the data is present.
             data_column_name (str): name of the column where the data is present.
         """
 
     @property
     def link_component(self) -> Any:
         """Returns selectable widget.
@@ -72,15 +77,15 @@
 
         Returns:
             str: field id from selectable widget
         """
         return self.__field
 
     @property
-    def dependency(self) -> AbstractWidgetDependency:
+    def dependency(self) -> WidgetSelectDependency:
         """Return Dependency."""
         return self.__widget.select_dependency()
 
     def _generate_templated_string(self, *, selection: int = 0) -> str:
         """Generates template string to be used in dependency.
 
         Args:
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/selected.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/selected.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/__init__.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/discrete_map.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/discrete_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Spec for Discrete color map."""
 
 from typing import Any
 from typing import List
 from typing import Protocol
 from typing import Union
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 from .palette import Palette
 from .single import Single
 
 
 class DiscreteMapIntervalItem(AbstractFactory):
     """Spec to create a color discrete map item with a value connected to a color."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         min_value: Union[float, int],
         max_value: Union[float, int],
         color: Union[Palette, Single],
         exclude_min: bool = False,
@@ -59,15 +58,15 @@
             excludeMin=self.__exclude_min,
         )
 
 
 class DiscreteMapValueItem(AbstractFactory):
     """Helper to create a color discrete map item with a value connected to a color."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         value: Union[float, int],
         color: Union[Palette, Single],
     ):
         """Construct spec to map a single value to a specific color.
 
@@ -93,15 +92,15 @@
 
 DiscreteMapItem = Union[DiscreteMapIntervalItem, DiscreteMapValueItem]
 
 
 class DiscreteMap(AbstractFactory):
     """Spec to create a discrete map of colors."""
 
-    @beartype
+    @type_check
     def __init__(self, *items: DiscreteMapItem):
         """Builds spec for a discrete map of colors.
 
         Args:
             items: list of values, intervals composing the
                 color map (DiscreteMapIntervalItem or DiscreteMapValueItem)
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/divergent.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/divergent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Spec for Color Divergent class."""
 
 from typing import Any
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.palette import Palette
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.utils import generate_input
 
 from .single import Single
 
 
 class Divergent(AbstractFactory):
     """Creates a class for a Color Divergent."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         mid_value: int,
         mid_color: Palette,
         above_color: ColorSpec,
         below_color: ColorSpec,
     ) -> None:
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/gradient.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/gradient.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec for Gradients."""
 
 from typing import Any
 from typing import Union
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.palette import Palette
 from engineai.sdk.dashboard.utils import generate_input
 
 from .single import Single
 
 
 class GradientItem(AbstractFactory):
     """Item of a color gradient."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         value: Union[float, int],
         color: Union[Palette, Single],
     ):
         """Item of a Color Gradient.
@@ -43,15 +42,15 @@
             "GradientItemInput", color=self.__color.build(), value=self.__value
         )
 
 
 class Gradient(AbstractFactory):
     """Gradient of transition between colors."""
 
-    @beartype
+    @type_check
     def __init__(self, *items: GradientItem, steps: int = 10):
         """Color Gradient spec.
 
         This class is used to create a gradient of colors using
 
         Args:
             items: map between color and intervals.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/palette.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/palette.py`

 * *Files 18% similar despite different names*

```diff
@@ -78,14 +78,28 @@
 
     TRAFFIC_RED = "#B54853"
     TRAFFIC_YELLOW = "#F0D582"
     TRAFFIC_GREEN = "#4C8056"
 
     LIGHTER_GREY = "#EEEEEE"
 
+    # all positive sequential
+    BLUE_POSITIVE_0 = "#D5E8F6"
+    BLUE_POSITIVE_1 = "#96C6E9"
+    BLUE_POSITIVE_2 = "#6CAFE0"
+    BLUE_POSITIVE_3 = "#2D8DD2"
+    BLUE_POSITIVE_4 = "#2574AD"
+
+    # all negative sequential
+    RED_NEGATIVE_0 = "#F3D7D7"
+    RED_NEGATIVE_1 = "#E8B0B0"
+    RED_NEGATIVE_2 = "#DD8888"
+    RED_NEGATIVE_3 = "#D26060"
+    RED_NEGATIVE_4 = "#C83C3C"
+
     @property
     def color(self) -> str:
         """Returns color without transparency.
 
         Returns:
             str: hex color
         """
@@ -127,14 +141,34 @@
     PEACOCK_GREEN = Palette.PEACOCK_GREEN.value
     LAGOON_GREEN = Palette.LAGOON_GREEN.value
     MINT_GREEN = Palette.MINT_GREEN.value
     AQUA_GREEN = Palette.AQUA_GREEN.value
     FROST_GREEN = Palette.FROST_GREEN.value
 
 
+class PercentageAllPositiveSequentialPalette(enum.Enum):
+    """All Positive Sequential Palette."""
+
+    POSITIVE_0 = Palette.BLUE_POSITIVE_0.value
+    POSITIVE_1 = Palette.BLUE_POSITIVE_1.value
+    POSITIVE_2 = Palette.BLUE_POSITIVE_2.value
+    POSITIVE_3 = Palette.BLUE_POSITIVE_3.value
+    POSITIVE_4 = Palette.BLUE_POSITIVE_4.value
+
+
+class PercentageAllNegativeSequentialPalette(enum.Enum):
+    """All Negative Sequential Palette."""
+
+    NEGATIVE_0 = Palette.RED_NEGATIVE_0.value
+    NEGATIVE_1 = Palette.RED_NEGATIVE_1.value
+    NEGATIVE_2 = Palette.RED_NEGATIVE_2.value
+    NEGATIVE_3 = Palette.RED_NEGATIVE_3.value
+    NEGATIVE_4 = Palette.RED_NEGATIVE_4.value
+
+
 def qualitative_palette(*, index: int) -> Palette:
     """Returns color of qualitative palette given index.
 
     Args:
         index: index of qualitative palette (e.g. index of series of a
             timeseries chart)
 
@@ -142,28 +176,30 @@
         Palette: returns corresponding color of qualitative palette
     """
     colors = list(QualitativePalette.__members__.values())
 
     return Palette(colors[index % len(colors)].value)
 
 
-def sequential_palette(*, index: int, n_series: Optional[int] = None) -> Palette:
+def sequential_palette(
+    *, index: int, n_series: Optional[int] = None, palette: Any = SequentialPalette
+) -> Palette:
     """Returns color of sequential palette given index.
 
     Args:
         index: index of sequential palette (e.g. index of series of a
             timeseries chart)
         n_series: total number of series used for sequential palette.
             Determines sub-versions of sequential palette to improve contrast.
             Defaults to None, i.e. uses entire palette.
+        palette: enum of sequential palettes to use.
 
     Returns:
         Palette: returns corresponding color of sequential palette
     """
-    palette: Any = SequentialPalette
     colors: Any = list(palette.__members__.values())
     if n_series:
         if n_series <= 2:
             palette = SequentialPaletteTwoSeries
         elif n_series == 3:
             palette = SequentialPaletteThreeSeries
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/single.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/single.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Spec for SingleColor class."""
 
 from typing import Any
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 from .palette import Palette
 
 
 class Single(AbstractFactory):
     """Creates a class for a single color."""
 
-    @beartype
+    @type_check
     def __init__(self, color: Palette):
         """Construct method for ColorSingle class.
 
         Args:
             color: a color from Palette.
         """
         super().__init__()
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/color/spec.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/spec.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/styling/icons.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/icons.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/templated_string.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/templated_string.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 """Base spec shared by all widgets."""
 import re
 from abc import abstractmethod
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
-from warnings import filterwarnings
 
 import pandas as pd
-from beartype import beartype
-from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.abstract.typing import PrepareParams
 from engineai.sdk.dashboard.data.manager.manager import DependencyManager
 from engineai.sdk.dashboard.data.manager.manager import WidgetDataType
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.dependencies import WidgetSelectDependency
 from engineai.sdk.dashboard.exceptions import WidgetDataNotFoundError
 from engineai.sdk.dashboard.exceptions import WidgetFieldNotFoundError
 from engineai.sdk.dashboard.interface import WidgetInterface
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.selected import Selected
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.exceptions import WidgetIdValueError
 
 from ..abstract.layout import AbstractLayoutItem
 from ..abstract.selectable_widgets import AbstractSelectWidget
 
-filterwarnings("ignore", category=BeartypeDecorHintPep585DeprecationWarning)
-
 WidgetTitleType = Optional[Union[str, GenericLink]]
 
 
 class Widget(DependencyManager, AbstractLayoutItem, WidgetInterface):
     """Base spec shared by all widgets."""
 
     _WIDGET_API_TYPE: Optional[str] = None
     _DEFAULT_HEIGHT: Union[int, float] = 4
     _FORCE_HEIGHT: bool = False
     _WIDGET_HEIGHT_STEP = 0.1
     _WIDGET_ID_COUNTER = 0
     _INPUT_KEY = "widget"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         widget_id: Optional[str] = None,
         data: Optional[WidgetDataType] = None,
     ):
         """Shared fields by all widgets.
@@ -199,15 +195,15 @@
 class _Selected(Selected[AbstractSelectWidget, WidgetField, Widget]):
     """Widget Selected property configuration."""
 
 
 class SelectableWidget(Widget, AbstractSelectWidget):
     """Base spec shared by all widgets that can be selected."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         widget_id: Optional[str] = None,
         data: WidgetDataType,
     ):
         """Shared fields by all widgets.
@@ -216,15 +212,15 @@
             widget_id: unique id amongst other widgets in a dashboard
             data: data to be used by widget. Accepts DataSource
                 method as well as raw data.
         """
         super().__init__(widget_id=widget_id, data=data)
         self.selected = _Selected(component=self)
 
-    @beartype
+    @type_check
     def select_dependency(self, *, dependency_id: str = "") -> WidgetSelectDependency:
         """Return dependency for selectable widget.
 
         Args:
             dependency_id (str): id of dependency to selectable widget.
                 Defaults to "" (i.e. uses widgetId as dependency id).
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/__init__.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/axis/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from abc import abstractmethod
 from typing import Any
 from typing import Mapping
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import AxisNumberFormatting
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScale
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScaleDynamic
@@ -20,15 +20,15 @@
 
 
 class CartesianBaseAxis(AbstractFactoryLinkItemsHandler):
     """Specs for X Axis of a Cartesian chart."""
 
     _API_TYPE: Optional[str] = None
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         title: Union[str, GenericLink] = "",
         enable_crosshair: bool = False,
         formatting: Optional[AxisNumberFormatting] = None,
         scale: Optional[AxisScale] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Specs for x axis of a Cartesian chart."""
 
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import AxisNumberFormatting
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.widgets.cartesian.exceptions import (
     CartesianValidateDataColumnNotFound,
 )
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScale
 
@@ -17,15 +17,15 @@
 
 
 class XAxis(CartesianBaseAxis):
     """Specs for X Axis of a Cartesian chart."""
 
     _API_TYPE = "ContinuousCartesianWidgetXAxisInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         data_column: Union[str, GenericLink],
         *,
         title: Union[str, GenericLink] = "X",
         enable_crosshair: bool = False,
         formatting: Optional[AxisNumberFormatting] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import Mapping
 from typing import Optional
 from typing import Set
 from typing import Union
 from typing import get_args
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import AxisNumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.widgets.cartesian.axis.typing import YAxisSeries
 from engineai.sdk.dashboard.widgets.cartesian.series.line import LineSeries
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScale
 from engineai.sdk.dashboard.widgets.components.charts.exceptions import (
@@ -26,15 +26,15 @@
 
 
 class YAxis(CartesianBaseAxis):
     """Specs for Y Axis of a Cartesian chart."""
 
     _API_TYPE = "ContinuousCartesianWidgetYAxisInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         series: YAxisSeries,
         *,
         title: Union[str, WidgetField] = "Y",
         enable_crosshair: bool = False,
         formatting: Optional[AxisNumberFormatting] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/cartesian.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/cartesian.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Spec for Cartesian widget."""
 
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
 from engineai.sdk.dashboard.data import DataSource
+from engineai.sdk.dashboard.data.http import Http
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.cartesian.axis.typing import YAxisSeries
 from engineai.sdk.dashboard.widgets.cartesian.axis.y_axis import YAxis
 from engineai.sdk.dashboard.widgets.components.charts.toolbar import build_chart_toolbar
 
@@ -26,18 +27,18 @@
 
 class Cartesian(Widget):
     """Spec for Cartesian widget."""
 
     _DEPENDENCY_ID = "__CARTESIAN_DATA_DEPENDENCY__"
     _WIDGET_API_TYPE = "continuousCartesian"
 
-    @beartype
+    @type_check
     def __init__(
         self,
-        data: Union[DataSource, pd.DataFrame],
+        data: Union[DataSource, pd.DataFrame, Http],
         *,
         widget_id: Optional[str] = None,
         x_axis: Union[str, GenericLink, XAxis],
         left_y_axis: Optional[Union[YAxisSeries, YAxis]] = None,
         right_y_axis: Optional[Union[YAxisSeries, YAxis]] = None,
         legend_position: LegendPosition = LegendPosition.BOTTOM,
         title: WidgetTitleType = "",
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/chart.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Spec for charts in a Cartesian widget."""
 
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.cartesian.axis.typing import YAxisSeries
 from engineai.sdk.dashboard.widgets.cartesian.exceptions import (
     CartesianMissingChartAxisError,
 )
@@ -18,15 +18,15 @@
 from .axis.x_axis import XAxis
 from .axis.y_axis import YAxis
 
 
 class Chart(AbstractFactoryLinkItemsHandler):
     """Spec for charts in a Cartesian widget."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         x_axis: Union[str, GenericLink, XAxis],
         *,
         data: Optional[pd.DataFrame] = None,
         left_y_axis: Optional[Union[YAxisSeries, YAxis]] = None,
         right_y_axis: Optional[Union[YAxisSeries, YAxis]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/legend.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/legend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-"""Spec for legend of a categorical widget."""
+"""Spec for legend of a timeseries widget."""
 from typing import Any
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.enum.legend_position import LegendPosition
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class Legend(AbstractFactory):
-    """Spec for legend of a categorical widget.
-
-    Args:
-        position: location of position relative to data, charts.
-    """
+    """Spec for legend of a timeseries widget."""
 
-    @beartype
+    @type_check
     def __init__(self, *, position: LegendPosition = LegendPosition.BOTTOM):
-        """Construct a legend for a categorical widget."""
+        """Construct a legend for a timeseries widget.
+
+        Args:
+            position: location of position relative to data, charts.
+        """
         super().__init__()
         self.__position = position
 
+    @property
+    def position(self) -> LegendPosition:
+        """Returns the current Legend Position."""
+        return self.__position
+
     def build(self) -> Any:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
         return generate_input(
-            "ContinuousCartesianWidgetLegendInput", position=self.__position.value
+            "TimeseriesWidgetLegendInput", position=self.__position.value
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/area.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/area.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Spec for a Area series of a Cartesian widget."""
 
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.styling import AreaSeriesStyling
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 from .base import CartesianBaseSeries
@@ -17,15 +16,15 @@
 class AreaSeries(CartesianBaseSeries):
     """Spec for a Area series of a Cartesian widget."""
 
     _API_TYPE = "ContinuousCartesianWidgetAreaSeriesInput"
     _INPUT_KEY = "area"
     _styling_class = AreaSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         formatting: Optional[NumberFormatting] = None,
         name: Optional[Union[str, WidgetField]] = None,
         styling: Optional[Union[Palette, AreaSeriesStyling]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.widgets.components.charts.styling import (
     AreaRangeSeriesStyling,
 )
@@ -23,15 +23,15 @@
 class AreaRangeSeries(CartesianBaseSeries):
     """Spec for a area range series of a Cartesian widget."""
 
     _API_TYPE = "ContinuousCartesianWidgetAreaRangeSeriesInput"
     _INPUT_KEY = "areaRange"
     _styling_class = AreaRangeSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         low_data_column: Union[str, WidgetField],
         high_data_column: Union[str, WidgetField],
         formatting: Optional[NumberFormatting] = None,
         name: Union[str, WidgetField],
@@ -82,15 +82,15 @@
 
     def validate(self, *, data: pd.DataFrame) -> None:
         """Validate if dataframe that will be used for series contains required columns.
 
         Args:
             data: pandas dataframe which will be used for table
             widget_id: id of table widget where this series is used
-            path: path in rubik linked to data
+            path: path in storage linked to data
 
         """
         super().validate(data=data)
 
         super()._validate_data_column(
             data=data,
             data_column=self._low_column,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import Dict
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color.palette import qualitative_palette
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
@@ -37,15 +37,15 @@
 
 class CartesianBaseSeries(ChartSeriesBase):
     """Spec for the CartesianBaseSeries widget."""
 
     _styling_class: Optional[Type[ColoredSeriesStyling]] = None
     _INPUT_KEY: Optional[str] = None
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Optional[Union[str, GenericLink]] = None,
         formatting: Optional[NumberFormatting] = None,
         name: Optional[Union[str, GenericLink]] = None,
         show_in_legend: bool = True,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Spec for a bubble series of a Cartesian widget."""
 
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
@@ -36,15 +36,15 @@
 class BubbleSeries(CartesianBaseSeries):
     """Spec for a bubble series of a Cartesian widget."""
 
     _API_TYPE = "ContinuousCartesianWidgetBubbleSeriesInput"
     _INPUT_KEY = "bubble"
     _styling_class = BubbleCircleSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         bubble_size_data_column: Union[str, GenericLink],
         data_column: Union[str, GenericLink],
         formatting: Optional[NumberFormatting] = None,
         bubble_name: Optional[Union[str, GenericLink]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/column.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/column.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Spec for a column series of a Cartesian widget."""
 
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.styling import ColumnSeriesStyling
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 from .base import CartesianBaseSeries
@@ -17,15 +16,15 @@
 class ColumnSeries(CartesianBaseSeries):
     """Spec for a column series of a Cartesian widget."""
 
     _API_TYPE = "ContinuousCartesianWidgetColumnSeriesInput"
     _INPUT_KEY = "column"
     _styling_class = ColumnSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         formatting: Optional[NumberFormatting] = None,
         name: Optional[Union[str, WidgetField]] = None,
         styling: Optional[Union[Palette, ColumnSeriesStyling]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/line.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/line.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Spec for a line series of a Cartesian widget."""
 
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.styling import LineSeriesStyling
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 from .base import CartesianBaseSeries
@@ -17,15 +16,15 @@
 class LineSeries(CartesianBaseSeries):
     """Spec for a line series of a Cartesian widget."""
 
     _API_TYPE = "ContinuousCartesianWidgetLineSeriesInput"
     _INPUT_KEY = "line"
     _styling_class = LineSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         formatting: Optional[NumberFormatting] = None,
         name: Optional[Union[str, WidgetField]] = None,
         styling: Optional[Union[Palette, LineSeriesStyling]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Spec for a scatter series of a Cartesian widget."""
 
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.styling import (
     ScatterSeriesStyling,
 )
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
@@ -19,15 +18,15 @@
 class ScatterSeries(CartesianBaseSeries):
     """Spec for a scatter series of a Cartesian widget."""
 
     _API_TYPE = "ContinuousCartesianWidgetScatterSeriesInput"
     _INPUT_KEY = "scatter"
     _styling_class = ScatterSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         formatting: Optional[NumberFormatting] = None,
         name: Optional[Union[str, WidgetField]] = None,
         styling: Optional[Union[Palette, ScatterSeriesStyling]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/cartesian/series/typing.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/chart_utils.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/chart_utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/actions/links/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import InternalDataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .exceptions import ActionLinkMissingColumnError
 
 
 class BaseLink(AbstractFactoryLinkItemsHandler):
     """Spec for Base Action Link."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         data_column: TemplatedStringItem,
         tooltip: Optional[Union[List[str], TemplatedStringItem, DataField]] = None,
     ):
         """Construct for ActionLink class.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 
 from typing import Any
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.actions.links.base import BaseLink
 
 
 class UrlLink(BaseLink):
     """Spec for Url Link."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         data_column: TemplatedStringItem,
         tooltip: Optional[Union[List[str], TemplatedStringItem, DataField]] = None,
     ):
         """Construct for ActionUrlLink class.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec for dynamic scale for y axis."""
 
 from typing import Any
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class AxisScaleDynamic(AbstractFactory):
     """Spec for dynamic scale for y axis.
 
     Axis extremes are calculated dynamically to minimize the amount of dead space
         in a chart.
     """
 
-    @beartype
+    @type_check
     def __init__(self, *, tick_amount: int = 3):
         """Construct dynamic scale for y axis.
 
         Args:
             tick_amount: number of ticks beyond min and max.
         """
         super().__init__()
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Spec for scale for y axis with only negative values."""
 
 from typing import Any
 from typing import Optional
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class AxisScaleNegative(AbstractFactory):
     """Spec for scale for y axis with only negative values.
 
     Assumes max value of chart to be fixed at 0.
 
     """
 
-    @beartype
+    @type_check
     def __init__(
         self, *, min_value: Optional[int] = None, intermediate_tick_amount: int = 3
     ):
         """Construct positive scale spec.
 
         Args:
             min_value: fixed minimum value for axis.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Spec for scale for y axis with only positive values."""
 
 from typing import Any
 from typing import Optional
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class AxisScalePositive(AbstractFactory):
     """Spec for scale for y axis with only negative values.
 
     Assumes min value of chart to be fixed at 0.
 
     """
 
-    @beartype
+    @type_check
     def __init__(
         self, *, max_value: Optional[int] = None, intermediate_tick_amount: int = 3
     ):
         """Construct positive scale spec.
 
         Args:
             max_value: fixed maximum value for axis.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """Spec for scale for y axis with only positive and negative values."""
 
 from typing import Any
 from typing import Optional
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.exceptions import (
     ChartScaleSymmetricValueError,
 )
 
 
 class AxisScaleSymmetric(AbstractFactory):
     """Spec for scale for y axis with only positive and negative values.
 
     Extremes determined by max(abs(data)) and 0 added as the middle tick.
 
     """
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         min_value: Optional[int] = None,
         max_value: Optional[int] = None,
         intermediate_tick_amount: int = 1,
         strict: Optional[bool] = None
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/series/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/area.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/area.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec to style an area series."""
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
 class AreaSeriesStyling(BaseChartSeriesStyling):
     """Spec to style an area series."""
 
     _API_TYPE = "ChartAreaSeriesStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec to style an area range series."""
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
 class AreaRangeSeriesStyling(BaseChartSeriesStyling):
     """Spec to style an area range series."""
 
     _API_TYPE = "ChartAreaRangeSeriesStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 
 from ..exceptions import ChartStylingNoDataColumnError
 from .base import BaseChartSeriesStyling
 
 
 class BubbleCircleSeriesStyling(BaseChartSeriesStyling):
     """Spec to style a bubble series as circles."""
 
     _API_TYPE = "ChartBubbleSeriesStylingCircleInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         label_column: Optional[TemplatedStringItem] = None,
         max_size_percentage: Optional[Union[float, int]] = 0.5,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Spec to style a bubble series using country flags."""
 
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.exceptions import (
     ChartStylingNoDataColumnError,
 )
 
 
 class BubbleCountrySeriesStyling(AbstractFactory):
     """Spec to style a bubble series using country flags."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         country_column: TemplatedStringItem,
         max_size_percentage: Optional[Union[float, int]] = 0.5,
         min_size_percentage: Optional[Union[float, int]] = 0.2,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/column.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/column.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec to style a column series."""
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
 class ColumnSeriesStyling(BaseChartSeriesStyling):
     """Spec to style a column series."""
 
     _API_TYPE = "ChartColumnSeriesStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.SQUARE,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec to style a column series."""
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
 class ErrorBarSeriesStyling(BaseChartSeriesStyling):
     """Spec to style error bar series."""
 
     _API_TYPE = "ChartErrorBarSeriesStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.SQUARE,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/line.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/line.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 from typing import get_args
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 
 from ...items.styling.exceptions import ItemStylingValidationError
 from ...items.styling.exceptions import StylingInvalidDashValuesError
@@ -21,15 +21,15 @@
 
 
 class LineSeriesStyling(BaseChartSeriesStyling):
     """Spec to style a line series."""
 
     _API_TYPE = "ChartLineSeriesStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
         dash_style: Union[DashStyle, TemplatedStringItem] = DashStyle.SOLID,
         marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/point.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/point.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec to style a point series."""
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
 class PointSeriesStyling(BaseChartSeriesStyling):
     """Spec to style a point series."""
 
     _API_TYPE = "ChartPointSeriesStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec to style a scatter series."""
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
 class ScatterSeriesStyling(BaseChartSeriesStyling):
     """Spec to style a scatter series."""
 
     _API_TYPE = "ChartScatterSeriesStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Base Tooltip Item class."""
 
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import DateTimeFormatting
 from engineai.sdk.dashboard.formatting import MapperFormatting
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.formatting import TextFormatting
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import InternalDataField
@@ -26,15 +26,15 @@
 
 
 class BaseTooltipItem(AbstractFactoryLinkItemsHandler):
     """Base Tooltip Item class."""
 
     _API_TYPE: Optional[str] = None
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
         formatting: TooltipItemFormatter,
         label: Optional[Union[str, DataField]] = None,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Specs for category item for a tooltip."""
 
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import MapperFormatting
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseTooltipItem
 
 
 class CategoryTooltipItem(BaseTooltipItem):
     """Specs for category tooltip item."""
 
     _API_TYPE = "TooltipCategoricalItemInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
         formatting: MapperFormatting,
         label: Optional[Union[str, DataField]] = None,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Specs for dateitem item for a tooltip."""
 
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import DateTimeFormatting
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseTooltipItem
 
 
 class DatetimeTooltipItem(BaseTooltipItem):
     """Specs for datetime item for a tooltip."""
 
     _API_TYPE = "TooltipDateTimeItemInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
         formatting: Optional[DateTimeFormatting] = None,
         label: Optional[Union[str, DataField]] = None,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Specs for number item for a tooltip."""
 
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseTooltipItem
 
 
 class NumberTooltipItem(BaseTooltipItem):
     """Specs for number item for a tooltip."""
 
     _API_TYPE = "TooltipNumberItemInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
         formatting: Optional[NumberFormatting] = None,
         label: Optional[Union[str, DataField]] = None,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Specs for text item for a tooltip."""
 
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import TextFormatting
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseTooltipItem
 
 
 class TextTooltipItem(BaseTooltipItem):
     """Specs for text item for a tooltip."""
 
     _API_TYPE = "TooltipTextItemInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
         formatting: Optional[TextFormatting] = None,
         label: Optional[Union[str, DataField]] = None,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/charts/typing.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 from typing import cast
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.exceptions import ImproperlyConfiguredError
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.styling.color import Single
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
@@ -25,15 +25,15 @@
 
 
 class BaseItemStyling(AbstractFactoryLinkItemsHandler):
     """Spec for Number Styling Base class."""
 
     _API_TYPE: Optional[str] = None
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
     ):
         """Construct for BaseItemStyling class.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """Spec fot Number Styling Arrow."""
 
 from typing import Any
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.divergent import Divergent
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 
 from ..base import BaseItemStyling
 
 
 class NumberStylingArrow(BaseItemStyling):
     """Spec for Number Arrow Styling class."""
 
     _API_TYPE: str = "NumberStylingArrowInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Optional[TemplatedStringItem] = None,
         color_divergent: Divergent,
     ):
         """Construct spec Number Arrow Styling.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-"""Spec fot Number Styling Chip."""
+"""Spec fot Number Styling Dot."""
 
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..base import BaseItemStyling
 
 
-class NumberStylingChip(BaseItemStyling):
-    """Spec for Number Chip Styling class."""
+class NumberStylingDot(BaseItemStyling):
+    """Spec for Number Dot Styling class."""
 
-    _API_TYPE: str = "NumberStylingChipInput"
+    _API_TYPE = "NumberStylingDotInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for Number Chip Styling.
+        """Construct spec for Number Dot Styling.
 
         Args:
             color_spec (ColorSpec): specs for color.
             data_column (Optional[TemplatedStringItem]): styling value key.
-                Defaults to None.
         """
-        super().__init__(data_column=data_column, color_spec=color_spec)
+        super().__init__(
+            color_spec=color_spec,
+            data_column=data_column,
+        )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-"""Spec fot Number Styling Dot."""
-
+"""Spec fot Text Styling Font."""
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..base import BaseItemStyling
 
 
-class NumberStylingDot(BaseItemStyling):
-    """Spec for Number Dot Styling class."""
+class TextStylingChip(BaseItemStyling):
+    """Spec for Text Chip Styling Class."""
 
-    _API_TYPE = "NumberStylingDotInput"
+    _API_TYPE = "TextStylingChipInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
-        color_spec: ColorSpec,
+        color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for Number Dot Styling.
+        """Construct spec for Text Chip Styling.
 
         Args:
-            color_spec (ColorSpec): specs for color.
+            color_spec (Optional[ColorSpec]): specs for color.
             data_column (Optional[TemplatedStringItem]): styling value key.
         """
-        super().__init__(
-            color_spec=color_spec,
-            data_column=data_column,
-        )
+        super().__init__(data_column=data_column, color_spec=color_spec)
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec fot Number Styling Font."""
 
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..base import BaseItemStyling
 
 
 class NumberStylingFont(BaseItemStyling):
     """Spec for Number Font Styling class."""
 
     _API_TYPE = "NumberStylingFontInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
     ):
         """Construct spec for Number Font Styling.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec for Number Styling Progress Bar."""
 from typing import Any
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.items.styling.base import BaseItemStyling
 
 
 class NumberStylingProgressBar(BaseItemStyling):
     """Spec for Number Styling Progress Bar class."""
 
     _API_TYPE = "NumberStylingProgressBarInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         column: Optional[TemplatedStringItem] = None,
     ):
         """Construct spec for Number Styling Progress Bar.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Spec fot Text Styling Font."""
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..base import BaseItemStyling
 
 
-class TextStylingChip(BaseItemStyling):
-    """Spec for Text Chip Styling Class."""
+class TextStylingFont(BaseItemStyling):
+    """Spec for Text Font Styling Class."""
 
-    _API_TYPE = "TextStylingChipInput"
+    _API_TYPE = "TextStylingFontInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for Text Chip Styling.
+        """Construct spec for Text Font Styling.
 
         Args:
-            color_spec (Optional[ColorSpec]): specs for color.
+            color_spec (ColorSpec): specs for color.
             data_column (Optional[TemplatedStringItem]): styling value key.
+                Defaults to None.
         """
         super().__init__(data_column=data_column, color_spec=color_spec)
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Spec fot Text Styling Font."""
 from typing import Any
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 
 from ..base import BaseItemStyling
 
 
 class TextStylingCountryFlag(BaseItemStyling):
     """Spec for Text Country Flag Styling Class."""
 
     _API_TYPE = "TextStylingCountryFlagInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         left: bool = True,
         data_column: Optional[TemplatedStringItem] = None,
     ):
         """Construct spec for Text Country Flag Styling.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec fot Text Styling Dot."""
 
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..base import BaseItemStyling
 
 
 class TextStylingDot(BaseItemStyling):
     """Spec for Text Dot Styling Class."""
 
     _API_TYPE = "TextStylingDotInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
     ):
         """Construct spec for Text Dot Styling.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/content/content.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/content.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.data import DataSource
+from engineai.sdk.dashboard.data.http import Http
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.utils import build_data
 
 from ..base import Widget
 from ..base import WidgetTitleType
 from .exceptions import ContentNoItemsError
 from .item import ContentItem
 from .item import build_content_item
 
-ContentData = Union[DataSource, Dict[str, Any]]
+ContentData = Union[DataSource, Dict[str, Any], Http]
 
 
 class Content(Widget):
     """Spec for Content widget."""
 
     _WIDGET_API_TYPE = "content"
     _DEPENDENCY_ID = "__CONTENT_DATA_DEPENDENCY__"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data: ContentData,
         widget_id: Optional[str] = None,
         title: Optional[WidgetTitleType] = None,
     ):
@@ -54,15 +54,15 @@
 
         Args:
             data (Dict[str, Any]): Dictionary where the data is present.
         """
         for item in self.__items:
             item.validate(data=data)
 
-    @beartype
+    @type_check
     def add_items(self, *items: ContentItem) -> "Content":
         """Add a new ContentItem to the list of items to show on Content Widget.
 
         Args:
             items (ContentItem): Content Items to add to the Content Widget.
 
         Returns:
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/content/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/content/item.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/item.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/content/markdown.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/markdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Spec for MarkdownItem class."""
 
 from typing import Any
 from typing import Dict
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.content.exceptions import ContentItemNoValueError
 
 
 class MarkdownItem(AbstractFactory):
     """Spec for MarkdownItem class."""
 
-    @beartype
+    @type_check
     def __init__(self, data_key: str):
         """Construct spec for MarkdownItem class.
 
         Args:
             data_key (str): Key inside the data with the content
                 for the markdown Item
         """
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/enums.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/geo/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/geo/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 from typing import Generic
 from typing import List
 from typing import Optional
 from typing import TypeVar
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 from pandas.api.types import is_datetime64_dtype
 from pandas.api.types import is_numeric_dtype
 from pandas.api.types import is_object_dtype
 from pandas.api.types import is_string_dtype
 
 from engineai.sdk.dashboard.data.decorator import DataSource
+from engineai.sdk.dashboard.data.http import Http
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.chart_utils import get_object_columns_tooltip
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.datetime import (
     DatetimeTooltipItem,
 )
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
     build_tooltip_item,
@@ -48,18 +49,18 @@
 
 class BaseMapGeo(Generic[T], Widget):
     """Spec for Base MapGeo widget."""
 
     _WIDGET_API_TYPE = "mapGeo"
     _DEPENDENCY_ID = "__MAP_GEO_DATA_DEPENDENCY__"
 
-    @beartype
+    @type_check
     def __init__(
         self,
-        data: Union[DataSource, T],
+        data: Union[DataSource, T, Http],
         *,
         series: Optional[MapSeries] = None,
         region_column: str = "region",
         widget_id: Optional[str] = None,
         title: Optional[WidgetTitleType] = None,
         legend_position: LegendPosition = LegendPosition.BOTTOM,
         region: Region = Region.WORLD,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/geo/geo.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/geo/geo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """Spec for Map Geo widget."""
 
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
 from engineai.sdk.dashboard.data import DataSource
+from engineai.sdk.dashboard.data.http import Http
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 from engineai.sdk.dashboard.widgets.maps.enums import LegendPosition
 from engineai.sdk.dashboard.widgets.maps.enums import Region
 
 from ...base import WidgetTitleType
 from ..series.series import MapSeries
 from .base import BaseMapGeo
 
 
 class Geo(BaseMapGeo[pd.DataFrame]):
     """Spec for MapGeo widget."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
-        data: Union[DataSource, pd.DataFrame],
+        data: Union[DataSource, pd.DataFrame, Http],
         *,
         series: Optional[MapSeries] = None,
         region_column: str = "region",
         widget_id: Optional[str] = None,
         title: Optional[WidgetTitleType] = None,
         legend_position: LegendPosition = LegendPosition.BOTTOM,
         region: Region = Region.WORLD,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/legend.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/legend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Spec for legend of a Map Shape widget."""
 
 from typing import Any
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.maps.enums import LegendPosition
 
 
 class Legend(AbstractFactory):
     """Spec for legend of a Map widget."""
 
-    @beartype
+    @type_check
     def __init__(self, *, position: LegendPosition = LegendPosition.BOTTOM):
         """Construct a legend for a Map Shape widget.
 
         Args:
             position (Position): location of position
                 relative to data, maps.
         """
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/series/numeric.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/numeric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Spec for a numeric series of a Map widget."""
 
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
@@ -23,15 +23,15 @@
 from ...utils import build_data
 from ...utils import get_tooltips
 
 
 class NumericSeries:
     """Spec for a numeric series of a Map widget."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem = "value",
         name: Optional[TemplatedStringItem] = None,
         formatting: Optional[NumberFormatting] = None,
         styling: Optional[Union[Palette, SeriesStyling]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/series/series.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/series.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/maps/series/styling.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/styling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Spec to style a line series."""
 
 from typing import Any
 from typing import Optional
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.discrete_map import DiscreteMap
 from engineai.sdk.dashboard.styling.color.gradient import Gradient
 from engineai.sdk.dashboard.styling.color.palette import Palette
 from engineai.sdk.dashboard.styling.color.single import Single
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.styling.enums import MarkerSymbol
 from engineai.sdk.dashboard.widgets.maps.exceptions import MapColumnDataNotFoundError
 
 
 class SeriesStyling:
     """Spec to style a numeric series."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[str] = None,
     ):
         """Construct style spec for numeric series.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/__init__.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/chart.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/chart.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Spec for Pie Chart."""
 
-import warnings
 from typing import Any
 from typing import Optional
 
 import pandas as pd
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.utils import generate_input
-from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItem
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 from .series.typings import ChartSeries
 from .tooltip import Tooltip
 
 
 class Chart(AbstractFactory):
@@ -31,30 +29,14 @@
         """
         self._series = series
         self._tooltip = Tooltip(
             category_column=series.category_column,
             tooltips=tooltips,
         )
 
-    def add_tooltips(self, *tooltips: TooltipItem) -> None:
-        """Add tooltip item(s) to Pie Widget.
-
-        Args:
-            tooltips (TooltipItem): item(s) to be added to the Pie Widget.
-
-        Returns:
-            Pie: reference to this widget to facilitate
-                inline manipulation
-        """
-        self._tooltip.add_tooltips(*tooltips)
-        warnings.warn(
-            "`add_tooltips` is deprecated. Use `tooltips` in constructor, instead.",
-            DeprecationWarning,
-        )
-
     def prepare(self, dependency_id: str, json_data: Any = None) -> None:
         """Prepare Widget Spec to be validated."""
         self._series.prepare(dependency_id=dependency_id, json_data=json_data)
         self._tooltip.prepare(dependency_id=dependency_id, json_data=json_data)
 
     def validate(self, *, data: pd.DataFrame) -> None:
         """Validates Pie Series Widget and the inner components specs.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/legend.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/legend.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/pie.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/pie.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Spec for Pie Widget."""
-import warnings
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 from pandas.api.types import is_datetime64_dtype
 from pandas.api.types import is_numeric_dtype
 from pandas.api.types import is_object_dtype
 from pandas.api.types import is_string_dtype
 
 from engineai.sdk.dashboard.data import DataSource
+from engineai.sdk.dashboard.data.http import Http
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.chart_utils import TooltipItem
 from engineai.sdk.dashboard.widgets.chart_utils import get_object_columns_tooltip
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.datetime import (
     DatetimeTooltipItem,
 )
@@ -39,18 +39,18 @@
 
 class Pie(Widget):
     """Spec for Pie Widget."""
 
     _WIDGET_API_TYPE = "pie"
     _DEPENDENCY_ID = "__PIE_DATA_DEPENDENCY__"
 
-    @beartype
+    @type_check
     def __init__(
         self,
-        data: Union[DataSource, pd.DataFrame],
+        data: Union[DataSource, pd.DataFrame, Http],
         *,
         series: Optional[ChartSeries] = None,
         legend_position: LegendPosition = LegendPosition.BOTTOM,
         widget_id: Optional[str] = None,
         title: Optional[WidgetTitleType] = None,
         tooltips: Optional[TooltipItems] = None,
     ):
@@ -139,31 +139,14 @@
                         column_data=aux_data[column_name], column_name=str(column_name)
                     )
                     if tooltip_item is not None:
                         tooltips.append(tooltip_item)
 
         return tooltips
 
-    def add_tooltips(self, *tooltips: TooltipItem) -> "Pie":
-        """Add tooltip item(s) to Pie Widget.
-
-        Args:
-            tooltips: item(s) to be added to the Pie Widget.
-
-        Returns:
-            Pie: reference to this widget to facilitate
-                inline manipulation
-        """
-        warnings.warn(
-            "`add_tooltips` is deprecated. Use `tooltips` in constructor, instead.",
-            DeprecationWarning,
-        )
-        self._chart.add_tooltips(*tooltips)
-        return self
-
     def validate(self, data: pd.DataFrame, **kwargs: Any) -> None:
         """Validates Pie Widget and the inner components specs."""
         self._chart.validate(data=data)
 
     def _prepare(self, **kwargs: object) -> None:
         """Method for each Widget prepare before building."""
         self._chart.prepare(self.dependency_id, kwargs.get("json_data", None))
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/series/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting.number import NumberFormatting
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
@@ -27,15 +27,15 @@
 
 class BaseSeries(AbstractFactoryLinkItemsHandler):
     """Spec for BaseSeries."""
 
     _API_TYPE: Optional[str] = None
     _INPUT_KEY: Optional[str] = None
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         name: TemplatedStringItem,
         category_column: TemplatedStringItem,
         data_column: TemplatedStringItem,
         formatting: Optional[NumberFormatting] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/series/country.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/country.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Spec for Pie Series."""
 
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting.number import NumberFormatting
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 from .base import BaseSeries
@@ -19,15 +19,15 @@
 
 class CountrySeries(BaseSeries):
     """Spec for Pie Country Series."""
 
     _API_TYPE = "PieWidgetChartSeriesCountryInput"
     _INPUT_KEY = "country"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         name: TemplatedStringItem = "Country Series",
         country_column: TemplatedStringItem = "country_code",
         data_column: TemplatedStringItem = "value",
         formatting: Optional[NumberFormatting] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/series/series.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/column.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,107 +1,92 @@
-"""Spec for Pie Series."""
-import warnings
+"""Spec for a column series of a Timeseries widget."""
+
+from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
-from engineai.sdk.dashboard.formatting.number import NumberFormatting
+from engineai.sdk.dashboard.decorator import type_check
+from engineai.sdk.dashboard.links import WidgetField
+from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
-from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItem
-from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
-
-from .base import BaseSeries
-from .styling import SeriesStyling
-
-
-class Series(BaseSeries):
-    """Spec for Pie Series."""
+from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
+    CountryEntity,
+)
+from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
+    Entities,
+)
+from engineai.sdk.dashboard.widgets.components.charts.styling import ColumnSeriesStyling
+
+from ...components.charts.typing import TooltipItems
+from .base import TimeseriesBaseSeries
+
+
+class ColumnSeries(TimeseriesBaseSeries):
+    """Spec for a column series of a Timeseries widget."""
+
+    _API_TYPE = "TimeseriesWidgetColumnSeriesInput"
+    _INPUT_KEY = "column"
+    _styling_class = ColumnSeriesStyling
 
-    _API_TYPE = "PieWidgetChartSeriesStandardInput"
-    _INPUT_KEY = "standard"
-
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
-        name: TemplatedStringItem = "Series",
-        category_column: TemplatedStringItem = "category",
-        data_column: TemplatedStringItem = "value",
-        formatting: Optional[NumberFormatting] = None,
-        styling: Optional[Union[Palette, SeriesStyling]] = None,
+        data_column: Union[str, WidgetField],
+        name: Optional[Union[str, GenericLink]] = None,
+        styling: Optional[Union[Palette, ColumnSeriesStyling]] = None,
+        entity: Optional[Entities] = None,
+        show_in_legend: bool = True,
+        required: bool = True,
+        visible: bool = True,
+        right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct spec for Pie Series.
+        """Construct column series.
 
         Args:
-            name: name for the Pie series.
-            category_column: name of column in pandas dataframe(s) that has category
-                info within the pie.
-            data_column: name of column in pandas dataframe(s) that has pie data.
-            formatting: spec for number formatting.
-            styling: spec for pie series styling.
+            data_column: name of column in pandas dataframe(s) used for the values of
+                this series.
+            name: series name (shown in legend and tooltip).
+            styling: styling spec, by default uses the values from the sequential
+                palette.
+            entity: entity spec.
+            show_in_legend: whether to show series in legend or not.
+            required: Flag to make the Series mandatory. If required == True and no
+                Data the widget will show an error. If required==False and no Data,
+                the widget hides the Series.
+            visible: Flag to make the Series visible when chart is loaded.
+            right_axis: Flag to make the Series visible on the right axis.
             tooltips: tooltip items to be displayed at Series level.
-
-        Examples:
-            ??? example "Customise Pie Widget series (e.g. changing data column)"
-                ```py linenums="1"
-                import pandas as pd
-                from engineai.sdk.dashboard.dashboard import Dashboard
-                from engineai.sdk.dashboard.widgets import pie
-                data = pd.DataFrame(
-                    {
-                        "name": ["X", "Y"],
-                        "volume": [10, 20],
-                    },
-                )
-                dashboard = Dashboard(
-                    content=pie.Pie(
-                        data=data,
-                        series=pie.Series(
-                            category_column="name",
-                            data_column="volume",
-                        )
-                    )
-                )
-                ```
         """
         super().__init__(
             name=name,
-            category_column=category_column,
             data_column=data_column,
-            formatting=formatting,
-            styling=styling,
+            show_in_legend=show_in_legend,
+            required=required,
+            visible=visible,
+            styling=ColumnSeriesStyling(color_spec=styling)
+            if isinstance(styling, Palette)
+            else styling,
+            entity=entity,
+            right_axis=right_axis,
             tooltips=tooltips,
         )
 
-    def validate(
-        self,
-        *,
-        data: pd.DataFrame,
-    ) -> None:
-        """Validates Pie Series Widget and the inner components specs."""
-        self._validate_field(
-            data=data,
-            field="category_column",
-            item=self._category_column,
-        )
-        super().validate(data=data)
-
-    def add_tooltips(self, *tooltips: TooltipItem) -> "Series":
-        """Add tooltip item(s) to the series.
+    def validate(self, *, data: pd.DataFrame) -> None:
+        """Validate if dataframe that will be used for series contains required columns.
 
         Args:
-            tooltips: item(s) to be added to the series.
-
-        Returns:
-            Series: reference to this widget to facilitate
-                inline manipulation
+            data: pandas dataframe which will be used for table
         """
-        warnings.warn(
-            "`add_tooltips` is deprecated. Use `tooltips` in constructor, instead.",
-            DeprecationWarning,
-        )
-        self._tooltip_items.extend(tooltips)
-        return self
+        super().validate(data=data)
+
+        if self._entity is not None and isinstance(self._entity, CountryEntity):
+            self._entity.validate_country_code()
+
+    def _build_extra_inputs(self) -> Dict[str, Any]:
+        return {
+            "transforms": [transform.build() for transform in self._transforms],
+        }
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/series/styling.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/styling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Spec for Pie Series Styling."""
 
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.palette import Palette
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.widgets.components.charts.styling.base import (
     BaseChartSeriesStyling,
 )
 
 
 class SeriesStyling(BaseChartSeriesStyling):
     """Spec for Pie Series Styling."""
 
     _API_TYPE = "ChartPieSeriesStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
     ):
         """Construct spec for Pie Series Styling.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/pie/tooltip.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/tooltip.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Spec for Pie Tooltip."""
 
-import warnings
 from typing import Any
 from typing import Optional
 
 import pandas as pd
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
     build_tooltip_item,
 )
-from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItem
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 from engineai.sdk.dashboard.widgets.utils import build_data
 
 
 class Tooltip(AbstractFactory):
     """Spec for Pie Tooltip."""
 
@@ -40,24 +38,14 @@
             if tooltips is None
             else [tooltips]
         )
         self._category_column = category_column
         self._dependency_id: str = " "
         self._json_data: Any = None
 
-    def add_tooltips(self, *tooltips: TooltipItem) -> None:
-        """Add tooltip item(s) to Pie Widget."""
-        warnings.warn(
-            "`add_tooltips` is deprecated. Use `tooltips` in constructor, instead.",
-            DeprecationWarning,
-        )
-        if len(tooltips) > 0:
-            self._tooltips = []
-        self._tooltips.extend(tooltips)
-
     def prepare(self, dependency_id: str, json_data: Any = None) -> None:
         """Prepare Widget Spec to be validated.
 
         Args:
             dependency_id: widget dependency id.
             json_data: json data object.
         """
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/build_result.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/build_result.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/number.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/number.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/styling/number.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/number.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/styling/text.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/text.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/results/text.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/text.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/search/search.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Union
 from typing import get_args
 
 import pandas as pd
-from beartype import beartype
 
 from engineai.sdk.dashboard.data.decorator import DataSource
+from engineai.sdk.dashboard.data.http import Http
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.chart_utils import column_is_of_type
 from engineai.sdk.dashboard.widgets.search.results.number import ResultNumberItem
 from engineai.sdk.dashboard.widgets.search.results.text import ResultTextItem
 from engineai.sdk.dashboard.widgets.search.results.typing import ResultItemType
@@ -32,19 +33,19 @@
     """Specs for Search Widget."""
 
     _WIDGET_API_TYPE = "search"
     _DEPENDENCY_ID = "__SEARCH_DATA_DEPENDENCY__"
     _DEFAULT_HEIGHT = 0.6
     _FORCE_HEIGHT = True
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
-        data: Union[DataSource, pd.DataFrame],
+        data: Union[DataSource, pd.DataFrame, Http],
         selected_text_column: TemplatedStringItem,
         widget_id: Optional[str] = None,
         items: Optional[Union[TemplatedStringItem, List[ResultItemType]]] = None,
         placeholder: Optional[TemplatedStringItem] = None,
     ):
         """Construct for Search widget.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/select/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/select/group.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/group.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/select/select.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Spec for Select widget."""
 
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
 from engineai.sdk.dashboard.data import DataSource
+from engineai.sdk.dashboard.data.http import Http
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.utils import build_data
 
 from ..base import SelectableWidget
 from .exceptions import SelectValidateUniqueIDError
@@ -25,18 +26,18 @@
     _DEPENDENCY_ID = "__SELECT_DATA_DEPENDENCY__"
 
     _WIDGET_API_TYPE = "select"
 
     _DEFAULT_HEIGHT = 0.5
     _FORCE_HEIGHT = True
 
-    @beartype
+    @type_check
     def __init__(
         self,
-        data: Union[DataSource, pd.DataFrame],
+        data: Union[DataSource, pd.DataFrame, Http],
         *,
         id_column: TemplatedStringItem = "id",
         default_selection: Optional[str] = None,
         label_column: Optional[TemplatedStringItem] = None,
         widget_id: Optional[str] = None,
         label: TemplatedStringItem = "",
         label_outside: bool = True,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/__init__.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from abc import abstractmethod
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.columns.items.exceptions import (
@@ -24,15 +24,15 @@
 
 
 class Column(AbstractFactoryLinkItemsHandler):
     """Base spec for columns in a Table widget."""
 
     _ITEM_ID_TYPE: Optional[str] = None
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/category.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import MapperFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.columns.items.exceptions import (
@@ -35,15 +35,15 @@
 
 
 class CategoryColumn(Column):
     """Specifications for CategoryColumn class."""
 
     _ITEM_ID_TYPE: str = "CATEGORY"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         formatting: MapperFormatting,
         styling: Optional[Union[Palette, CategoryColumnStyling]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
@@ -24,15 +24,15 @@
 
 
 class AreaChartColumn(ChartColumn):
     """Specifications for AreaChartColumn class."""
 
     _ITEM_ID_TYPE: str = "AREA_CHART"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         data_key: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         formatting: Optional[NumberFormatting] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import InternalDataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.templated_string import build_templated_strings
 
 from ...styling.base import TableColumnStylingBase
 from ..base import Column
 from ..exceptions import TableColumnChartIncorrectLengthError
 from ..exceptions import TableColumnDataTypeError
 from ..exceptions import TableDataColumnValueKeyError
 from ..exceptions import TableDataColumnValueTypeError
@@ -98,21 +97,15 @@
             self.__reference_line = None
         elif isinstance(reference_line, (DataField)):
             self.__reference_line = InternalDataField(reference_line)
         else:
             self.__reference_line = InternalDataField(str(reference_line))
 
     def _build_styling(self) -> Any:
-        styling_spec = None
-        if self.styling:
-            styling_spec = self.styling.build()
-            key = "dataKey" if hasattr(styling_spec, "dataKey") else "valueKey"
-            setattr(styling_spec, key, build_templated_strings(items=self.data_key))
-
-        return styling_spec
+        return None if self.styling is None else self.styling.build()
 
     def _validate_list_row_data(self, *, row_data: List[Dict[str, Any]]) -> None:
         for value in row_data:
             if not isinstance(value, dict):
                 raise TableDataColumnValueTypeError(
                     data_column=self.data_column, value=value
                 )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
@@ -24,15 +24,15 @@
 
 
 class ColumnChartColumn(ChartColumn):
     """Specifications for ColumnChartColumn class."""
 
     _ITEM_ID_TYPE: str = "COLUMN_CHART"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         data_key: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         formatting: Optional[NumberFormatting] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
@@ -24,15 +24,15 @@
 
 
 class LineChartColumn(ChartColumn):
     """Specifications for LineChartColumn class."""
 
     _ITEM_ID_TYPE: str = "LINE_CHART"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         data_key: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         formatting: Optional[NumberFormatting] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Specification for staked bar chart columns in Table widget."""
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 
@@ -19,15 +18,15 @@
 
 
 class StackedBarColumn(ChartColumn):
     """Specifications for StackedBarColumn class."""
 
     _ITEM_ID_TYPE: str = "STACKED_BAR"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         data_key: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         styling: StackedBarStyling,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/country.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/country.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import enum
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import TextFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
 
@@ -35,15 +35,15 @@
 
 
 class CountryColumn(Column):
     """Specifications for CountryColumn class."""
 
     _ITEM_ID_TYPE: str = "COUNTRY"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         formatting: Optional[TextFormatting] = None,
         flag_position: FlagPositions = FlagPositions.LEFT,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import DateTimeFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
@@ -33,15 +33,15 @@
 
 
 class DatetimeColumn(Column):
     """Specifications for DatetimeColumn class."""
 
     _ITEM_ID_TYPE: str = "DATETIME"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         formatting: Optional[DateTimeFormatting] = None,
         styling: Optional[Union[Palette, DatetimeColumnStyling]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/number.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/number.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
@@ -38,15 +38,15 @@
 
 
 class NumberColumn(Column):
     """Specifications for NumberColumn class."""
 
     _ITEM_ID_TYPE: str = "NUMBER"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         formatting: Optional[NumberFormatting] = None,
         styling: Optional[Union[Palette, NumberColumnStyling]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/range.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/range.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
@@ -23,15 +23,15 @@
 
 
 class RangeColumn(Column):
     """Specifications for RangeColumn class."""
 
     _ITEM_ID_TYPE: str = "RANGE"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         formatting: Optional[NumberFormatting] = None,
         styling: Optional[Union[Palette, RangeStyling]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/text.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import TextFormatting
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.links.widget_field import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
@@ -34,23 +34,23 @@
 
 
 class TextColumn(Column):
     """Specifications for TextColumn class."""
 
     _ITEM_ID_TYPE: str = "TEXT"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         formatting: Optional[TextFormatting] = None,
         styling: Optional[Union[Palette, TextColumnStyling]] = None,
-        align: HorizontalAlignment = HorizontalAlignment.CENTER,
+        align: HorizontalAlignment = HorizontalAlignment.LEFT,
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
         sortable: bool = True,
         optional: bool = False,
     ):
         """Class TextColumn is used as text column for the Table Widget.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.actions.links import UrlLink
 
 from .base import Column
 
 
 class UrlColumn(Column):
     """Specifications for UrlColumn class."""
 
     _ITEM_ID_TYPE: str = "URL_COLUMN"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         url_tooltip: Optional[DataField] = None,
         label: Union[str, WidgetField] = "",
         hiding_priority: int = 0,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/area.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/area.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Specification for Area Chart Styling."""
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableSparklineColumnStylingBase
 
 
 class AreaChartStyling(TableSparklineColumnStylingBase):
     """Specifications for AreaChartStyling."""
 
     _API_TYPE = "SparkChartAreaStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_key: Optional[Union[str, WidgetField]] = None,
     ):
         """Construct for AreaChartStyling class.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/font.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,39 @@
-"""Specifications for styling a column with an arrow next to value."""
+"""Specification for column font styling."""
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
-from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 
 
-class ArrowStyling(TableColumnStylingBase):
-    """Specification for styling a column with an arrow next to value."""
+class FontStyling(TableColumnStylingBase):
+    """Specification for column font styling."""
 
-    _API_TYPE = "TableColumnStylingArrowInput"
+    _API_TYPE = "TableColumnStylingFontInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
+        color_spec: ColorSpec,
         data_column: Optional[Union[str, WidgetField]] = None,
-        mid: Union[float, int] = 0,
-        color_spec: Optional[ColorSpec] = None,
+        highlight_background: bool = False
     ):
-        """Construct for ArrowStyling class.
+        """Construct for FontStyling class.
 
         Args:
             data_column: id of column which values are used to determine behavior of
-                arrow. By default, will use values of column to which styling is
-                applied.
-            mid: value that determines when arrow flips up/down.
-            color_spec: spec for color of arrows. By default, used the
-                PositiveNegativeDiscreteMap.
+                color of dot. Optional if color_spec is a single color.
+            color_spec: spec for color of dot.
+            highlight_background: Highlight value background.
         """
-        super().__init__(
-            color_spec=color_spec
-            if color_spec
-            else color.PositiveNegativeDiscreteMap(),
-            data_column=data_column,
-        )
-        self.__mid = mid
+        super().__init__(data_column=data_column, color_spec=color_spec)
+        self.__highlight_background = highlight_background
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {"mid": self.__mid}
+        return {"highlightBackground": self.__highlight_background}
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Any
 from typing import Dict
 from typing import Mapping
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.exceptions import ImproperlyConfiguredError
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.styling.color import DiscreteMap
 from engineai.sdk.dashboard.styling.color import Gradient
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
@@ -26,37 +26,32 @@
 )
 
 
 class TableColumnStylingBase(AbstractFactoryLinkItemsHandler):
     """Specification for Table Column Styling Base class."""
 
     _API_TYPE: Optional[str] = None
+    _API_DATA_KEY: Optional[str] = "dataKey"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[Union[str, WidgetField]] = None,
     ):
         """Construct for TableColumnStylingBase class.
 
         Args:
             data_column: id of column which values are used for chart. By default,
                 will use values of column to which styling is applied.
             color_spec: spec for color class.
         """
         super().__init__()
-
-        self._data_column: Optional[Union[str, WidgetField]] = None
-
-        if data_column is not None:
-            self._data_column = (
-                data_column if isinstance(data_column, WidgetField) else data_column
-            )
+        self._data_column = data_column
         self.__color_spec = color_spec
 
     @property
     def color_spec(self) -> Optional[ColorSpec]:
         """Return color spec."""
         return self.__color_spec
 
@@ -125,15 +120,17 @@
             ) or (isinstance(data, dict) and self.data_column not in data):
                 raise TableColumnStylingValidationError(
                     class_name=self.__class__.__name__,
                     data_column=f"{self.data_column}",
                 )
 
     def _build_key_input(self) -> Mapping[str, Any]:
-        return {"dataKey": build_templated_strings(items=self._data_column or " ")}
+        return {
+            self._API_DATA_KEY: build_templated_strings(items=self._data_column or " ")
+        }
 
     def build(self) -> Any:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
@@ -144,9 +141,8 @@
             **self._build_extra_inputs(),
         )
 
 
 class TableSparklineColumnStylingBase(TableColumnStylingBase):
     """Specification for Table Sparkline Column Styling Base class."""
 
-    def _build_key_input(self) -> Mapping[str, Any]:
-        return {"valueKey": build_templated_strings(items=self._data_column or " ")}
+    _API_DATA_KEY: Optional[str] = "valueKey"
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Specification for styling a column with an arrow next to value."""
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 
 
 class CellStyling(TableColumnStylingBase):
     """Specification for styling a column with an arrow next to value."""
 
     _API_TYPE = "TableColumnStylingCellInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[Union[str, WidgetField]] = None,
         percentage_fill: Optional[Union[float, int]] = 1,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """Specification for styling a column with a color bar."""
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 from .exceptions import TableColumnStylingMinMaxValueError
 
 
 class ColorBarStyling(TableColumnStylingBase):
     """Specification for styling a column with a color bar."""
 
     _API_TYPE = "TableColumnStylingColorBarInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[Union[str, WidgetField]] = None,
         left_to_right: bool = True,
         min_value: Optional[Union[float, int]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/column.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/line.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-"""Specification for styling a column chart."""
+"""Specification for styling a line chart."""
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableSparklineColumnStylingBase
 
 
-class ColumnChartStyling(TableSparklineColumnStylingBase):
-    """Specification for styling a column chart."""
+class LineChartStyling(TableSparklineColumnStylingBase):
+    """Specification for styling a line chart."""
 
-    _API_TYPE = "SparkChartColumnStylingInput"
+    _API_TYPE = "SparkChartLineStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_key: Optional[Union[str, WidgetField]] = None,
     ):
-        """Construct for ColumnChartStyling class.
+        """Construct for LineChartStyling class.
 
         Args:
             data_key: Dictionary key, stored in data, that is used for chart.
                 By default, will use values of column to which styling is applied.
-            color_spec: spec for color of column chart.
+            color_spec: spec for color of line chart.
         """
         super().__init__(
             data_column=data_key,
             color_spec=color_spec,
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Specification for styling a column with a country flag to a value."""
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 
 from .base import TableColumnStylingBase
 
 
 class CountryFlagStyling(TableColumnStylingBase):
     """Specification for styling a column with a country flag to a value."""
 
     _API_TYPE = "TableColumnStylingCountryFlagInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         left: bool = True,
         data_column: Optional[Union[str, WidgetField]] = None,
     ):
         """Construct for CountryFlagStyling class.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,47 @@
-"""Specification for styling a column with an arrow next to value."""
+"""Specifications for styling a column with an arrow next to value."""
+from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 
 
-class DotStyling(TableColumnStylingBase):
-    """Specification for styling a column with a colored dot left to the value."""
+class ArrowStyling(TableColumnStylingBase):
+    """Specification for styling a column with an arrow next to value."""
 
-    _API_TYPE = "TableColumnStylingDotInput"
+    _API_TYPE = "TableColumnStylingArrowInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
-        color_spec: Optional[ColorSpec] = None,
         data_column: Optional[Union[str, WidgetField]] = None,
+        mid: Union[float, int] = 0,
+        color_spec: Optional[ColorSpec] = None,
     ):
-        """Construct for DotStyling class.
+        """Construct for ArrowStyling class.
 
         Args:
             data_column: id of column which values are used to determine behavior of
-                color of dot. Optional if color_spec is a single color.
-            color_spec: spec for color of dot.
+                arrow. By default, will use values of column to which styling is
+                applied.
+            mid: value that determines when arrow flips up/down.
+            color_spec: spec for color of arrows. By default, used the
+                PositiveNegativeDiscreteMap.
         """
         super().__init__(
             color_spec=color_spec
-            if color_spec is not None
-            else color.Palette.MINT_GREEN,
+            if color_spec
+            else color.PositiveNegativeDiscreteMap(),
             data_column=data_column,
         )
+        self.__mid = mid
+
+    def _build_extra_inputs(self) -> Dict[str, Any]:
+        return {"mid": self.__mid}
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/font.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/range.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,50 @@
-"""Specification for column font styling."""
+"""Specification for styling a column with an arrow next to value."""
+import enum
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 
 
-class FontStyling(TableColumnStylingBase):
-    """Specification for column font styling."""
+class RangeShape(enum.Enum):
+    """Range shape options."""
+
+    CIRCLE = "CIRCLE"
+    RECTANGLE = "RECTANGLE"
+
+
+class RangeStyling(TableColumnStylingBase):
+    """Specification for styling a column with a range next to value."""
 
-    _API_TYPE = "TableColumnStylingFontInput"
+    _API_TYPE = "TableColumnStylingRangeInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[Union[str, WidgetField]] = None,
-        highlight_background: bool = False
+        shape: RangeShape = RangeShape.CIRCLE,
     ):
-        """Construct for FontStyling class.
+        """Construct for RangeStyling class.
 
         Args:
             data_column: id of column which values are used to determine behavior of
-                color of dot. Optional if color_spec is a single color.
-            color_spec: spec for color of dot.
-            highlight_background: Highlight value background.
+                arrow.
+            color_spec: spec for color of range value.
+            shape: shape of range indicator.
         """
-        super().__init__(data_column=data_column, color_spec=color_spec)
-        self.__highlight_background = highlight_background
+        super().__init__(
+            data_column=data_column,
+            color_spec=color_spec,
+        )
+        self.__shape = shape
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {"highlightBackground": self.__highlight_background}
+        return {"shape": self.__shape.value}
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Specification for styling a column with an icon to a value."""
 from typing import Any
 from typing import Dict
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 
 from .base import TableColumnStylingBase
 
 
 class IconStyling(TableColumnStylingBase):
     """Specification for styling a column with an icon to a value."""
 
     _API_TYPE = "TableColumnStylingIconInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         left: bool = True,
     ):
         """Construct for IconStyling class.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/line.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/column.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-"""Specification for styling a line chart."""
+"""Specification for styling a column chart."""
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableSparklineColumnStylingBase
 
 
-class LineChartStyling(TableSparklineColumnStylingBase):
-    """Specification for styling a line chart."""
+class ColumnChartStyling(TableSparklineColumnStylingBase):
+    """Specification for styling a column chart."""
 
-    _API_TYPE = "SparkChartLineStylingInput"
+    _API_TYPE = "SparkChartColumnStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_key: Optional[Union[str, WidgetField]] = None,
     ):
-        """Construct for LineChartStyling class.
+        """Construct for ColumnChartStyling class.
 
         Args:
             data_key: Dictionary key, stored in data, that is used for chart.
                 By default, will use values of column to which styling is applied.
-            color_spec: spec for color of line chart.
+            color_spec: spec for color of column chart.
         """
         super().__init__(
             data_column=data_key,
             color_spec=color_spec,
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Specification for styling a column with a split color bar."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 from .exceptions import TableColumnStylingMinMaxValueError
@@ -20,15 +19,15 @@
     """Specification for styling a column with a split color bar.
 
     Use for positive and negative values.
     """
 
     _API_TYPE = "TableColumnStylingSplitBarInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Optional[Union[str, WidgetField]] = None,
         color_spec: Optional[ColorSpec] = None,
         min_value: Optional[Union[float, int]] = None,
         max_value: Optional[Union[float, int]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """Specification for styling the stacked bar column."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color import DiscreteMap
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 
 from .base import TableSparklineColumnStylingBase
 
 
 class StackedBarStyling(TableSparklineColumnStylingBase):
     """Specification for styling a Stack Bar chart table column."""
 
     _API_TYPE = "SparkChartStackedBarStylingInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         color_spec: DiscreteMap,
         data_column: Optional[Union[str, WidgetField]] = None,
         show_total_on_tooltip: bool = False
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     """TableHeader Levels Error."""
 
     def __init__(self, *args: object) -> None:
         """Constructor for TableHeaderLevelsError class."""
         super().__init__(None, *args)
         self.error_strings.append(
             "Please specify the 'columns' argument for the 'Table' when "
-            "using 'DataSource' as the data source. This argument is "
+            "using 'DataSource' or 'Http' as the data source. This argument is "
             "essential to determine which columns should be used. "
             "Alternatively, you can provide the data as a Pandas "
             "DataFrame for automatic column inference."
         )
 
 
 class TableDataWithoutColumnsError(TableWidgetError):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/group.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/group.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Spec for Table group column."""
 
 from typing import Any
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 
 from .exceptions import TableGroupColumnKeyNotFoundError
 
 
 class Group(AbstractFactoryLinkItemsHandler):
     """Spec for Table group column."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         data_column: Union[str, WidgetField],
         label: Union[str, WidgetField],
     ):
         """Construct Table group column.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/header.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.columns.items.text import TextColumn
 
@@ -24,15 +24,15 @@
 
 TableColumns = Union[str, Column, "Header", List[Union[str, Column, "Header"]]]
 
 
 class Header(AbstractFactoryLinkItemsHandler):
     """Spec for table header columns (i.e. above normal columns)."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         columns: TableColumns,
         label: Union[str, GenericLink],
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
     ):
         """Construct Table header columns.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/initial_state.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/initial_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Spec for Table widget state."""
 
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import cast
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 from .exceptions import TableInitialStateIncompatiblePreSelectedIndexError
 from .exceptions import TableInitialStateIncompatiblePreSelectedRowsError
 
 
 class InitialState(AbstractFactory):
     """Spec for Table widget state."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         page: int = 0,
         search_text: str = "",
         selected: Optional[List[str]] = None,
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/styling.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/styling.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Spec for Table widget styling."""
 
 from typing import Any
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class TableStyling(AbstractFactory):
     """Spec for Table widget styling."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         has_borders: bool = True,
         has_column_lines: bool = True,
         has_body_column_lines: bool = True,
         has_row_lines: bool = True,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/table/table.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,32 +4,40 @@
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 from pandas.api.types import is_datetime64_dtype
 from pandas.api.types import is_numeric_dtype
 from pandas.api.types import is_period_dtype
 
 from engineai.sdk.dashboard.base import HEIGHT_ROUND_VALUE
 from engineai.sdk.dashboard.data.decorator import DataSource
+from engineai.sdk.dashboard.data.http import Http
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting.number import NumberFormatting
 from engineai.sdk.dashboard.formatting.number import NumberScale
 from engineai.sdk.dashboard.styling.color.default_specs import (
+    PercentageAllNegativeSequentialColorGradient,
+)
+from engineai.sdk.dashboard.styling.color.default_specs import (
+    PercentageAllPositiveSequentialColorGradient,
+)
+from engineai.sdk.dashboard.styling.color.default_specs import (
     PositiveNegativeDiscreteMap,
 )
 from engineai.sdk.dashboard.styling.color.default_specs import ScoreColorDiscreteMap
-from engineai.sdk.dashboard.styling.color.default_specs import SequentialColorGradient
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.pandas_utils import are_values_relative
+from engineai.sdk.dashboard.widgets.pandas_utils import only_integers
 from engineai.sdk.dashboard.widgets.pandas_utils import only_negative_or_positive_values
+from engineai.sdk.dashboard.widgets.pandas_utils import only_negative_values
 from engineai.sdk.dashboard.widgets.pandas_utils import only_positive_values
 from engineai.sdk.dashboard.widgets.table.columns.items.datetime import DatetimeColumn
 from engineai.sdk.dashboard.widgets.table.columns.items.number import NumberColumn
 from engineai.sdk.dashboard.widgets.table.columns.items.text import TextColumn
 from engineai.sdk.dashboard.widgets.table.columns.styling.arrow import ArrowStyling
 from engineai.sdk.dashboard.widgets.table.columns.styling.cell import CellStyling
 from engineai.sdk.dashboard.widgets.table.columns.styling.color_bar import (
@@ -78,18 +86,18 @@
     _SCORE_CHANGE_MIN = -5
     _SCORE_CHANGE_MAX = 5
 
     _WINSORIZATION_LIMIT_LOWER = 0.05
     _WINSORIZATION_LIMIT_UPPER = 0.95
     _PERCENTAGE_LIMIT = 2
 
-    @beartype
+    @type_check
     def __init__(
         self,
-        data: Union[DataSource, pd.DataFrame],
+        data: Union[DataSource, pd.DataFrame, Http],
         *,
         columns: Optional[TableColumns] = None,
         widget_id: Optional[str] = None,
         title: WidgetTitleType = None,
         styling: Optional[TableStyling] = None,
         row_selection: int = 1,
         rows_per_page: int = 10,
@@ -200,17 +208,19 @@
                     )
                 item.prepare()
 
         self._json_data = kwargs.get("json_data", None)
 
     def __generate_columns(
         self,
-        data: Union[DataSource, pd.DataFrame],
+        data: Union[DataSource, pd.DataFrame, Http],
         columns: Optional[TableColumns],
     ) -> List[Union[Header, Column]]:
+        if isinstance(data, Http) and columns is None:
+            raise TableNoColumnError()
         self.__validate_columns(data=data, columns=columns)
         if self.__can_set_columns_from_data(data, columns):
             return self.__get_columns_from_data(data=data)
         else:
             return self.__generate_columns_from_argument(columns=columns)
 
     @staticmethod
@@ -243,23 +253,36 @@
             if self._is_numeric_and_relative(data, column):
                 items.append(
                     NumberColumn(
                         data_column=column,
                         formatting=NumberFormatting(scale=NumberScale.DYNAMIC_RELATIVE),
                         styling=ArrowStyling()
                         if not only_negative_or_positive_values(data[column])
-                        else ColorBarStyling(color_spec=SequentialColorGradient())
+                        else ColorBarStyling(
+                            min_value=0,
+                            max_value=1,
+                            color_spec=PercentageAllPositiveSequentialColorGradient(),
+                        )
                         if only_positive_values(data[column])
+                        else ColorBarStyling(
+                            min_value=0,
+                            max_value=-1,
+                            color_spec=PercentageAllNegativeSequentialColorGradient(),
+                        )
+                        if only_negative_values(data[column])
                         else None,
                     )
                 )
             elif is_numeric_dtype(data[column]):
                 items.append(
                     NumberColumn(
                         data_column=column,
+                        formatting=NumberFormatting(decimals=0)
+                        if only_integers(data[column])
+                        else None,
                         styling=CellStyling(color_spec=ScoreColorDiscreteMap())
                         if self._has_positive_score_values(data[column])
                         else SplitBarStyling()
                         if self._has_score_change_values(data[column])
                         else CellStyling(color_spec=PositiveNegativeDiscreteMap())
                         if self._has_score_values(data[column])
                         else FontStyling(color_spec=PositiveNegativeDiscreteMap())
@@ -272,25 +295,30 @@
             else:
                 items.append(TextColumn(data_column=column))
         return items
 
     def _is_numeric_and_relative(
         self, data: pd.DataFrame, column: pd.DataFrame
     ) -> bool:
-        return is_numeric_dtype(data[column]) and are_values_relative(
-            data[column],
+        non_na_column = data[column].dropna()
+        return is_numeric_dtype(non_na_column) and are_values_relative(
+            non_na_column,
             self._WINSORIZATION_LIMIT_UPPER,
             self._WINSORIZATION_LIMIT_LOWER,
             self._PERCENTAGE_LIMIT,
         )
 
     def _has_positive_score_values(self, column: pd.DataFrame) -> bool:
-        return (
-            column.ge(self._POSITIVE_SCORE_MIN) & column.le(self._POSITIVE_SCORE_MAX)
-        ).all()
+        non_na_column = column.dropna()
+        return bool(
+            (
+                non_na_column.ge(self._POSITIVE_SCORE_MIN)
+                & non_na_column.le(self._POSITIVE_SCORE_MAX)
+            ).all()
+        )
 
     def _has_score_change_values(self, column: pd.DataFrame) -> bool:
         scores = column.ge(self._SCORE_MIN) & column.le(self._SCORE_MAX)
         score_changes = column.ge(self._SCORE_CHANGE_MIN) & column.le(
             self._SCORE_CHANGE_MAX
         )
         if (
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/__init__.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Specs for a Base Timeseries chart."""
 
 from typing import Any
 from typing import Mapping
 from typing import Optional
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class TimeseriesBaseAxis(AbstractFactoryLinkItemsHandler):
     """Specs for a Base Timeseries chart."""
 
     _API_TYPE: Optional[str] = None
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         enable_crosshair: bool = False,
     ) -> None:
         """Construct TimeseriesBaseAxis.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Set
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import AxisNumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScale
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScaleDynamic
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import build_axis_scale
@@ -26,15 +26,15 @@
 from ...series.typing import TimeseriesSeries
 from ..base import TimeseriesBaseAxis
 
 
 class BaseTimeseriesYAxis(TimeseriesBaseAxis):
     """Specs for y axis of a Timeseries chart."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         formatting: Optional[AxisNumberFormatting] = None,
         title: Union[str, WidgetField] = "",
         enable_crosshair: bool = False,
         scale: Optional[AxisScale] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Union
 from typing import cast
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import AxisNumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScale
 
 from ...series.typing import TimeseriesSeries
 from .base import BaseTimeseriesYAxis
 
 
 class YAxis(BaseTimeseriesYAxis):
     """Specs for y axis of a Timeseries chart."""
 
     _API_TYPE = "TimeseriesWidgetChartStandardYAxisInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         formatting: Optional[AxisNumberFormatting] = None,
         title: Union[str, WidgetField] = "",
         enable_crosshair: bool = False,
         scale: Optional[AxisScale] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Union
 from typing import cast
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import AxisNumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScale
 
 from ...series.typing import TimeseriesSeries
 from .base import BaseTimeseriesYAxis
 
 
 class MirrorYAxis(BaseTimeseriesYAxis):
     """Specs for mirror y axis of a Timeseries chart."""
 
     _API_TYPE = "TimeseriesWidgetChartMirrorYAxisInput"
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         formatting: Optional[AxisNumberFormatting] = None,
         title: Union[str, WidgetField] = "",
         enable_crosshair: bool = False,
         scale: Optional[AxisScale] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/chart.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Spec for charts in a Timeseries widget."""
 
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
     build_tooltip_item,
@@ -34,15 +34,15 @@
 
 class Chart(AbstractFactoryLinkItemsHandler):
     """Spec for charts in a Timeseries widget."""
 
     _HEIGHT_TIMESERIES_CHART_TITLE = 0.19
     __height: float  # Added here to use property logic for all entries
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         left_y_axis: Optional[Union[YAxisSpec, TimeseriesSeries]] = None,
         height_percentage: Optional[Union[float, int]] = None,
         height: Union[float, int] = 3,
         x_axis: Optional[XAxis] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/consts.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/consts.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/enums.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,26 +242,14 @@
         super().__init__(None, *args)
         self.error_strings.append(
             "`set_series` methods was called without any instances. "
             "Please define at least one."
         )
 
 
-class TimeseriesTooltipsEmptyDefinitionError(TimeseriesError):
-    """Timeseries Tooltips Empty Definition Error."""
-
-    def __init__(self, *args: object) -> None:
-        """Constructor for TimeseriesTooltipsEmptyDefinitionError class."""
-        super().__init__(None, *args)
-        self.error_strings.append(
-            "`add_tooltips` method was called without any tooltips instances. "
-            "Please define at least one tooltip."
-        )
-
-
 class TimeseriesAxisEmptyDefinitionError(TimeseriesError):
     """Timeseries Axis Empty Definition Error."""
 
     def __init__(self, *args: object) -> None:
         """Construct for TimeseriesAxisEmptyDefinitionError class.
 
         Args:
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/legend.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/legend.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-"""Spec for legend of a timeseries widget."""
+"""Spec for legend of a categorical widget."""
 from typing import Any
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.enum.legend_position import LegendPosition
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class Legend(AbstractFactory):
-    """Spec for legend of a timeseries widget."""
+    """Spec for legend of a categorical widget.
 
-    @beartype
-    def __init__(self, *, position: LegendPosition = LegendPosition.BOTTOM):
-        """Construct a legend for a timeseries widget.
+    Args:
+        position: location of position relative to data, charts.
+    """
 
-        Args:
-            position: location of position relative to data, charts.
-        """
+    @type_check
+    def __init__(self, *, position: LegendPosition = LegendPosition.BOTTOM):
+        """Construct a legend for a categorical widget."""
         super().__init__()
         self.__position = position
 
-    @property
-    def position(self) -> LegendPosition:
-        """Returns the current Legend Position."""
-        return self.__position
-
     def build(self) -> Any:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
         return generate_input(
-            "TimeseriesWidgetLegendInput", position=self.__position.value
+            "ContinuousCartesianWidgetLegendInput", position=self.__position.value
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/navigator.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/navigator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Spec for navigator of a timeseries widget."""
 
 from typing import Any
 from typing import Optional
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.base import WidgetTitleType
 
 from .exceptions import TimeseriesNavigatorEmptyDefinitionError
 from .series.typing import TimeseriesSeries
 
 
 class Navigator(AbstractFactoryLinkItemsHandler):
     """Spec for navigator of a timeseries widget."""
 
-    @beartype
+    @type_check
     def __init__(
         self, *series: TimeseriesSeries, title: Optional[WidgetTitleType] = None
     ) -> None:
         """Construct a navigator for a timeseries widget.
 
         Args:
             title: title to be added to navigator
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 from datetime import datetime
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.utils import generate_input
 
 from ..exceptions import TimeseriesPeriodSelectorDatesDefinitionError
 
 
 class CustomPeriod(AbstractFactoryLinkItemsHandler):
     """Spec for a custom period for a period selector."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         label: Optional[str] = None,
         start_date: Union[str, datetime],
         end_date: Union[str, datetime]
     ):
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """Spec for period selector of a timeseries widget."""
 
 from typing import Any
 from typing import List
 from typing import Optional
 
-from beartype import beartype
-
 from engineai.sdk.dashboard.base import AbstractFactory
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 from ..exceptions import TimeseriesPeriodSelectorHiddenPeriodsError
 from ..exceptions import TimeseriesPeriodSelectorNoAvailableDefaultOptionError
 from .custom_period import CustomPeriod
 from .period import PeriodType
 from .period import build_timeseries_period
 from .standard import Period
 
 
 class PeriodSelector(AbstractFactory):
     """Spec for period selector of a timeseries widget."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *periods: PeriodType,
         default_selection: Optional[int] = None,
         visible: bool = True,
     ) -> None:
         """Construct period selector.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/area.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/area.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
@@ -26,15 +26,15 @@
 class AreaSeries(TimeseriesBaseSeries):
     """Spec for a area series of a Timeseries widget."""
 
     _API_TYPE = "TimeseriesWidgetAreaSeriesInput"
     _INPUT_KEY = "area"
     _styling_class = AreaSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         name: Optional[Union[str, GenericLink]] = None,
         styling: Optional[Union[Palette, AreaSeriesStyling]] = None,
         entity: Optional[Entities] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
@@ -29,15 +29,15 @@
 class AreaRangeSeries(TimeseriesBaseSeries):
     """Spec for a area range series of a Timeseries widget."""
 
     _API_TYPE = "TimeseriesWidgetAreaRangeSeriesInput"
     _INPUT_KEY = "range"
     _styling_class = AreaRangeSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         low_data_column: Union[str, WidgetField],
         high_data_column: Union[str, WidgetField],
         name: Union[str, GenericLink],
         styling: Optional[Union[Palette, AreaRangeSeriesStyling]] = None,
@@ -69,15 +69,17 @@
         """
         super().__init__(
             name=name,
             data_column=None,
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
-            styling=styling,
+            styling=AreaRangeSeriesStyling(color_spec=styling)
+            if isinstance(styling, Palette)
+            else styling,
             entity=entity,
             right_axis=right_axis,
             tooltips=tooltips,
         )
         self._low_data_column: Union[str, WidgetField] = (
             low_data_column if isinstance(low_data_column, str) else low_data_column
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/base.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Spec for a area series of a Timeseries widget."""
 import re
-import warnings
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color.palette import qualitative_palette
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.series.base import ChartSeriesBase
@@ -27,29 +26,27 @@
 from engineai.sdk.dashboard.widgets.components.charts.styling.typing import (
     SeriesStyling,
 )
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
     build_tooltip_item,
 )
 
-from ...components.charts.typing import TooltipItem
 from ...components.charts.typing import TooltipItems
 from ...utils import get_tooltips
-from ..exceptions import TimeseriesTooltipsEmptyDefinitionError
 from ..exceptions import TimeseriesValidateSeriesDataColumnNotFound
 from ..transform import Transform
 
 
 class TimeseriesBaseSeries(ChartSeriesBase):
     """Spec for a Base Series of a Timeseries widget."""
 
     _styling_class: Optional[Type[ColoredSeriesStyling]] = None
     _INPUT_KEY: Optional[str] = None
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         name: Optional[Union[str, GenericLink]] = None,
         data_column: Optional[Union[str, GenericLink]],
         styling: Optional[SeriesStyling] = None,
         entity: Optional[Entities] = None,
@@ -99,26 +96,14 @@
         """Returns styling Input Key argument value."""
         if self._INPUT_KEY is None:
             raise NotImplementedError(
                 f"Class {self.__class__.__name__}._INPUT_KEY not defined."
             )
         return self._INPUT_KEY
 
-    def add_tooltips(self, *tooltips: TooltipItem) -> "TimeseriesBaseSeries":
-        """Add extra tooltip items (i.e. in addition to the value of this series)."""
-        warnings.warn(
-            "`add_tooltips` is deprecated. Use `tooltips` in constructor, instead.",
-            DeprecationWarning,
-        )
-        if len(tooltips) == 0:
-            raise TimeseriesTooltipsEmptyDefinitionError()
-
-        self._tooltip_items.extend(tooltips)
-        return self
-
     def add_transforms(self, *transform: Transform) -> "TimeseriesBaseSeries":
         """Add transform (i.e. apply transform to series data with low column data).
 
         Returns:
             AreaSeries: reference to this series to facilitate inline
                 manipulation
         """
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
@@ -37,15 +37,15 @@
 class BubbleSeries(TimeseriesBaseSeries):
     """Spec for a bubble series of a Timeseries widget."""
 
     _API_TYPE = "TimeseriesWidgetBubbleSeriesInput"
     _INPUT_KEY = "bubble"
     _styling_class = BubbleCircleSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         bubble_size_data_column: Union[str, WidgetField],
         name: Optional[Union[str, GenericLink]] = None,
         bubble_name: Optional[Union[str, WidgetField]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/column.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/point.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-"""Spec for a column series of a Timeseries widget."""
+"""Spec for a point series of a Timeseries widget."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
     Entities,
 )
-from engineai.sdk.dashboard.widgets.components.charts.styling import ColumnSeriesStyling
+from engineai.sdk.dashboard.widgets.components.charts.styling import PointSeriesStyling
 
 from ...components.charts.typing import TooltipItems
 from .base import TimeseriesBaseSeries
 
 
-class ColumnSeries(TimeseriesBaseSeries):
-    """Spec for a column series of a Timeseries widget."""
+class PointSeries(TimeseriesBaseSeries):
+    """Spec for a point series of a Timeseries widget."""
 
-    _API_TYPE = "TimeseriesWidgetColumnSeriesInput"
-    _INPUT_KEY = "column"
-    _styling_class = ColumnSeriesStyling
+    _API_TYPE = "TimeseriesWidgetPointSeriesInput"
+    _INPUT_KEY = "point"
+    _styling_class = PointSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         name: Optional[Union[str, GenericLink]] = None,
-        styling: Optional[Union[Palette, ColumnSeriesStyling]] = None,
+        styling: Optional[Union[Palette, PointSeriesStyling]] = None,
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct column series.
+        """Construct point series.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for the values of
                 this series.
             name: series name (shown in legend and tooltip).
             styling: styling spec, by default uses the values from the sequential
                 palette.
@@ -63,15 +63,15 @@
         """
         super().__init__(
             name=name,
             data_column=data_column,
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
-            styling=ColumnSeriesStyling(color_spec=styling)
+            styling=PointSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling,
             entity=entity,
             right_axis=right_axis,
             tooltips=tooltips,
         )
 
@@ -83,10 +83,8 @@
         """
         super().validate(data=data)
 
         if self._entity is not None and isinstance(self._entity, CountryEntity):
             self._entity.validate_country_code()
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {
-            "transforms": [transform.build() for transform in self._transforms],
-        }
+        return {"transforms": [transform.build() for transform in self._transforms]}
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
@@ -29,15 +29,15 @@
 class ErrorBarSeries(TimeseriesBaseSeries):
     """Spec for error bar series of a Timeseries widget."""
 
     _API_TYPE = "TimeseriesWidgetErrorBarSeriesInput"
     _INPUT_KEY = "errorBar"
     _styling_class = ErrorBarSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         low_data_column: Union[str, WidgetField],
         high_data_column: Union[str, WidgetField],
         name: Optional[Union[str, GenericLink]] = None,
         styling: Optional[Union[Palette, ErrorBarSeriesStyling]] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/line.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/line.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
@@ -26,15 +26,15 @@
 class LineSeries(TimeseriesBaseSeries):
     """Spec for a line series of a Timeseries widget."""
 
     _API_TYPE = "TimeseriesWidgetLineSeriesInput"
     _INPUT_KEY = "line"
     _styling_class = LineSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         name: Optional[Union[str, GenericLink]] = None,
         styling: Optional[Union[Palette, LineSeriesStyling]] = None,
         entity: Optional[Entities] = None,
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/point.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-"""Spec for a point series of a Timeseries widget."""
+"""Spec for a scatter series of a Timeseries widget."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
     Entities,
 )
-from engineai.sdk.dashboard.widgets.components.charts.styling import PointSeriesStyling
+from engineai.sdk.dashboard.widgets.components.charts.styling import (
+    ScatterSeriesStyling,
+)
 
 from ...components.charts.typing import TooltipItems
 from .base import TimeseriesBaseSeries
 
 
-class PointSeries(TimeseriesBaseSeries):
-    """Spec for a point series of a Timeseries widget."""
+class ScatterSeries(TimeseriesBaseSeries):
+    """Spec for a scatter series of a Timeseries widget."""
 
-    _API_TYPE = "TimeseriesWidgetPointSeriesInput"
-    _INPUT_KEY = "point"
-    _styling_class = PointSeriesStyling
+    _API_TYPE = "TimeseriesWidgetScatterSeriesInput"
+    _INPUT_KEY = "scatter"
+    _styling_class = ScatterSeriesStyling
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         name: Optional[Union[str, GenericLink]] = None,
-        styling: Optional[Union[Palette, PointSeriesStyling]] = None,
+        styling: Optional[Union[Palette, ScatterSeriesStyling]] = None,
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct point series.
+        """Construct scatter series.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for the values of
                 this series.
             name: series name (shown in legend and tooltip).
             styling: styling spec, by default uses the values from the sequential
                 palette.
@@ -63,15 +65,15 @@
         """
         super().__init__(
             name=name,
             data_column=data_column,
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
-            styling=PointSeriesStyling(color_spec=styling)
+            styling=ScatterSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling,
             entity=entity,
             right_axis=right_axis,
             tooltips=tooltips,
         )
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/series/typing.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/timeseries.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 from typing import cast
 
 import pandas as pd
-from beartype import beartype
 
 from engineai.sdk.dashboard import formatting
 from engineai.sdk.dashboard.base import HEIGHT_ROUND_VALUE
 from engineai.sdk.dashboard.data import DataSource
+from engineai.sdk.dashboard.data.http import Http
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.default_specs import (
     PositiveNegativeDiscreteMap,
 )
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.toolbar import build_chart_toolbar
@@ -58,18 +59,18 @@
     _HEIGHT_TIMESERIES_PERIOD_SELECTOR = 0.32
     _HEIGHT_TIMESERIES_PERIOD_NAVIGATOR = 0.48
     _HEIGHT_TIMESERIES_LEGENDS_BOTTOM = 0.18
     _HEIGHT_TIMESERIES_LEGENDS_BOTTOM_GROUPED = 0.37
     _WIDGET_API_TYPE = "timeseries"
     _DEPENDENCY_ID = "__TIMESERIES_DATA_DEPENDENCY__"
 
-    @beartype
+    @type_check
     def __init__(
         self,
-        data: Union[DataSource, pd.DataFrame],
+        data: Union[DataSource, pd.DataFrame, Http],
         *,
         date_column: Optional[TemplatedStringItem] = None,
         widget_id: Optional[str] = None,
         period_selector: Optional[PeriodSelector] = None,
         title: Optional[WidgetTitleType] = None,
         legend: Optional[LegendPosition] = None,
         navigator: Optional[Union[Navigator, TimeseriesSeries]] = None,
@@ -241,15 +242,16 @@
                         }
                         if spec_class == NumberTooltipItem
                         else {
                             "styling": LineSeriesStyling(
                                 color_spec=PositiveNegativeDiscreteMap(),
                                 data_column=element,
                             )
-                            if self.__has_positive_and_negative_value(data[element])
+                            if len(group) == 1
+                            and self.__has_positive_and_negative_value(data[element])
                             else None,
                         }
                     ),
                 )
             )
 
         return result
@@ -274,15 +276,15 @@
         self, navigator: Optional[Union[Navigator, TimeseriesSeries]]
     ) -> None:
         if navigator is None or isinstance(navigator, Navigator):
             self.__navigator = navigator
         else:
             self.__navigator = Navigator(navigator)
 
-    @beartype
+    @type_check
     def set_series(self, *items: Union[str, TimeseriesSeries]) -> "Timeseries":
         """Set series to a chart in timeseries widget.
 
         Args:
             items: series to be added to timeseries widget, using this method you can
                 add multiple series to the same chart. If you want to add multiple
                 charts to the same widget, use set_charts method instead.
@@ -371,15 +373,15 @@
         series: List[TimeseriesSeries] = [
             item
             for item in list(items)
             if not isinstance(item, str) and item.is_right_axis
         ]
         return YAxis().add_series(*series) if len(series) > 0 else None
 
-    @beartype
+    @type_check
     def set_charts(self, *items: Union[str, TimeseriesSeries, Chart]) -> "Timeseries":
         """Set chart(s) into timeseries widget.
 
         Args:
             items: chart(s) to be added to timeseries widget, using this method you
                 can add multiple charts to the same widget.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/timeseries/transform.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Spec for legend of a timeseries widget."""
 from typing import Any
 from typing import Optional
 from typing import Union
 
-from beartype import beartype
-
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.utils import generate_input
 
 from .enums import TransformChoices
 from .exceptions import TimeseriesTransformScalarRequiredError
 
 
 class Transform(AbstractFactoryLinkItemsHandler):
     """Spec for transforms of a timeseries series."""
 
-    @beartype
+    @type_check
     def __init__(
         self,
         *,
         transform: TransformChoices,
         scalar: Optional[Union[float, int]] = None,
     ):
         """Construct a transform for a timeseries widget.
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/toggle/exceptions.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/toggle/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/toggle/toggle.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/toggle/toggle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Spec for Toggle Widget."""
 
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import pandas as pd
-from beartype import beartype
 
 from engineai.sdk.dashboard.data import DataSource
+from engineai.sdk.dashboard.data.http import Http
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.utils import build_data
 
 from ..base import SelectableWidget
 from .exceptions import ToggleValidateValueError
@@ -21,18 +22,18 @@
     """Spec for Toggle Widget."""
 
     _DEPENDENCY_ID = "__TOGGLE_DATA_DEPENDENCY__"
     _WIDGET_API_TYPE = "toggle"
     _DEFAULT_HEIGHT = 0.5
     _FORCE_HEIGHT = True
 
-    @beartype
+    @type_check
     def __init__(
         self,
-        data: Union[DataSource, pd.DataFrame],
+        data: Union[DataSource, pd.DataFrame, Http],
         *,
         id_column: str = "id",
         label: Union[str, WidgetField] = "",
         label_column: Optional[str] = None,
         widget_id: Optional[str] = None,
         default_selection: Optional[str] = None,
     ) -> None:
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/dashboard/widgets/utils.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/internal/authentication/auth0.py` & `engineai_sdk-0.83.1/engineai/sdk/internal/authentication/auth0.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,8 +19,14 @@
     },
     "api.engineai.com": {
         "device_code_url": "https://login.engineai.com/oauth/device/code",
         "token_url": "https://login.engineai.com/oauth/token",
         "client_id": "PeBZtJkx9cFmoDUY7v6wlXBVA1I2Wigd",
         "audience": "https://api.dystematic.com",
     },
+    "localhost:4000": {
+        "device_code_url": "https://login.dystematic.dev/oauth/device/code",
+        "token_url": "https://login.dystematic.dev/oauth/token",
+        "client_id": "UxR3Nhc03f0MlURPGKK4W7uuj0m8ZH9t",
+        "audience": "http://api.dystematic.local:4000",
+    },
 }
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/internal/graphql_dataclasses/schema.py` & `engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/schema.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/internal/graphql_dataclasses/types.py` & `engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/types.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.49.2/engineai/sdk/internal/rubik/rubik.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/decorator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,469 +1,377 @@
-"""Rubik module."""
-import concurrent.futures
+"""Data Decorator Module."""
+import functools
+import inspect
+import itertools
 import logging
-import os
-import queue
-from pathlib import Path
-from time import perf_counter_ns
-from typing import TYPE_CHECKING
 from typing import Any
+from typing import Callable
 from typing import Dict
-from typing import Final
 from typing import Iterable
-from typing import Iterator
-from typing import KeysView
 from typing import List
-from typing import Mapping
-from typing import MutableMapping
 from typing import Optional
+from typing import Set
 from typing import Tuple
-from typing import TypeVar
 from typing import Union
 from typing import cast
-from typing import overload
 
-import brotli
-import fsspec
-from azure.storage.blob import ContentSettings
-from pandas import DataFrame
-
-from engineai.sdk.internal.rubik.serialization import default_deserialize
-from engineai.sdk.internal.rubik.serialization import default_serialize
-
-if TYPE_CHECKING:
-    from _typeshed import SupportsKeysAndGetItem
-
-_COMPRESSION_MIN_LENGTH: Final[int] = 1_000  # 1Kb
-_THREAD_POOL_MAX_WORKERS: Final[int] = 8
-_DATA_EXT: Final[str] = ".json"
-_SCHEMA_EXT: Final[str] = ".schema" + _DATA_EXT
-
-_VT_co = TypeVar("_VT_co", covariant=True)
-DataT = Union[
-    bool,
-    int,
-    float,
-    str,
-    List[Any],
-    Dict[str, Any],
-    DataFrame,
-]
-"""Type representing possible data values."""
+import pandas as pd
 
-logger = logging.getLogger(__name__)
-
-
-class ThreadPoolExecutorWithQueueSizeLimit(concurrent.futures.ThreadPoolExecutor):
-    """`ThreadPoolExecutorWithQueueSizeLimit` class."""
-
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
-        """Initializes a `ThreadPoolExecutorWithQueueSizeLimit` instance."""
-        super().__init__(*args, **kwargs)
-        self._work_queue = cast("queue.SimpleQueue[Any]", queue.Queue(maxsize=50))
-
-
-class RubikKeysViewStartsWith(KeysView[str]):
-    """KeysView implementation with support for starts_with."""
-
-    _mapping: "Rubik"
-    _starts_with: str
-
-    def __init__(self, mapping: "Rubik", starts_with: str) -> None:
-        """Instantiates a `RubikKeysViewStartsWith` object."""
-        super().__init__(mapping)
-        self._starts_with = starts_with
-
-    def __len__(self) -> int:
-        return sum(1 for _ in self.__iter__())
-
-    def __contains__(self, key: object) -> bool:
-        if not isinstance(key, str):
-            return False
-        return key in self.__iter__()
-
-    def __iter__(self) -> Iterator[str]:
-        base_path_len = len(str(Path(self._mapping.fs_mapper.root))) + 1
-
-        def _walk(base_path: str, starts_with: str) -> Iterable[str]:
-            for path, dirs, files in self._mapping.fs_mapper.fs.walk(
-                base_path, maxdepth=1
-            ):
-                base_key = path[base_path_len:]
-
-                for dir_ in dirs:
-                    key = os.path.join(base_key, dir_)
-                    if key.startswith(starts_with[0 : len(key)]):
-                        yield from _walk(f"{path}/{dir_}", starts_with)
-
-                for file in files:
-                    if file.endswith(_SCHEMA_EXT):
-                        continue
+from engineai.sdk.dashboard.clients.storage import Storage
+from engineai.sdk.dashboard.clients.storage import StorageConfig
+from engineai.sdk.dashboard.config import SKIP_DATA_VALIDATION
+from engineai.sdk.dashboard.data.exceptions import DataProcessError
+from engineai.sdk.dashboard.data.exceptions import DataRouteWithArgumentsError
+from engineai.sdk.dashboard.data.exceptions import DataValidationError
+from engineai.sdk.dashboard.exceptions import BaseDataValidationError
+from engineai.sdk.dashboard.interface import OperationInterface as OperationItem
+from engineai.sdk.dashboard.links import WidgetField
+from engineai.sdk.dashboard.links.typing import GenericLink
+
+from .duplicated import DuplicatesChecker
+from .enums import StorageType
+from .io_handler import IOReader
+from .io_handler import IOWriter
+from .manager.interface import DependencyManagerInterface as DependencyManager
+from .manager.interface import StaticDataType
 
-                    key = os.path.join(base_key, file)[: -len(_DATA_EXT)]
-                    if key.startswith(starts_with):
-                        yield key
-
-        yield from _walk(self._mapping._base_path, self._starts_with)
+Func = Callable[..., StaticDataType]
 
+logger = logging.getLogger(__name__)
 
-class Rubik(MutableMapping[str, DataT]):
-    """The `Rubik` class."""
 
-    __executor: Optional[ThreadPoolExecutorWithQueueSizeLimit]
-    _base_path: str
-    _protocol: str
-    _fs_mapper: fsspec.mapping.FSMap
+class DataSource:
+    """Decorator Class that stores data in the Dashboard Storage."""
 
     def __init__(
         self,
-        base_path: str,
-        protocol: str,
-        storage_options: Optional[Dict[str, Any]] = None,
+        func: Union[Func, StaticDataType],
+        *args: GenericLink,
+        operations: Optional[List[OperationItem]] = None,
+        base_path: Optional[str] = None,
+        storage_type: Optional[StorageType] = None,
+        **kwargs: Any,
     ) -> None:
-        """Instantiates a `Rubik` object.
-
-        Args:
-            base_path (str): The rubik's base path.
-            protocol (str): A protocol.
-            storage_options (Dict[str, Any]): Backend parameters.
-        """
-        self.__executor = None
-        self._base_path = base_path
-        self._protocol = protocol
-
-        default_options = {
-            "create": True,
-            "skip_instance_cache": True,
-            "use_listings_cache": False,
-        }
-        storage_options = storage_options or {}
-        self._fs_mapper = fsspec.get_mapper(
-            f"{protocol}://{base_path}",
-            **{**default_options, **storage_options},
+        """Decorator Class that stores data in the Dashboard Storage."""
+        self.func: Func = (
+            cast(Func, (lambda: func))
+            if isinstance(func, (pd.DataFrame, Dict))
+            else func
         )
 
-    @property
-    def fs_mapper(self) -> fsspec.mapping.FSMap:
-        """The rubik's fs mapper.
-
-        Returns:
-            fsspec.mapping.FSMap: A fs mapper.
-        """
-        return self._fs_mapper
-
-    def __read_schema(self, key: str, /) -> Optional[bytes]:
-        try:
-            return self._read(key + _SCHEMA_EXT)
-        except KeyError:
-            return None
-
-    def __getitem__(self, key: str, /) -> DataT:
-        serialized_value = self._read(key + _DATA_EXT)
-        value: DataT = default_deserialize(
-            serialized_value,
-            schema=lambda: self.__read_schema(key),
-        )
-        return value
-
-    def __setitem__(self, key: str, value: Optional[DataT], /) -> None:
-        serialized_value, serialized_schema = default_serialize(value)
-        if isinstance(value, list):
-            try:
-                self.__delitem__(key + _SCHEMA_EXT)
-            except KeyError:
-                pass
-
-        self._write(key + _DATA_EXT, serialized_value)
-
-        if serialized_schema is not None:
-            self._write(key + _SCHEMA_EXT, serialized_schema)
-
-    def __delitem__(self, key: str, /) -> None:
-        self._fs_mapper.__delitem__(key + _DATA_EXT)
-        try:
-            self.__delitem__(key + _SCHEMA_EXT)
-        except KeyError:
-            pass
-
-    def __iter__(self) -> Iterator[str]:
-        return (x[: -len(_DATA_EXT)] for x in self._fs_mapper.__iter__())
-
-    def __len__(self) -> int:
-        return cast(int, self._fs_mapper.__len__())
-
-    def __contains__(self, key: object, /) -> bool:
-        return cast(
-            bool,
-            self._fs_mapper.__contains__(self._fs_mapper._key_to_str(key) + _DATA_EXT),
-        )
-
-    def __del__(self) -> None:
-        if self.__executor is not None:
-            self.__executor.shutdown()
-
-    def __repr__(self) -> str:
-        return (
-            "<"
-            f"{self.__class__.__name__} ("
-            f"base_path={self.base_path},"
-            f"protocol={self._protocol}"
-            ")>"
+        self.args: Tuple[GenericLink, ...] = args
+        self.__base_path = (
+            base_path
+            if base_path is not None
+            else f"{self.func.__module__}.{self.func.__name__}".replace(".", "/")
         )
+        self.__separator = "/"
+        self.__storage_type = storage_type
+        self.kwargs: Dict[str, Any] = kwargs
+        self.__operations: Optional[List[OperationItem]] = operations
+        self.__component: DependencyManager
 
     @property
-    def _executor(self) -> ThreadPoolExecutorWithQueueSizeLimit:
-        if self.__executor is None:
-            self.__executor = ThreadPoolExecutorWithQueueSizeLimit(
-                max_workers=_THREAD_POOL_MAX_WORKERS,
-                thread_name_prefix="rubik_ops",
-            )
-
-        return self.__executor
+    def component(self) -> DependencyManager:
+        """Component."""
+        return self.__component
+
+    @component.setter
+    def component(self, component: DependencyManager) -> None:
+        """Set component."""
+        self.__component = component
 
     @property
-    def base_path(self) -> str:
-        """The rubik's base path.
-
-        Returns:
-            str: A path like object.
-        """
-        return self._base_path
+    def storage_type(self) -> StorageType:
+        """Storage type."""
+        if self.__storage_type is None:
+            raise NotImplementedError("Storage type not defined.")
+        return self.__storage_type
+
+    @storage_type.setter
+    def storage_type(self, storage_type: StorageType) -> None:
+        """Set storage type."""
+        if self.__storage_type is None:
+            self.__storage_type = storage_type
 
     @property
-    def protocol(self) -> str:
-        """The rubik's protocol.
+    def operations(self) -> Optional[List[OperationItem]]:
+        """Get Operations."""
+        return self.__operations
+
+    def __validate_route_args(self, component: Any) -> None:
+        if component.data_id == "route" and self.args:
+            raise DataRouteWithArgumentsError()
+
+    def __check_http_dependencies(self) -> None:
+        if len(self.args) > 0 and any("http" in repr(arg) for arg in self.args):
+            raise DataProcessError(
+                data_id=self.component.data_id,
+                class_name=self.component.__class__.__name__,
+                error_string="Currently, HTTP dependencies are not supported "
+                "as data source's inputs.",
+                function_name=self.func.__name__,
+                options=None,
+                function_arguments=self.func_args,
+            )
 
-        Returns:
-            str: A protocol.
+    @classmethod
+    def decorator(
+        cls,
+        _func: Optional[Func] = None,
+        *,
+        storage_type: Optional[StorageType] = None,
+    ) -> Any:
+        """Decorator to store data in the Dashboard Storage. Call as @data_source.
+
+        Args:
+            _func: Function to be decorated.
+            storage_type: Storage type to use. This will override the storage
+                type parameter, defined in dashboard instance.
         """
-        return self._protocol
 
-    def _read(self, path: str) -> bytes:
-        t_start = perf_counter_ns()
-        try:
-            f = self._fs_mapper.fs.open(self._base_path + "/" + path)
-        except FileNotFoundError as err:
-            raise KeyError from err
-
-        value: bytes = f.read()
-        if (
-            self._protocol == "abfs"
-            # _details attr only available in abfs protocol
-            and f._details["content_settings"][  # pylint: disable=W0212
-                "content_encoding"
-            ]
-            == "br"
-        ):
-            value = brotli.decompress(value)
+        def inner_decorator(func: Func) -> "Any":
+            @functools.wraps(func)
+            def wrapper(*args: GenericLink, **kwargs: Any) -> "DataSource":
+                return cls(
+                    func,
+                    *args,
+                    storage_type=storage_type,
+                    **kwargs,
+                )
 
-        size = len(value)
-        t_elapsed = (perf_counter_ns() - t_start) * 1e-6
+            return wrapper
 
-        logger.info(
-            "Read operation finished: (base_path='%s', path='%s', size='%s')",
-            self._base_path,
-            path,
-            size,
-            extra={
-                "function": "_read",
-                "base_path": self._base_path,
-                "path": path,
-                "size": size,
-                "elapsed": t_elapsed,
-            },
-        )
+        if _func is None:
+            return inner_decorator
+        else:
+            return inner_decorator(_func)
 
-        return value
+    @property
+    def base_path(self) -> str:
+        """Returns the base path of the data."""
+        return self.__base_path
 
-    def _write(self, path: str, data: bytes) -> None:
-        t_start = perf_counter_ns()
-        size = len(data)
-        kwargs = {}
-        if self._protocol == "abfs" and len(data) >= _COMPRESSION_MIN_LENGTH:
-            data = brotli.compress(data, quality=1)
-            content_settings = ContentSettings(
-                content_type="application/json",
-                content_encoding="br",
-            )
-            kwargs.update({"content_settings": content_settings})
+    @property
+    def separator(self) -> str:
+        """Returns the separator of the data."""
+        return self.__separator
 
-        if len(directory := path.rsplit("/", maxsplit=1)) > 1:
-            self._fs_mapper.fs.makedirs(
-                os.path.join(self.base_path, directory[0]),
-                exist_ok=True,
+    @property
+    def func_args(self) -> List[Any]:
+        """Returns data source signature."""
+        return list(
+            filter(
+                lambda x: x if "*" not in str(x) else None,
+                list(inspect.signature(self.func).parameters.values()),
             )
-
-        self._fs_mapper.fs.write_bytes(
-            f"{self.base_path}/{path}",
-            data,
-            overwrite=True,
-            **kwargs,
         )
-        t_elapsed = (perf_counter_ns() - t_start) * 1e-6
 
-        logger.info(
-            "Write operation finished: (base_path='%s', path='%s', size='%s')",
-            self._base_path,
-            path,
-            size,
-            extra={
-                "function": "_write",
-                "path": path,
-                "size": size,
-                "elapsed": t_elapsed,
-            },
+    def __call__(
+        self,
+        storage_config: StorageConfig,
+        write_keys: bool,
+        metadata: Set[str],
+        duplicated_path: Optional[str] = None,
+    ) -> None:
+        """Stores the data in the storage."""
+        storage = Storage(
+            base_path=storage_config.base_path,
+            headers=storage_config.headers,
         )
+        try:
+            self.__validate_route_args(self.component)
+            self.__check_http_dependencies()
+            self.__store_data(
+                storage=storage,
+                write_keys=write_keys,
+                function_name=self.__base_path,
+                metadata=metadata,
+                duplicated_path=duplicated_path,
+            )
+        except Exception as error:  # Force the parallel task to raise
+            raise error
+        finally:
+            storage.close()
 
-    def clear(self) -> None:
-        """Remove all items from current rubik instance and its backend."""
-        futures = []
-        for path, dirs, files in self._fs_mapper.fs.walk(
-            self._fs_mapper.root, maxdepth=1
-        ):
-            for dir_ in dirs:
-                futures.append(
-                    self._executor.submit(
-                        self._fs_mapper.fs.rm,
-                        os.path.join(path, dir_),
-                        recursive=True,
+    def __store_data(
+        self,
+        storage: Storage,
+        write_keys: bool,
+        function_name: Optional[str],
+        metadata: Set[str],
+        duplicated_path: Optional[str] = None,
+    ) -> None:
+        all_options = self.get_args_data() if self.args else iter([None])
+        duplicated = DuplicatesChecker(duplicated_path=duplicated_path)
+        with IOWriter(self.__base_path, write_keys=write_keys) as writer:
+            for options in all_options:
+                try:
+                    options_data = options if options else None
+                    if duplicated.content is not None:
+                        if options_data in duplicated.content:
+                            continue
+                        duplicated.write(options_data)
+                    data = (
+                        self.func(*options_data, **self.kwargs)
+                        if options_data is not None
+                        else self.func(**self.kwargs)
                     )
-                )
-            for file in files:
-                futures.append(
-                    self._executor.submit(
-                        self._fs_mapper.fs.rm,
-                        os.path.join(path, file),
-                        recursive=True,
+                except BaseException as error:
+                    raise DataProcessError(
+                        data_id=self.component.data_id,
+                        class_name=self.component.__class__.__name__,
+                        error_string=str(error),
+                        function_name=function_name,
+                        options=options,
+                        function_arguments=self.func_args,
+                    ) from error
+
+                if self.component.data_id == "route":
+                    self.__validate_and_store_route_data(
+                        storage=storage,
+                        data=data,
+                        function_name=function_name,
+                        writer=writer,
                     )
-                )
-        concurrent.futures.wait(futures, return_when=concurrent.futures.ALL_COMPLETED)
-
-    @overload
-    def keys(self) -> KeysView[str]:
-        ...
-
-    @overload
-    def keys(self, starts_with: Optional[str]) -> KeysView[str]:
-        ...
-
-    def keys(self, starts_with: Optional[str] = None) -> KeysView[str]:
-        """A list of keys.
-
-        Args:
-            starts_with (Optional[str]): Lists keys only with the same starting path.
-                Defaults to `None`.
-
-        Returns:
-            Iterable[str]: An iterable of keys.
-        """
-        if starts_with is None:
-            return super().keys()
-
-        return RubikKeysViewStartsWith(self, starts_with)
-
-    def getitems(
-        self, keys: Iterable[str], /, default: Optional[_VT_co] = None
-    ) -> Dict[str, Union[DataT, Optional[_VT_co]]]:
-        """Returns a dict object containing the data for the respective given keys.
-
-        Args:
-            keys (Iterable[str]): A list of keys.
-            default (Optional[Any]): The default to use if data is not found for a key.
-                If not initialized and a key data is not found an exception will occur.
-                Defaults to `missing`.
+                else:
+                    self.__validate_and_store_remaining_data(
+                        storage=storage,
+                        data=data,
+                        options=options_data,
+                        function_name=function_name,
+                        writer=writer,
+                    )
+                    writer.write_metadata(
+                        cast(pd.DataFrame, data),
+                        metadata,
+                        self._resolve_path(options_data),
+                    )
+            duplicated.close()
 
-        Returns:
-            Dict[str, DataT]: A dictionary containing the filtered keys and their data.
-        """
-        futures = {
-            key: self._executor.submit(self.get, key, default)  # type: ignore[call-arg]
-            for key in keys
-        }
-        return {k: f.result() for k, f in futures.items()}
-
-    @overload
-    def update(
-        self, other: "SupportsKeysAndGetItem[str, DataT]", /, **kwargs: DataT
+    def __validate_and_store_route_data(
+        self,
+        storage: Storage,
+        data: StaticDataType,
+        writer: IOWriter,
+        function_name: Optional[str] = None,
     ) -> None:
-        ...
-
-    @overload
-    def update(self, other: Iterable[Tuple[str, DataT]], /, **kwargs: DataT) -> None:
-        ...
-
-    @overload
-    def update(self, /, **kwargs: DataT) -> None:
-        ...
+        for row in cast(pd.DataFrame, data).itertuples(index=False):
+            route_options = [getattr(row, self.component.query_parameter)]
+            self.__validate_and_store_remaining_data(
+                storage=storage,
+                data=pd.DataFrame([row]),
+                options=route_options,
+                function_name=function_name,
+                writer=writer,
+            )
 
-    def update(
+    def __validate_and_store_remaining_data(
         self,
-        other: Union[
-            "SupportsKeysAndGetItem[str, DataT]", Iterable[Tuple[str, DataT]]
-        ] = (),
-        /,
-        **kwargs: DataT,
+        storage: Storage,
+        data: StaticDataType,
+        options: Any,
+        writer: IOWriter,
+        function_name: Optional[str] = None,
     ) -> None:
-        """Updates current instance key-values pairs.
-
-        Args:
-            other (Union[SupportsKeysAndGetItem[str, DataT], Mapping[str, DataT]):
-                A mapping like object.
-            kwargs (DataT): Keyword arguments to write as key-value pairs.
-        """
-        futures = []
-
-        if isinstance(other, Mapping):
-            for key in other:
-                futures.append(
-                    self._executor.submit(
-                        self.__setitem__,
-                        key,
-                        other[key],
-                    )
-                )
-        elif hasattr(other, "keys") and hasattr(other, "__getitem__"):
-            for key in other.keys():
-                futures.append(
-                    self._executor.submit(
-                        self.__setitem__,
-                        key,
-                        other[key],
-                    )
-                )
-        else:
-            for key, value in other:
-                futures.append(
-                    self._executor.submit(
-                        self.__setitem__,
-                        key,
-                        value,
-                    )
-                )
+        self._validate_and_store(
+            storage=storage,
+            data=data,
+            options=options,
+            function_name=function_name,
+        )
+        writer.write_key(options)
 
-        for key, value in kwargs.items():
-            futures.append(
-                self._executor.submit(
-                    self.__setitem__,
-                    key,
-                    value,
+    def get_args_data(self) -> Iterable[Tuple[str, ...]]:
+        """Merge the arguments with the data."""
+        paths = self._resolve_paths()
+        for data in itertools.product(
+            *(
+                self._get_data(
+                    arg=arg,
+                    field=self.args[i].field,
                 )
+                for i, arg in enumerate(paths)
             )
-        concurrent.futures.wait(futures, return_when=concurrent.futures.ALL_COMPLETED)
+        ):
+            yield data
+
+    def _resolve_paths(self) -> List[Tuple[str, GenericLink]]:
+        """Get paths from the arguments."""
+        return [self._get_arg_path(arg) for arg in self.args] if self.args else []
+
+    def _get_arg_path(self, arg) -> Tuple[str, GenericLink]:
+        separator = (
+            self.__separator
+            if not isinstance(arg, WidgetField)
+            or any(d.args for d in arg.link_component.data)
+            else ""
+        )
+        return (
+            f"{next(iter(arg.link_component.data)).base_path}{separator}",
+            arg.link_component,
+        )
 
-    def copy_from(self, other: "Rubik", /, starts_with: Optional[str] = None) -> None:
-        """Copies `other` items into current rubik's instance.
+    def _get_data(self, arg: Tuple[str, GenericLink], field: str) -> Iterable[Any]:
+        """Get data from the storage, based on the path inserted."""
+        path, component = arg
+        logger.debug("Get DATA path: '%s'.", path)
+
+        for key in IOReader.keys(path, self.separator):
+            if component.data_id != "route":
+                values = IOReader.read_metadata(key)
+                for value in values[field].tolist():
+                    yield value
+            else:
+                yield key.replace(path, "")
+
+        logger.debug("Finished get data.")
+
+    def __skip_validation(self) -> bool:
+        return SKIP_DATA_VALIDATION or (
+            any(operation.force_skip_validation for operation in self.operations)
+            if self.operations is not None
+            else False
+        )
 
-        Args:
-            other (Rubik): A rubik object.
-            starts_with (Optional[str]): Copies data only with the same starting path.
-                Defaults to `None`.
-        """
+    def _validate_and_store(
+        self,
+        storage: Storage,
+        data: StaticDataType,
+        options: Optional[List[str]],
+        function_name: Optional[str],
+    ) -> None:
+        if data is not None:  # Button use case
+            if not self.__skip_validation():
+                try:
+                    self.component.validate(data, storage=storage)
+                except BaseDataValidationError as error:
+                    raise DataValidationError(
+                        data=data,
+                        data_id=self.component.data_id,
+                        class_name=self.component.__class__.__name__,
+                        error_string=str(error),
+                        function_name=function_name,
+                        options=options,
+                    ) from error
+
+            path = self._resolve_path(options)
+            storage[
+                f"{self.storage_type.value}/{path}"
+            ] = self.component.post_process_data(data)
+
+    def _resolve_path(
+        self,
+        options: Optional[List[str]],
+    ) -> str:
+        if self.__base_path == options:
+            return self.__base_path
+
+        return (
+            f"{self.__base_path}/"
+            f"{f'{self.__separator}'.join(tuple(map(str, options)))}"
+            if options
+            else self.__base_path
+        )
 
-        def _set_other_item(other: "Rubik", key: str) -> None:
-            self[key] = other[key]
 
-        futures = [
-            self._executor.submit(_set_other_item, other, key)
-            for key in other.keys(starts_with)
-        ]
-        concurrent.futures.wait(futures, return_when=concurrent.futures.ALL_COMPLETED)
+data_source = DataSource.decorator
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/internal/rubik/serialization/dataframe.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import numpy as np
 import orjson
 import pandas as pd
 from pandas.api.types import infer_dtype
 
 SCHEMA_VERSION = "0.1.0"
-SCHEMA_ID = "rubik_schema"
+SCHEMA_ID = "storage_schema"
 PERIOD_REGEX = re.compile(r"period\[([A-Z\-]+)\]")
 DATETIME_REGEX = re.compile(r"datetime(?:64)?(?:\[([a-zA-Z]+)(?:,\s*(.*))?\])?")
 INDEX_NAME = "__index"
 
 
 class IncompatibleSchemaError(TypeError):
     """The DataFrame being deserialized does not match the current schema version."""
```

### Comparing `engineai_sdk-0.49.2/engineai/sdk/internal/rubik/serialization/json.py` & `engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/serialization/json.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """Serialization utils."""
+import logging
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import TypeVar
 from typing import Union
 from typing import cast
 
 import orjson
 import pandas as pd
 
-from engineai.sdk.internal.rubik.serialization import dataframe
+from engineai.sdk.dashboard.clients.storage.serialization import dataframe
+
+logger = logging.getLogger(__name__)
+
 
 JSONType = TypeVar("JSONType", bool, int, float, str, List[Any], Dict[str, Any], None)
 """JSON value types."""
 
 
 def serialize(value: Union[pd.DataFrame, JSONType]) -> Tuple[bytes, Optional[bytes]]:
     """Serializes a value.
@@ -62,14 +66,15 @@
     Args:
         value (str): Value to be deserialized.
         schema (Optional[Dict[str, Any]]): The value schema, if any. Defaults to `None`.
 
     Returns:
         Union[pd.DataFrame, JSONType]: The deserialized value.
     """
+    logger.info("deserialize value: %s", value)
     deserialized_value = orjson.loads(value)
     if isinstance(deserialized_value, list) and schema is not None:
         serialized_schema = schema if not callable(schema) else schema()
         if serialized_schema is not None:
             return dataframe.from_records(
                 deserialized_value, orjson.loads(serialized_schema)
             )
```

### Comparing `engineai_sdk-0.49.2/pyproject.toml` & `engineai_sdk-0.83.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 [tool.poetry]
 name = "engineai.sdk"
-version = "0.49.2"
+version = "0.83.1"
 description = "EngineAI's Platform SDK"
 authors = ["Pedro Rodrigues <pedro@dystematic.com>"]
 maintainers = [
-  "Pedro Cunha <cunha@dystematic.com>",
-  "Pedro Feiteira <feiteira@dystematic.com>",
-  "Li Zixiang <li.zixiang@dystematic.com>",
-  "Joao Matos <matos@dystematic.com>",
+  "Pedro Cunha <cunha@engineai.com>",
+  "Pedro Feiteira <feiteira@engineai.com>",
+  "Li Zixiang <li.zixiang@engineai.com>",
+  "Joao Matos <matos@engineai.com>",
+  "Nuno Silva <nuno@engineai.com>",
 ]
 packages = [{ include = "engineai" }]
+readme = "README.md"
 license = "MIT"
 documentation = "https://docs.engineai.com/"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8,<3.12"
 numpy = "^1"
 pandas = "^1.0 || ^2.0"
-environs = "^9.3.2"
-azure-storage-blob = "^12"
+environs = "^11.0.0"
 pyjwt = "^2.3.0"
 more-itertools = "^9"
-beartype = "^0.12.0"
+beartype = "^0.17.0"
 tenacity = "^8.2.1"
-tqdm = "^4.64.1"
 pync = "^2.0.3"
 toml = "^0.10.2"
 click = "^8.1.3"
 typing-extensions = "^4.5.0"
 networkx = "^3.1"
+requests = "^2.31.0"
 
 dataclasses-json = "^0.5.2"
 toposort = "^1.5"
 
-orjson = "^3.6.6"
+orjson = "3.9.10"
 brotli = "^1.0.9"
-fsspec = "^2023.1.0"
-adlfs = "^2023.10.0"
 aiohttp = "^3.9.0b0"
-
+rich = "^13.6.0"
+inquirer = "3.1.4"
 
 [tool.poetry.dev-dependencies]
 types-backports = "^0.1.3"
 bandit = "^1.6.2"
 black = "^23.1.0"
 blacken-docs = "^1.16.0"
 coverage = "^7.2.0"
@@ -73,17 +73,16 @@
 mkdocs-click = "^0.8.0"
 mkdocstrings = { extras = ["python"], version = "^0.22.0" }
 mkdocs-macros-plugin = "^1.0.4"
 pygments = "^2.15.1"
 types-toposort = "^1.10"
 
 [[tool.poetry.source]]
-name = "dystematicpypidev"
-url = "https://nexus.dystematic.dev/repository/pypi-dystematic-dev/simple"
-priority = "default"
+name = "engineaipypi"
+url = "https://nexus.engineai.dev/repository/pypi-dystematic-dev/simple"
 
 [build-system]
 requires = ["poetry>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 engineai = "engineai.sdk.cli.console:process"
```

### Comparing `engineai_sdk-0.49.2/PKG-INFO` & `engineai_sdk-0.83.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,80 @@
 Metadata-Version: 2.1
 Name: engineai.sdk
-Version: 0.49.2
+Version: 0.83.1
 Summary: EngineAI's Platform SDK
 License: MIT
 Author: Pedro Rodrigues
 Author-email: pedro@dystematic.com
 Maintainer: Pedro Cunha
-Maintainer-email: cunha@dystematic.com
-Requires-Python: >=3.8,<4.0
+Maintainer-email: cunha@engineai.com
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: adlfs (>=2023.10.0,<2024.0.0)
 Requires-Dist: aiohttp (>=3.9.0b0,<4.0.0)
-Requires-Dist: azure-storage-blob (>=12,<13)
-Requires-Dist: beartype (>=0.12.0,<0.13.0)
+Requires-Dist: beartype (>=0.17.0,<0.18.0)
 Requires-Dist: brotli (>=1.0.9,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dataclasses-json (>=0.5.2,<0.6.0)
-Requires-Dist: environs (>=9.3.2,<10.0.0)
-Requires-Dist: fsspec (>=2023.1.0,<2024.0.0)
+Requires-Dist: environs (>=11.0.0,<12.0.0)
+Requires-Dist: inquirer (==3.1.4)
 Requires-Dist: more-itertools (>=9,<10)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numpy (>=1,<2)
-Requires-Dist: orjson (>=3.6.6,<4.0.0)
+Requires-Dist: orjson (==3.9.10)
 Requires-Dist: pandas (>=1.0,<3.0)
 Requires-Dist: pyjwt (>=2.3.0,<3.0.0)
 Requires-Dist: pync (>=2.0.3,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.6.0,<14.0.0)
 Requires-Dist: tenacity (>=8.2.1,<9.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: toposort (>=1.5,<2.0)
-Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Documentation, https://docs.engineai.com/
+Description-Content-Type: text/markdown
+
+# EngineAI SDK
+
+We’ve built the EngineAI Platform SDK as a powerful Python library for developing data-driven applications. Designed with both technical and non-technical users in mind, the SDK offers ease of use, an extensive catalog of widgets, and flexible layouts.
+
+### Requirements
+
+- Python 3.8 or higher
+
+### Installation
+
+To install the SDK, run the following command:
+
+```bash
+pip install engineai-sdk
+```
+
+### Create your First Dashboard
+
+To create your dashboard, you need to run the following command:
+
+```bash
+engineai dashboard init
+```
+
+Then, to publish your dashboard, run the following command:
+
+```bash
+engineai dashboard publish
+```
+
+You will be redirected to you first Dashboard. You can now start adding more widgets 
+to your dashboard.
+
+### Documentation
+
+To find all the documentation for the EngineAI Platform SDK, go [here](https://docs.engineai.com).
+
+### License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

