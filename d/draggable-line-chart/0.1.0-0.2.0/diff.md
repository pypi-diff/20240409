# Comparing `tmp/draggable-line-chart-0.1.0.tar.gz` & `tmp/draggable-line-chart-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draggable-line-chart-0.1.0.tar", last modified: Sun Apr  7 21:29:29 2024, max compression
+gzip compressed data, was "draggable-line-chart-0.2.0.tar", last modified: Mon Apr  8 22:32:50 2024, max compression
```

## Comparing `draggable-line-chart-0.1.0.tar` & `draggable-line-chart-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 21:29:29.936474 draggable-line-chart-0.1.0/
--rw-rw-rw-   0        0        0     1082 2024-04-05 22:58:34.000000 draggable-line-chart-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       57 2024-04-06 22:46:10.000000 draggable-line-chart-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1350 2024-04-07 21:29:29.934481 draggable-line-chart-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      895 2024-04-07 20:34:25.000000 draggable-line-chart-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 21:29:29.873451 draggable-line-chart-0.1.0/draggable_line_chart/
--rw-rw-rw-   0        0        0     2816 2024-04-07 21:27:17.000000 draggable-line-chart-0.1.0/draggable_line_chart/__init__.py
--rw-rw-rw-   0        0        0      573 2024-04-07 21:02:33.000000 draggable-line-chart-0.1.0/draggable_line_chart/example.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:29:29.841175 draggable-line-chart-0.1.0/draggable_line_chart/frontend/
-drwxrwxrwx   0        0        0        0 2024-04-07 21:29:29.907780 draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-04-07 20:58:33.000000 draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-05 22:58:35.000000 draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-04-07 20:58:33.000000 draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-04-07 21:29:29.843170 draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-04-07 21:29:29.923542 draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/static/js/
--rw-rw-rw-   0        0        0   560504 2024-04-07 20:58:33.000000 draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/static/js/main.a519b502.js
--rw-rw-rw-   0        0        0     1831 2024-04-07 20:58:33.000000 draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/static/js/main.a519b502.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2400116 2024-04-07 20:58:33.000000 draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/static/js/main.a519b502.js.map
-drwxrwxrwx   0        0        0        0 2024-04-07 21:29:29.892603 draggable-line-chart-0.1.0/draggable_line_chart.egg-info/
--rw-rw-rw-   0        0        0     1350 2024-04-07 21:29:29.000000 draggable-line-chart-0.1.0/draggable_line_chart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      684 2024-04-07 21:29:29.000000 draggable-line-chart-0.1.0/draggable_line_chart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 21:29:29.000000 draggable-line-chart-0.1.0/draggable_line_chart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-07 21:29:29.000000 draggable-line-chart-0.1.0/draggable_line_chart.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-07 21:29:29.000000 draggable-line-chart-0.1.0/draggable_line_chart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 21:29:29.937683 draggable-line-chart-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1077 2024-04-07 20:53:20.000000 draggable-line-chart-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:32:50.362429 draggable-line-chart-0.2.0/
+-rw-rw-rw-   0        0        0     1082 2024-04-05 22:58:34.000000 draggable-line-chart-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       57 2024-04-06 22:46:10.000000 draggable-line-chart-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1392 2024-04-08 22:32:50.360363 draggable-line-chart-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      937 2024-04-08 21:36:12.000000 draggable-line-chart-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 22:32:50.262256 draggable-line-chart-0.2.0/draggable_line_chart/
+-rw-rw-rw-   0        0        0     3200 2024-04-08 22:27:47.000000 draggable-line-chart-0.2.0/draggable_line_chart/__init__.py
+-rw-rw-rw-   0        0        0      615 2024-04-08 22:05:18.000000 draggable-line-chart-0.2.0/draggable_line_chart/example.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:32:50.223720 draggable-line-chart-0.2.0/draggable_line_chart/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-08 22:32:50.317834 draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-04-08 22:29:29.000000 draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-05 22:58:35.000000 draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2024-04-08 22:29:29.000000 draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-08 22:32:50.225716 draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-08 22:32:50.342757 draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   560616 2024-04-08 22:29:29.000000 draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/static/js/main.8e0bbc33.js
+-rw-rw-rw-   0        0        0     1831 2024-04-08 22:29:29.000000 draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/static/js/main.8e0bbc33.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2400954 2024-04-08 22:29:29.000000 draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/static/js/main.8e0bbc33.js.map
+drwxrwxrwx   0        0        0        0 2024-04-08 22:32:50.294259 draggable-line-chart-0.2.0/draggable_line_chart.egg-info/
+-rw-rw-rw-   0        0        0     1392 2024-04-08 22:32:49.000000 draggable-line-chart-0.2.0/draggable_line_chart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2024-04-08 22:32:50.000000 draggable-line-chart-0.2.0/draggable_line_chart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 22:32:49.000000 draggable-line-chart-0.2.0/draggable_line_chart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-08 22:32:49.000000 draggable-line-chart-0.2.0/draggable_line_chart.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-08 22:32:49.000000 draggable-line-chart-0.2.0/draggable_line_chart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 22:32:50.363436 draggable-line-chart-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1077 2024-04-08 22:32:09.000000 draggable-line-chart-0.2.0/setup.py
```

### Comparing `draggable-line-chart-0.1.0/LICENSE` & `draggable-line-chart-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `draggable-line-chart-0.1.0/PKG-INFO` & `draggable-line-chart-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-line-chart
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Streamlit component that displays a line chart with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.
 Home-page: 
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
@@ -38,11 +38,13 @@
 
 
 plot_options = {
     "title": "My Plot",
     "colors": ['#1f77b4', '#ff7f0e', '#2ca02c'],
     "x_label": "X Axis",
     "y_label": "Y Axis",
+    "x_grid": True,
+    "y_grid": True,
 }
 new_data = draggable_line_chart(data=initial_data.to_dict(), options=plot_options)
 new_data
 ```
```

### Comparing `draggable-line-chart-0.1.0/README.md` & `draggable-line-chart-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,11 +26,13 @@
 
 
 plot_options = {
     "title": "My Plot",
     "colors": ['#1f77b4', '#ff7f0e', '#2ca02c'],
     "x_label": "X Axis",
     "y_label": "Y Axis",
+    "x_grid": True,
+    "y_grid": True,
 }
 new_data = draggable_line_chart(data=initial_data.to_dict(), options=plot_options)
 new_data
 ```
```

### Comparing `draggable-line-chart-0.1.0/draggable_line_chart/__init__.py` & `draggable-line-chart-0.2.0/draggable_line_chart/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,20 +41,26 @@
         The data to display in the chart. It can be df.to_dict() with only numbers.
     options : dict[str: any], optional
         A dictionary of options for the chart. It can include the following keys:
         - 'title': The title of the chart.
         - 'colors': A list of colors for the lines in the chart. Each color should be a string in a format accepted by CSS, such as a hex color code. The order of the colors corresponds to the order of the datasets.
         - 'x_label': The label for the x-axis.
         - 'y_label': The label for the y-axis.
+        - 'x_grid': A boolean indicating whether to display the grid for the x-axis. If not provided, the grid will be displayed by default.
+        - 'y_grid': A boolean indicating whether to display the grid for the y-axis. If not provided, the grid will be displayed by default.
         If not provided, default options will be used.
     key : str, optional
         An optional string to use as the unique key for the widget. If this is None, and the component's arguments are changed, the component will be re-mounted in the Streamlit frontend and lose its current state.
 
     Returns
     -------
     dict[dict[str: float]]
         The data of the chart after user interaction. The format is the same as the input format.
     """
+    if not options:
+        options = {
+            "x_grid": True,
+            "y_grid": True}
     component_value = _draggable_line_chart(
         data=data, options=options, key=key, default=data)
 
     return component_value
```

### Comparing `draggable-line-chart-0.1.0/draggable_line_chart/example.py` & `draggable-line-chart-0.2.0/draggable_line_chart/example.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,10 +13,12 @@
 
 
 plot_options = {
     "title": "My Plot",
     "colors": ['#1f77b4', '#ff7f0e', '#2ca02c'],
     "x_label": "X Axis",
     "y_label": "Y Axis",
+    "x_grid": True,
+    "y_grid": True,
 }
 new_data = draggable_line_chart(data=initial_data.to_dict(), options=plot_options)
 new_data
```

### Comparing `draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/bootstrap.min.css` & `draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/static/js/main.a519b502.js` & `draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/static/js/main.8e0bbc33.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.a519b502.js.LICENSE.txt */
+/*! For license information please see main.8e0bbc33.js.LICENSE.txt */
 (() => {
     var t = {
             895: (t, e, n) => {
                 var i;
                 ! function(r, s, o, a) {
                     "use strict";
                     var l, c = ["", "webkit", "Moz", "MS", "ms", "o"],
@@ -17262,53 +17262,780 @@
                 const e = this._offsets,
                     n = this.getDecimalForPixel(t) / e.factor - e.end;
                 return Ro(this._table, n * this._tableRange + this._minPos, !0)
             }
         }
         s(zo, "id", "timeseries"), s(zo, "defaults", Bo.defaults);
         const Uo = [ui, cs, oo, Object.freeze({
-                __proto__: null,
-                CategoryScale: co,
-                LinearScale: po,
-                LogarithmicScale: _o,
-                RadialLinearScale: Oo,
-                TimeScale: Bo,
-                TimeSeriesScale: zo
-            })],
-            Vo = "label";
+            __proto__: null,
+            CategoryScale: co,
+            LinearScale: po,
+            LogarithmicScale: _o,
+            RadialLinearScale: Oo,
+            TimeScale: Bo,
+            TimeSeriesScale: zo
+        })];
+        var Vo = n(895),
+            jo = n.n(Vo);
+        const Wo = t => t && t.enabled && t.modifierKey,
+            Ho = (t, e) => t && e[t + "Key"],
+            Yo = (t, e) => t && !e[t + "Key"];
+
+        function $o(t, e, n) {
+            return void 0 === t || ("string" === typeof t ? -1 !== t.indexOf(e) : "function" === typeof t && -1 !== t({
+                chart: n
+            }).indexOf(e))
+        }
+
+        function Ko(t, e) {
+            return "function" === typeof t && (t = t({
+                chart: e
+            })), "string" === typeof t ? {
+                x: -1 !== t.indexOf("x"),
+                y: -1 !== t.indexOf("y")
+            } : {
+                x: !1,
+                y: !1
+            }
+        }
+
+        function Xo(t, e, n) {
+            const {
+                mode: i = "xy",
+                scaleMode: r,
+                overScaleMode: s
+            } = t || {}, o = function(t, e) {
+                let {
+                    x: n,
+                    y: i
+                } = t;
+                const r = e.scales,
+                    s = Object.keys(r);
+                for (let o = 0; o < s.length; o++) {
+                    const t = r[s[o]];
+                    if (i >= t.top && i <= t.bottom && n >= t.left && n <= t.right) return t
+                }
+                return null
+            }(e, n), a = Ko(i, n), l = Ko(r, n);
+            if (s) {
+                const t = Ko(s, n);
+                for (const e of ["x", "y"]) t[e] && (l[e] = a[e], a[e] = !1)
+            }
+            if (o && l[o.axis]) return [o];
+            const c = [];
+            return q(n.scales, (function(t) {
+                a[t.axis] && c.push(t)
+            })), c
+        }
+        const qo = new WeakMap;
+
+        function Qo(t) {
+            let e = qo.get(t);
+            return e || (e = {
+                originalScaleLimits: {},
+                updatedScaleLimits: {},
+                handlers: {},
+                panDelta: {}
+            }, qo.set(t, e)), e
+        }
+
+        function Zo(t, e, n) {
+            const i = t.max - t.min,
+                r = i * (e - 1),
+                s = t.isHorizontal() ? n.x : n.y,
+                o = Math.max(0, Math.min(1, (t.getValueForPixel(s) - t.min) / i || 0));
+            return {
+                min: r * o,
+                max: r * (1 - o)
+            }
+        }
+
+        function Go(t, e, n, i, r) {
+            let s = n[i];
+            if ("original" === s) {
+                const n = t.originalScaleLimits[e.id][i];
+                s = $(n.options, n.scale)
+            }
+            return $(s, r)
+        }
+
+        function Jo(t, e, n) {
+            let {
+                min: i,
+                max: r
+            } = e, s = arguments.length > 3 && void 0 !== arguments[3] && arguments[3];
+            const o = Qo(t.chart),
+                {
+                    id: a,
+                    axis: l,
+                    options: c
+                } = t,
+                u = n && (n[a] || n[l]) || {},
+                {
+                    minRange: h = 0
+                } = u,
+                d = Go(o, t, u, "min", -1 / 0),
+                f = Go(o, t, u, "max", 1 / 0),
+                p = s ? Math.max(r - i, h) : t.max - t.min,
+                g = (p - r + i) / 2;
+            return i -= g, r += g, i < d ? (i = d, r = Math.min(d + p, f)) : r > f && (r = f, i = Math.max(f - p, d)), c.min = i, c.max = r, o.updatedScaleLimits[t.id] = {
+                min: i,
+                max: r
+            }, t.parse(i) !== t.min || t.parse(r) !== t.max
+        }
+        const ta = t => 0 === t || isNaN(t) ? 0 : t < 0 ? Math.min(Math.round(t), -1) : Math.max(Math.round(t), 1);
+        const ea = {
+            second: 500,
+            minute: 3e4,
+            hour: 18e5,
+            day: 432e5,
+            week: 3024e5,
+            month: 1296e6,
+            quarter: 5184e6,
+            year: 157248e5
+        };
+
+        function na(t, e, n) {
+            let i = arguments.length > 3 && void 0 !== arguments[3] && arguments[3];
+            const {
+                min: r,
+                max: s,
+                options: o
+            } = t, a = o.time && o.time.round, l = ea[a] || 0, c = t.getValueForPixel(t.getPixelForValue(r + l) - e), u = t.getValueForPixel(t.getPixelForValue(s + l) - e), {
+                min: h = -1 / 0,
+                max: d = 1 / 0
+            } = i && n && n[t.axis] || {};
+            return !!(isNaN(c) || isNaN(u) || c < h || u > d) || Jo(t, {
+                min: c,
+                max: u
+            }, n, i)
+        }
+
+        function ia(t, e, n) {
+            return na(t, e, n, !0)
+        }
+        const ra = {
+                category: function(t, e, n, i) {
+                    const r = Zo(t, e, n);
+                    return t.min === t.max && e < 1 && function(t) {
+                        const e = t.getLabels().length - 1;
+                        t.min > 0 && (t.min -= 1), t.max < e && (t.max += 1)
+                    }(t), Jo(t, {
+                        min: t.min + ta(r.min),
+                        max: t.max - ta(r.max)
+                    }, i, !0)
+                },
+                default: function(t, e, n, i) {
+                    const r = Zo(t, e, n);
+                    return Jo(t, {
+                        min: t.min + r.min,
+                        max: t.max - r.max
+                    }, i, !0)
+                }
+            },
+            sa = {
+                default: function(t, e, n, i) {
+                    Jo(t, function(t, e, n) {
+                        const i = t.getValueForPixel(e),
+                            r = t.getValueForPixel(n);
+                        return {
+                            min: Math.min(i, r),
+                            max: Math.max(i, r)
+                        }
+                    }(t, e, n), i, !0)
+                }
+            },
+            oa = {
+                category: function(t, e, n) {
+                    const i = t.getLabels().length - 1;
+                    let {
+                        min: r,
+                        max: s
+                    } = t;
+                    const o = Math.max(s - r, 1),
+                        a = Math.round(function(t) {
+                            return t.isHorizontal() ? t.width : t.height
+                        }(t) / Math.max(o, 10)),
+                        l = Math.round(Math.abs(e / a));
+                    let c;
+                    return e < -a ? (s = Math.min(s + l, i), r = 1 === o ? s : s - o, c = s === i) : e > a && (r = Math.max(0, r - l), s = 1 === o ? r : r + o, c = 0 === r), Jo(t, {
+                        min: r,
+                        max: s
+                    }, n) || c
+                },
+                default: na,
+                logarithmic: ia,
+                timeseries: ia
+            };
+
+        function aa(t, e) {
+            q(t, ((n, i) => {
+                e[i] || delete t[i]
+            }))
+        }
+
+        function la(t, e) {
+            const {
+                scales: n
+            } = t, {
+                originalScaleLimits: i,
+                updatedScaleLimits: r
+            } = e;
+            return q(n, (function(t) {
+                (function(t, e, n) {
+                    const {
+                        id: i,
+                        options: {
+                            min: r,
+                            max: s
+                        }
+                    } = t;
+                    if (!e[i] || !n[i]) return !0;
+                    const o = n[i];
+                    return o.min !== r || o.max !== s
+                })(t, i, r) && (i[t.id] = {
+                    min: {
+                        scale: t.min,
+                        options: t.options.min
+                    },
+                    max: {
+                        scale: t.max,
+                        options: t.options.max
+                    }
+                })
+            })), aa(i, n), aa(r, n), i
+        }
+
+        function ca(t, e, n, i) {
+            X(ra[t.type] || ra.default, [t, e, n, i])
+        }
+
+        function ua(t, e, n, i, r) {
+            X(sa[t.type] || sa.default, [t, e, n, i, r])
+        }
+
+        function ha(t) {
+            const e = t.chartArea;
+            return {
+                x: (e.left + e.right) / 2,
+                y: (e.top + e.bottom) / 2
+            }
+        }
+
+        function da(t, e) {
+            let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "none";
+            const {
+                x: i = 1,
+                y: r = 1,
+                focalPoint: s = ha(t)
+            } = "number" === typeof e ? {
+                x: e,
+                y: e
+            } : e, o = Qo(t), {
+                options: {
+                    limits: a,
+                    zoom: l
+                }
+            } = o;
+            la(t, o);
+            const c = 1 !== i,
+                u = 1 !== r;
+            q(Xo(l, s, t) || t.scales, (function(t) {
+                t.isHorizontal() && c ? ca(t, i, s, a) : !t.isHorizontal() && u && ca(t, r, s, a)
+            })), t.update(n), X(l.onZoom, [{
+                chart: t
+            }])
+        }
+
+        function fa(t, e, n) {
+            let i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : "none";
+            const r = Qo(t),
+                {
+                    options: {
+                        limits: s,
+                        zoom: o
+                    }
+                } = r,
+                {
+                    mode: a = "xy"
+                } = o;
+            la(t, r);
+            const l = $o(a, "x", t),
+                c = $o(a, "y", t);
+            q(t.scales, (function(t) {
+                t.isHorizontal() && l ? ua(t, e.x, n.x, s) : !t.isHorizontal() && c && ua(t, e.y, n.y, s)
+            })), t.update(i), X(o.onZoom, [{
+                chart: t
+            }])
+        }
+
+        function pa(t) {
+            const e = Qo(t);
+            let n = 1,
+                i = 1;
+            return q(t.scales, (function(t) {
+                const r = function(t, e) {
+                    const n = t.originalScaleLimits[e];
+                    if (!n) return;
+                    const {
+                        min: i,
+                        max: r
+                    } = n;
+                    return $(r.options, r.scale) - $(i.options, i.scale)
+                }(e, t.id);
+                if (r) {
+                    const e = Math.round(r / (t.max - t.min) * 100) / 100;
+                    n = Math.min(n, e), i = Math.max(i, e)
+                }
+            })), n < 1 ? n : i
+        }
+
+        function ga(t, e, n, i) {
+            const {
+                panDelta: r
+            } = i, s = r[t.id] || 0;
+            bt(s) === bt(e) && (e += s);
+            X(oa[t.type] || oa.default, [t, e, n]) ? r[t.id] = 0 : r[t.id] = e
+        }
+
+        function ma(t, e, n) {
+            let i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : "none";
+            const {
+                x: r = 0,
+                y: s = 0
+            } = "number" === typeof e ? {
+                x: e,
+                y: e
+            } : e, o = Qo(t), {
+                options: {
+                    pan: a,
+                    limits: l
+                }
+            } = o, {
+                onPan: c
+            } = a || {};
+            la(t, o);
+            const u = 0 !== r,
+                h = 0 !== s;
+            q(n || t.scales, (function(t) {
+                t.isHorizontal() && u ? ga(t, r, l, o) : !t.isHorizontal() && h && ga(t, s, l, o)
+            })), t.update(i), X(c, [{
+                chart: t
+            }])
+        }
+
+        function ya(t) {
+            const e = Qo(t);
+            la(t, e);
+            const n = {};
+            for (const i of Object.keys(t.scales)) {
+                const {
+                    min: t,
+                    max: r
+                } = e.originalScaleLimits[i] || {
+                    min: {},
+                    max: {}
+                };
+                n[i] = {
+                    min: t.scale,
+                    max: r.scale
+                }
+            }
+            return n
+        }
+
+        function ba(t, e) {
+            const {
+                handlers: n
+            } = Qo(t), i = n[e];
+            i && i.target && (i.target.removeEventListener(e, i), delete n[e])
+        }
+
+        function va(t, e, n, i) {
+            const {
+                handlers: r,
+                options: s
+            } = Qo(t), o = r[n];
+            o && o.target === e || (ba(t, n), r[n] = e => i(t, e, s), r[n].target = e, e.addEventListener(n, r[n]))
+        }
+
+        function _a(t, e) {
+            const n = Qo(t);
+            n.dragStart && (n.dragging = !0, n.dragEnd = e, t.update("none"))
+        }
+
+        function xa(t, e) {
+            const n = Qo(t);
+            n.dragStart && "Escape" === e.key && (ba(t, "keydown"), n.dragging = !1, n.dragStart = n.dragEnd = null, t.update("none"))
+        }
+
+        function wa(t, e, n) {
+            const {
+                onZoomStart: i,
+                onZoomRejected: r
+            } = n;
+            if (i) {
+                if (!1 === X(i, [{
+                        chart: t,
+                        event: e,
+                        point: hn(e, t)
+                    }])) return X(r, [{
+                    chart: t,
+                    event: e
+                }]), !1
+            }
+        }
+
+        function Sa(t, e) {
+            const n = Qo(t),
+                {
+                    pan: i,
+                    zoom: r = {}
+                } = n.options;
+            if (0 !== e.button || Ho(Wo(i), e) || Yo(Wo(r.drag), e)) return X(r.onZoomRejected, [{
+                chart: t,
+                event: e
+            }]);
+            !1 !== wa(t, e, r) && (n.dragStart = e, va(t, t.canvas, "mousemove", _a), va(t, window.document, "keydown", xa))
+        }
+
+        function Ta(t, e, n, i) {
+            const r = $o(e, "x", t),
+                s = $o(e, "y", t);
+            let {
+                top: o,
+                left: a,
+                right: l,
+                bottom: c,
+                width: u,
+                height: h
+            } = t.chartArea;
+            const d = hn(n, t),
+                f = hn(i, t);
+            r && (a = Math.min(d.x, f.x), l = Math.max(d.x, f.x)), s && (o = Math.min(d.y, f.y), c = Math.max(d.y, f.y));
+            const p = l - a,
+                g = c - o;
+            return {
+                left: a,
+                top: o,
+                right: l,
+                bottom: c,
+                width: p,
+                height: g,
+                zoomX: r && p ? 1 + (u - p) / u : 1,
+                zoomY: s && g ? 1 + (h - g) / h : 1
+            }
+        }
+
+        function ka(t, e) {
+            const n = Qo(t);
+            if (!n.dragStart) return;
+            ba(t, "mousemove");
+            const {
+                mode: i,
+                onZoomComplete: r,
+                drag: {
+                    threshold: s = 0
+                }
+            } = n.options.zoom, o = Ta(t, i, n.dragStart, e), a = $o(i, "x", t) ? o.width : 0, l = $o(i, "y", t) ? o.height : 0, c = Math.sqrt(a * a + l * l);
+            if (n.dragStart = n.dragEnd = null, c <= s) return n.dragging = !1, void t.update("none");
+            fa(t, {
+                x: o.left,
+                y: o.top
+            }, {
+                x: o.right,
+                y: o.bottom
+            }, "zoom"), setTimeout((() => n.dragging = !1), 500), X(r, [{
+                chart: t
+            }])
+        }
+
+        function Ma(t, e) {
+            const {
+                handlers: {
+                    onZoomComplete: n
+                },
+                options: {
+                    zoom: i
+                }
+            } = Qo(t);
+            if (! function(t, e, n) {
+                    if (Yo(Wo(n.wheel), e)) X(n.onZoomRejected, [{
+                        chart: t,
+                        event: e
+                    }]);
+                    else if (!1 !== wa(t, e, n) && (e.cancelable && e.preventDefault(), void 0 !== e.deltaY)) return !0
+                }(t, e, i)) return;
+            const r = e.target.getBoundingClientRect(),
+                s = 1 + (e.deltaY >= 0 ? -i.wheel.speed : i.wheel.speed);
+            da(t, {
+                x: s,
+                y: s,
+                focalPoint: {
+                    x: e.clientX - r.left,
+                    y: e.clientY - r.top
+                }
+            }), n && n()
+        }
+
+        function Ia(t, e, n, i) {
+            n && (Qo(t).handlers[e] = function(t, e) {
+                let n;
+                return function() {
+                    return clearTimeout(n), n = setTimeout(t, e), e
+                }
+            }((() => X(n, [{
+                chart: t
+            }])), i))
+        }
 
-        function jo(t, e) {
+        function Ea(t, e) {
+            return function(n, i) {
+                const {
+                    pan: r,
+                    zoom: s = {}
+                } = e.options;
+                if (!r || !r.enabled) return !1;
+                const o = i && i.srcEvent;
+                return !o || (!(!e.panning && "mouse" === i.pointerType && (Yo(Wo(r), o) || Ho(Wo(s.drag), o))) || (X(r.onPanRejected, [{
+                    chart: t,
+                    event: i
+                }]), !1))
+            }
+        }
+
+        function Oa(t, e, n) {
+            if (e.scale) {
+                const {
+                    center: i,
+                    pointers: r
+                } = n, s = 1 / e.scale * n.scale, o = n.target.getBoundingClientRect(), a = function(t, e) {
+                    const n = Math.abs(t.clientX - e.clientX),
+                        i = Math.abs(t.clientY - e.clientY),
+                        r = n / i;
+                    let s, o;
+                    return r > .3 && r < 1.7 ? s = o = !0 : n > i ? s = !0 : o = !0, {
+                        x: s,
+                        y: o
+                    }
+                }(r[0], r[1]), l = e.options.zoom.mode;
+                da(t, {
+                    x: a.x && $o(l, "x", t) ? s : 1,
+                    y: a.y && $o(l, "y", t) ? s : 1,
+                    focalPoint: {
+                        x: i.x - o.left,
+                        y: i.y - o.top
+                    }
+                }), e.scale = n.scale
+            }
+        }
+
+        function Da(t, e, n) {
+            const i = e.delta;
+            i && (e.panning = !0, ma(t, {
+                x: n.deltaX - i.x,
+                y: n.deltaY - i.y
+            }, e.panScales), e.delta = {
+                x: n.deltaX,
+                y: n.deltaY
+            })
+        }
+        const Aa = new WeakMap;
+
+        function Ca(t, e) {
+            const n = Qo(t),
+                i = t.canvas,
+                {
+                    pan: r,
+                    zoom: s
+                } = e,
+                o = new(jo().Manager)(i);
+            s && s.pinch.enabled && (o.add(new(jo().Pinch)), o.on("pinchstart", (() => function(t, e) {
+                e.options.zoom.pinch.enabled && (e.scale = 1)
+            }(0, n))), o.on("pinch", (e => Oa(t, n, e))), o.on("pinchend", (e => function(t, e, n) {
+                e.scale && (Oa(t, e, n), e.scale = null, X(e.options.zoom.onZoomComplete, [{
+                    chart: t
+                }]))
+            }(t, n, e)))), r && r.enabled && (o.add(new(jo().Pan)({
+                threshold: r.threshold,
+                enable: Ea(t, n)
+            })), o.on("panstart", (e => function(t, e, n) {
+                const {
+                    enabled: i,
+                    onPanStart: r,
+                    onPanRejected: s
+                } = e.options.pan;
+                if (!i) return;
+                const o = n.target.getBoundingClientRect(),
+                    a = {
+                        x: n.center.x - o.left,
+                        y: n.center.y - o.top
+                    };
+                if (!1 === X(r, [{
+                        chart: t,
+                        event: n,
+                        point: a
+                    }])) return X(s, [{
+                    chart: t,
+                    event: n
+                }]);
+                e.panScales = Xo(e.options.pan, a, t), e.delta = {
+                    x: 0,
+                    y: 0
+                }, clearTimeout(e.panEndTimeout), Da(t, e, n)
+            }(t, n, e))), o.on("panmove", (e => Da(t, n, e))), o.on("panend", (() => function(t, e) {
+                e.delta = null, e.panning && (e.panEndTimeout = setTimeout((() => e.panning = !1), 500), X(e.options.pan.onPanComplete, [{
+                    chart: t
+                }]))
+            }(t, n)))), Aa.set(t, o)
+        }
+
+        function Pa(t, e, n) {
+            const i = n.zoom.drag,
+                {
+                    dragStart: r,
+                    dragEnd: s
+                } = Qo(t);
+            if (i.drawTime !== e || !s) return;
+            const {
+                left: o,
+                top: a,
+                width: l,
+                height: c
+            } = Ta(t, n.zoom.mode, r, s), u = t.ctx;
+            u.save(), u.beginPath(), u.fillStyle = i.backgroundColor || "rgba(225,225,225,0.3)", u.fillRect(o, a, l, c), i.borderWidth > 0 && (u.lineWidth = i.borderWidth, u.strokeStyle = i.borderColor || "rgba(225,225,225)", u.strokeRect(o, a, l, c)), u.restore()
+        }
+        var Fa = {
+            id: "zoom",
+            version: "2.0.1",
+            defaults: {
+                pan: {
+                    enabled: !1,
+                    mode: "xy",
+                    threshold: 10,
+                    modifierKey: null
+                },
+                zoom: {
+                    wheel: {
+                        enabled: !1,
+                        speed: .1,
+                        modifierKey: null
+                    },
+                    drag: {
+                        enabled: !1,
+                        drawTime: "beforeDatasetsDraw",
+                        modifierKey: null
+                    },
+                    pinch: {
+                        enabled: !1
+                    },
+                    mode: "xy"
+                }
+            },
+            start: function(t, e, n) {
+                Qo(t).options = n, Object.prototype.hasOwnProperty.call(n.zoom, "enabled") && console.warn("The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`."), (Object.prototype.hasOwnProperty.call(n.zoom, "overScaleMode") || Object.prototype.hasOwnProperty.call(n.pan, "overScaleMode")) && console.warn("The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired)."), jo() && Ca(t, n), t.pan = (e, n, i) => ma(t, e, n, i), t.zoom = (e, n) => da(t, e, n), t.zoomRect = (e, n, i) => fa(t, e, n, i), t.zoomScale = (e, n, i) => function(t, e, n) {
+                    let i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : "none";
+                    la(t, Qo(t)), Jo(t.scales[e], n, void 0, !0), t.update(i)
+                }(t, e, n, i), t.resetZoom = e => function(t) {
+                    let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "default";
+                    const n = Qo(t),
+                        i = la(t, n);
+                    q(t.scales, (function(t) {
+                        const e = t.options;
+                        i[t.id] ? (e.min = i[t.id].min.options, e.max = i[t.id].max.options) : (delete e.min, delete e.max)
+                    })), t.update(e), X(n.options.zoom.onZoomComplete, [{
+                        chart: t
+                    }])
+                }(t, e), t.getZoomLevel = () => pa(t), t.getInitialScaleBounds = () => ya(t), t.isZoomedOrPanned = () => function(t) {
+                    const e = ya(t);
+                    for (const n of Object.keys(t.scales)) {
+                        const {
+                            min: i,
+                            max: r
+                        } = e[n];
+                        if (void 0 !== i && t.scales[n].min !== i) return !0;
+                        if (void 0 !== r && t.scales[n].max !== r) return !0
+                    }
+                    return !1
+                }(t)
+            },
+            beforeEvent(t) {
+                const e = Qo(t);
+                if (e.panning || e.dragging) return !1
+            },
+            beforeUpdate: function(t, e, n) {
+                Qo(t).options = n,
+                    function(t, e) {
+                        const n = t.canvas,
+                            {
+                                wheel: i,
+                                drag: r,
+                                onZoomComplete: s
+                            } = e.zoom;
+                        i.enabled ? (va(t, n, "wheel", Ma), Ia(t, "onZoomComplete", s, 250)) : ba(t, "wheel"), r.enabled ? (va(t, n, "mousedown", Sa), va(t, n.ownerDocument, "mouseup", ka)) : (ba(t, "mousedown"), ba(t, "mousemove"), ba(t, "mouseup"), ba(t, "keydown"))
+                    }(t, n)
+            },
+            beforeDatasetsDraw(t, e, n) {
+                Pa(t, "beforeDatasetsDraw", n)
+            },
+            afterDatasetsDraw(t, e, n) {
+                Pa(t, "afterDatasetsDraw", n)
+            },
+            beforeDraw(t, e, n) {
+                Pa(t, "beforeDraw", n)
+            },
+            afterDraw(t, e, n) {
+                Pa(t, "afterDraw", n)
+            },
+            stop: function(t) {
+                ! function(t) {
+                    ba(t, "mousedown"), ba(t, "mousemove"), ba(t, "mouseup"), ba(t, "wheel"), ba(t, "click"), ba(t, "keydown")
+                }(t), jo() && function(t) {
+                        const e = Aa.get(t);
+                        e && (e.remove("pinchstart"), e.remove("pinch"), e.remove("pinchend"), e.remove("panstart"), e.remove("pan"), e.remove("panend"), e.destroy(), Aa.delete(t))
+                    }(t),
+                    function(t) {
+                        qo.delete(t)
+                    }(t)
+            },
+            panFunctions: oa,
+            zoomFunctions: ra,
+            zoomRectFunctions: sa
+        };
+        const La = "label";
+
+        function Na(t, e) {
             "function" === typeof t ? t(e) : t && (t.current = e)
         }
 
-        function Wo(t, e) {
+        function Ba(t, e) {
             t.labels = e
         }
 
-        function Ho(t, e) {
-            let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : Vo;
+        function Ra(t, e) {
+            let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : La;
             const i = [];
             t.datasets = e.map((e => {
                 const r = t.datasets.find((t => t[n] === e[n]));
                 return r && e.data && !i.includes(r) ? (i.push(r), Object.assign(r, e), r) : {
                     ...e
                 }
             }))
         }
 
-        function Yo(t) {
-            let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Vo;
+        function za(t) {
+            let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : La;
             const n = {
                 labels: [],
                 datasets: []
             };
-            return Wo(n, t.labels), Ho(n, t.datasets, e), n
+            return Ba(n, t.labels), Ra(n, t.datasets, e), n
         }
 
-        function $o(e, n) {
+        function Ua(e, n) {
             const {
                 height: i = 150,
                 width: r = 300,
                 redraw: s = !1,
                 datasetIdKey: o,
                 type: a,
                 data: l,
@@ -17316,95 +18043,95 @@
                 plugins: u = [],
                 fallbackContent: h,
                 updateMode: d,
                 ...f
             } = e, p = (0, t.useRef)(null), g = (0, t.useRef)(), m = () => {
                 p.current && (g.current = new Rr(p.current, {
                     type: a,
-                    data: Yo(l, o),
+                    data: za(l, o),
                     options: c && {
                         ...c
                     },
                     plugins: u
-                }), jo(n, g.current))
+                }), Na(n, g.current))
             }, y = () => {
-                jo(n, null), g.current && (g.current.destroy(), g.current = null)
+                Na(n, null), g.current && (g.current.destroy(), g.current = null)
             };
             return (0, t.useEffect)((() => {
                 !s && g.current && c && function(t, e) {
                     const n = t.options;
                     n && e && Object.assign(n, e)
                 }(g.current, c)
             }), [s, c]), (0, t.useEffect)((() => {
-                !s && g.current && Wo(g.current.config.data, l.labels)
+                !s && g.current && Ba(g.current.config.data, l.labels)
             }), [s, l.labels]), (0, t.useEffect)((() => {
-                !s && g.current && l.datasets && Ho(g.current.config.data, l.datasets, o)
+                !s && g.current && l.datasets && Ra(g.current.config.data, l.datasets, o)
             }), [s, l.datasets]), (0, t.useEffect)((() => {
                 g.current && (s ? (y(), setTimeout(m)) : g.current.update(d))
             }), [s, c, l.labels, l.datasets, d]), (0, t.useEffect)((() => {
                 g.current && (y(), setTimeout(m))
             }), [a]), (0, t.useEffect)((() => (m(), () => y())), []), t.createElement("canvas", Object.assign({
                 ref: p,
                 role: "img",
                 height: i,
                 width: r
             }, f), h)
         }
-        const Ko = (0, t.forwardRef)($o);
+        const Va = (0, t.forwardRef)(Ua);
 
-        function Xo(e, n) {
-            return Rr.register(n), (0, t.forwardRef)(((n, i) => t.createElement(Ko, Object.assign({}, n, {
+        function ja(e, n) {
+            return Rr.register(n), (0, t.forwardRef)(((n, i) => t.createElement(Va, Object.assign({}, n, {
                 ref: i,
                 type: e
             }))))
         }
-        const qo = Xo("line", si);
-        var Qo, Zo, Go, Jo, ta, ea, na, ia, ra, sa = n(219),
-            oa = n.n(sa);
+        const Wa = ja("line", si);
+        var Ha, Ya, $a, Ka, Xa, qa, Qa, Za, Ga, Ja = n(219),
+            tl = n.n(Ja);
         ! function(t) {
             t[t.V1 = 0] = "V1", t[t.V2 = 1] = "V2", t[t.V3 = 2] = "V3", t[t.V4 = 3] = "V4", t[t.V5 = 4] = "V5"
-        }(Qo || (Qo = {})),
+        }(Ha || (Ha = {})),
         function(t) {
             t[t.Sparse = 0] = "Sparse", t[t.Dense = 1] = "Dense"
-        }(Zo || (Zo = {})),
+        }(Ya || (Ya = {})),
         function(t) {
             t[t.HALF = 0] = "HALF", t[t.SINGLE = 1] = "SINGLE", t[t.DOUBLE = 2] = "DOUBLE"
-        }(Go || (Go = {})),
+        }($a || ($a = {})),
         function(t) {
             t[t.DAY = 0] = "DAY", t[t.MILLISECOND = 1] = "MILLISECOND"
-        }(Jo || (Jo = {})),
+        }(Ka || (Ka = {})),
         function(t) {
             t[t.SECOND = 0] = "SECOND", t[t.MILLISECOND = 1] = "MILLISECOND", t[t.MICROSECOND = 2] = "MICROSECOND", t[t.NANOSECOND = 3] = "NANOSECOND"
-        }(ta || (ta = {})),
+        }(Xa || (Xa = {})),
         function(t) {
             t[t.YEAR_MONTH = 0] = "YEAR_MONTH", t[t.DAY_TIME = 1] = "DAY_TIME", t[t.MONTH_DAY_NANO = 2] = "MONTH_DAY_NANO"
-        }(ea || (ea = {})),
+        }(qa || (qa = {})),
         function(t) {
             t[t.NONE = 0] = "NONE", t[t.Schema = 1] = "Schema", t[t.DictionaryBatch = 2] = "DictionaryBatch", t[t.RecordBatch = 3] = "RecordBatch", t[t.Tensor = 4] = "Tensor", t[t.SparseTensor = 5] = "SparseTensor"
-        }(na || (na = {})),
+        }(Qa || (Qa = {})),
         function(t) {
             t[t.NONE = 0] = "NONE", t[t.Null = 1] = "Null", t[t.Int = 2] = "Int", t[t.Float = 3] = "Float", t[t.Binary = 4] = "Binary", t[t.Utf8 = 5] = "Utf8", t[t.Bool = 6] = "Bool", t[t.Decimal = 7] = "Decimal", t[t.Date = 8] = "Date", t[t.Time = 9] = "Time", t[t.Timestamp = 10] = "Timestamp", t[t.Interval = 11] = "Interval", t[t.List = 12] = "List", t[t.Struct = 13] = "Struct", t[t.Union = 14] = "Union", t[t.FixedSizeBinary = 15] = "FixedSizeBinary", t[t.FixedSizeList = 16] = "FixedSizeList", t[t.Map = 17] = "Map", t[t.Dictionary = -1] = "Dictionary", t[t.Int8 = -2] = "Int8", t[t.Int16 = -3] = "Int16", t[t.Int32 = -4] = "Int32", t[t.Int64 = -5] = "Int64", t[t.Uint8 = -6] = "Uint8", t[t.Uint16 = -7] = "Uint16", t[t.Uint32 = -8] = "Uint32", t[t.Uint64 = -9] = "Uint64", t[t.Float16 = -10] = "Float16", t[t.Float32 = -11] = "Float32", t[t.Float64 = -12] = "Float64", t[t.DateDay = -13] = "DateDay", t[t.DateMillisecond = -14] = "DateMillisecond", t[t.TimestampSecond = -15] = "TimestampSecond", t[t.TimestampMillisecond = -16] = "TimestampMillisecond", t[t.TimestampMicrosecond = -17] = "TimestampMicrosecond", t[t.TimestampNanosecond = -18] = "TimestampNanosecond", t[t.TimeSecond = -19] = "TimeSecond", t[t.TimeMillisecond = -20] = "TimeMillisecond", t[t.TimeMicrosecond = -21] = "TimeMicrosecond", t[t.TimeNanosecond = -22] = "TimeNanosecond", t[t.DenseUnion = -23] = "DenseUnion", t[t.SparseUnion = -24] = "SparseUnion", t[t.IntervalDayTime = -25] = "IntervalDayTime", t[t.IntervalYearMonth = -26] = "IntervalYearMonth"
-        }(ia || (ia = {})),
+        }(Za || (Za = {})),
         function(t) {
             t[t.OFFSET = 0] = "OFFSET", t[t.DATA = 1] = "DATA", t[t.VALIDITY = 2] = "VALIDITY", t[t.TYPE = 3] = "TYPE"
-        }(ra || (ra = {}));
-        const [aa, la] = (() => {
+        }(Ga || (Ga = {}));
+        const [el, nl] = (() => {
             const t = () => {
                 throw new Error("BigInt is not available in this environment")
             };
 
             function e() {
                 throw t()
             }
             return e.asIntN = () => {
                 throw t()
             }, e.asUintN = () => {
                 throw t()
             }, "undefined" !== typeof BigInt ? [BigInt, !0] : [e, !1]
-        })(), [ca, ua] = (() => {
+        })(), [il, rl] = (() => {
             const t = () => {
                 throw new Error("BigInt64Array is not available in this environment")
             };
             return "undefined" !== typeof BigInt64Array ? [BigInt64Array, !0] : [class {
                 static get BYTES_PER_ELEMENT() {
                     return 8
                 }
@@ -17414,15 +18141,15 @@
                 static from() {
                     throw t()
                 }
                 constructor() {
                     throw t()
                 }
             }, !1]
-        })(), [ha, da] = (() => {
+        })(), [sl, ol] = (() => {
             const t = () => {
                 throw new Error("BigUint64Array is not available in this environment")
             };
             return "undefined" !== typeof BigUint64Array ? [BigUint64Array, !0] : [class {
                 static get BYTES_PER_ELEMENT() {
                     return 8
                 }
@@ -17432,30 +18159,30 @@
                 static from() {
                     throw t()
                 }
                 constructor() {
                     throw t()
                 }
             }, !1]
-        })(), fa = t => "number" === typeof t, pa = t => "boolean" === typeof t, ga = t => "function" === typeof t, ma = t => null != t && Object(t) === t, ya = t => ma(t) && ga(t.then), ba = t => ma(t) && ga(t[Symbol.iterator]), va = t => ma(t) && ga(t[Symbol.asyncIterator]), _a = t => ma(t) && ma(t.schema), xa = t => ma(t) && "done" in t && "value" in t, wa = t => ma(t) && ga(t.stat) && fa(t.fd), Sa = t => ma(t) && ka(t.body), Ta = t => "_getDOMStream" in t && "_getNodeStream" in t, ka = t => ma(t) && ga(t.cancel) && ga(t.getReader) && !Ta(t), Ma = t => ma(t) && ga(t.read) && ga(t.pipe) && pa(t.readable) && !Ta(t), Ia = t => ma(t) && ga(t.clear) && ga(t.bytes) && ga(t.position) && ga(t.setPosition) && ga(t.capacity) && ga(t.getBufferIdentifier) && ga(t.createLong);
+        })(), al = t => "number" === typeof t, ll = t => "boolean" === typeof t, cl = t => "function" === typeof t, ul = t => null != t && Object(t) === t, hl = t => ul(t) && cl(t.then), dl = t => ul(t) && cl(t[Symbol.iterator]), fl = t => ul(t) && cl(t[Symbol.asyncIterator]), pl = t => ul(t) && ul(t.schema), gl = t => ul(t) && "done" in t && "value" in t, ml = t => ul(t) && cl(t.stat) && al(t.fd), yl = t => ul(t) && vl(t.body), bl = t => "_getDOMStream" in t && "_getNodeStream" in t, vl = t => ul(t) && cl(t.cancel) && cl(t.getReader) && !bl(t), _l = t => ul(t) && cl(t.read) && cl(t.pipe) && ll(t.readable) && !bl(t), xl = t => ul(t) && cl(t.clear) && cl(t.bytes) && cl(t.position) && cl(t.setPosition) && cl(t.capacity) && cl(t.getBufferIdentifier) && cl(t.createLong);
 
-        function Ea(t) {
+        function wl(t) {
             if (null === t) return "null";
             if (undefined === t) return "undefined";
             switch (typeof t) {
                 case "number":
                 case "bigint":
                     return "".concat(t);
                 case "string":
                     return '"'.concat(t, '"')
             }
-            return "function" === typeof t[Symbol.toPrimitive] ? t[Symbol.toPrimitive]("string") : ArrayBuffer.isView(t) ? "[".concat(t instanceof ca || t instanceof ha ? [...t].map((t => Ea(t))) : t, "]") : ArrayBuffer.isView(t) ? "[".concat(t, "]") : JSON.stringify(t, ((t, e) => "bigint" === typeof e ? "".concat(e) : e))
+            return "function" === typeof t[Symbol.toPrimitive] ? t[Symbol.toPrimitive]("string") : ArrayBuffer.isView(t) ? "[".concat(t instanceof il || t instanceof sl ? [...t].map((t => wl(t))) : t, "]") : ArrayBuffer.isView(t) ? "[".concat(t, "]") : JSON.stringify(t, ((t, e) => "bigint" === typeof e ? "".concat(e) : e))
         }
 
-        function Oa(t, e, n, i) {
+        function Sl(t, e, n, i) {
             return new(n || (n = Promise))((function(r, s) {
                 function o(t) {
                     try {
                         l(i.next(t))
                     } catch (e) {
                         s(e)
                     }
@@ -17476,15 +18203,15 @@
                     }))).then(o, a)
                 }
                 l((i = i.apply(t, e || [])).next())
             }))
         }
         Object.create;
 
-        function Da(t) {
+        function Tl(t) {
             var e = "function" === typeof Symbol && Symbol.iterator,
                 n = e && t[e],
                 i = 0;
             if (n) return n.call(t);
             if (t && "number" === typeof t.length) return {
                 next: function() {
                     return t && i >= t.length && (t = void 0), {
@@ -17492,19 +18219,19 @@
                         done: !t
                     }
                 }
             };
             throw new TypeError(e ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Aa(t) {
-            return this instanceof Aa ? (this.v = t, this) : new Aa(t)
+        function kl(t) {
+            return this instanceof kl ? (this.v = t, this) : new kl(t)
         }
 
-        function Ca(t, e, n) {
+        function Ml(t, e, n) {
             if (!Symbol.asyncIterator) throw new TypeError("Symbol.asyncIterator is not defined.");
             var i, r = n.apply(t, e || []),
                 s = [];
             return i = {}, o("next"), o("throw"), o("return"), i[Symbol.asyncIterator] = function() {
                 return this
             }, i;
 
@@ -17514,15 +18241,15 @@
                         s.push([t, e, n, i]) > 1 || a(t, e)
                     }))
                 })
             }
 
             function a(t, e) {
                 try {
-                    (n = r[t](e)).value instanceof Aa ? Promise.resolve(n.value.v).then(l, c) : u(s[0][2], n)
+                    (n = r[t](e)).value instanceof kl ? Promise.resolve(n.value.v).then(l, c) : u(s[0][2], n)
                 } catch (i) {
                     u(s[0][3], i)
                 }
                 var n
             }
 
             function l(t) {
@@ -17534,36 +18261,36 @@
             }
 
             function u(t, e) {
                 t(e), s.shift(), s.length && a(s[0][0], s[0][1])
             }
         }
 
-        function Pa(t) {
+        function Il(t) {
             var e, n;
             return e = {}, i("next"), i("throw", (function(t) {
                 throw t
             })), i("return"), e[Symbol.iterator] = function() {
                 return this
             }, e;
 
             function i(i, r) {
                 e[i] = t[i] ? function(e) {
                     return (n = !n) ? {
-                        value: Aa(t[i](e)),
+                        value: kl(t[i](e)),
                         done: !1
                     } : r ? r(e) : e
                 } : r
             }
         }
 
-        function Fa(t) {
+        function El(t) {
             if (!Symbol.asyncIterator) throw new TypeError("Symbol.asyncIterator is not defined.");
             var e, n = t[Symbol.asyncIterator];
-            return n ? n.call(t) : (t = Da(t), e = {}, i("next"), i("throw"), i("return"), e[Symbol.asyncIterator] = function() {
+            return n ? n.call(t) : (t = Tl(t), e = {}, i("next"), i("throw"), i("return"), e[Symbol.asyncIterator] = function() {
                 return this
             }, e);
 
             function i(n) {
                 e[n] = t[n] && function(e) {
                     return new Promise((function(i, r) {
                         (function(t, e, n, i) {
@@ -17576,30 +18303,30 @@
                         })(i, r, (e = t[n](e)).done, e.value)
                     }))
                 }
             }
         }
         Object.create;
         "function" === typeof SuppressedError && SuppressedError;
-        const La = new TextDecoder("utf-8"),
-            Na = t => La.decode(t),
-            Ba = new TextEncoder,
-            Ra = t => Ba.encode(t),
-            za = "undefined" !== typeof SharedArrayBuffer ? SharedArrayBuffer : ArrayBuffer;
+        const Ol = new TextDecoder("utf-8"),
+            Dl = t => Ol.decode(t),
+            Al = new TextEncoder,
+            Cl = t => Al.encode(t),
+            Pl = "undefined" !== typeof SharedArrayBuffer ? SharedArrayBuffer : ArrayBuffer;
 
-        function Ua(t, e) {
+        function Fl(t, e) {
             let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 0,
                 i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : e.byteLength;
             const r = t.byteLength,
                 s = new Uint8Array(t.buffer, t.byteOffset, r),
                 o = new Uint8Array(e.buffer, e.byteOffset, Math.min(i, r));
             return s.set(o, n), t
         }
 
-        function Va(t, e) {
+        function Ll(t, e) {
             const n = function(t) {
                     const e = t[0] ? [t[0]] : [];
                     let n, i, r, s;
                     for (let o, a, l = 0, c = 0, u = t.length; ++l < u;) o = e[c], a = t[l], !o || !a || o.buffer !== a.buffer || a.byteOffset < o.byteOffset ? a && (e[++c] = a) : (({
                         byteOffset: n,
                         byteLength: r
                     } = o), ({
@@ -17610,625 +18337,625 @@
                 }(t),
                 i = n.reduce(((t, e) => t + e.byteLength), 0);
             let r, s, o, a = 0,
                 l = -1;
             const c = Math.min(e || Number.POSITIVE_INFINITY, i);
             for (const u = n.length; ++l < u;) {
                 if (r = n[l], s = r.subarray(0, Math.min(r.length, c - a)), c <= a + s.length) {
-                    s.length < r.length ? n[l] = r.subarray(s.length) : s.length === r.length && l++, o ? Ua(o, s, a) : o = s;
+                    s.length < r.length ? n[l] = r.subarray(s.length) : s.length === r.length && l++, o ? Fl(o, s, a) : o = s;
                     break
                 }
-                Ua(o || (o = new Uint8Array(c)), s, a), a += s.length
+                Fl(o || (o = new Uint8Array(c)), s, a), a += s.length
             }
             return [o || new Uint8Array(0), n.slice(l), i - (o ? o.byteLength : 0)]
         }
 
-        function ja(t, e) {
-            let n = xa(e) ? e.value : e;
-            return n instanceof t ? t === Uint8Array ? new t(n.buffer, n.byteOffset, n.byteLength) : n : n ? ("string" === typeof n && (n = Ra(n)), n instanceof ArrayBuffer || n instanceof za ? new t(n) : Ia(n) ? ja(t, n.bytes()) : ArrayBuffer.isView(n) ? n.byteLength <= 0 ? new t(0) : new t(n.buffer, n.byteOffset, n.byteLength / t.BYTES_PER_ELEMENT) : t.from(n)) : new t(0)
-        }
-        const Wa = t => ja(Int32Array, t),
-            Ha = t => ja(Uint8Array, t),
-            Ya = t => (t.next(), t);
+        function Nl(t, e) {
+            let n = gl(e) ? e.value : e;
+            return n instanceof t ? t === Uint8Array ? new t(n.buffer, n.byteOffset, n.byteLength) : n : n ? ("string" === typeof n && (n = Cl(n)), n instanceof ArrayBuffer || n instanceof Pl ? new t(n) : xl(n) ? Nl(t, n.bytes()) : ArrayBuffer.isView(n) ? n.byteLength <= 0 ? new t(0) : new t(n.buffer, n.byteOffset, n.byteLength / t.BYTES_PER_ELEMENT) : t.from(n)) : new t(0)
+        }
+        const Bl = t => Nl(Int32Array, t),
+            Rl = t => Nl(Uint8Array, t),
+            zl = t => (t.next(), t);
 
-        function* $a(t, e) {
+        function* Ul(t, e) {
             const n = function*(t) {
                     yield t
                 },
-                i = "string" === typeof e || ArrayBuffer.isView(e) || e instanceof ArrayBuffer || e instanceof za ? n(e) : ba(e) ? e : n(e);
-            return yield* Ya(function*(e) {
+                i = "string" === typeof e || ArrayBuffer.isView(e) || e instanceof ArrayBuffer || e instanceof Pl ? n(e) : dl(e) ? e : n(e);
+            return yield* zl(function*(e) {
                 let n = null;
                 do {
-                    n = e.next(yield ja(t, n))
+                    n = e.next(yield Nl(t, n))
                 } while (!n.done)
             }(i[Symbol.iterator]())), new t
         }
 
-        function Ka(t, e) {
-            return Ca(this, arguments, (function*() {
-                if (ya(e)) return yield Aa(yield Aa(yield* Pa(Fa(Ka(t, yield Aa(e))))));
+        function Vl(t, e) {
+            return Ml(this, arguments, (function*() {
+                if (hl(e)) return yield kl(yield kl(yield* Il(El(Vl(t, yield kl(e))))));
                 const n = function(t) {
-                        return Ca(this, arguments, (function*() {
-                            yield yield Aa(yield Aa(t))
+                        return Ml(this, arguments, (function*() {
+                            yield yield kl(yield kl(t))
                         }))
                     },
-                    i = "string" === typeof e || ArrayBuffer.isView(e) || e instanceof ArrayBuffer || e instanceof za ? n(e) : ba(e) ? function(t) {
-                        return Ca(this, arguments, (function*() {
-                            yield Aa(yield* Pa(Fa(Ya(function*(t) {
+                    i = "string" === typeof e || ArrayBuffer.isView(e) || e instanceof ArrayBuffer || e instanceof Pl ? n(e) : dl(e) ? function(t) {
+                        return Ml(this, arguments, (function*() {
+                            yield kl(yield* Il(El(zl(function*(t) {
                                 let e = null;
                                 do {
                                     e = t.next(yield null === e || void 0 === e ? void 0 : e.value)
                                 } while (!e.done)
                             }(t[Symbol.iterator]())))))
                         }))
-                    }(e) : va(e) ? e : n(e);
-                return yield Aa(yield* Pa(Fa(Ya(function(e) {
-                    return Ca(this, arguments, (function*() {
+                    }(e) : fl(e) ? e : n(e);
+                return yield kl(yield* Il(El(zl(function(e) {
+                    return Ml(this, arguments, (function*() {
                         let n = null;
                         do {
-                            n = yield Aa(e.next(yield yield Aa(ja(t, n))))
+                            n = yield kl(e.next(yield yield kl(Nl(t, n))))
                         } while (!n.done)
                     }))
-                }(i[Symbol.asyncIterator]()))))), yield Aa(new t)
+                }(i[Symbol.asyncIterator]()))))), yield kl(new t)
             }))
         }
 
-        function Xa(t, e, n) {
+        function jl(t, e, n) {
             if (0 !== t) {
                 n = n.slice(0, e + 1);
                 for (let i = -1; ++i <= e;) n[i] += t
             }
             return n
         }
-        const qa = Symbol.for("isArrowBigNum");
+        const Wl = Symbol.for("isArrowBigNum");
 
-        function Qa(t) {
+        function Hl(t) {
             for (var e = arguments.length, n = new Array(e > 1 ? e - 1 : 0), i = 1; i < e; i++) n[i - 1] = arguments[i];
-            return 0 === n.length ? Object.setPrototypeOf(ja(this.TypedArray, t), this.constructor.prototype) : Object.setPrototypeOf(new this.TypedArray(t, ...n), this.constructor.prototype)
+            return 0 === n.length ? Object.setPrototypeOf(Nl(this.TypedArray, t), this.constructor.prototype) : Object.setPrototypeOf(new this.TypedArray(t, ...n), this.constructor.prototype)
         }
 
-        function Za() {
+        function Yl() {
             for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-            return Qa.apply(this, e)
+            return Hl.apply(this, e)
         }
 
-        function Ga() {
+        function $l() {
             for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-            return Qa.apply(this, e)
+            return Hl.apply(this, e)
         }
 
-        function Ja() {
+        function Kl() {
             for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-            return Qa.apply(this, e)
+            return Hl.apply(this, e)
         }
 
-        function tl(t) {
+        function Xl(t) {
             const {
                 buffer: e,
                 byteOffset: n,
                 length: i,
                 signed: r
-            } = t, s = new ha(e, n, i), o = r && s[s.length - 1] & BigInt(1) << BigInt(63);
+            } = t, s = new sl(e, n, i), o = r && s[s.length - 1] & BigInt(1) << BigInt(63);
             let a = o ? BigInt(1) : BigInt(0),
                 l = BigInt(0);
             if (o) {
                 for (const t of s) a += ~t * (BigInt(1) << BigInt(32) * l++);
                 a *= BigInt(-1)
             } else
                 for (const c of s) a += c * (BigInt(1) << BigInt(32) * l++);
             return a
         }
-        let el, nl;
+        let ql, Ql;
 
-        function il(t) {
+        function Zl(t) {
             let e = "";
             const n = new Uint32Array(2);
             let i = new Uint16Array(t.buffer, t.byteOffset, t.byteLength / 2);
             const r = new Uint32Array((i = new Uint16Array(i).reverse()).buffer);
             let s = -1;
             const o = i.length - 1;
             do {
                 for (n[0] = i[s = 0]; s < o;) i[s++] = n[1] = n[0] / 10, n[0] = (n[0] - 10 * n[1] << 16) + i[s];
                 i[s] = n[1] = n[0] / 10, n[0] = n[0] - 10 * n[1], e = "".concat(n[0]).concat(e)
             } while (r[0] || r[1] || r[2] || r[3]);
             return null !== e && void 0 !== e ? e : "0"
         }
-        Qa.prototype[qa] = !0, Qa.prototype.toJSON = function() {
-            return '"'.concat(el(this), '"')
-        }, Qa.prototype.valueOf = function() {
-            return tl(this)
-        }, Qa.prototype.toString = function() {
-            return el(this)
-        }, Qa.prototype[Symbol.toPrimitive] = function() {
+        Hl.prototype[Wl] = !0, Hl.prototype.toJSON = function() {
+            return '"'.concat(ql(this), '"')
+        }, Hl.prototype.valueOf = function() {
+            return Xl(this)
+        }, Hl.prototype.toString = function() {
+            return ql(this)
+        }, Hl.prototype[Symbol.toPrimitive] = function() {
             switch (arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "default") {
                 case "number":
-                    return tl(this);
+                    return Xl(this);
                 case "string":
-                    return el(this);
+                    return ql(this);
                 case "default":
-                    return nl(this)
+                    return Ql(this)
             }
-            return el(this)
-        }, Object.setPrototypeOf(Za.prototype, Object.create(Int32Array.prototype)), Object.setPrototypeOf(Ga.prototype, Object.create(Uint32Array.prototype)), Object.setPrototypeOf(Ja.prototype, Object.create(Uint32Array.prototype)), Object.assign(Za.prototype, Qa.prototype, {
-            constructor: Za,
+            return ql(this)
+        }, Object.setPrototypeOf(Yl.prototype, Object.create(Int32Array.prototype)), Object.setPrototypeOf($l.prototype, Object.create(Uint32Array.prototype)), Object.setPrototypeOf(Kl.prototype, Object.create(Uint32Array.prototype)), Object.assign(Yl.prototype, Hl.prototype, {
+            constructor: Yl,
             signed: !0,
             TypedArray: Int32Array,
-            BigIntArray: ca
-        }), Object.assign(Ga.prototype, Qa.prototype, {
-            constructor: Ga,
+            BigIntArray: il
+        }), Object.assign($l.prototype, Hl.prototype, {
+            constructor: $l,
             signed: !1,
             TypedArray: Uint32Array,
-            BigIntArray: ha
-        }), Object.assign(Ja.prototype, Qa.prototype, {
-            constructor: Ja,
+            BigIntArray: sl
+        }), Object.assign(Kl.prototype, Hl.prototype, {
+            constructor: Kl,
             signed: !0,
             TypedArray: Uint32Array,
-            BigIntArray: ha
-        }), la ? (nl = t => 8 === t.byteLength ? new t.BigIntArray(t.buffer, t.byteOffset, 1)[0] : il(t), el = t => 8 === t.byteLength ? "".concat(new t.BigIntArray(t.buffer, t.byteOffset, 1)[0]) : il(t)) : (el = il, nl = el);
-        class rl {
+            BigIntArray: sl
+        }), nl ? (Ql = t => 8 === t.byteLength ? new t.BigIntArray(t.buffer, t.byteOffset, 1)[0] : Zl(t), ql = t => 8 === t.byteLength ? "".concat(new t.BigIntArray(t.buffer, t.byteOffset, 1)[0]) : Zl(t)) : (ql = Zl, Ql = ql);
+        class Gl {
             static new(t, e) {
                 switch (e) {
                     case !0:
-                        return new Za(t);
+                        return new Yl(t);
                     case !1:
-                        return new Ga(t)
+                        return new $l(t)
                 }
                 switch (t.constructor) {
                     case Int8Array:
                     case Int16Array:
                     case Int32Array:
-                    case ca:
-                        return new Za(t)
+                    case il:
+                        return new Yl(t)
                 }
-                return 16 === t.byteLength ? new Ja(t) : new Ga(t)
+                return 16 === t.byteLength ? new Kl(t) : new $l(t)
             }
             static signed(t) {
-                return new Za(t)
+                return new Yl(t)
             }
             static unsigned(t) {
-                return new Ga(t)
+                return new $l(t)
             }
             static decimal(t) {
-                return new Ja(t)
+                return new Kl(t)
             }
             constructor(t, e) {
-                return rl.new(t, e)
+                return Gl.new(t, e)
             }
         }
-        var sl, ol, al, ll, cl, ul, hl, dl, fl, pl, gl, ml, yl, bl, vl, _l, xl, wl, Sl, Tl;
-        class kl {
+        var Jl, tc, ec, nc, ic, rc, sc, oc, ac, lc, cc, uc, hc, dc, fc, pc, gc, mc, yc, bc;
+        class vc {
             static isNull(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Null
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Null
             }
             static isInt(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Int
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Int
             }
             static isFloat(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Float
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Float
             }
             static isBinary(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Binary
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Binary
             }
             static isUtf8(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Utf8
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Utf8
             }
             static isBool(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Bool
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Bool
             }
             static isDecimal(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Decimal
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Decimal
             }
             static isDate(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Date
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Date
             }
             static isTime(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Time
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Time
             }
             static isTimestamp(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Timestamp
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Timestamp
             }
             static isInterval(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Interval
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Interval
             }
             static isList(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.List
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.List
             }
             static isStruct(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Struct
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Struct
             }
             static isUnion(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Union
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Union
             }
             static isFixedSizeBinary(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.FixedSizeBinary
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.FixedSizeBinary
             }
             static isFixedSizeList(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.FixedSizeList
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.FixedSizeList
             }
             static isMap(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Map
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Map
             }
             static isDictionary(t) {
-                return (null === t || void 0 === t ? void 0 : t.typeId) === ia.Dictionary
+                return (null === t || void 0 === t ? void 0 : t.typeId) === Za.Dictionary
             }
             static isDenseUnion(t) {
-                return kl.isUnion(t) && t.mode === Zo.Dense
+                return vc.isUnion(t) && t.mode === Ya.Dense
             }
             static isSparseUnion(t) {
-                return kl.isUnion(t) && t.mode === Zo.Sparse
+                return vc.isUnion(t) && t.mode === Ya.Sparse
             }
             get typeId() {
-                return ia.NONE
+                return Za.NONE
             }
         }
-        sl = Symbol.toStringTag, kl[sl] = ((Tl = kl.prototype).children = null, Tl.ArrayType = Array, Tl[Symbol.toStringTag] = "DataType");
-        class Ml extends kl {
+        Jl = Symbol.toStringTag, vc[Jl] = ((bc = vc.prototype).children = null, bc.ArrayType = Array, bc[Symbol.toStringTag] = "DataType");
+        class _c extends vc {
             toString() {
                 return "Null"
             }
             get typeId() {
-                return ia.Null
+                return Za.Null
             }
         }
-        ol = Symbol.toStringTag, Ml[ol] = (t => t[Symbol.toStringTag] = "Null")(Ml.prototype);
-        class Il extends kl {
+        tc = Symbol.toStringTag, _c[tc] = (t => t[Symbol.toStringTag] = "Null")(_c.prototype);
+        class xc extends vc {
             constructor(t, e) {
                 super(), this.isSigned = t, this.bitWidth = e
             }
             get typeId() {
-                return ia.Int
+                return Za.Int
             }
             get ArrayType() {
                 switch (this.bitWidth) {
                     case 8:
                         return this.isSigned ? Int8Array : Uint8Array;
                     case 16:
                         return this.isSigned ? Int16Array : Uint16Array;
                     case 32:
                         return this.isSigned ? Int32Array : Uint32Array;
                     case 64:
-                        return this.isSigned ? ca : ha
+                        return this.isSigned ? il : sl
                 }
                 throw new Error("Unrecognized ".concat(this[Symbol.toStringTag], " type"))
             }
             toString() {
                 return "".concat(this.isSigned ? "I" : "Ui", "nt").concat(this.bitWidth)
             }
         }
-        al = Symbol.toStringTag, Il[al] = (t => (t.isSigned = null, t.bitWidth = null, t[Symbol.toStringTag] = "Int"))(Il.prototype);
-        class El extends Il {
+        ec = Symbol.toStringTag, xc[ec] = (t => (t.isSigned = null, t.bitWidth = null, t[Symbol.toStringTag] = "Int"))(xc.prototype);
+        class wc extends xc {
             constructor() {
                 super(!0, 32)
             }
             get ArrayType() {
                 return Int32Array
             }
         }
-        Object.defineProperty(class extends Il {
+        Object.defineProperty(class extends xc {
             constructor() {
                 super(!0, 8)
             }
             get ArrayType() {
                 return Int8Array
             }
         }.prototype, "ArrayType", {
             value: Int8Array
-        }), Object.defineProperty(class extends Il {
+        }), Object.defineProperty(class extends xc {
             constructor() {
                 super(!0, 16)
             }
             get ArrayType() {
                 return Int16Array
             }
         }.prototype, "ArrayType", {
             value: Int16Array
-        }), Object.defineProperty(El.prototype, "ArrayType", {
+        }), Object.defineProperty(wc.prototype, "ArrayType", {
             value: Int32Array
-        }), Object.defineProperty(class extends Il {
+        }), Object.defineProperty(class extends xc {
             constructor() {
                 super(!0, 64)
             }
             get ArrayType() {
-                return ca
+                return il
             }
         }.prototype, "ArrayType", {
-            value: ca
-        }), Object.defineProperty(class extends Il {
+            value: il
+        }), Object.defineProperty(class extends xc {
             constructor() {
                 super(!1, 8)
             }
             get ArrayType() {
                 return Uint8Array
             }
         }.prototype, "ArrayType", {
             value: Uint8Array
-        }), Object.defineProperty(class extends Il {
+        }), Object.defineProperty(class extends xc {
             constructor() {
                 super(!1, 16)
             }
             get ArrayType() {
                 return Uint16Array
             }
         }.prototype, "ArrayType", {
             value: Uint16Array
-        }), Object.defineProperty(class extends Il {
+        }), Object.defineProperty(class extends xc {
             constructor() {
                 super(!1, 32)
             }
             get ArrayType() {
                 return Uint32Array
             }
         }.prototype, "ArrayType", {
             value: Uint32Array
-        }), Object.defineProperty(class extends Il {
+        }), Object.defineProperty(class extends xc {
             constructor() {
                 super(!1, 64)
             }
             get ArrayType() {
-                return ha
+                return sl
             }
         }.prototype, "ArrayType", {
-            value: ha
+            value: sl
         });
-        class Ol extends kl {
+        class Sc extends vc {
             constructor(t) {
                 super(), this.precision = t
             }
             get typeId() {
-                return ia.Float
+                return Za.Float
             }
             get ArrayType() {
                 switch (this.precision) {
-                    case Go.HALF:
+                    case $a.HALF:
                         return Uint16Array;
-                    case Go.SINGLE:
+                    case $a.SINGLE:
                         return Float32Array;
-                    case Go.DOUBLE:
+                    case $a.DOUBLE:
                         return Float64Array
                 }
                 throw new Error("Unrecognized ".concat(this[Symbol.toStringTag], " type"))
             }
             toString() {
                 return "Float".concat(this.precision << 5 || 16)
             }
         }
-        ll = Symbol.toStringTag, Ol[ll] = (t => (t.precision = null, t[Symbol.toStringTag] = "Float"))(Ol.prototype);
-        Object.defineProperty(class extends Ol {
+        nc = Symbol.toStringTag, Sc[nc] = (t => (t.precision = null, t[Symbol.toStringTag] = "Float"))(Sc.prototype);
+        Object.defineProperty(class extends Sc {
             constructor() {
-                super(Go.HALF)
+                super($a.HALF)
             }
         }.prototype, "ArrayType", {
             value: Uint16Array
-        }), Object.defineProperty(class extends Ol {
+        }), Object.defineProperty(class extends Sc {
             constructor() {
-                super(Go.SINGLE)
+                super($a.SINGLE)
             }
         }.prototype, "ArrayType", {
             value: Float32Array
-        }), Object.defineProperty(class extends Ol {
+        }), Object.defineProperty(class extends Sc {
             constructor() {
-                super(Go.DOUBLE)
+                super($a.DOUBLE)
             }
         }.prototype, "ArrayType", {
             value: Float64Array
         });
-        class Dl extends kl {
+        class Tc extends vc {
             constructor() {
                 super()
             }
             get typeId() {
-                return ia.Binary
+                return Za.Binary
             }
             toString() {
                 return "Binary"
             }
         }
-        cl = Symbol.toStringTag, Dl[cl] = (t => (t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "Binary"))(Dl.prototype);
-        class Al extends kl {
+        ic = Symbol.toStringTag, Tc[ic] = (t => (t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "Binary"))(Tc.prototype);
+        class kc extends vc {
             constructor() {
                 super()
             }
             get typeId() {
-                return ia.Utf8
+                return Za.Utf8
             }
             toString() {
                 return "Utf8"
             }
         }
-        ul = Symbol.toStringTag, Al[ul] = (t => (t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "Utf8"))(Al.prototype);
-        class Cl extends kl {
+        rc = Symbol.toStringTag, kc[rc] = (t => (t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "Utf8"))(kc.prototype);
+        class Mc extends vc {
             constructor() {
                 super()
             }
             get typeId() {
-                return ia.Bool
+                return Za.Bool
             }
             toString() {
                 return "Bool"
             }
         }
-        hl = Symbol.toStringTag, Cl[hl] = (t => (t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "Bool"))(Cl.prototype);
-        class Pl extends kl {
+        sc = Symbol.toStringTag, Mc[sc] = (t => (t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "Bool"))(Mc.prototype);
+        class Ic extends vc {
             constructor(t, e) {
                 let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 128;
                 super(), this.scale = t, this.precision = e, this.bitWidth = n
             }
             get typeId() {
-                return ia.Decimal
+                return Za.Decimal
             }
             toString() {
                 return "Decimal[".concat(this.precision, "e").concat(this.scale > 0 ? "+" : "").concat(this.scale, "]")
             }
         }
-        dl = Symbol.toStringTag, Pl[dl] = (t => (t.scale = null, t.precision = null, t.ArrayType = Uint32Array, t[Symbol.toStringTag] = "Decimal"))(Pl.prototype);
-        class Fl extends kl {
+        oc = Symbol.toStringTag, Ic[oc] = (t => (t.scale = null, t.precision = null, t.ArrayType = Uint32Array, t[Symbol.toStringTag] = "Decimal"))(Ic.prototype);
+        class Ec extends vc {
             constructor(t) {
                 super(), this.unit = t
             }
             get typeId() {
-                return ia.Date
+                return Za.Date
             }
             toString() {
-                return "Date".concat(32 * (this.unit + 1), "<").concat(Jo[this.unit], ">")
+                return "Date".concat(32 * (this.unit + 1), "<").concat(Ka[this.unit], ">")
             }
         }
-        fl = Symbol.toStringTag, Fl[fl] = (t => (t.unit = null, t.ArrayType = Int32Array, t[Symbol.toStringTag] = "Date"))(Fl.prototype);
-        class Ll extends kl {
+        ac = Symbol.toStringTag, Ec[ac] = (t => (t.unit = null, t.ArrayType = Int32Array, t[Symbol.toStringTag] = "Date"))(Ec.prototype);
+        class Oc extends vc {
             constructor(t, e) {
                 super(), this.unit = t, this.bitWidth = e
             }
             get typeId() {
-                return ia.Time
+                return Za.Time
             }
             toString() {
-                return "Time".concat(this.bitWidth, "<").concat(ta[this.unit], ">")
+                return "Time".concat(this.bitWidth, "<").concat(Xa[this.unit], ">")
             }
             get ArrayType() {
                 switch (this.bitWidth) {
                     case 32:
                         return Int32Array;
                     case 64:
-                        return ca
+                        return il
                 }
                 throw new Error("Unrecognized ".concat(this[Symbol.toStringTag], " type"))
             }
         }
-        pl = Symbol.toStringTag, Ll[pl] = (t => (t.unit = null, t.bitWidth = null, t[Symbol.toStringTag] = "Time"))(Ll.prototype);
-        class Nl extends kl {
+        lc = Symbol.toStringTag, Oc[lc] = (t => (t.unit = null, t.bitWidth = null, t[Symbol.toStringTag] = "Time"))(Oc.prototype);
+        class Dc extends vc {
             constructor(t, e) {
                 super(), this.unit = t, this.timezone = e
             }
             get typeId() {
-                return ia.Timestamp
+                return Za.Timestamp
             }
             toString() {
-                return "Timestamp<".concat(ta[this.unit]).concat(this.timezone ? ", ".concat(this.timezone) : "", ">")
+                return "Timestamp<".concat(Xa[this.unit]).concat(this.timezone ? ", ".concat(this.timezone) : "", ">")
             }
         }
-        gl = Symbol.toStringTag, Nl[gl] = (t => (t.unit = null, t.timezone = null, t.ArrayType = Int32Array, t[Symbol.toStringTag] = "Timestamp"))(Nl.prototype);
-        class Bl extends kl {
+        cc = Symbol.toStringTag, Dc[cc] = (t => (t.unit = null, t.timezone = null, t.ArrayType = Int32Array, t[Symbol.toStringTag] = "Timestamp"))(Dc.prototype);
+        class Ac extends vc {
             constructor(t) {
                 super(), this.unit = t
             }
             get typeId() {
-                return ia.Interval
+                return Za.Interval
             }
             toString() {
-                return "Interval<".concat(ea[this.unit], ">")
+                return "Interval<".concat(qa[this.unit], ">")
             }
         }
-        ml = Symbol.toStringTag, Bl[ml] = (t => (t.unit = null, t.ArrayType = Int32Array, t[Symbol.toStringTag] = "Interval"))(Bl.prototype);
-        class Rl extends kl {
+        uc = Symbol.toStringTag, Ac[uc] = (t => (t.unit = null, t.ArrayType = Int32Array, t[Symbol.toStringTag] = "Interval"))(Ac.prototype);
+        class Cc extends vc {
             constructor(t) {
                 super(), this.children = [t]
             }
             get typeId() {
-                return ia.List
+                return Za.List
             }
             toString() {
                 return "List<".concat(this.valueType, ">")
             }
             get valueType() {
                 return this.children[0].type
             }
             get valueField() {
                 return this.children[0]
             }
             get ArrayType() {
                 return this.valueType.ArrayType
             }
         }
-        yl = Symbol.toStringTag, Rl[yl] = (t => (t.children = null, t[Symbol.toStringTag] = "List"))(Rl.prototype);
-        class zl extends kl {
+        hc = Symbol.toStringTag, Cc[hc] = (t => (t.children = null, t[Symbol.toStringTag] = "List"))(Cc.prototype);
+        class Pc extends vc {
             constructor(t) {
                 super(), this.children = t
             }
             get typeId() {
-                return ia.Struct
+                return Za.Struct
             }
             toString() {
                 return "Struct<{".concat(this.children.map((t => "".concat(t.name, ":").concat(t.type))).join(", "), "}>")
             }
         }
-        bl = Symbol.toStringTag, zl[bl] = (t => (t.children = null, t[Symbol.toStringTag] = "Struct"))(zl.prototype);
-        class Ul extends kl {
+        dc = Symbol.toStringTag, Pc[dc] = (t => (t.children = null, t[Symbol.toStringTag] = "Struct"))(Pc.prototype);
+        class Fc extends vc {
             constructor(t, e, n) {
                 super(), this.mode = t, this.children = n, this.typeIds = e = Int32Array.from(e), this.typeIdToChildIndex = e.reduce(((t, e, n) => (t[e] = n) && t || t), Object.create(null))
             }
             get typeId() {
-                return ia.Union
+                return Za.Union
             }
             toString() {
                 return "".concat(this[Symbol.toStringTag], "<").concat(this.children.map((t => "".concat(t.type))).join(" | "), ">")
             }
         }
-        vl = Symbol.toStringTag, Ul[vl] = (t => (t.mode = null, t.typeIds = null, t.children = null, t.typeIdToChildIndex = null, t.ArrayType = Int8Array, t[Symbol.toStringTag] = "Union"))(Ul.prototype);
-        class Vl extends kl {
+        fc = Symbol.toStringTag, Fc[fc] = (t => (t.mode = null, t.typeIds = null, t.children = null, t.typeIdToChildIndex = null, t.ArrayType = Int8Array, t[Symbol.toStringTag] = "Union"))(Fc.prototype);
+        class Lc extends vc {
             constructor(t) {
                 super(), this.byteWidth = t
             }
             get typeId() {
-                return ia.FixedSizeBinary
+                return Za.FixedSizeBinary
             }
             toString() {
                 return "FixedSizeBinary[".concat(this.byteWidth, "]")
             }
         }
-        _l = Symbol.toStringTag, Vl[_l] = (t => (t.byteWidth = null, t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "FixedSizeBinary"))(Vl.prototype);
-        class jl extends kl {
+        pc = Symbol.toStringTag, Lc[pc] = (t => (t.byteWidth = null, t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "FixedSizeBinary"))(Lc.prototype);
+        class Nc extends vc {
             constructor(t, e) {
                 super(), this.listSize = t, this.children = [e]
             }
             get typeId() {
-                return ia.FixedSizeList
+                return Za.FixedSizeList
             }
             get valueType() {
                 return this.children[0].type
             }
             get valueField() {
                 return this.children[0]
             }
             get ArrayType() {
                 return this.valueType.ArrayType
             }
             toString() {
                 return "FixedSizeList[".concat(this.listSize, "]<").concat(this.valueType, ">")
             }
         }
-        xl = Symbol.toStringTag, jl[xl] = (t => (t.children = null, t.listSize = null, t[Symbol.toStringTag] = "FixedSizeList"))(jl.prototype);
-        class Wl extends kl {
+        gc = Symbol.toStringTag, Nc[gc] = (t => (t.children = null, t.listSize = null, t[Symbol.toStringTag] = "FixedSizeList"))(Nc.prototype);
+        class Bc extends vc {
             constructor(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] && arguments[1];
                 super(), this.children = [t], this.keysSorted = e
             }
             get typeId() {
-                return ia.Map
+                return Za.Map
             }
             get keyType() {
                 return this.children[0].type.children[0].type
             }
             get valueType() {
                 return this.children[0].type.children[1].type
             }
             get childType() {
                 return this.children[0].type
             }
             toString() {
                 return "Map<{".concat(this.children[0].type.children.map((t => "".concat(t.name, ":").concat(t.type))).join(", "), "}>")
             }
         }
-        wl = Symbol.toStringTag, Wl[wl] = (t => (t.children = null, t.keysSorted = null, t[Symbol.toStringTag] = "Map_"))(Wl.prototype);
-        const Hl = (Yl = -1, () => ++Yl);
-        var Yl;
-        class $l extends kl {
+        mc = Symbol.toStringTag, Bc[mc] = (t => (t.children = null, t.keysSorted = null, t[Symbol.toStringTag] = "Map_"))(Bc.prototype);
+        const Rc = (zc = -1, () => ++zc);
+        var zc;
+        class Uc extends vc {
             constructor(t, e, n, i) {
-                super(), this.indices = e, this.dictionary = t, this.isOrdered = i || !1, this.id = null == n ? Hl() : "number" === typeof n ? n : n.low
+                super(), this.indices = e, this.dictionary = t, this.isOrdered = i || !1, this.id = null == n ? Rc() : "number" === typeof n ? n : n.low
             }
             get typeId() {
-                return ia.Dictionary
+                return Za.Dictionary
             }
             get children() {
                 return this.dictionary.children
             }
             get valueType() {
                 return this.dictionary
             }
@@ -18236,54 +18963,54 @@
                 return this.dictionary.ArrayType
             }
             toString() {
                 return "Dictionary<".concat(this.indices, ", ").concat(this.dictionary, ">")
             }
         }
 
-        function Kl(t) {
+        function Vc(t) {
             const e = t;
             switch (t.typeId) {
-                case ia.Decimal:
+                case Za.Decimal:
                     return t.bitWidth / 32;
-                case ia.Timestamp:
+                case Za.Timestamp:
                     return 2;
-                case ia.Date:
-                case ia.Interval:
+                case Za.Date:
+                case Za.Interval:
                     return 1 + e.unit;
-                case ia.FixedSizeList:
+                case Za.FixedSizeList:
                     return e.listSize;
-                case ia.FixedSizeBinary:
+                case Za.FixedSizeBinary:
                     return e.byteWidth;
                 default:
                     return 1
             }
         }
-        Sl = Symbol.toStringTag, $l[Sl] = (t => (t.id = null, t.indices = null, t.isOrdered = null, t.dictionary = null, t[Symbol.toStringTag] = "Dictionary"))($l.prototype);
-        class Xl {
+        yc = Symbol.toStringTag, Uc[yc] = (t => (t.id = null, t.indices = null, t.isOrdered = null, t.dictionary = null, t[Symbol.toStringTag] = "Dictionary"))(Uc.prototype);
+        class jc {
             visitMany(t) {
                 for (var e = arguments.length, n = new Array(e > 1 ? e - 1 : 0), i = 1; i < e; i++) n[i - 1] = arguments[i];
                 return t.map(((t, e) => this.visit(t, ...n.map((t => t[e])))))
             }
             visit() {
                 for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
                 return this.getVisitFn(e[0], !1).apply(this, e)
             }
             getVisitFn(t) {
                 return function(t, e) {
                     let n = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2];
-                    if ("number" === typeof e) return ql(t, e, n);
-                    if ("string" === typeof e && e in ia) return ql(t, ia[e], n);
-                    if (e && e instanceof kl) return ql(t, Ql(e), n);
-                    if ((null === e || void 0 === e ? void 0 : e.type) && e.type instanceof kl) return ql(t, Ql(e.type), n);
-                    return ql(t, ia.NONE, n)
+                    if ("number" === typeof e) return Wc(t, e, n);
+                    if ("string" === typeof e && e in Za) return Wc(t, Za[e], n);
+                    if (e && e instanceof vc) return Wc(t, Hc(e), n);
+                    if ((null === e || void 0 === e ? void 0 : e.type) && e.type instanceof vc) return Wc(t, Hc(e.type), n);
+                    return Wc(t, Za.NONE, n)
                 }(this, t, !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1])
             }
             getVisitFnByTypeId(t) {
-                return ql(this, t, !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1])
+                return Wc(this, t, !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1])
             }
             visitNull(t) {
                 return null
             }
             visitBool(t) {
                 return null
             }
@@ -18333,933 +19060,933 @@
                 return null
             }
             visitMap(t) {
                 return null
             }
         }
 
-        function ql(t, e) {
+        function Wc(t, e) {
             let n = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2],
                 i = null;
             switch (e) {
-                case ia.Null:
+                case Za.Null:
                     i = t.visitNull;
                     break;
-                case ia.Bool:
+                case Za.Bool:
                     i = t.visitBool;
                     break;
-                case ia.Int:
+                case Za.Int:
                     i = t.visitInt;
                     break;
-                case ia.Int8:
+                case Za.Int8:
                     i = t.visitInt8 || t.visitInt;
                     break;
-                case ia.Int16:
+                case Za.Int16:
                     i = t.visitInt16 || t.visitInt;
                     break;
-                case ia.Int32:
+                case Za.Int32:
                     i = t.visitInt32 || t.visitInt;
                     break;
-                case ia.Int64:
+                case Za.Int64:
                     i = t.visitInt64 || t.visitInt;
                     break;
-                case ia.Uint8:
+                case Za.Uint8:
                     i = t.visitUint8 || t.visitInt;
                     break;
-                case ia.Uint16:
+                case Za.Uint16:
                     i = t.visitUint16 || t.visitInt;
                     break;
-                case ia.Uint32:
+                case Za.Uint32:
                     i = t.visitUint32 || t.visitInt;
                     break;
-                case ia.Uint64:
+                case Za.Uint64:
                     i = t.visitUint64 || t.visitInt;
                     break;
-                case ia.Float:
+                case Za.Float:
                     i = t.visitFloat;
                     break;
-                case ia.Float16:
+                case Za.Float16:
                     i = t.visitFloat16 || t.visitFloat;
                     break;
-                case ia.Float32:
+                case Za.Float32:
                     i = t.visitFloat32 || t.visitFloat;
                     break;
-                case ia.Float64:
+                case Za.Float64:
                     i = t.visitFloat64 || t.visitFloat;
                     break;
-                case ia.Utf8:
+                case Za.Utf8:
                     i = t.visitUtf8;
                     break;
-                case ia.Binary:
+                case Za.Binary:
                     i = t.visitBinary;
                     break;
-                case ia.FixedSizeBinary:
+                case Za.FixedSizeBinary:
                     i = t.visitFixedSizeBinary;
                     break;
-                case ia.Date:
+                case Za.Date:
                     i = t.visitDate;
                     break;
-                case ia.DateDay:
+                case Za.DateDay:
                     i = t.visitDateDay || t.visitDate;
                     break;
-                case ia.DateMillisecond:
+                case Za.DateMillisecond:
                     i = t.visitDateMillisecond || t.visitDate;
                     break;
-                case ia.Timestamp:
+                case Za.Timestamp:
                     i = t.visitTimestamp;
                     break;
-                case ia.TimestampSecond:
+                case Za.TimestampSecond:
                     i = t.visitTimestampSecond || t.visitTimestamp;
                     break;
-                case ia.TimestampMillisecond:
+                case Za.TimestampMillisecond:
                     i = t.visitTimestampMillisecond || t.visitTimestamp;
                     break;
-                case ia.TimestampMicrosecond:
+                case Za.TimestampMicrosecond:
                     i = t.visitTimestampMicrosecond || t.visitTimestamp;
                     break;
-                case ia.TimestampNanosecond:
+                case Za.TimestampNanosecond:
                     i = t.visitTimestampNanosecond || t.visitTimestamp;
                     break;
-                case ia.Time:
+                case Za.Time:
                     i = t.visitTime;
                     break;
-                case ia.TimeSecond:
+                case Za.TimeSecond:
                     i = t.visitTimeSecond || t.visitTime;
                     break;
-                case ia.TimeMillisecond:
+                case Za.TimeMillisecond:
                     i = t.visitTimeMillisecond || t.visitTime;
                     break;
-                case ia.TimeMicrosecond:
+                case Za.TimeMicrosecond:
                     i = t.visitTimeMicrosecond || t.visitTime;
                     break;
-                case ia.TimeNanosecond:
+                case Za.TimeNanosecond:
                     i = t.visitTimeNanosecond || t.visitTime;
                     break;
-                case ia.Decimal:
+                case Za.Decimal:
                     i = t.visitDecimal;
                     break;
-                case ia.List:
+                case Za.List:
                     i = t.visitList;
                     break;
-                case ia.Struct:
+                case Za.Struct:
                     i = t.visitStruct;
                     break;
-                case ia.Union:
+                case Za.Union:
                     i = t.visitUnion;
                     break;
-                case ia.DenseUnion:
+                case Za.DenseUnion:
                     i = t.visitDenseUnion || t.visitUnion;
                     break;
-                case ia.SparseUnion:
+                case Za.SparseUnion:
                     i = t.visitSparseUnion || t.visitUnion;
                     break;
-                case ia.Dictionary:
+                case Za.Dictionary:
                     i = t.visitDictionary;
                     break;
-                case ia.Interval:
+                case Za.Interval:
                     i = t.visitInterval;
                     break;
-                case ia.IntervalDayTime:
+                case Za.IntervalDayTime:
                     i = t.visitIntervalDayTime || t.visitInterval;
                     break;
-                case ia.IntervalYearMonth:
+                case Za.IntervalYearMonth:
                     i = t.visitIntervalYearMonth || t.visitInterval;
                     break;
-                case ia.FixedSizeList:
+                case Za.FixedSizeList:
                     i = t.visitFixedSizeList;
                     break;
-                case ia.Map:
+                case Za.Map:
                     i = t.visitMap
             }
             if ("function" === typeof i) return i;
             if (!n) return () => null;
-            throw new Error("Unrecognized type '".concat(ia[e], "'"))
+            throw new Error("Unrecognized type '".concat(Za[e], "'"))
         }
 
-        function Ql(t) {
+        function Hc(t) {
             switch (t.typeId) {
-                case ia.Null:
-                    return ia.Null;
-                case ia.Int: {
+                case Za.Null:
+                    return Za.Null;
+                case Za.Int: {
                     const {
                         bitWidth: e,
                         isSigned: n
                     } = t;
                     switch (e) {
                         case 8:
-                            return n ? ia.Int8 : ia.Uint8;
+                            return n ? Za.Int8 : Za.Uint8;
                         case 16:
-                            return n ? ia.Int16 : ia.Uint16;
+                            return n ? Za.Int16 : Za.Uint16;
                         case 32:
-                            return n ? ia.Int32 : ia.Uint32;
+                            return n ? Za.Int32 : Za.Uint32;
                         case 64:
-                            return n ? ia.Int64 : ia.Uint64
+                            return n ? Za.Int64 : Za.Uint64
                     }
-                    return ia.Int
+                    return Za.Int
                 }
-                case ia.Float:
+                case Za.Float:
                     switch (t.precision) {
-                        case Go.HALF:
-                            return ia.Float16;
-                        case Go.SINGLE:
-                            return ia.Float32;
-                        case Go.DOUBLE:
-                            return ia.Float64
-                    }
-                    return ia.Float;
-                case ia.Binary:
-                    return ia.Binary;
-                case ia.Utf8:
-                    return ia.Utf8;
-                case ia.Bool:
-                    return ia.Bool;
-                case ia.Decimal:
-                    return ia.Decimal;
-                case ia.Time:
+                        case $a.HALF:
+                            return Za.Float16;
+                        case $a.SINGLE:
+                            return Za.Float32;
+                        case $a.DOUBLE:
+                            return Za.Float64
+                    }
+                    return Za.Float;
+                case Za.Binary:
+                    return Za.Binary;
+                case Za.Utf8:
+                    return Za.Utf8;
+                case Za.Bool:
+                    return Za.Bool;
+                case Za.Decimal:
+                    return Za.Decimal;
+                case Za.Time:
                     switch (t.unit) {
-                        case ta.SECOND:
-                            return ia.TimeSecond;
-                        case ta.MILLISECOND:
-                            return ia.TimeMillisecond;
-                        case ta.MICROSECOND:
-                            return ia.TimeMicrosecond;
-                        case ta.NANOSECOND:
-                            return ia.TimeNanosecond
+                        case Xa.SECOND:
+                            return Za.TimeSecond;
+                        case Xa.MILLISECOND:
+                            return Za.TimeMillisecond;
+                        case Xa.MICROSECOND:
+                            return Za.TimeMicrosecond;
+                        case Xa.NANOSECOND:
+                            return Za.TimeNanosecond
                     }
-                    return ia.Time;
-                case ia.Timestamp:
+                    return Za.Time;
+                case Za.Timestamp:
                     switch (t.unit) {
-                        case ta.SECOND:
-                            return ia.TimestampSecond;
-                        case ta.MILLISECOND:
-                            return ia.TimestampMillisecond;
-                        case ta.MICROSECOND:
-                            return ia.TimestampMicrosecond;
-                        case ta.NANOSECOND:
-                            return ia.TimestampNanosecond
+                        case Xa.SECOND:
+                            return Za.TimestampSecond;
+                        case Xa.MILLISECOND:
+                            return Za.TimestampMillisecond;
+                        case Xa.MICROSECOND:
+                            return Za.TimestampMicrosecond;
+                        case Xa.NANOSECOND:
+                            return Za.TimestampNanosecond
                     }
-                    return ia.Timestamp;
-                case ia.Date:
+                    return Za.Timestamp;
+                case Za.Date:
                     switch (t.unit) {
-                        case Jo.DAY:
-                            return ia.DateDay;
-                        case Jo.MILLISECOND:
-                            return ia.DateMillisecond
+                        case Ka.DAY:
+                            return Za.DateDay;
+                        case Ka.MILLISECOND:
+                            return Za.DateMillisecond
                     }
-                    return ia.Date;
-                case ia.Interval:
+                    return Za.Date;
+                case Za.Interval:
                     switch (t.unit) {
-                        case ea.DAY_TIME:
-                            return ia.IntervalDayTime;
-                        case ea.YEAR_MONTH:
-                            return ia.IntervalYearMonth
-                    }
-                    return ia.Interval;
-                case ia.Map:
-                    return ia.Map;
-                case ia.List:
-                    return ia.List;
-                case ia.Struct:
-                    return ia.Struct;
-                case ia.Union:
+                        case qa.DAY_TIME:
+                            return Za.IntervalDayTime;
+                        case qa.YEAR_MONTH:
+                            return Za.IntervalYearMonth
+                    }
+                    return Za.Interval;
+                case Za.Map:
+                    return Za.Map;
+                case Za.List:
+                    return Za.List;
+                case Za.Struct:
+                    return Za.Struct;
+                case Za.Union:
                     switch (t.mode) {
-                        case Zo.Dense:
-                            return ia.DenseUnion;
-                        case Zo.Sparse:
-                            return ia.SparseUnion
-                    }
-                    return ia.Union;
-                case ia.FixedSizeBinary:
-                    return ia.FixedSizeBinary;
-                case ia.FixedSizeList:
-                    return ia.FixedSizeList;
-                case ia.Dictionary:
-                    return ia.Dictionary
-            }
-            throw new Error("Unrecognized type '".concat(ia[t.typeId], "'"))
-        }
-        Xl.prototype.visitInt8 = null, Xl.prototype.visitInt16 = null, Xl.prototype.visitInt32 = null, Xl.prototype.visitInt64 = null, Xl.prototype.visitUint8 = null, Xl.prototype.visitUint16 = null, Xl.prototype.visitUint32 = null, Xl.prototype.visitUint64 = null, Xl.prototype.visitFloat16 = null, Xl.prototype.visitFloat32 = null, Xl.prototype.visitFloat64 = null, Xl.prototype.visitDateDay = null, Xl.prototype.visitDateMillisecond = null, Xl.prototype.visitTimestampSecond = null, Xl.prototype.visitTimestampMillisecond = null, Xl.prototype.visitTimestampMicrosecond = null, Xl.prototype.visitTimestampNanosecond = null, Xl.prototype.visitTimeSecond = null, Xl.prototype.visitTimeMillisecond = null, Xl.prototype.visitTimeMicrosecond = null, Xl.prototype.visitTimeNanosecond = null, Xl.prototype.visitDenseUnion = null, Xl.prototype.visitSparseUnion = null, Xl.prototype.visitIntervalDayTime = null, Xl.prototype.visitIntervalYearMonth = null;
-        const Zl = new Float64Array(1),
-            Gl = new Uint32Array(Zl.buffer);
+                        case Ya.Dense:
+                            return Za.DenseUnion;
+                        case Ya.Sparse:
+                            return Za.SparseUnion
+                    }
+                    return Za.Union;
+                case Za.FixedSizeBinary:
+                    return Za.FixedSizeBinary;
+                case Za.FixedSizeList:
+                    return Za.FixedSizeList;
+                case Za.Dictionary:
+                    return Za.Dictionary
+            }
+            throw new Error("Unrecognized type '".concat(Za[t.typeId], "'"))
+        }
+        jc.prototype.visitInt8 = null, jc.prototype.visitInt16 = null, jc.prototype.visitInt32 = null, jc.prototype.visitInt64 = null, jc.prototype.visitUint8 = null, jc.prototype.visitUint16 = null, jc.prototype.visitUint32 = null, jc.prototype.visitUint64 = null, jc.prototype.visitFloat16 = null, jc.prototype.visitFloat32 = null, jc.prototype.visitFloat64 = null, jc.prototype.visitDateDay = null, jc.prototype.visitDateMillisecond = null, jc.prototype.visitTimestampSecond = null, jc.prototype.visitTimestampMillisecond = null, jc.prototype.visitTimestampMicrosecond = null, jc.prototype.visitTimestampNanosecond = null, jc.prototype.visitTimeSecond = null, jc.prototype.visitTimeMillisecond = null, jc.prototype.visitTimeMicrosecond = null, jc.prototype.visitTimeNanosecond = null, jc.prototype.visitDenseUnion = null, jc.prototype.visitSparseUnion = null, jc.prototype.visitIntervalDayTime = null, jc.prototype.visitIntervalYearMonth = null;
+        const Yc = new Float64Array(1),
+            $c = new Uint32Array(Yc.buffer);
 
-        function Jl(t) {
+        function Kc(t) {
             const e = (31744 & t) >> 10,
                 n = (1023 & t) / 1024,
                 i = Math.pow(-1, (32768 & t) >> 15);
             switch (e) {
                 case 31:
                     return i * (n ? Number.NaN : 1 / 0);
                 case 0:
                     return i * (n ? 6103515625e-14 * n : 0)
             }
             return i * Math.pow(2, e - 15) * (1 + n)
         }
-        class tc extends Xl {}
+        class Xc extends jc {}
 
-        function ec(t) {
+        function qc(t) {
             return (e, n, i) => {
                 if (e.setValid(n, null != i)) return t(e, n, i)
             }
         }
-        const nc = (t, e, n) => {
+        const Qc = (t, e, n) => {
                 t[e] = Math.trunc(n % 4294967296), t[e + 1] = Math.trunc(n / 4294967296)
             },
-            ic = (t, e, n, i) => {
+            Zc = (t, e, n, i) => {
                 if (n + 1 < e.length) {
                     const {
                         [n]: r, [n + 1]: s
                     } = e;
                     t.set(i.subarray(0, s - r), r)
                 }
             },
-            rc = (t, e, n) => {
+            Gc = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 i[e] = n
             },
-            sc = (t, e, n) => {
+            Jc = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 i[e] = n
             },
-            oc = (t, e, n) => {
+            tu = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 i[e] = function(t) {
                     if (t !== t) return 32256;
-                    Zl[0] = t;
-                    const e = (2147483648 & Gl[1]) >> 16 & 65535;
-                    let n = 2146435072 & Gl[1],
+                    Yc[0] = t;
+                    const e = (2147483648 & $c[1]) >> 16 & 65535;
+                    let n = 2146435072 & $c[1],
                         i = 0;
-                    return n >= 1089470464 ? Gl[0] > 0 ? n = 31744 : (n = (2080374784 & n) >> 16, i = (1048575 & Gl[1]) >> 10) : n <= 1056964608 ? (i = 1048576 + (1048575 & Gl[1]), i = 1048576 + (i << (n >> 20) - 998) >> 21, n = 0) : (n = n - 1056964608 >> 10, i = 512 + (1048575 & Gl[1]) >> 10), e | n | 65535 & i
+                    return n >= 1089470464 ? $c[0] > 0 ? n = 31744 : (n = (2080374784 & n) >> 16, i = (1048575 & $c[1]) >> 10) : n <= 1056964608 ? (i = 1048576 + (1048575 & $c[1]), i = 1048576 + (i << (n >> 20) - 998) >> 21, n = 0) : (n = n - 1056964608 >> 10, i = 512 + (1048575 & $c[1]) >> 10), e | n | 65535 & i
                 }(n)
             },
-            ac = (t, e, n) => {
+            eu = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 ((t, e, n) => {
                     t[e] = Math.trunc(n / 864e5)
                 })(i, e, n.valueOf())
             },
-            lc = (t, e, n) => {
+            nu = (t, e, n) => {
                 let {
                     values: i
                 } = t;
-                nc(i, 2 * e, n.valueOf())
+                Qc(i, 2 * e, n.valueOf())
             },
-            cc = (t, e, n) => {
+            iu = (t, e, n) => {
                 let {
                     values: i
                 } = t;
-                return nc(i, 2 * e, n / 1e3)
+                return Qc(i, 2 * e, n / 1e3)
             },
-            uc = (t, e, n) => {
+            ru = (t, e, n) => {
                 let {
                     values: i
                 } = t;
-                return nc(i, 2 * e, n)
+                return Qc(i, 2 * e, n)
             },
-            hc = (t, e, n) => {
+            su = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 return ((t, e, n) => {
                     t[e] = Math.trunc(1e3 * n % 4294967296), t[e + 1] = Math.trunc(1e3 * n / 4294967296)
                 })(i, 2 * e, n)
             },
-            dc = (t, e, n) => {
+            ou = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 return ((t, e, n) => {
                     t[e] = Math.trunc(1e6 * n % 4294967296), t[e + 1] = Math.trunc(1e6 * n / 4294967296)
                 })(i, 2 * e, n)
             },
-            fc = (t, e, n) => {
+            au = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 i[e] = n
             },
-            pc = (t, e, n) => {
+            lu = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 i[e] = n
             },
-            gc = (t, e, n) => {
+            cu = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 i[e] = n
             },
-            mc = (t, e, n) => {
+            uu = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 i[e] = n
             },
-            yc = (t, e, n) => {
+            hu = (t, e, n) => {
                 const i = t.type.typeIdToChildIndex[t.typeIds[e]],
                     r = t.children[i];
-                xc.visit(r, t.valueOffsets[e], n)
+                gu.visit(r, t.valueOffsets[e], n)
             },
-            bc = (t, e, n) => {
+            du = (t, e, n) => {
                 const i = t.type.typeIdToChildIndex[t.typeIds[e]],
                     r = t.children[i];
-                xc.visit(r, e, n)
+                gu.visit(r, e, n)
             },
-            vc = (t, e, n) => {
+            fu = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 i.set(n.subarray(0, 2), 2 * e)
             },
-            _c = (t, e, n) => {
+            pu = (t, e, n) => {
                 let {
                     values: i
                 } = t;
                 i[e] = 12 * n[0] + n[1] % 12
             };
-        tc.prototype.visitBool = ec(((t, e, n) => {
+        Xc.prototype.visitBool = qc(((t, e, n) => {
             let {
                 offset: i,
                 values: r
             } = t;
             const s = i + e;
             n ? r[s >> 3] |= 1 << s % 8 : r[s >> 3] &= ~(1 << s % 8)
-        })), tc.prototype.visitInt = ec(rc), tc.prototype.visitInt8 = ec(rc), tc.prototype.visitInt16 = ec(rc), tc.prototype.visitInt32 = ec(rc), tc.prototype.visitInt64 = ec(rc), tc.prototype.visitUint8 = ec(rc), tc.prototype.visitUint16 = ec(rc), tc.prototype.visitUint32 = ec(rc), tc.prototype.visitUint64 = ec(rc), tc.prototype.visitFloat = ec(((t, e, n) => {
+        })), Xc.prototype.visitInt = qc(Gc), Xc.prototype.visitInt8 = qc(Gc), Xc.prototype.visitInt16 = qc(Gc), Xc.prototype.visitInt32 = qc(Gc), Xc.prototype.visitInt64 = qc(Gc), Xc.prototype.visitUint8 = qc(Gc), Xc.prototype.visitUint16 = qc(Gc), Xc.prototype.visitUint32 = qc(Gc), Xc.prototype.visitUint64 = qc(Gc), Xc.prototype.visitFloat = qc(((t, e, n) => {
             switch (t.type.precision) {
-                case Go.HALF:
-                    return oc(t, e, n);
-                case Go.SINGLE:
-                case Go.DOUBLE:
-                    return sc(t, e, n)
+                case $a.HALF:
+                    return tu(t, e, n);
+                case $a.SINGLE:
+                case $a.DOUBLE:
+                    return Jc(t, e, n)
             }
-        })), tc.prototype.visitFloat16 = ec(oc), tc.prototype.visitFloat32 = ec(sc), tc.prototype.visitFloat64 = ec(sc), tc.prototype.visitUtf8 = ec(((t, e, n) => {
+        })), Xc.prototype.visitFloat16 = qc(tu), Xc.prototype.visitFloat32 = qc(Jc), Xc.prototype.visitFloat64 = qc(Jc), Xc.prototype.visitUtf8 = qc(((t, e, n) => {
             let {
                 values: i,
                 valueOffsets: r
             } = t;
-            ic(i, r, e, Ra(n))
-        })), tc.prototype.visitBinary = ec(((t, e, n) => {
+            Zc(i, r, e, Cl(n))
+        })), Xc.prototype.visitBinary = qc(((t, e, n) => {
             let {
                 values: i,
                 valueOffsets: r
             } = t;
-            return ic(i, r, e, n)
-        })), tc.prototype.visitFixedSizeBinary = ec(((t, e, n) => {
+            return Zc(i, r, e, n)
+        })), Xc.prototype.visitFixedSizeBinary = qc(((t, e, n) => {
             let {
                 stride: i,
                 values: r
             } = t;
             r.set(n.subarray(0, i), i * e)
-        })), tc.prototype.visitDate = ec(((t, e, n) => {
-            t.type.unit === Jo.DAY ? ac(t, e, n) : lc(t, e, n)
-        })), tc.prototype.visitDateDay = ec(ac), tc.prototype.visitDateMillisecond = ec(lc), tc.prototype.visitTimestamp = ec(((t, e, n) => {
+        })), Xc.prototype.visitDate = qc(((t, e, n) => {
+            t.type.unit === Ka.DAY ? eu(t, e, n) : nu(t, e, n)
+        })), Xc.prototype.visitDateDay = qc(eu), Xc.prototype.visitDateMillisecond = qc(nu), Xc.prototype.visitTimestamp = qc(((t, e, n) => {
             switch (t.type.unit) {
-                case ta.SECOND:
-                    return cc(t, e, n);
-                case ta.MILLISECOND:
-                    return uc(t, e, n);
-                case ta.MICROSECOND:
-                    return hc(t, e, n);
-                case ta.NANOSECOND:
-                    return dc(t, e, n)
+                case Xa.SECOND:
+                    return iu(t, e, n);
+                case Xa.MILLISECOND:
+                    return ru(t, e, n);
+                case Xa.MICROSECOND:
+                    return su(t, e, n);
+                case Xa.NANOSECOND:
+                    return ou(t, e, n)
             }
-        })), tc.prototype.visitTimestampSecond = ec(cc), tc.prototype.visitTimestampMillisecond = ec(uc), tc.prototype.visitTimestampMicrosecond = ec(hc), tc.prototype.visitTimestampNanosecond = ec(dc), tc.prototype.visitTime = ec(((t, e, n) => {
+        })), Xc.prototype.visitTimestampSecond = qc(iu), Xc.prototype.visitTimestampMillisecond = qc(ru), Xc.prototype.visitTimestampMicrosecond = qc(su), Xc.prototype.visitTimestampNanosecond = qc(ou), Xc.prototype.visitTime = qc(((t, e, n) => {
             switch (t.type.unit) {
-                case ta.SECOND:
-                    return fc(t, e, n);
-                case ta.MILLISECOND:
-                    return pc(t, e, n);
-                case ta.MICROSECOND:
-                    return gc(t, e, n);
-                case ta.NANOSECOND:
-                    return mc(t, e, n)
+                case Xa.SECOND:
+                    return au(t, e, n);
+                case Xa.MILLISECOND:
+                    return lu(t, e, n);
+                case Xa.MICROSECOND:
+                    return cu(t, e, n);
+                case Xa.NANOSECOND:
+                    return uu(t, e, n)
             }
-        })), tc.prototype.visitTimeSecond = ec(fc), tc.prototype.visitTimeMillisecond = ec(pc), tc.prototype.visitTimeMicrosecond = ec(gc), tc.prototype.visitTimeNanosecond = ec(mc), tc.prototype.visitDecimal = ec(((t, e, n) => {
+        })), Xc.prototype.visitTimeSecond = qc(au), Xc.prototype.visitTimeMillisecond = qc(lu), Xc.prototype.visitTimeMicrosecond = qc(cu), Xc.prototype.visitTimeNanosecond = qc(uu), Xc.prototype.visitDecimal = qc(((t, e, n) => {
             let {
                 values: i,
                 stride: r
             } = t;
             i.set(n.subarray(0, r), r * e)
-        })), tc.prototype.visitList = ec(((t, e, n) => {
+        })), Xc.prototype.visitList = qc(((t, e, n) => {
             const i = t.children[0],
                 r = t.valueOffsets,
-                s = xc.getVisitFn(i);
+                s = gu.getVisitFn(i);
             if (Array.isArray(n))
                 for (let o = -1, a = r[e], l = r[e + 1]; a < l;) s(i, a++, n[++o]);
             else
                 for (let o = -1, a = r[e], l = r[e + 1]; a < l;) s(i, a++, n.get(++o))
-        })), tc.prototype.visitStruct = ec(((t, e, n) => {
-            const i = t.type.children.map((t => xc.getVisitFn(t.type))),
-                r = n instanceof Map ? (s = e, o = n, (t, e, n, i) => e && t(e, s, o.get(n.name))) : n instanceof Ru ? ((t, e) => (n, i, r, s) => i && n(i, t, e.get(s)))(e, n) : Array.isArray(n) ? ((t, e) => (n, i, r, s) => i && n(i, t, e[s]))(e, n) : ((t, e) => (n, i, r, s) => i && n(i, t, e[r.name]))(e, n);
+        })), Xc.prototype.visitStruct = qc(((t, e, n) => {
+            const i = t.type.children.map((t => gu.getVisitFn(t.type))),
+                r = n instanceof Map ? (s = e, o = n, (t, e, n, i) => e && t(e, s, o.get(n.name))) : n instanceof Ch ? ((t, e) => (n, i, r, s) => i && n(i, t, e.get(s)))(e, n) : Array.isArray(n) ? ((t, e) => (n, i, r, s) => i && n(i, t, e[s]))(e, n) : ((t, e) => (n, i, r, s) => i && n(i, t, e[r.name]))(e, n);
             var s, o;
             t.type.children.forEach(((e, n) => r(i[n], t.children[n], e, n)))
-        })), tc.prototype.visitUnion = ec(((t, e, n) => {
-            t.type.mode === Zo.Dense ? yc(t, e, n) : bc(t, e, n)
-        })), tc.prototype.visitDenseUnion = ec(yc), tc.prototype.visitSparseUnion = ec(bc), tc.prototype.visitDictionary = ec(((t, e, n) => {
+        })), Xc.prototype.visitUnion = qc(((t, e, n) => {
+            t.type.mode === Ya.Dense ? hu(t, e, n) : du(t, e, n)
+        })), Xc.prototype.visitDenseUnion = qc(hu), Xc.prototype.visitSparseUnion = qc(du), Xc.prototype.visitDictionary = qc(((t, e, n) => {
             var i;
             null === (i = t.dictionary) || void 0 === i || i.set(t.values[e], n)
-        })), tc.prototype.visitInterval = ec(((t, e, n) => {
-            t.type.unit === ea.DAY_TIME ? vc(t, e, n) : _c(t, e, n)
-        })), tc.prototype.visitIntervalDayTime = ec(vc), tc.prototype.visitIntervalYearMonth = ec(_c), tc.prototype.visitFixedSizeList = ec(((t, e, n) => {
+        })), Xc.prototype.visitInterval = qc(((t, e, n) => {
+            t.type.unit === qa.DAY_TIME ? fu(t, e, n) : pu(t, e, n)
+        })), Xc.prototype.visitIntervalDayTime = qc(fu), Xc.prototype.visitIntervalYearMonth = qc(pu), Xc.prototype.visitFixedSizeList = qc(((t, e, n) => {
             const {
                 stride: i
-            } = t, r = t.children[0], s = xc.getVisitFn(r);
+            } = t, r = t.children[0], s = gu.getVisitFn(r);
             if (Array.isArray(n))
                 for (let o = -1, a = e * i; ++o < i;) s(r, a + o, n[o]);
             else
                 for (let o = -1, a = e * i; ++o < i;) s(r, a + o, n.get(o))
-        })), tc.prototype.visitMap = ec(((t, e, n) => {
+        })), Xc.prototype.visitMap = qc(((t, e, n) => {
             const i = t.children[0],
                 {
                     valueOffsets: r
                 } = t,
-                s = xc.getVisitFn(i);
+                s = gu.getVisitFn(i);
             let {
                 [e]: o, [e + 1]: a
             } = r;
             const l = n instanceof Map ? n.entries() : Object.entries(n);
             for (const c of l)
                 if (s(i, o, c), ++o >= a) break
         }));
-        const xc = new tc,
-            wc = Symbol.for("parent"),
-            Sc = Symbol.for("rowIndex");
-        class Tc {
+        const gu = new Xc,
+            mu = Symbol.for("parent"),
+            yu = Symbol.for("rowIndex");
+        class bu {
             constructor(t, e) {
-                return this[wc] = t, this[Sc] = e, new Proxy(this, new Mc)
+                return this[mu] = t, this[yu] = e, new Proxy(this, new _u)
             }
             toArray() {
                 return Object.values(this.toJSON())
             }
             toJSON() {
-                const t = this[Sc],
-                    e = this[wc],
+                const t = this[yu],
+                    e = this[mu],
                     n = e.type.children,
                     i = {};
-                for (let r = -1, s = n.length; ++r < s;) i[n[r].name] = Xc.visit(e.children[r], t);
+                for (let r = -1, s = n.length; ++r < s;) i[n[r].name] = ju.visit(e.children[r], t);
                 return i
             }
             toString() {
                 return "{".concat([...this].map((t => {
                     let [e, n] = t;
-                    return "".concat(Ea(e), ": ").concat(Ea(n))
+                    return "".concat(wl(e), ": ").concat(wl(n))
                 })).join(", "), "}")
             } [Symbol.for("nodejs.util.inspect.custom")]() {
                 return this.toString()
             } [Symbol.iterator]() {
-                return new kc(this[wc], this[Sc])
+                return new vu(this[mu], this[yu])
             }
         }
-        class kc {
+        class vu {
             constructor(t, e) {
                 this.childIndex = 0, this.children = t.children, this.rowIndex = e, this.childFields = t.type.children, this.numChildren = this.childFields.length
             } [Symbol.iterator]() {
                 return this
             }
             next() {
                 const t = this.childIndex;
                 return t < this.numChildren ? (this.childIndex = t + 1, {
                     done: !1,
-                    value: [this.childFields[t].name, Xc.visit(this.children[t], this.rowIndex)]
+                    value: [this.childFields[t].name, ju.visit(this.children[t], this.rowIndex)]
                 }) : {
                     done: !0,
                     value: null
                 }
             }
         }
-        Object.defineProperties(Tc.prototype, {
+        Object.defineProperties(bu.prototype, {
             [Symbol.toStringTag]: {
                 enumerable: !1,
                 configurable: !1,
                 value: "Row"
             },
-            [wc]: {
+            [mu]: {
                 writable: !0,
                 enumerable: !1,
                 configurable: !1,
                 value: null
             },
-            [Sc]: {
+            [yu]: {
                 writable: !0,
                 enumerable: !1,
                 configurable: !1,
                 value: -1
             }
         });
-        class Mc {
+        class _u {
             isExtensible() {
                 return !1
             }
             deleteProperty() {
                 return !1
             }
             preventExtensions() {
                 return !0
             }
             ownKeys(t) {
-                return t[wc].type.children.map((t => t.name))
+                return t[mu].type.children.map((t => t.name))
             }
             has(t, e) {
-                return -1 !== t[wc].type.children.findIndex((t => t.name === e))
+                return -1 !== t[mu].type.children.findIndex((t => t.name === e))
             }
             getOwnPropertyDescriptor(t, e) {
-                if (-1 !== t[wc].type.children.findIndex((t => t.name === e))) return {
+                if (-1 !== t[mu].type.children.findIndex((t => t.name === e))) return {
                     writable: !0,
                     enumerable: !0,
                     configurable: !0
                 }
             }
             get(t, e) {
                 if (Reflect.has(t, e)) return t[e];
-                const n = t[wc].type.children.findIndex((t => t.name === e));
+                const n = t[mu].type.children.findIndex((t => t.name === e));
                 if (-1 !== n) {
-                    const i = Xc.visit(t[wc].children[n], t[Sc]);
+                    const i = ju.visit(t[mu].children[n], t[yu]);
                     return Reflect.set(t, e, i), i
                 }
             }
             set(t, e, n) {
-                const i = t[wc].type.children.findIndex((t => t.name === e));
-                return -1 !== i ? (xc.visit(t[wc].children[i], t[Sc], n), Reflect.set(t, e, n)) : !(!Reflect.has(t, e) && "symbol" !== typeof e) && Reflect.set(t, e, n)
+                const i = t[mu].type.children.findIndex((t => t.name === e));
+                return -1 !== i ? (gu.visit(t[mu].children[i], t[yu], n), Reflect.set(t, e, n)) : !(!Reflect.has(t, e) && "symbol" !== typeof e) && Reflect.set(t, e, n)
             }
         }
-        class Ic extends Xl {}
+        class xu extends jc {}
 
-        function Ec(t) {
+        function wu(t) {
             return (e, n) => e.getValid(n) ? t(e, n) : null
         }
-        const Oc = (t, e) => 4294967296 * t[e + 1] + (t[e] >>> 0),
-            Dc = t => new Date(t),
-            Ac = (t, e, n) => {
+        const Su = (t, e) => 4294967296 * t[e + 1] + (t[e] >>> 0),
+            Tu = t => new Date(t),
+            ku = (t, e, n) => {
                 if (n + 1 >= e.length) return null;
                 const i = e[n],
                     r = e[n + 1];
                 return t.subarray(i, r)
             },
-            Cc = (t, e) => {
+            Mu = (t, e) => {
                 let {
                     values: n
                 } = t;
-                return ((t, e) => Dc(((t, e) => 864e5 * t[e])(t, e)))(n, e)
+                return ((t, e) => Tu(((t, e) => 864e5 * t[e])(t, e)))(n, e)
             },
-            Pc = (t, e) => {
+            Iu = (t, e) => {
                 let {
                     values: n
                 } = t;
-                return ((t, e) => Dc(Oc(t, e)))(n, 2 * e)
+                return ((t, e) => Tu(Su(t, e)))(n, 2 * e)
             },
-            Fc = (t, e) => {
+            Eu = (t, e) => {
                 let {
                     stride: n,
                     values: i
                 } = t;
                 return i[n * e]
             },
-            Lc = (t, e) => {
+            Ou = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n[e]
             },
-            Nc = (t, e) => {
+            Du = (t, e) => {
                 let {
                     values: n
                 } = t;
-                return 1e3 * Oc(n, 2 * e)
+                return 1e3 * Su(n, 2 * e)
             },
-            Bc = (t, e) => {
+            Au = (t, e) => {
                 let {
                     values: n
                 } = t;
-                return Oc(n, 2 * e)
+                return Su(n, 2 * e)
             },
-            Rc = (t, e) => {
+            Cu = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return ((t, e) => t[e + 1] / 1e3 * 4294967296 + (t[e] >>> 0) / 1e3)(n, 2 * e)
             },
-            zc = (t, e) => {
+            Pu = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return ((t, e) => t[e + 1] / 1e6 * 4294967296 + (t[e] >>> 0) / 1e6)(n, 2 * e)
             },
-            Uc = (t, e) => {
+            Fu = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n[e]
             },
-            Vc = (t, e) => {
+            Lu = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n[e]
             },
-            jc = (t, e) => {
+            Nu = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n[e]
             },
-            Wc = (t, e) => {
+            Bu = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n[e]
             },
-            Hc = (t, e) => {
+            Ru = (t, e) => {
                 const n = t.type.typeIdToChildIndex[t.typeIds[e]],
                     i = t.children[n];
-                return Xc.visit(i, t.valueOffsets[e])
+                return ju.visit(i, t.valueOffsets[e])
             },
-            Yc = (t, e) => {
+            zu = (t, e) => {
                 const n = t.type.typeIdToChildIndex[t.typeIds[e]],
                     i = t.children[n];
-                return Xc.visit(i, e)
+                return ju.visit(i, e)
             },
-            $c = (t, e) => {
+            Uu = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n.subarray(2 * e, 2 * (e + 1))
             },
-            Kc = (t, e) => {
+            Vu = (t, e) => {
                 let {
                     values: n
                 } = t;
                 const i = n[e],
                     r = new Int32Array(2);
                 return r[0] = Math.trunc(i / 12), r[1] = Math.trunc(i % 12), r
             };
-        Ic.prototype.visitNull = Ec(((t, e) => null)), Ic.prototype.visitBool = Ec(((t, e) => {
+        xu.prototype.visitNull = wu(((t, e) => null)), xu.prototype.visitBool = wu(((t, e) => {
             let {
                 offset: n,
                 values: i
             } = t;
             const r = n + e;
             return 0 !== (i[r >> 3] & 1 << r % 8)
-        })), Ic.prototype.visitInt = Ec(((t, e) => {
+        })), xu.prototype.visitInt = wu(((t, e) => {
             let {
                 values: n
             } = t;
             return n[e]
-        })), Ic.prototype.visitInt8 = Ec(Fc), Ic.prototype.visitInt16 = Ec(Fc), Ic.prototype.visitInt32 = Ec(Fc), Ic.prototype.visitInt64 = Ec(Lc), Ic.prototype.visitUint8 = Ec(Fc), Ic.prototype.visitUint16 = Ec(Fc), Ic.prototype.visitUint32 = Ec(Fc), Ic.prototype.visitUint64 = Ec(Lc), Ic.prototype.visitFloat = Ec(((t, e) => {
+        })), xu.prototype.visitInt8 = wu(Eu), xu.prototype.visitInt16 = wu(Eu), xu.prototype.visitInt32 = wu(Eu), xu.prototype.visitInt64 = wu(Ou), xu.prototype.visitUint8 = wu(Eu), xu.prototype.visitUint16 = wu(Eu), xu.prototype.visitUint32 = wu(Eu), xu.prototype.visitUint64 = wu(Ou), xu.prototype.visitFloat = wu(((t, e) => {
             let {
                 type: n,
                 values: i
             } = t;
-            return n.precision !== Go.HALF ? i[e] : Jl(i[e])
-        })), Ic.prototype.visitFloat16 = Ec(((t, e) => {
+            return n.precision !== $a.HALF ? i[e] : Kc(i[e])
+        })), xu.prototype.visitFloat16 = wu(((t, e) => {
             let {
                 stride: n,
                 values: i
             } = t;
-            return Jl(i[n * e])
-        })), Ic.prototype.visitFloat32 = Ec(Fc), Ic.prototype.visitFloat64 = Ec(Fc), Ic.prototype.visitUtf8 = Ec(((t, e) => {
+            return Kc(i[n * e])
+        })), xu.prototype.visitFloat32 = wu(Eu), xu.prototype.visitFloat64 = wu(Eu), xu.prototype.visitUtf8 = wu(((t, e) => {
             let {
                 values: n,
                 valueOffsets: i
             } = t;
-            const r = Ac(n, i, e);
-            return null !== r ? Na(r) : null
-        })), Ic.prototype.visitBinary = Ec(((t, e) => {
+            const r = ku(n, i, e);
+            return null !== r ? Dl(r) : null
+        })), xu.prototype.visitBinary = wu(((t, e) => {
             let {
                 values: n,
                 valueOffsets: i
             } = t;
-            return Ac(n, i, e)
-        })), Ic.prototype.visitFixedSizeBinary = Ec(((t, e) => {
+            return ku(n, i, e)
+        })), xu.prototype.visitFixedSizeBinary = wu(((t, e) => {
             let {
                 stride: n,
                 values: i
             } = t;
             return i.subarray(n * e, n * (e + 1))
-        })), Ic.prototype.visitDate = Ec(((t, e) => t.type.unit === Jo.DAY ? Cc(t, e) : Pc(t, e))), Ic.prototype.visitDateDay = Ec(Cc), Ic.prototype.visitDateMillisecond = Ec(Pc), Ic.prototype.visitTimestamp = Ec(((t, e) => {
+        })), xu.prototype.visitDate = wu(((t, e) => t.type.unit === Ka.DAY ? Mu(t, e) : Iu(t, e))), xu.prototype.visitDateDay = wu(Mu), xu.prototype.visitDateMillisecond = wu(Iu), xu.prototype.visitTimestamp = wu(((t, e) => {
             switch (t.type.unit) {
-                case ta.SECOND:
-                    return Nc(t, e);
-                case ta.MILLISECOND:
-                    return Bc(t, e);
-                case ta.MICROSECOND:
-                    return Rc(t, e);
-                case ta.NANOSECOND:
-                    return zc(t, e)
+                case Xa.SECOND:
+                    return Du(t, e);
+                case Xa.MILLISECOND:
+                    return Au(t, e);
+                case Xa.MICROSECOND:
+                    return Cu(t, e);
+                case Xa.NANOSECOND:
+                    return Pu(t, e)
             }
-        })), Ic.prototype.visitTimestampSecond = Ec(Nc), Ic.prototype.visitTimestampMillisecond = Ec(Bc), Ic.prototype.visitTimestampMicrosecond = Ec(Rc), Ic.prototype.visitTimestampNanosecond = Ec(zc), Ic.prototype.visitTime = Ec(((t, e) => {
+        })), xu.prototype.visitTimestampSecond = wu(Du), xu.prototype.visitTimestampMillisecond = wu(Au), xu.prototype.visitTimestampMicrosecond = wu(Cu), xu.prototype.visitTimestampNanosecond = wu(Pu), xu.prototype.visitTime = wu(((t, e) => {
             switch (t.type.unit) {
-                case ta.SECOND:
-                    return Uc(t, e);
-                case ta.MILLISECOND:
-                    return Vc(t, e);
-                case ta.MICROSECOND:
-                    return jc(t, e);
-                case ta.NANOSECOND:
-                    return Wc(t, e)
+                case Xa.SECOND:
+                    return Fu(t, e);
+                case Xa.MILLISECOND:
+                    return Lu(t, e);
+                case Xa.MICROSECOND:
+                    return Nu(t, e);
+                case Xa.NANOSECOND:
+                    return Bu(t, e)
             }
-        })), Ic.prototype.visitTimeSecond = Ec(Uc), Ic.prototype.visitTimeMillisecond = Ec(Vc), Ic.prototype.visitTimeMicrosecond = Ec(jc), Ic.prototype.visitTimeNanosecond = Ec(Wc), Ic.prototype.visitDecimal = Ec(((t, e) => {
+        })), xu.prototype.visitTimeSecond = wu(Fu), xu.prototype.visitTimeMillisecond = wu(Lu), xu.prototype.visitTimeMicrosecond = wu(Nu), xu.prototype.visitTimeNanosecond = wu(Bu), xu.prototype.visitDecimal = wu(((t, e) => {
             let {
                 values: n,
                 stride: i
             } = t;
-            return rl.decimal(n.subarray(i * e, i * (e + 1)))
-        })), Ic.prototype.visitList = Ec(((t, e) => {
+            return Gl.decimal(n.subarray(i * e, i * (e + 1)))
+        })), xu.prototype.visitList = wu(((t, e) => {
             const {
                 valueOffsets: n,
                 stride: i,
                 children: r
             } = t, {
                 [e * i]: s,
                 [e * i + 1]: o
             } = n, a = r[0].slice(s, o - s);
-            return new Ru([a])
-        })), Ic.prototype.visitStruct = Ec(((t, e) => new Tc(t, e))), Ic.prototype.visitUnion = Ec(((t, e) => t.type.mode === Zo.Dense ? Hc(t, e) : Yc(t, e))), Ic.prototype.visitDenseUnion = Ec(Hc), Ic.prototype.visitSparseUnion = Ec(Yc), Ic.prototype.visitDictionary = Ec(((t, e) => {
+            return new Ch([a])
+        })), xu.prototype.visitStruct = wu(((t, e) => new bu(t, e))), xu.prototype.visitUnion = wu(((t, e) => t.type.mode === Ya.Dense ? Ru(t, e) : zu(t, e))), xu.prototype.visitDenseUnion = wu(Ru), xu.prototype.visitSparseUnion = wu(zu), xu.prototype.visitDictionary = wu(((t, e) => {
             var n;
             return null === (n = t.dictionary) || void 0 === n ? void 0 : n.get(t.values[e])
-        })), Ic.prototype.visitInterval = Ec(((t, e) => t.type.unit === ea.DAY_TIME ? $c(t, e) : Kc(t, e))), Ic.prototype.visitIntervalDayTime = Ec($c), Ic.prototype.visitIntervalYearMonth = Ec(Kc), Ic.prototype.visitFixedSizeList = Ec(((t, e) => {
+        })), xu.prototype.visitInterval = wu(((t, e) => t.type.unit === qa.DAY_TIME ? Uu(t, e) : Vu(t, e))), xu.prototype.visitIntervalDayTime = wu(Uu), xu.prototype.visitIntervalYearMonth = wu(Vu), xu.prototype.visitFixedSizeList = wu(((t, e) => {
             const {
                 stride: n,
                 children: i
             } = t, r = i[0].slice(e * n, n);
-            return new Ru([r])
-        })), Ic.prototype.visitMap = Ec(((t, e) => {
+            return new Ch([r])
+        })), xu.prototype.visitMap = wu(((t, e) => {
             const {
                 valueOffsets: n,
                 children: i
             } = t, {
                 [e]: r,
                 [e + 1]: s
             } = n, o = i[0];
-            return new Zc(o.slice(r, s - r))
+            return new Yu(o.slice(r, s - r))
         }));
-        const Xc = new Ic,
-            qc = Symbol.for("keys"),
-            Qc = Symbol.for("vals");
-        class Zc {
+        const ju = new xu,
+            Wu = Symbol.for("keys"),
+            Hu = Symbol.for("vals");
+        class Yu {
             constructor(t) {
-                return this[qc] = new Ru([t.children[0]]).memoize(), this[Qc] = t.children[1], new Proxy(this, new Jc)
+                return this[Wu] = new Ch([t.children[0]]).memoize(), this[Hu] = t.children[1], new Proxy(this, new Ku)
             } [Symbol.iterator]() {
-                return new Gc(this[qc], this[Qc])
+                return new $u(this[Wu], this[Hu])
             }
             get size() {
-                return this[qc].length
+                return this[Wu].length
             }
             toArray() {
                 return Object.values(this.toJSON())
             }
             toJSON() {
-                const t = this[qc],
-                    e = this[Qc],
+                const t = this[Wu],
+                    e = this[Hu],
                     n = {};
-                for (let i = -1, r = t.length; ++i < r;) n[t.get(i)] = Xc.visit(e, i);
+                for (let i = -1, r = t.length; ++i < r;) n[t.get(i)] = ju.visit(e, i);
                 return n
             }
             toString() {
                 return "{".concat([...this].map((t => {
                     let [e, n] = t;
-                    return "".concat(Ea(e), ": ").concat(Ea(n))
+                    return "".concat(wl(e), ": ").concat(wl(n))
                 })).join(", "), "}")
             } [Symbol.for("nodejs.util.inspect.custom")]() {
                 return this.toString()
             }
         }
-        class Gc {
+        class $u {
             constructor(t, e) {
                 this.keys = t, this.vals = e, this.keyIndex = 0, this.numKeys = t.length
             } [Symbol.iterator]() {
                 return this
             }
             next() {
                 const t = this.keyIndex;
                 return t === this.numKeys ? {
                     done: !0,
                     value: null
                 } : (this.keyIndex++, {
                     done: !1,
-                    value: [this.keys.get(t), Xc.visit(this.vals, t)]
+                    value: [this.keys.get(t), ju.visit(this.vals, t)]
                 })
             }
         }
-        class Jc {
+        class Ku {
             isExtensible() {
                 return !1
             }
             deleteProperty() {
                 return !1
             }
             preventExtensions() {
                 return !0
             }
             ownKeys(t) {
-                return t[qc].toArray().map(String)
+                return t[Wu].toArray().map(String)
             }
             has(t, e) {
-                return t[qc].includes(e)
+                return t[Wu].includes(e)
             }
             getOwnPropertyDescriptor(t, e) {
-                if (-1 !== t[qc].indexOf(e)) return {
+                if (-1 !== t[Wu].indexOf(e)) return {
                     writable: !0,
                     enumerable: !0,
                     configurable: !0
                 }
             }
             get(t, e) {
                 if (Reflect.has(t, e)) return t[e];
-                const n = t[qc].indexOf(e);
+                const n = t[Wu].indexOf(e);
                 if (-1 !== n) {
-                    const i = Xc.visit(Reflect.get(t, Qc), n);
+                    const i = ju.visit(Reflect.get(t, Hu), n);
                     return Reflect.set(t, e, i), i
                 }
             }
             set(t, e, n) {
-                const i = t[qc].indexOf(e);
-                return -1 !== i ? (xc.visit(Reflect.get(t, Qc), i, n), Reflect.set(t, e, n)) : !!Reflect.has(t, e) && Reflect.set(t, e, n)
+                const i = t[Wu].indexOf(e);
+                return -1 !== i ? (gu.visit(Reflect.get(t, Hu), i, n), Reflect.set(t, e, n)) : !!Reflect.has(t, e) && Reflect.set(t, e, n)
             }
         }
-        let tu;
+        let Xu;
 
-        function eu(t, e, n, i) {
+        function qu(t, e, n, i) {
             const {
                 length: r = 0
             } = t;
             let s = "number" !== typeof e ? 0 : e,
                 o = "number" !== typeof n ? r : n;
-            return s < 0 && (s = (s % r + r) % r), o < 0 && (o = (o % r + r) % r), o < s && (tu = s, s = o, o = tu), o > r && (o = r), i ? i(t, s, o) : [s, o]
+            return s < 0 && (s = (s % r + r) % r), o < 0 && (o = (o % r + r) % r), o < s && (Xu = s, s = o, o = Xu), o > r && (o = r), i ? i(t, s, o) : [s, o]
         }
-        Object.defineProperties(Zc.prototype, {
+        Object.defineProperties(Yu.prototype, {
             [Symbol.toStringTag]: {
                 enumerable: !1,
                 configurable: !1,
                 value: "Row"
             },
-            [qc]: {
+            [Wu]: {
                 writable: !0,
                 enumerable: !1,
                 configurable: !1,
                 value: null
             },
-            [Qc]: {
+            [Hu]: {
                 writable: !0,
                 enumerable: !1,
                 configurable: !1,
                 value: null
             }
         });
-        const nu = t => t !== t;
+        const Qu = t => t !== t;
 
-        function iu(t) {
-            if ("object" !== typeof t || null === t) return nu(t) ? nu : e => e === t;
+        function Zu(t) {
+            if ("object" !== typeof t || null === t) return Qu(t) ? Qu : e => e === t;
             if (t instanceof Date) {
                 const e = t.valueOf();
                 return t => t instanceof Date && t.valueOf() === e
             }
             return ArrayBuffer.isView(t) ? e => !!e && function(t, e) {
                 let n = 0;
                 const i = t.length;
@@ -19268,77 +19995,77 @@
                     do {
                         if (t[n] !== e[n]) return !1
                     } while (++n < i);
                 return !0
             }(t, e) : t instanceof Map ? function(t) {
                 let e = -1;
                 const n = [];
-                for (const i of t.values()) n[++e] = iu(i);
-                return ru(n)
+                for (const i of t.values()) n[++e] = Zu(i);
+                return Gu(n)
             }(t) : Array.isArray(t) ? function(t) {
                 const e = [];
-                for (let n = -1, i = t.length; ++n < i;) e[n] = iu(t[n]);
-                return ru(e)
-            }(t) : t instanceof Ru ? function(t) {
+                for (let n = -1, i = t.length; ++n < i;) e[n] = Zu(t[n]);
+                return Gu(e)
+            }(t) : t instanceof Ch ? function(t) {
                 const e = [];
-                for (let n = -1, i = t.length; ++n < i;) e[n] = iu(t.get(n));
-                return ru(e)
+                for (let n = -1, i = t.length; ++n < i;) e[n] = Zu(t.get(n));
+                return Gu(e)
             }(t) : function(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] && arguments[1];
                 const n = Object.keys(t);
                 if (!e && 0 === n.length) return () => !1;
                 const i = [];
-                for (let r = -1, s = n.length; ++r < s;) i[r] = iu(t[n[r]]);
-                return ru(i, n)
+                for (let r = -1, s = n.length; ++r < s;) i[r] = Zu(t[n[r]]);
+                return Gu(i, n)
             }(t, !0)
         }
 
-        function ru(t, e) {
+        function Gu(t, e) {
             return n => {
                 if (!n || "object" !== typeof n) return !1;
                 switch (n.constructor) {
                     case Array:
                         return function(t, e) {
                             const n = t.length;
                             if (e.length !== n) return !1;
                             for (let i = -1; ++i < n;)
                                 if (!t[i](e[i])) return !1;
                             return !0
                         }(t, n);
                     case Map:
-                        return su(t, n, n.keys());
-                    case Zc:
-                    case Tc:
+                        return Ju(t, n, n.keys());
+                    case Yu:
+                    case bu:
                     case Object:
                     case void 0:
-                        return su(t, n, e || Object.keys(n))
+                        return Ju(t, n, e || Object.keys(n))
                 }
-                return n instanceof Ru && function(t, e) {
+                return n instanceof Ch && function(t, e) {
                     const n = t.length;
                     if (e.length !== n) return !1;
                     for (let i = -1; ++i < n;)
                         if (!t[i](e.get(i))) return !1;
                     return !0
                 }(t, n)
             }
         }
 
-        function su(t, e, n) {
+        function Ju(t, e, n) {
             const i = n[Symbol.iterator](),
                 r = e instanceof Map ? e.keys() : Object.keys(e)[Symbol.iterator](),
                 s = e instanceof Map ? e.values() : Object.values(e)[Symbol.iterator]();
             let o = 0;
             const a = t.length;
             let l = s.next(),
                 c = i.next(),
                 u = r.next();
             for (; o < a && !c.done && !u.done && !l.done && (c.value === u.value && t[o](l.value)); ++o, c = i.next(), u = r.next(), l = s.next());
             return !!(o === a && c.done && u.done && l.done) || (i.return && i.return(), r.return && r.return(), s.return && s.return(), !1)
         }
-        class ou {
+        class th {
             constructor() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 0,
                     e = arguments.length > 1 ? arguments[1] : void 0;
                 this.numChunks = t, this.getChunkIterator = e, this.chunkIndex = 0, this.chunkIterator = this.getChunkIterator(0)
             }
             next() {
                 for (; this.chunkIndex < this.numChunks;) {
@@ -19351,23 +20078,23 @@
                     value: null
                 }
             } [Symbol.iterator]() {
                 return this
             }
         }
 
-        function au(t) {
+        function eh(t) {
             return t.reduce(((t, e) => t + e.nullCount), 0)
         }
 
-        function lu(t) {
+        function nh(t) {
             return t.reduce(((t, e, n) => (t[n + 1] = t[n] + e.length, t)), new Uint32Array(t.length + 1))
         }
 
-        function cu(t, e, n, i) {
+        function ih(t, e, n, i) {
             const r = [];
             for (let s = -1, o = t.length; ++s < o;) {
                 const o = t[s],
                     a = e[s],
                     {
                         length: l
                     } = o;
@@ -19380,52 +20107,52 @@
                 const c = Math.max(0, n - a),
                     u = Math.min(i - a, l);
                 r.push(o.slice(c, u - c))
             }
             return 0 === r.length && r.push(t[0].slice(0, 0)), r
         }
 
-        function uu(t, e, n, i) {
+        function rh(t, e, n, i) {
             let r = 0,
                 s = 0,
                 o = e.length - 1;
             do {
                 if (r >= o - 1) return n < e[o] ? i(t, r, n - e[r]) : null;
                 s = r + Math.trunc(.5 * (o - r)), n < e[s] ? o = s : r = s
             } while (r < o)
         }
 
-        function hu(t, e) {
+        function sh(t, e) {
             return t.getValid(e)
         }
 
-        function du(t) {
+        function oh(t) {
             function e(e, n, i) {
                 return t(e[n], i)
             }
             return function(t) {
-                return uu(this.data, this._offsets, t, e)
+                return rh(this.data, this._offsets, t, e)
             }
         }
 
-        function fu(t) {
+        function ah(t) {
             let e;
 
             function n(n, i, r) {
                 return t(n[i], r, e)
             }
             return function(t, i) {
                 const r = this.data;
                 e = i;
-                const s = uu(r, this._offsets, t, n);
+                const s = rh(r, this._offsets, t, n);
                 return e = void 0, s
             }
         }
 
-        function pu(t) {
+        function lh(t) {
             let e;
 
             function n(n, i, r) {
                 let s = r,
                     o = 0,
                     a = 0;
                 for (let l = i - 1, c = n.length; ++l < c;) {
@@ -19434,47 +20161,47 @@
                     s = 0, a += i.length
                 }
                 return -1
             }
             return function(t, i) {
                 e = t;
                 const r = this.data,
-                    s = "number" !== typeof i ? n(r, 0, 0) : uu(r, this._offsets, i, n);
+                    s = "number" !== typeof i ? n(r, 0, 0) : rh(r, this._offsets, i, n);
                 return e = void 0, s
             }
         }
 
-        function gu(t, e, n, i) {
+        function ch(t, e, n, i) {
             return 0 !== (n & 1 << i)
         }
 
-        function mu(t, e, n, i) {
+        function uh(t, e, n, i) {
             return (n & 1 << i) >> i
         }
 
-        function yu(t, e, n) {
+        function hh(t, e, n) {
             const i = n.byteLength + 7 & -8;
             if (t > 0 || n.byteLength < i) {
                 const r = new Uint8Array(i);
-                return r.set(t % 8 === 0 ? n.subarray(t >> 3) : bu(new vu(n, t, e, null, gu)).subarray(0, i)), r
+                return r.set(t % 8 === 0 ? n.subarray(t >> 3) : dh(new fh(n, t, e, null, ch)).subarray(0, i)), r
             }
             return n
         }
 
-        function bu(t) {
+        function dh(t) {
             const e = [];
             let n = 0,
                 i = 0,
                 r = 0;
             for (const o of t) o && (r |= 1 << i), 8 === ++i && (e[n++] = r, r = i = 0);
             (0 === n || i > 0) && (e[n++] = r);
             const s = new Uint8Array(e.length + 7 & -8);
             return s.set(e), s
         }
-        class vu {
+        class fh {
             constructor(t, e, n, i, r) {
                 this.bytes = t, this.length = n, this.context = i, this.get = r, this.bit = e % 8, this.byteIndex = e >> 3, this.byte = t[this.byteIndex++], this.index = 0
             }
             next() {
                 return this.index < this.length ? (8 === this.bit && (this.bit = 0, this.byte = this.bytes[this.byteIndex++]), {
                     value: this.get(this.context, this.index++, this.byte, this.bit++)
                 }) : {
@@ -19482,109 +20209,109 @@
                     value: null
                 }
             } [Symbol.iterator]() {
                 return this
             }
         }
 
-        function _u(t, e, n) {
+        function ph(t, e, n) {
             if (n - e <= 0) return 0;
             if (n - e < 8) {
                 let i = 0;
-                for (const r of new vu(t, e, n - e, t, mu)) i += r;
+                for (const r of new fh(t, e, n - e, t, uh)) i += r;
                 return i
             }
             const i = n >> 3 << 3,
                 r = e + (e % 8 === 0 ? 0 : 8 - e % 8);
-            return _u(t, e, r) + _u(t, i, n) + function(t, e, n) {
+            return ph(t, e, r) + ph(t, i, n) + function(t, e, n) {
                 let i = 0,
                     r = Math.trunc(e);
                 const s = new DataView(t.buffer, t.byteOffset, t.byteLength),
                     o = void 0 === n ? t.byteLength : r + n;
-                for (; o - r >= 4;) i += xu(s.getUint32(r)), r += 4;
-                for (; o - r >= 2;) i += xu(s.getUint16(r)), r += 2;
-                for (; o - r >= 1;) i += xu(s.getUint8(r)), r += 1;
+                for (; o - r >= 4;) i += gh(s.getUint32(r)), r += 4;
+                for (; o - r >= 2;) i += gh(s.getUint16(r)), r += 2;
+                for (; o - r >= 1;) i += gh(s.getUint8(r)), r += 1;
                 return i
             }(t, r >> 3, i - r >> 3)
         }
 
-        function xu(t) {
+        function gh(t) {
             let e = Math.trunc(t);
             return e -= e >>> 1 & 1431655765, e = (858993459 & e) + (e >>> 2 & 858993459), 16843009 * (e + (e >>> 4) & 252645135) >>> 24
         }
-        class wu extends Xl {}
+        class mh extends jc {}
 
-        function Su(t, e, n) {
+        function yh(t, e, n) {
             if (void 0 === e) return -1;
             if (null === e) return function(t, e) {
                 const {
                     nullBitmap: n
                 } = t;
                 if (!n || t.nullCount <= 0) return -1;
                 let i = 0;
-                for (const r of new vu(n, t.offset + (e || 0), t.length, n, gu)) {
+                for (const r of new fh(n, t.offset + (e || 0), t.length, n, ch)) {
                     if (!r) return i;
                     ++i
                 }
                 return -1
             }(t, n);
-            const i = Xc.getVisitFn(t),
-                r = iu(e);
+            const i = ju.getVisitFn(t),
+                r = Zu(e);
             for (let s = (n || 0) - 1, o = t.length; ++s < o;)
                 if (r(i(t, s))) return s;
             return -1
         }
 
-        function Tu(t, e, n) {
-            const i = Xc.getVisitFn(t),
-                r = iu(e);
+        function bh(t, e, n) {
+            const i = ju.getVisitFn(t),
+                r = Zu(e);
             for (let s = (n || 0) - 1, o = t.length; ++s < o;)
                 if (r(i(t, s))) return s;
             return -1
         }
-        wu.prototype.visitNull = function(t, e) {
+        mh.prototype.visitNull = function(t, e) {
             return null === e && t.length > 0 ? 0 : -1
-        }, wu.prototype.visitBool = Su, wu.prototype.visitInt = Su, wu.prototype.visitInt8 = Su, wu.prototype.visitInt16 = Su, wu.prototype.visitInt32 = Su, wu.prototype.visitInt64 = Su, wu.prototype.visitUint8 = Su, wu.prototype.visitUint16 = Su, wu.prototype.visitUint32 = Su, wu.prototype.visitUint64 = Su, wu.prototype.visitFloat = Su, wu.prototype.visitFloat16 = Su, wu.prototype.visitFloat32 = Su, wu.prototype.visitFloat64 = Su, wu.prototype.visitUtf8 = Su, wu.prototype.visitBinary = Su, wu.prototype.visitFixedSizeBinary = Su, wu.prototype.visitDate = Su, wu.prototype.visitDateDay = Su, wu.prototype.visitDateMillisecond = Su, wu.prototype.visitTimestamp = Su, wu.prototype.visitTimestampSecond = Su, wu.prototype.visitTimestampMillisecond = Su, wu.prototype.visitTimestampMicrosecond = Su, wu.prototype.visitTimestampNanosecond = Su, wu.prototype.visitTime = Su, wu.prototype.visitTimeSecond = Su, wu.prototype.visitTimeMillisecond = Su, wu.prototype.visitTimeMicrosecond = Su, wu.prototype.visitTimeNanosecond = Su, wu.prototype.visitDecimal = Su, wu.prototype.visitList = Su, wu.prototype.visitStruct = Su, wu.prototype.visitUnion = Su, wu.prototype.visitDenseUnion = Tu, wu.prototype.visitSparseUnion = Tu, wu.prototype.visitDictionary = Su, wu.prototype.visitInterval = Su, wu.prototype.visitIntervalDayTime = Su, wu.prototype.visitIntervalYearMonth = Su, wu.prototype.visitFixedSizeList = Su, wu.prototype.visitMap = Su;
-        const ku = new wu;
-        class Mu extends Xl {}
+        }, mh.prototype.visitBool = yh, mh.prototype.visitInt = yh, mh.prototype.visitInt8 = yh, mh.prototype.visitInt16 = yh, mh.prototype.visitInt32 = yh, mh.prototype.visitInt64 = yh, mh.prototype.visitUint8 = yh, mh.prototype.visitUint16 = yh, mh.prototype.visitUint32 = yh, mh.prototype.visitUint64 = yh, mh.prototype.visitFloat = yh, mh.prototype.visitFloat16 = yh, mh.prototype.visitFloat32 = yh, mh.prototype.visitFloat64 = yh, mh.prototype.visitUtf8 = yh, mh.prototype.visitBinary = yh, mh.prototype.visitFixedSizeBinary = yh, mh.prototype.visitDate = yh, mh.prototype.visitDateDay = yh, mh.prototype.visitDateMillisecond = yh, mh.prototype.visitTimestamp = yh, mh.prototype.visitTimestampSecond = yh, mh.prototype.visitTimestampMillisecond = yh, mh.prototype.visitTimestampMicrosecond = yh, mh.prototype.visitTimestampNanosecond = yh, mh.prototype.visitTime = yh, mh.prototype.visitTimeSecond = yh, mh.prototype.visitTimeMillisecond = yh, mh.prototype.visitTimeMicrosecond = yh, mh.prototype.visitTimeNanosecond = yh, mh.prototype.visitDecimal = yh, mh.prototype.visitList = yh, mh.prototype.visitStruct = yh, mh.prototype.visitUnion = yh, mh.prototype.visitDenseUnion = bh, mh.prototype.visitSparseUnion = bh, mh.prototype.visitDictionary = yh, mh.prototype.visitInterval = yh, mh.prototype.visitIntervalDayTime = yh, mh.prototype.visitIntervalYearMonth = yh, mh.prototype.visitFixedSizeList = yh, mh.prototype.visitMap = yh;
+        const vh = new mh;
+        class _h extends jc {}
 
-        function Iu(t) {
+        function xh(t) {
             const {
                 type: e
             } = t;
-            if (0 === t.nullCount && 1 === t.stride && (e.typeId === ia.Timestamp || e instanceof Il && 64 !== e.bitWidth || e instanceof Ll && 64 !== e.bitWidth || e instanceof Ol && e.precision !== Go.HALF)) return new ou(t.data.length, (e => {
+            if (0 === t.nullCount && 1 === t.stride && (e.typeId === Za.Timestamp || e instanceof xc && 64 !== e.bitWidth || e instanceof Oc && 64 !== e.bitWidth || e instanceof Sc && e.precision !== $a.HALF)) return new th(t.data.length, (e => {
                 const n = t.data[e];
                 return n.values.subarray(0, n.length)[Symbol.iterator]()
             }));
             let n = 0;
-            return new ou(t.data.length, (e => {
+            return new th(t.data.length, (e => {
                 const i = t.data[e].length,
                     r = t.slice(n, n + i);
-                return n += i, new Eu(r)
+                return n += i, new wh(r)
             }))
         }
-        class Eu {
+        class wh {
             constructor(t) {
                 this.vector = t, this.index = 0
             }
             next() {
                 return this.index < this.vector.length ? {
                     value: this.vector.get(this.index++)
                 } : {
                     done: !0,
                     value: null
                 }
             } [Symbol.iterator]() {
                 return this
             }
         }
-        Mu.prototype.visitNull = Iu, Mu.prototype.visitBool = Iu, Mu.prototype.visitInt = Iu, Mu.prototype.visitInt8 = Iu, Mu.prototype.visitInt16 = Iu, Mu.prototype.visitInt32 = Iu, Mu.prototype.visitInt64 = Iu, Mu.prototype.visitUint8 = Iu, Mu.prototype.visitUint16 = Iu, Mu.prototype.visitUint32 = Iu, Mu.prototype.visitUint64 = Iu, Mu.prototype.visitFloat = Iu, Mu.prototype.visitFloat16 = Iu, Mu.prototype.visitFloat32 = Iu, Mu.prototype.visitFloat64 = Iu, Mu.prototype.visitUtf8 = Iu, Mu.prototype.visitBinary = Iu, Mu.prototype.visitFixedSizeBinary = Iu, Mu.prototype.visitDate = Iu, Mu.prototype.visitDateDay = Iu, Mu.prototype.visitDateMillisecond = Iu, Mu.prototype.visitTimestamp = Iu, Mu.prototype.visitTimestampSecond = Iu, Mu.prototype.visitTimestampMillisecond = Iu, Mu.prototype.visitTimestampMicrosecond = Iu, Mu.prototype.visitTimestampNanosecond = Iu, Mu.prototype.visitTime = Iu, Mu.prototype.visitTimeSecond = Iu, Mu.prototype.visitTimeMillisecond = Iu, Mu.prototype.visitTimeMicrosecond = Iu, Mu.prototype.visitTimeNanosecond = Iu, Mu.prototype.visitDecimal = Iu, Mu.prototype.visitList = Iu, Mu.prototype.visitStruct = Iu, Mu.prototype.visitUnion = Iu, Mu.prototype.visitDenseUnion = Iu, Mu.prototype.visitSparseUnion = Iu, Mu.prototype.visitDictionary = Iu, Mu.prototype.visitInterval = Iu, Mu.prototype.visitIntervalDayTime = Iu, Mu.prototype.visitIntervalYearMonth = Iu, Mu.prototype.visitFixedSizeList = Iu, Mu.prototype.visitMap = Iu;
-        const Ou = new Mu,
-            Du = (t, e) => t + e;
-        class Au extends Xl {
+        _h.prototype.visitNull = xh, _h.prototype.visitBool = xh, _h.prototype.visitInt = xh, _h.prototype.visitInt8 = xh, _h.prototype.visitInt16 = xh, _h.prototype.visitInt32 = xh, _h.prototype.visitInt64 = xh, _h.prototype.visitUint8 = xh, _h.prototype.visitUint16 = xh, _h.prototype.visitUint32 = xh, _h.prototype.visitUint64 = xh, _h.prototype.visitFloat = xh, _h.prototype.visitFloat16 = xh, _h.prototype.visitFloat32 = xh, _h.prototype.visitFloat64 = xh, _h.prototype.visitUtf8 = xh, _h.prototype.visitBinary = xh, _h.prototype.visitFixedSizeBinary = xh, _h.prototype.visitDate = xh, _h.prototype.visitDateDay = xh, _h.prototype.visitDateMillisecond = xh, _h.prototype.visitTimestamp = xh, _h.prototype.visitTimestampSecond = xh, _h.prototype.visitTimestampMillisecond = xh, _h.prototype.visitTimestampMicrosecond = xh, _h.prototype.visitTimestampNanosecond = xh, _h.prototype.visitTime = xh, _h.prototype.visitTimeSecond = xh, _h.prototype.visitTimeMillisecond = xh, _h.prototype.visitTimeMicrosecond = xh, _h.prototype.visitTimeNanosecond = xh, _h.prototype.visitDecimal = xh, _h.prototype.visitList = xh, _h.prototype.visitStruct = xh, _h.prototype.visitUnion = xh, _h.prototype.visitDenseUnion = xh, _h.prototype.visitSparseUnion = xh, _h.prototype.visitDictionary = xh, _h.prototype.visitInterval = xh, _h.prototype.visitIntervalDayTime = xh, _h.prototype.visitIntervalYearMonth = xh, _h.prototype.visitFixedSizeList = xh, _h.prototype.visitMap = xh;
+        const Sh = new _h,
+            Th = (t, e) => t + e;
+        class kh extends jc {
             visitNull(t, e) {
                 return 0
             }
             visitInt(t, e) {
                 return t.type.bitWidth / 8
             }
             visitFloat(t, e) {
@@ -19599,132 +20326,132 @@
             visitDate(t, e) {
                 return 4 * (t.type.unit + 1)
             }
             visitTime(t, e) {
                 return t.type.bitWidth / 8
             }
             visitTimestamp(t, e) {
-                return t.type.unit === ta.SECOND ? 4 : 8
+                return t.type.unit === Xa.SECOND ? 4 : 8
             }
             visitInterval(t, e) {
                 return 4 * (t.type.unit + 1)
             }
             visitStruct(t, e) {
-                return t.children.reduce(((t, n) => t + Fu.visit(n, e)), 0)
+                return t.children.reduce(((t, n) => t + Eh.visit(n, e)), 0)
             }
             visitFixedSizeBinary(t, e) {
                 return t.type.byteWidth
             }
             visitMap(t, e) {
-                return 8 + t.children.reduce(((t, n) => t + Fu.visit(n, e)), 0)
+                return 8 + t.children.reduce(((t, n) => t + Eh.visit(n, e)), 0)
             }
             visitDictionary(t, e) {
                 var n;
                 return t.type.indices.bitWidth / 8 + ((null === (n = t.dictionary) || void 0 === n ? void 0 : n.getByteLength(t.values[e])) || 0)
             }
         }
-        const Cu = (t, e) => {
+        const Mh = (t, e) => {
                 let {
                     type: n,
                     children: i,
                     typeIds: r,
                     valueOffsets: s
                 } = t;
                 const o = n.typeIdToChildIndex[r[e]];
-                return 8 + Fu.visit(i[o], s[e])
+                return 8 + Eh.visit(i[o], s[e])
             },
-            Pu = (t, e) => {
+            Ih = (t, e) => {
                 let {
                     children: n
                 } = t;
-                return 4 + Fu.visitMany(n, n.map((() => e))).reduce(Du, 0)
+                return 4 + Eh.visitMany(n, n.map((() => e))).reduce(Th, 0)
             };
-        Au.prototype.visitUtf8 = (t, e) => {
+        kh.prototype.visitUtf8 = (t, e) => {
             let {
                 valueOffsets: n
             } = t;
             return n[e + 1] - n[e] + 8
-        }, Au.prototype.visitBinary = (t, e) => {
+        }, kh.prototype.visitBinary = (t, e) => {
             let {
                 valueOffsets: n
             } = t;
             return n[e + 1] - n[e] + 8
-        }, Au.prototype.visitList = (t, e) => {
+        }, kh.prototype.visitList = (t, e) => {
             let {
                 valueOffsets: n,
                 stride: i,
                 children: r
             } = t;
             const s = r[0],
                 {
                     [e * i]: o
                 } = n,
                 {
                     [e * i + 1]: a
                 } = n,
-                l = Fu.getVisitFn(s.type),
+                l = Eh.getVisitFn(s.type),
                 c = s.slice(o, a - o);
             let u = 8;
             for (let h = -1, d = a - o; ++h < d;) u += l(c, h);
             return u
-        }, Au.prototype.visitFixedSizeList = (t, e) => {
+        }, kh.prototype.visitFixedSizeList = (t, e) => {
             let {
                 stride: n,
                 children: i
             } = t;
             const r = i[0],
                 s = r.slice(e * n, n),
-                o = Fu.getVisitFn(r.type);
+                o = Eh.getVisitFn(r.type);
             let a = 0;
             for (let l = -1, c = s.length; ++l < c;) a += o(s, l);
             return a
-        }, Au.prototype.visitUnion = (t, e) => t.type.mode === Zo.Dense ? Cu(t, e) : Pu(t, e), Au.prototype.visitDenseUnion = Cu, Au.prototype.visitSparseUnion = Pu;
-        const Fu = new Au;
-        var Lu;
-        const Nu = {},
-            Bu = {};
-        class Ru {
+        }, kh.prototype.visitUnion = (t, e) => t.type.mode === Ya.Dense ? Mh(t, e) : Ih(t, e), kh.prototype.visitDenseUnion = Mh, kh.prototype.visitSparseUnion = Ih;
+        const Eh = new kh;
+        var Oh;
+        const Dh = {},
+            Ah = {};
+        class Ch {
             constructor(t) {
                 var e, n, i;
-                const r = t[0] instanceof Ru ? t.flatMap((t => t.data)) : t;
-                if (0 === r.length || r.some((t => !(t instanceof Uu)))) throw new TypeError("Vector constructor expects an Array of Data instances.");
+                const r = t[0] instanceof Ch ? t.flatMap((t => t.data)) : t;
+                if (0 === r.length || r.some((t => !(t instanceof Fh)))) throw new TypeError("Vector constructor expects an Array of Data instances.");
                 const s = null === (e = r[0]) || void 0 === e ? void 0 : e.type;
                 switch (r.length) {
                     case 0:
                         this._offsets = [0];
                         break;
                     case 1: {
                         const {
                             get: t,
                             set: e,
                             indexOf: n,
                             byteLength: i
-                        } = Nu[s.typeId], o = r[0];
-                        this.isValid = t => hu(o, t), this.get = e => t(o, e), this.set = (t, n) => e(o, t, n), this.indexOf = t => n(o, t), this.getByteLength = t => i(o, t), this._offsets = [0, o.length];
+                        } = Dh[s.typeId], o = r[0];
+                        this.isValid = t => sh(o, t), this.get = e => t(o, e), this.set = (t, n) => e(o, t, n), this.indexOf = t => n(o, t), this.getByteLength = t => i(o, t), this._offsets = [0, o.length];
                         break
                     }
                     default:
-                        Object.setPrototypeOf(this, Bu[s.typeId]), this._offsets = lu(r)
+                        Object.setPrototypeOf(this, Ah[s.typeId]), this._offsets = nh(r)
                 }
-                this.data = r, this.type = s, this.stride = Kl(s), this.numChildren = null !== (i = null === (n = s.children) || void 0 === n ? void 0 : n.length) && void 0 !== i ? i : 0, this.length = this._offsets[this._offsets.length - 1]
+                this.data = r, this.type = s, this.stride = Vc(s), this.numChildren = null !== (i = null === (n = s.children) || void 0 === n ? void 0 : n.length) && void 0 !== i ? i : 0, this.length = this._offsets[this._offsets.length - 1]
             }
             get byteLength() {
                 return -1 === this._byteLength && (this._byteLength = this.data.reduce(((t, e) => t + e.byteLength), 0)), this._byteLength
             }
             get nullCount() {
-                return -1 === this._nullCount && (this._nullCount = au(this.data)), this._nullCount
+                return -1 === this._nullCount && (this._nullCount = eh(this.data)), this._nullCount
             }
             get ArrayType() {
                 return this.type.ArrayType
             }
             get[Symbol.toStringTag]() {
                 return "".concat(this.VectorName, "<").concat(this.type[Symbol.toStringTag], ">")
             }
             get VectorName() {
-                return "".concat(ia[this.type.typeId], "Vector")
+                return "".concat(Za[this.type.typeId], "Vector")
             }
             isValid(t) {
                 return !1
             }
             get(t) {
                 return null
             }
@@ -19734,46 +20461,46 @@
             }
             includes(t, e) {
                 return this.indexOf(t, e) > 0
             }
             getByteLength(t) {
                 return 0
             } [Symbol.iterator]() {
-                return Ou.visit(this)
+                return Sh.visit(this)
             }
             concat() {
                 for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-                return new Ru(this.data.concat(e.flatMap((t => t.data)).flat(Number.POSITIVE_INFINITY)))
+                return new Ch(this.data.concat(e.flatMap((t => t.data)).flat(Number.POSITIVE_INFINITY)))
             }
             slice(t, e) {
-                return new Ru(eu(this, t, e, ((t, e, n) => {
+                return new Ch(qu(this, t, e, ((t, e, n) => {
                     let {
                         data: i,
                         _offsets: r
                     } = t;
-                    return cu(i, r, e, n)
+                    return ih(i, r, e, n)
                 })))
             }
             toJSON() {
                 return [...this]
             }
             toArray() {
                 const {
                     type: t,
                     data: e,
                     length: n,
                     stride: i,
                     ArrayType: r
                 } = this;
                 switch (t.typeId) {
-                    case ia.Int:
-                    case ia.Float:
-                    case ia.Decimal:
-                    case ia.Time:
-                    case ia.Timestamp:
+                    case Za.Int:
+                    case Za.Float:
+                    case Za.Decimal:
+                    case Za.Time:
+                    case Za.Timestamp:
                         switch (e.length) {
                             case 0:
                                 return new r;
                             case 1:
                                 return e[0].values.subarray(0, n * i);
                             default:
                                 return e.reduce(((t, e) => {
@@ -19794,81 +20521,81 @@
                 return "[".concat([...this].join(","), "]")
             }
             getChild(t) {
                 var e;
                 return this.getChildAt(null === (e = this.type.children) || void 0 === e ? void 0 : e.findIndex((e => e.name === t)))
             }
             getChildAt(t) {
-                return t > -1 && t < this.numChildren ? new Ru(this.data.map((e => {
+                return t > -1 && t < this.numChildren ? new Ch(this.data.map((e => {
                     let {
                         children: n
                     } = e;
                     return n[t]
                 }))) : null
             }
             get isMemoized() {
-                return !!kl.isDictionary(this.type) && this.data[0].dictionary.isMemoized
+                return !!vc.isDictionary(this.type) && this.data[0].dictionary.isMemoized
             }
             memoize() {
-                if (kl.isDictionary(this.type)) {
-                    const t = new zu(this.data[0].dictionary),
+                if (vc.isDictionary(this.type)) {
+                    const t = new Ph(this.data[0].dictionary),
                         e = this.data.map((e => {
                             const n = e.clone();
                             return n.dictionary = t, n
                         }));
-                    return new Ru(e)
+                    return new Ch(e)
                 }
-                return new zu(this)
+                return new Ph(this)
             }
             unmemoize() {
-                if (kl.isDictionary(this.type) && this.isMemoized) {
+                if (vc.isDictionary(this.type) && this.isMemoized) {
                     const t = this.data[0].dictionary.unmemoize(),
                         e = this.data.map((e => {
                             const n = e.clone();
                             return n.dictionary = t, n
                         }));
-                    return new Ru(e)
+                    return new Ch(e)
                 }
                 return this
             }
         }
-        Lu = Symbol.toStringTag, Ru[Lu] = (t => {
-            t.type = kl.prototype, t.data = [], t.length = 0, t.stride = 1, t.numChildren = 0, t._nullCount = -1, t._byteLength = -1, t._offsets = new Uint32Array([0]), t[Symbol.isConcatSpreadable] = !0;
-            const e = Object.keys(ia).map((t => ia[t])).filter((t => "number" === typeof t && t !== ia.NONE));
+        Oh = Symbol.toStringTag, Ch[Oh] = (t => {
+            t.type = vc.prototype, t.data = [], t.length = 0, t.stride = 1, t.numChildren = 0, t._nullCount = -1, t._byteLength = -1, t._offsets = new Uint32Array([0]), t[Symbol.isConcatSpreadable] = !0;
+            const e = Object.keys(Za).map((t => Za[t])).filter((t => "number" === typeof t && t !== Za.NONE));
             for (const n of e) {
-                const e = Xc.getVisitFnByTypeId(n),
-                    i = xc.getVisitFnByTypeId(n),
-                    r = ku.getVisitFnByTypeId(n),
-                    s = Fu.getVisitFnByTypeId(n);
-                Nu[n] = {
+                const e = ju.getVisitFnByTypeId(n),
+                    i = gu.getVisitFnByTypeId(n),
+                    r = vh.getVisitFnByTypeId(n),
+                    s = Eh.getVisitFnByTypeId(n);
+                Dh[n] = {
                     get: e,
                     set: i,
                     indexOf: r,
                     byteLength: s
-                }, Bu[n] = Object.create(t, {
+                }, Ah[n] = Object.create(t, {
                     isValid: {
-                        value: du(hu)
+                        value: oh(sh)
                     },
                     get: {
-                        value: du(Xc.getVisitFnByTypeId(n))
+                        value: oh(ju.getVisitFnByTypeId(n))
                     },
                     set: {
-                        value: fu(xc.getVisitFnByTypeId(n))
+                        value: ah(gu.getVisitFnByTypeId(n))
                     },
                     indexOf: {
-                        value: pu(ku.getVisitFnByTypeId(n))
+                        value: lh(vh.getVisitFnByTypeId(n))
                     },
                     getByteLength: {
-                        value: du(Fu.getVisitFnByTypeId(n))
+                        value: oh(Eh.getVisitFnByTypeId(n))
                     }
                 })
             }
             return "Vector"
-        })(Ru.prototype);
-        class zu extends Ru {
+        })(Ch.prototype);
+        class Ph extends Ch {
             constructor(t) {
                 super(t.data);
                 const e = this.get,
                     n = this.set,
                     i = this.slice,
                     r = new Array(this.length);
                 Object.defineProperty(this, "get", {
@@ -19879,29 +20606,29 @@
                         return r[t] = i, i
                     }
                 }), Object.defineProperty(this, "set", {
                     value(t, e) {
                         n.call(this, t, e), r[t] = e
                     }
                 }), Object.defineProperty(this, "slice", {
-                    value: (t, e) => new zu(i.call(this, t, e))
+                    value: (t, e) => new Ph(i.call(this, t, e))
                 }), Object.defineProperty(this, "isMemoized", {
                     value: !0
                 }), Object.defineProperty(this, "unmemoize", {
-                    value: () => new Ru(this.data)
+                    value: () => new Ch(this.data)
                 }), Object.defineProperty(this, "memoize", {
                     value: () => this
                 })
             }
         }
-        class Uu {
+        class Fh {
             constructor(t, e, n, i, r) {
                 let s, o = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : [],
                     a = arguments.length > 6 ? arguments[6] : void 0;
-                this.type = t, this.children = o, this.dictionary = a, this.offset = Math.floor(Math.max(e || 0, 0)), this.length = Math.floor(Math.max(n || 0, 0)), this._nullCount = Math.floor(Math.max(i || 0, -1)), r instanceof Uu ? (this.stride = r.stride, this.values = r.values, this.typeIds = r.typeIds, this.nullBitmap = r.nullBitmap, this.valueOffsets = r.valueOffsets) : (this.stride = Kl(t), r && ((s = r[0]) && (this.valueOffsets = s), (s = r[1]) && (this.values = s), (s = r[2]) && (this.nullBitmap = s), (s = r[3]) && (this.typeIds = s))), this.nullable = 0 !== this._nullCount && this.nullBitmap && this.nullBitmap.byteLength > 0
+                this.type = t, this.children = o, this.dictionary = a, this.offset = Math.floor(Math.max(e || 0, 0)), this.length = Math.floor(Math.max(n || 0, 0)), this._nullCount = Math.floor(Math.max(i || 0, -1)), r instanceof Fh ? (this.stride = r.stride, this.values = r.values, this.typeIds = r.typeIds, this.nullBitmap = r.nullBitmap, this.valueOffsets = r.valueOffsets) : (this.stride = Vc(t), r && ((s = r[0]) && (this.valueOffsets = s), (s = r[1]) && (this.values = s), (s = r[2]) && (this.nullBitmap = s), (s = r[3]) && (this.typeIds = s))), this.nullable = 0 !== this._nullCount && this.nullBitmap && this.nullBitmap.byteLength > 0
             }
             get typeId() {
                 return this.type.typeId
             }
             get ArrayType() {
                 return this.type.ArrayType
             }
@@ -19916,15 +20643,15 @@
                     nullBitmap: i,
                     typeIds: r
                 } = this;
                 return e && (t += e.byteLength), n && (t += n.byteLength), i && (t += i.byteLength), r && (t += r.byteLength), this.children.reduce(((t, e) => t + e.byteLength), t)
             }
             get nullCount() {
                 let t, e = this._nullCount;
-                return e <= -1 && (t = this.nullBitmap) && (this._nullCount = e = this.length - _u(t, this.offset, this.offset + this.length)), e
+                return e <= -1 && (t = this.nullBitmap) && (this._nullCount = e = this.length - ph(t, this.offset, this.offset + this.length)), e
             }
             getValid(t) {
                 if (this.nullable && this.nullCount > 0) {
                     const e = this.offset + t;
                     return 0 !== (this.nullBitmap[e >> 3] & 1 << e % 8)
                 }
                 return !0
@@ -19949,306 +20676,306 @@
             clone() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this.type,
                     e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.offset,
                     n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : this.length,
                     i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : this._nullCount,
                     r = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : this,
                     s = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : this.children;
-                return new Uu(t, e, n, i, r, s, this.dictionary)
+                return new Fh(t, e, n, i, r, s, this.dictionary)
             }
             slice(t, e) {
                 const {
                     stride: n,
                     typeId: i,
                     children: r
                 } = this, s = +(0 === this._nullCount) - 1, o = 16 === i ? n : 1, a = this._sliceBuffers(t, e, n, i);
                 return this.clone(this.type, this.offset + t, e, s, a, 0 === r.length || this.valueOffsets ? r : this._sliceChildren(r, o * t, o * e))
             }
             _changeLengthAndBackfillNullBitmap(t) {
-                if (this.typeId === ia.Null) return this.clone(this.type, 0, t, 0);
+                if (this.typeId === Za.Null) return this.clone(this.type, 0, t, 0);
                 const {
                     length: e,
                     nullCount: n
                 } = this, i = new Uint8Array((t + 63 & -64) >> 3).fill(255, 0, e >> 3);
-                i[e >> 3] = (1 << e - (-8 & e)) - 1, n > 0 && i.set(yu(this.offset, e, this.nullBitmap), 0);
+                i[e >> 3] = (1 << e - (-8 & e)) - 1, n > 0 && i.set(hh(this.offset, e, this.nullBitmap), 0);
                 const r = this.buffers;
-                return r[ra.VALIDITY] = i, this.clone(this.type, 0, t, n + (t - e), r)
+                return r[Ga.VALIDITY] = i, this.clone(this.type, 0, t, n + (t - e), r)
             }
             _sliceBuffers(t, e, n, i) {
                 let r;
                 const {
                     buffers: s
                 } = this;
-                return (r = s[ra.TYPE]) && (s[ra.TYPE] = r.subarray(t, t + e)), (r = s[ra.OFFSET]) && (s[ra.OFFSET] = r.subarray(t, t + e + 1)) || (r = s[ra.DATA]) && (s[ra.DATA] = 6 === i ? r : r.subarray(n * t, n * (t + e))), s
+                return (r = s[Ga.TYPE]) && (s[Ga.TYPE] = r.subarray(t, t + e)), (r = s[Ga.OFFSET]) && (s[Ga.OFFSET] = r.subarray(t, t + e + 1)) || (r = s[Ga.DATA]) && (s[Ga.DATA] = 6 === i ? r : r.subarray(n * t, n * (t + e))), s
             }
             _sliceChildren(t, e, n) {
                 return t.map((t => t.slice(e, n)))
             }
         }
-        Uu.prototype.children = Object.freeze([]);
-        class Vu extends Xl {
+        Fh.prototype.children = Object.freeze([]);
+        class Lh extends jc {
             visit(t) {
                 return this.getVisitFn(t.type).call(this, t)
             }
             visitNull(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     length: i = 0
                 } = t;
-                return new Uu(e, n, i, 0)
+                return new Fh(e, n, i, 0)
             }
             visitBool(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.nullBitmap), r = ja(e.ArrayType, t.data), {
+                } = t, i = Rl(t.nullBitmap), r = Nl(e.ArrayType, t.data), {
                     length: s = r.length >> 3,
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, s, o, [void 0, r, i])
+                return new Fh(e, n, s, o, [void 0, r, i])
             }
             visitInt(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.nullBitmap), r = ja(e.ArrayType, t.data), {
+                } = t, i = Rl(t.nullBitmap), r = Nl(e.ArrayType, t.data), {
                     length: s = r.length,
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, s, o, [void 0, r, i])
+                return new Fh(e, n, s, o, [void 0, r, i])
             }
             visitFloat(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.nullBitmap), r = ja(e.ArrayType, t.data), {
+                } = t, i = Rl(t.nullBitmap), r = Nl(e.ArrayType, t.data), {
                     length: s = r.length,
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, s, o, [void 0, r, i])
+                return new Fh(e, n, s, o, [void 0, r, i])
             }
             visitUtf8(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.data), r = Ha(t.nullBitmap), s = Wa(t.valueOffsets), {
+                } = t, i = Rl(t.data), r = Rl(t.nullBitmap), s = Bl(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, o, a, [s, i, r])
+                return new Fh(e, n, o, a, [s, i, r])
             }
             visitBinary(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.data), r = Ha(t.nullBitmap), s = Wa(t.valueOffsets), {
+                } = t, i = Rl(t.data), r = Rl(t.nullBitmap), s = Bl(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, o, a, [s, i, r])
+                return new Fh(e, n, o, a, [s, i, r])
             }
             visitFixedSizeBinary(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.nullBitmap), r = ja(e.ArrayType, t.data), {
-                    length: s = r.length / Kl(e),
+                } = t, i = Rl(t.nullBitmap), r = Nl(e.ArrayType, t.data), {
+                    length: s = r.length / Vc(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, s, o, [void 0, r, i])
+                return new Fh(e, n, s, o, [void 0, r, i])
             }
             visitDate(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.nullBitmap), r = ja(e.ArrayType, t.data), {
-                    length: s = r.length / Kl(e),
+                } = t, i = Rl(t.nullBitmap), r = Nl(e.ArrayType, t.data), {
+                    length: s = r.length / Vc(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, s, o, [void 0, r, i])
+                return new Fh(e, n, s, o, [void 0, r, i])
             }
             visitTimestamp(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.nullBitmap), r = ja(e.ArrayType, t.data), {
-                    length: s = r.length / Kl(e),
+                } = t, i = Rl(t.nullBitmap), r = Nl(e.ArrayType, t.data), {
+                    length: s = r.length / Vc(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, s, o, [void 0, r, i])
+                return new Fh(e, n, s, o, [void 0, r, i])
             }
             visitTime(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.nullBitmap), r = ja(e.ArrayType, t.data), {
-                    length: s = r.length / Kl(e),
+                } = t, i = Rl(t.nullBitmap), r = Nl(e.ArrayType, t.data), {
+                    length: s = r.length / Vc(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, s, o, [void 0, r, i])
+                return new Fh(e, n, s, o, [void 0, r, i])
             }
             visitDecimal(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.nullBitmap), r = ja(e.ArrayType, t.data), {
-                    length: s = r.length / Kl(e),
+                } = t, i = Rl(t.nullBitmap), r = Nl(e.ArrayType, t.data), {
+                    length: s = r.length / Vc(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, s, o, [void 0, r, i])
+                return new Fh(e, n, s, o, [void 0, r, i])
             }
             visitList(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     child: i
-                } = t, r = Ha(t.nullBitmap), s = Wa(t.valueOffsets), {
+                } = t, r = Rl(t.nullBitmap), s = Bl(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, o, a, [s, void 0, r], [i])
+                return new Fh(e, n, o, a, [s, void 0, r], [i])
             }
             visitStruct(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     children: i = []
-                } = t, r = Ha(t.nullBitmap), {
+                } = t, r = Rl(t.nullBitmap), {
                     length: s = i.reduce(((t, e) => {
                         let {
                             length: n
                         } = e;
                         return Math.max(t, n)
                     }), 0),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, s, o, [void 0, void 0, r], i)
+                return new Fh(e, n, s, o, [void 0, void 0, r], i)
             }
             visitUnion(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     children: i = []
-                } = t, r = Ha(t.nullBitmap), s = ja(e.ArrayType, t.typeIds), {
+                } = t, r = Rl(t.nullBitmap), s = Nl(e.ArrayType, t.typeIds), {
                     length: o = s.length,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                if (kl.isSparseUnion(e)) return new Uu(e, n, o, a, [void 0, void 0, r, s], i);
-                const l = Wa(t.valueOffsets);
-                return new Uu(e, n, o, a, [l, void 0, r, s], i)
+                if (vc.isSparseUnion(e)) return new Fh(e, n, o, a, [void 0, void 0, r, s], i);
+                const l = Bl(t.valueOffsets);
+                return new Fh(e, n, o, a, [l, void 0, r, s], i)
             }
             visitDictionary(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.nullBitmap), r = ja(e.indices.ArrayType, t.data), {
-                    dictionary: s = new Ru([(new Vu).visit({
+                } = t, i = Rl(t.nullBitmap), r = Nl(e.indices.ArrayType, t.data), {
+                    dictionary: s = new Ch([(new Lh).visit({
                         type: e.dictionary
                     })])
                 } = t, {
                     length: o = r.length,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, o, a, [void 0, r, i], [], s)
+                return new Fh(e, n, o, a, [void 0, r, i], [], s)
             }
             visitInterval(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = Ha(t.nullBitmap), r = ja(e.ArrayType, t.data), {
-                    length: s = r.length / Kl(e),
+                } = t, i = Rl(t.nullBitmap), r = Nl(e.ArrayType, t.data), {
+                    length: s = r.length / Vc(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, s, o, [void 0, r, i])
+                return new Fh(e, n, s, o, [void 0, r, i])
             }
             visitFixedSizeList(t) {
                 const {
                     type: e,
                     offset: n = 0,
-                    child: i = (new Vu).visit({
+                    child: i = (new Lh).visit({
                         type: e.valueType
                     })
-                } = t, r = Ha(t.nullBitmap), {
-                    length: s = i.length / Kl(e),
+                } = t, r = Rl(t.nullBitmap), {
+                    length: s = i.length / Vc(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, s, o, [void 0, void 0, r], [i])
+                return new Fh(e, n, s, o, [void 0, void 0, r], [i])
             }
             visitMap(t) {
                 const {
                     type: e,
                     offset: n = 0,
-                    child: i = (new Vu).visit({
+                    child: i = (new Lh).visit({
                         type: e.childType
                     })
-                } = t, r = Ha(t.nullBitmap), s = Wa(t.valueOffsets), {
+                } = t, r = Rl(t.nullBitmap), s = Bl(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Uu(e, n, o, a, [s, void 0, r], [i])
+                return new Fh(e, n, o, a, [s, void 0, r], [i])
             }
         }
 
-        function ju(t) {
-            return (new Vu).visit(t)
+        function Nh(t) {
+            return (new Lh).visit(t)
         }
-        class Wu {
+        class Bh {
             constructor() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : [],
                     e = arguments.length > 1 ? arguments[1] : void 0,
                     n = arguments.length > 2 ? arguments[2] : void 0;
-                this.fields = t || [], this.metadata = e || new Map, n || (n = $u(t)), this.dictionaries = n
+                this.fields = t || [], this.metadata = e || new Map, n || (n = Uh(t)), this.dictionaries = n
             }
             get[Symbol.toStringTag]() {
                 return "Schema"
             }
             get names() {
                 return this.fields.map((t => t.name))
             }
             toString() {
                 return "Schema<{ ".concat(this.fields.map(((t, e) => "".concat(e, ": ").concat(t))).join(", "), " }>")
             }
             select(t) {
                 const e = new Set(t),
                     n = this.fields.filter((t => e.has(t.name)));
-                return new Wu(n, this.metadata)
+                return new Bh(n, this.metadata)
             }
             selectAt(t) {
                 const e = t.map((t => this.fields[t])).filter(Boolean);
-                return new Wu(e, this.metadata)
+                return new Bh(e, this.metadata)
             }
             assign() {
                 for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-                const i = e[0] instanceof Wu ? e[0] : Array.isArray(e[0]) ? new Wu(e[0]) : new Wu(e),
+                const i = e[0] instanceof Bh ? e[0] : Array.isArray(e[0]) ? new Bh(e[0]) : new Bh(e),
                     r = [...this.fields],
-                    s = Yu(Yu(new Map, this.metadata), i.metadata),
+                    s = zh(zh(new Map, this.metadata), i.metadata),
                     o = i.fields.filter((t => {
                         const e = r.findIndex((e => e.name === t.name));
                         return !~e || (r[e] = t.clone({
-                            metadata: Yu(Yu(new Map, r[e].metadata), t.metadata)
+                            metadata: zh(zh(new Map, r[e].metadata), t.metadata)
                         })) && !1
                     })),
-                    a = $u(o, new Map);
-                return new Wu([...r, ...o], s, new Map([...this.dictionaries, ...a]))
+                    a = Uh(o, new Map);
+                return new Bh([...r, ...o], s, new Map([...this.dictionaries, ...a]))
             }
         }
-        Wu.prototype.fields = null, Wu.prototype.metadata = null, Wu.prototype.dictionaries = null;
-        class Hu {
+        Bh.prototype.fields = null, Bh.prototype.metadata = null, Bh.prototype.dictionaries = null;
+        class Rh {
             constructor(t, e) {
                 let n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2],
                     i = arguments.length > 3 ? arguments[3] : void 0;
                 this.name = t, this.type = e, this.nullable = n, this.metadata = i || new Map
             }
             static new() {
                 for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
                 let [i, r, s, o] = e;
                 return e[0] && "object" === typeof e[0] && (({
                     name: i
-                } = e[0]), void 0 === r && (r = e[0].type), void 0 === s && (s = e[0].nullable), void 0 === o && (o = e[0].metadata)), new Hu("".concat(i), r, s, o)
+                } = e[0]), void 0 === r && (r = e[0].type), void 0 === s && (s = e[0].nullable), void 0 === o && (o = e[0].metadata)), new Rh("".concat(i), r, s, o)
             }
             get typeId() {
                 return this.type.typeId
             }
             get[Symbol.toStringTag]() {
                 return "Field"
             }
@@ -20259,370 +20986,370 @@
                 for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
                 let [i, r, s, o] = e;
                 return e[0] && "object" === typeof e[0] ? ({
                     name: i = this.name,
                     type: r = this.type,
                     nullable: s = this.nullable,
                     metadata: o = this.metadata
-                } = e[0]) : [i = this.name, r = this.type, s = this.nullable, o = this.metadata] = e, Hu.new(i, r, s, o)
+                } = e[0]) : [i = this.name, r = this.type, s = this.nullable, o = this.metadata] = e, Rh.new(i, r, s, o)
             }
         }
 
-        function Yu(t, e) {
+        function zh(t, e) {
             return new Map([...t || new Map, ...e || new Map])
         }
 
-        function $u(t) {
+        function Uh(t) {
             let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Map;
             for (let n = -1, i = t.length; ++n < i;) {
                 const i = t[n].type;
-                if (kl.isDictionary(i))
+                if (vc.isDictionary(i))
                     if (e.has(i.id)) {
                         if (e.get(i.id) !== i.dictionary) throw new Error("Cannot create Schema containing two different dictionaries with the same Id")
                     } else e.set(i.id, i.dictionary);
-                i.children && i.children.length > 0 && $u(i.children, e)
+                i.children && i.children.length > 0 && Uh(i.children, e)
             }
             return e
         }
-        Hu.prototype.type = null, Hu.prototype.name = null, Hu.prototype.nullable = null, Hu.prototype.metadata = null;
-        class Ku extends Xl {
+        Rh.prototype.type = null, Rh.prototype.name = null, Rh.prototype.nullable = null, Rh.prototype.metadata = null;
+        class Vh extends jc {
             compareSchemas(t, e) {
                 return t === e || e instanceof t.constructor && this.compareManyFields(t.fields, e.fields)
             }
             compareManyFields(t, e) {
                 return t === e || Array.isArray(t) && Array.isArray(e) && t.length === e.length && t.every(((t, n) => this.compareFields(t, e[n])))
             }
             compareFields(t, e) {
                 return t === e || e instanceof t.constructor && t.name === e.name && t.nullable === e.nullable && this.visit(t.type, e.type)
             }
         }
 
-        function Xu(t, e) {
+        function jh(t, e) {
             return e instanceof t.constructor
         }
 
-        function qu(t, e) {
-            return t === e || Xu(t, e)
+        function Wh(t, e) {
+            return t === e || jh(t, e)
         }
 
-        function Qu(t, e) {
-            return t === e || Xu(t, e) && t.bitWidth === e.bitWidth && t.isSigned === e.isSigned
+        function Hh(t, e) {
+            return t === e || jh(t, e) && t.bitWidth === e.bitWidth && t.isSigned === e.isSigned
         }
 
-        function Zu(t, e) {
-            return t === e || Xu(t, e) && t.precision === e.precision
+        function Yh(t, e) {
+            return t === e || jh(t, e) && t.precision === e.precision
         }
 
-        function Gu(t, e) {
-            return t === e || Xu(t, e) && t.unit === e.unit
+        function $h(t, e) {
+            return t === e || jh(t, e) && t.unit === e.unit
         }
 
-        function Ju(t, e) {
-            return t === e || Xu(t, e) && t.unit === e.unit && t.timezone === e.timezone
+        function Kh(t, e) {
+            return t === e || jh(t, e) && t.unit === e.unit && t.timezone === e.timezone
         }
 
-        function th(t, e) {
-            return t === e || Xu(t, e) && t.unit === e.unit && t.bitWidth === e.bitWidth
+        function Xh(t, e) {
+            return t === e || jh(t, e) && t.unit === e.unit && t.bitWidth === e.bitWidth
         }
 
-        function eh(t, e) {
-            return t === e || Xu(t, e) && t.mode === e.mode && t.typeIds.every(((t, n) => t === e.typeIds[n])) && ih.compareManyFields(t.children, e.children)
+        function qh(t, e) {
+            return t === e || jh(t, e) && t.mode === e.mode && t.typeIds.every(((t, n) => t === e.typeIds[n])) && Zh.compareManyFields(t.children, e.children)
         }
 
-        function nh(t, e) {
-            return t === e || Xu(t, e) && t.unit === e.unit
+        function Qh(t, e) {
+            return t === e || jh(t, e) && t.unit === e.unit
         }
-        Ku.prototype.visitNull = qu, Ku.prototype.visitBool = qu, Ku.prototype.visitInt = Qu, Ku.prototype.visitInt8 = Qu, Ku.prototype.visitInt16 = Qu, Ku.prototype.visitInt32 = Qu, Ku.prototype.visitInt64 = Qu, Ku.prototype.visitUint8 = Qu, Ku.prototype.visitUint16 = Qu, Ku.prototype.visitUint32 = Qu, Ku.prototype.visitUint64 = Qu, Ku.prototype.visitFloat = Zu, Ku.prototype.visitFloat16 = Zu, Ku.prototype.visitFloat32 = Zu, Ku.prototype.visitFloat64 = Zu, Ku.prototype.visitUtf8 = qu, Ku.prototype.visitBinary = qu, Ku.prototype.visitFixedSizeBinary = function(t, e) {
-            return t === e || Xu(t, e) && t.byteWidth === e.byteWidth
-        }, Ku.prototype.visitDate = Gu, Ku.prototype.visitDateDay = Gu, Ku.prototype.visitDateMillisecond = Gu, Ku.prototype.visitTimestamp = Ju, Ku.prototype.visitTimestampSecond = Ju, Ku.prototype.visitTimestampMillisecond = Ju, Ku.prototype.visitTimestampMicrosecond = Ju, Ku.prototype.visitTimestampNanosecond = Ju, Ku.prototype.visitTime = th, Ku.prototype.visitTimeSecond = th, Ku.prototype.visitTimeMillisecond = th, Ku.prototype.visitTimeMicrosecond = th, Ku.prototype.visitTimeNanosecond = th, Ku.prototype.visitDecimal = qu, Ku.prototype.visitList = function(t, e) {
-            return t === e || Xu(t, e) && t.children.length === e.children.length && ih.compareManyFields(t.children, e.children)
-        }, Ku.prototype.visitStruct = function(t, e) {
-            return t === e || Xu(t, e) && t.children.length === e.children.length && ih.compareManyFields(t.children, e.children)
-        }, Ku.prototype.visitUnion = eh, Ku.prototype.visitDenseUnion = eh, Ku.prototype.visitSparseUnion = eh, Ku.prototype.visitDictionary = function(t, e) {
-            return t === e || Xu(t, e) && t.id === e.id && t.isOrdered === e.isOrdered && ih.visit(t.indices, e.indices) && ih.visit(t.dictionary, e.dictionary)
-        }, Ku.prototype.visitInterval = nh, Ku.prototype.visitIntervalDayTime = nh, Ku.prototype.visitIntervalYearMonth = nh, Ku.prototype.visitFixedSizeList = function(t, e) {
-            return t === e || Xu(t, e) && t.listSize === e.listSize && t.children.length === e.children.length && ih.compareManyFields(t.children, e.children)
-        }, Ku.prototype.visitMap = function(t, e) {
-            return t === e || Xu(t, e) && t.keysSorted === e.keysSorted && t.children.length === e.children.length && ih.compareManyFields(t.children, e.children)
+        Vh.prototype.visitNull = Wh, Vh.prototype.visitBool = Wh, Vh.prototype.visitInt = Hh, Vh.prototype.visitInt8 = Hh, Vh.prototype.visitInt16 = Hh, Vh.prototype.visitInt32 = Hh, Vh.prototype.visitInt64 = Hh, Vh.prototype.visitUint8 = Hh, Vh.prototype.visitUint16 = Hh, Vh.prototype.visitUint32 = Hh, Vh.prototype.visitUint64 = Hh, Vh.prototype.visitFloat = Yh, Vh.prototype.visitFloat16 = Yh, Vh.prototype.visitFloat32 = Yh, Vh.prototype.visitFloat64 = Yh, Vh.prototype.visitUtf8 = Wh, Vh.prototype.visitBinary = Wh, Vh.prototype.visitFixedSizeBinary = function(t, e) {
+            return t === e || jh(t, e) && t.byteWidth === e.byteWidth
+        }, Vh.prototype.visitDate = $h, Vh.prototype.visitDateDay = $h, Vh.prototype.visitDateMillisecond = $h, Vh.prototype.visitTimestamp = Kh, Vh.prototype.visitTimestampSecond = Kh, Vh.prototype.visitTimestampMillisecond = Kh, Vh.prototype.visitTimestampMicrosecond = Kh, Vh.prototype.visitTimestampNanosecond = Kh, Vh.prototype.visitTime = Xh, Vh.prototype.visitTimeSecond = Xh, Vh.prototype.visitTimeMillisecond = Xh, Vh.prototype.visitTimeMicrosecond = Xh, Vh.prototype.visitTimeNanosecond = Xh, Vh.prototype.visitDecimal = Wh, Vh.prototype.visitList = function(t, e) {
+            return t === e || jh(t, e) && t.children.length === e.children.length && Zh.compareManyFields(t.children, e.children)
+        }, Vh.prototype.visitStruct = function(t, e) {
+            return t === e || jh(t, e) && t.children.length === e.children.length && Zh.compareManyFields(t.children, e.children)
+        }, Vh.prototype.visitUnion = qh, Vh.prototype.visitDenseUnion = qh, Vh.prototype.visitSparseUnion = qh, Vh.prototype.visitDictionary = function(t, e) {
+            return t === e || jh(t, e) && t.id === e.id && t.isOrdered === e.isOrdered && Zh.visit(t.indices, e.indices) && Zh.visit(t.dictionary, e.dictionary)
+        }, Vh.prototype.visitInterval = Qh, Vh.prototype.visitIntervalDayTime = Qh, Vh.prototype.visitIntervalYearMonth = Qh, Vh.prototype.visitFixedSizeList = function(t, e) {
+            return t === e || jh(t, e) && t.listSize === e.listSize && t.children.length === e.children.length && Zh.compareManyFields(t.children, e.children)
+        }, Vh.prototype.visitMap = function(t, e) {
+            return t === e || jh(t, e) && t.keysSorted === e.keysSorted && t.children.length === e.children.length && Zh.compareManyFields(t.children, e.children)
         };
-        const ih = new Ku;
+        const Zh = new Vh;
 
-        function rh(t, e) {
-            return ih.compareSchemas(t, e)
+        function Gh(t, e) {
+            return Zh.compareSchemas(t, e)
         }
-        var sh, oh;
-        class ah {
+        var Jh, td;
+        class ed {
             constructor() {
                 for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
                 switch (e.length) {
                     case 2:
-                        if ([this.schema] = e, !(this.schema instanceof Wu)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
-                        if ([, this.data = ju({
+                        if ([this.schema] = e, !(this.schema instanceof Bh)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
+                        if ([, this.data = Nh({
                                 nullCount: 0,
-                                type: new zl(this.schema.fields),
-                                children: this.schema.fields.map((t => ju({
+                                type: new Pc(this.schema.fields),
+                                children: this.schema.fields.map((t => Nh({
                                     type: t.type,
                                     nullCount: 0
                                 })))
-                            })] = e, !(this.data instanceof Uu)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
-                        [this.schema, this.data] = lh(this.schema, this.data.children);
+                            })] = e, !(this.data instanceof Fh)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
+                        [this.schema, this.data] = nd(this.schema, this.data.children);
                         break;
                     case 1: {
                         const [t] = e, {
                             fields: n,
                             children: i,
                             length: r
-                        } = Object.keys(t).reduce(((e, n, i) => (e.children[i] = t[n], e.length = Math.max(e.length, t[n].length), e.fields[i] = Hu.new({
+                        } = Object.keys(t).reduce(((e, n, i) => (e.children[i] = t[n], e.length = Math.max(e.length, t[n].length), e.fields[i] = Rh.new({
                             name: n,
                             type: t[n].type,
                             nullable: !0
                         }), e)), {
                             length: 0,
                             fields: new Array,
                             children: new Array
-                        }), s = new Wu(n), o = ju({
-                            type: new zl(n),
+                        }), s = new Bh(n), o = Nh({
+                            type: new Pc(n),
                             length: r,
                             children: i,
                             nullCount: 0
                         });
-                        [this.schema, this.data] = lh(s, o.children, r);
+                        [this.schema, this.data] = nd(s, o.children, r);
                         break
                     }
                     default:
                         throw new TypeError("RecordBatch constructor expects an Object mapping names to child Data, or a [Schema, Data] pair.")
                 }
             }
             get dictionaries() {
-                return this._dictionaries || (this._dictionaries = ch(this.schema.fields, this.data.children))
+                return this._dictionaries || (this._dictionaries = id(this.schema.fields, this.data.children))
             }
             get numCols() {
                 return this.schema.fields.length
             }
             get numRows() {
                 return this.data.length
             }
             get nullCount() {
                 return this.data.nullCount
             }
             isValid(t) {
                 return this.data.getValid(t)
             }
             get(t) {
-                return Xc.visit(this.data, t)
+                return ju.visit(this.data, t)
             }
             set(t, e) {
-                return xc.visit(this.data, t, e)
+                return gu.visit(this.data, t, e)
             }
             indexOf(t, e) {
-                return ku.visit(this.data, t, e)
+                return vh.visit(this.data, t, e)
             }
             getByteLength(t) {
-                return Fu.visit(this.data, t)
+                return Eh.visit(this.data, t)
             } [Symbol.iterator]() {
-                return Ou.visit(new Ru([this.data]))
+                return Sh.visit(new Ch([this.data]))
             }
             toArray() {
                 return [...this]
             }
             concat() {
                 for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-                return new fh(this.schema, [this, ...e])
+                return new ad(this.schema, [this, ...e])
             }
             slice(t, e) {
-                const [n] = new Ru([this.data]).slice(t, e).data;
-                return new ah(this.schema, n)
+                const [n] = new Ch([this.data]).slice(t, e).data;
+                return new ed(this.schema, n)
             }
             getChild(t) {
                 var e;
                 return this.getChildAt(null === (e = this.schema.fields) || void 0 === e ? void 0 : e.findIndex((e => e.name === t)))
             }
             getChildAt(t) {
-                return t > -1 && t < this.schema.fields.length ? new Ru([this.data.children[t]]) : null
+                return t > -1 && t < this.schema.fields.length ? new Ch([this.data.children[t]]) : null
             }
             setChild(t, e) {
                 var n;
                 return this.setChildAt(null === (n = this.schema.fields) || void 0 === n ? void 0 : n.findIndex((e => e.name === t)), e)
             }
             setChildAt(t, e) {
                 let n = this.schema,
                     i = this.data;
                 if (t > -1 && t < this.numCols) {
-                    e || (e = new Ru([ju({
-                        type: new Ml,
+                    e || (e = new Ch([Nh({
+                        type: new _c,
                         length: this.numRows
                     })]));
                     const r = n.fields.slice(),
                         s = i.children.slice(),
                         o = r[t].clone({
                             type: e.type
                         });
-                    [r[t], s[t]] = [o, e.data[0]], n = new Wu(r, new Map(this.schema.metadata)), i = ju({
-                        type: new zl(r),
+                    [r[t], s[t]] = [o, e.data[0]], n = new Bh(r, new Map(this.schema.metadata)), i = Nh({
+                        type: new Pc(r),
                         children: s
                     })
                 }
-                return new ah(n, i)
+                return new ed(n, i)
             }
             select(t) {
                 const e = this.schema.select(t),
-                    n = new zl(e.fields),
+                    n = new Pc(e.fields),
                     i = [];
                 for (const r of t) {
                     const t = this.schema.fields.findIndex((t => t.name === r));
                     ~t && (i[t] = this.data.children[t])
                 }
-                return new ah(e, ju({
+                return new ed(e, Nh({
                     type: n,
                     length: this.numRows,
                     children: i
                 }))
             }
             selectAt(t) {
                 const e = this.schema.selectAt(t),
                     n = t.map((t => this.data.children[t])).filter(Boolean),
-                    i = ju({
-                        type: new zl(e.fields),
+                    i = Nh({
+                        type: new Pc(e.fields),
                         length: this.numRows,
                         children: n
                     });
-                return new ah(e, i)
+                return new ed(e, i)
             }
         }
 
-        function lh(t, e) {
+        function nd(t, e) {
             let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : e.reduce(((t, e) => Math.max(t, e.length)), 0);
             var i;
             const r = [...t.fields],
                 s = [...e],
                 o = (n + 63 & -64) >> 3;
             for (const [a, l] of t.fields.entries()) {
                 const t = e[a];
                 t && t.length === n || (r[a] = l.clone({
                     nullable: !0
-                }), s[a] = null !== (i = null === t || void 0 === t ? void 0 : t._changeLengthAndBackfillNullBitmap(n)) && void 0 !== i ? i : ju({
+                }), s[a] = null !== (i = null === t || void 0 === t ? void 0 : t._changeLengthAndBackfillNullBitmap(n)) && void 0 !== i ? i : Nh({
                     type: l.type,
                     length: n,
                     nullCount: n,
                     nullBitmap: new Uint8Array(o)
                 }))
             }
-            return [t.assign(r), ju({
-                type: new zl(r),
+            return [t.assign(r), Nh({
+                type: new Pc(r),
                 length: n,
                 children: s
             })]
         }
 
-        function ch(t, e) {
+        function id(t, e) {
             let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : new Map;
             for (let i = -1, r = t.length; ++i < r;) {
                 const r = t[i].type,
                     s = e[i];
-                if (kl.isDictionary(r))
+                if (vc.isDictionary(r))
                     if (n.has(r.id)) {
                         if (n.get(r.id) !== s.dictionary) throw new Error("Cannot create Schema containing two different dictionaries with the same Id")
                     } else s.dictionary && n.set(r.id, s.dictionary);
-                r.children && r.children.length > 0 && ch(r.children, s.children, n)
+                r.children && r.children.length > 0 && id(r.children, s.children, n)
             }
             return n
         }
-        sh = Symbol.toStringTag, ah[sh] = (t => (t._nullCount = -1, t[Symbol.isConcatSpreadable] = !0, "RecordBatch"))(ah.prototype);
-        class uh extends ah {
+        Jh = Symbol.toStringTag, ed[Jh] = (t => (t._nullCount = -1, t[Symbol.isConcatSpreadable] = !0, "RecordBatch"))(ed.prototype);
+        class rd extends ed {
             constructor(t) {
-                const e = t.fields.map((t => ju({
+                const e = t.fields.map((t => Nh({
                     type: t.type
                 })));
-                super(t, ju({
-                    type: new zl(t.fields),
+                super(t, Nh({
+                    type: new Pc(t.fields),
                     nullCount: 0,
                     children: e
                 }))
             }
         }
 
-        function hh(t, e) {
+        function sd(t, e) {
             return function(t, e) {
                 const n = [...t.fields],
                     i = [],
                     r = {
                         numBatches: e.reduce(((t, e) => Math.max(t, e.length)), 0)
                     };
                 let s = 0,
                     o = 0,
                     a = -1;
                 const l = e.length;
                 let c, u = [];
                 for (; r.numBatches-- > 0;) {
                     for (o = Number.POSITIVE_INFINITY, a = -1; ++a < l;) u[a] = c = e[a].shift(), o = Math.min(o, c ? c.length : o);
-                    Number.isFinite(o) && (u = dh(n, o, u, e, r), o > 0 && (i[s++] = ju({
-                        type: new zl(n),
+                    Number.isFinite(o) && (u = od(n, o, u, e, r), o > 0 && (i[s++] = Nh({
+                        type: new Pc(n),
                         length: o,
                         nullCount: 0,
                         children: u.slice()
                     })))
                 }
-                return [t = t.assign(n), i.map((e => new ah(t, e)))]
+                return [t = t.assign(n), i.map((e => new ed(t, e)))]
             }(t, e.map((t => t.data.concat())))
         }
 
-        function dh(t, e, n, i, r) {
+        function od(t, e, n, i, r) {
             var s;
             const o = (e + 63 & -64) >> 3;
             for (let a = -1, l = i.length; ++a < l;) {
                 const l = n[a],
                     c = null === l || void 0 === l ? void 0 : l.length;
                 if (c >= e) c === e ? n[a] = l : (n[a] = l.slice(0, e), r.numBatches = Math.max(r.numBatches, i[a].unshift(l.slice(e, c - e))));
                 else {
                     const i = t[a];
                     t[a] = i.clone({
                         nullable: !0
-                    }), n[a] = null !== (s = null === l || void 0 === l ? void 0 : l._changeLengthAndBackfillNullBitmap(e)) && void 0 !== s ? s : ju({
+                    }), n[a] = null !== (s = null === l || void 0 === l ? void 0 : l._changeLengthAndBackfillNullBitmap(e)) && void 0 !== s ? s : Nh({
                         type: i.type,
                         length: e,
                         nullCount: e,
                         nullBitmap: new Uint8Array(o)
                     })
                 }
             }
             return n
         }
-        class fh {
+        class ad {
             constructor() {
                 for (var t, e, n = arguments.length, i = new Array(n), r = 0; r < n; r++) i[r] = arguments[r];
-                if (0 === i.length) return this.batches = [], this.schema = new Wu([]), this._offsets = [0], this;
+                if (0 === i.length) return this.batches = [], this.schema = new Bh([]), this._offsets = [0], this;
                 let s, o;
-                i[0] instanceof Wu && (s = i.shift()), i[i.length - 1] instanceof Uint32Array && (o = i.pop());
+                i[0] instanceof Bh && (s = i.shift()), i[i.length - 1] instanceof Uint32Array && (o = i.pop());
                 const a = t => {
                         if (t) {
-                            if (t instanceof ah) return [t];
-                            if (t instanceof fh) return t.batches;
-                            if (t instanceof Uu) {
-                                if (t.type instanceof zl) return [new ah(new Wu(t.type.children), t)]
+                            if (t instanceof ed) return [t];
+                            if (t instanceof ad) return t.batches;
+                            if (t instanceof Fh) {
+                                if (t.type instanceof Pc) return [new ed(new Bh(t.type.children), t)]
                             } else {
                                 if (Array.isArray(t)) return t.flatMap((t => a(t)));
                                 if ("function" === typeof t[Symbol.iterator]) return [...t].flatMap((t => a(t)));
                                 if ("object" === typeof t) {
                                     const e = Object.keys(t),
-                                        n = e.map((e => new Ru([t[e]]))),
-                                        i = new Wu(e.map(((t, e) => new Hu(String(t), n[e].type)))),
-                                        [, r] = hh(i, n);
-                                    return 0 === r.length ? [new ah(t)] : r
+                                        n = e.map((e => new Ch([t[e]]))),
+                                        i = new Bh(e.map(((t, e) => new Rh(String(t), n[e].type)))),
+                                        [, r] = sd(i, n);
+                                    return 0 === r.length ? [new ed(t)] : r
                                 }
                             }
                         }
                         return []
                     },
                     l = i.flatMap((t => a(t)));
-                if (s = null !== (e = null !== s && void 0 !== s ? s : null === (t = l[0]) || void 0 === t ? void 0 : t.schema) && void 0 !== e ? e : new Wu([]), !(s instanceof Wu)) throw new TypeError("Table constructor expects a [Schema, RecordBatch[]] pair.");
+                if (s = null !== (e = null !== s && void 0 !== s ? s : null === (t = l[0]) || void 0 === t ? void 0 : t.schema) && void 0 !== e ? e : new Bh([]), !(s instanceof Bh)) throw new TypeError("Table constructor expects a [Schema, RecordBatch[]] pair.");
                 for (const c of l) {
-                    if (!(c instanceof ah)) throw new TypeError("Table constructor expects a [Schema, RecordBatch[]] pair.");
-                    if (!rh(s, c.schema)) throw new TypeError("Table and inner RecordBatch schemas must be equivalent.")
+                    if (!(c instanceof ed)) throw new TypeError("Table constructor expects a [Schema, RecordBatch[]] pair.");
+                    if (!Gh(s, c.schema)) throw new TypeError("Table and inner RecordBatch schemas must be equivalent.")
                 }
-                this.schema = s, this.batches = l, this._offsets = null !== o && void 0 !== o ? o : lu(this.data)
+                this.schema = s, this.batches = l, this._offsets = null !== o && void 0 !== o ? o : nh(this.data)
             }
             get data() {
                 return this.batches.map((t => {
                     let {
                         data: e
                     } = t;
                     return e
@@ -20631,30 +21358,30 @@
             get numCols() {
                 return this.schema.fields.length
             }
             get numRows() {
                 return this.data.reduce(((t, e) => t + e.length), 0)
             }
             get nullCount() {
-                return -1 === this._nullCount && (this._nullCount = au(this.data)), this._nullCount
+                return -1 === this._nullCount && (this._nullCount = eh(this.data)), this._nullCount
             }
             isValid(t) {
                 return !1
             }
             get(t) {
                 return null
             }
             set(t, e) {}
             indexOf(t, e) {
                 return -1
             }
             getByteLength(t) {
                 return 0
             } [Symbol.iterator]() {
-                return this.batches.length > 0 ? Ou.visit(new Ru(this.data)) : new Array(0)[Symbol.iterator]()
+                return this.batches.length > 0 ? Sh.visit(new Ch(this.data)) : new Array(0)[Symbol.iterator]()
             }
             toArray() {
                 return [...this]
             }
             toString() {
                 return "[\n  ".concat(this.toArray().join(",\n  "), "\n]")
             }
@@ -20663,73 +21390,73 @@
                 for (var e = arguments.length, n = new Array(e), i = 0; i < e; i++) n[i] = arguments[i];
                 const r = this.data.concat(n.flatMap((t => {
                     let {
                         data: e
                     } = t;
                     return e
                 })));
-                return new fh(t, r.map((e => new ah(t, e))))
+                return new ad(t, r.map((e => new ed(t, e))))
             }
             slice(t, e) {
                 const n = this.schema;
-                [t, e] = eu({
+                [t, e] = qu({
                     length: this.numRows
                 }, t, e);
-                const i = cu(this.data, this._offsets, t, e);
-                return new fh(n, i.map((t => new ah(n, t))))
+                const i = ih(this.data, this._offsets, t, e);
+                return new ad(n, i.map((t => new ed(n, t))))
             }
             getChild(t) {
                 return this.getChildAt(this.schema.fields.findIndex((e => e.name === t)))
             }
             getChildAt(t) {
                 if (t > -1 && t < this.schema.fields.length) {
                     const e = this.data.map((e => e.children[t]));
                     if (0 === e.length) {
                         const {
                             type: n
-                        } = this.schema.fields[t], i = ju({
+                        } = this.schema.fields[t], i = Nh({
                             type: n,
                             length: 0,
                             nullCount: 0
                         });
                         e.push(i._changeLengthAndBackfillNullBitmap(this.numRows))
                     }
-                    return new Ru(e)
+                    return new Ch(e)
                 }
                 return null
             }
             setChild(t, e) {
                 var n;
                 return this.setChildAt(null === (n = this.schema.fields) || void 0 === n ? void 0 : n.findIndex((e => e.name === t)), e)
             }
             setChildAt(t, e) {
                 let n = this.schema,
                     i = [...this.batches];
                 if (t > -1 && t < this.numCols) {
-                    e || (e = new Ru([ju({
-                        type: new Ml,
+                    e || (e = new Ch([Nh({
+                        type: new _c,
                         length: this.numRows
                     })]));
                     const r = n.fields.slice(),
                         s = r[t].clone({
                             type: e.type
                         }),
                         o = this.schema.fields.map(((t, e) => this.getChildAt(e)));
-                    [r[t], o[t]] = [s, e], [n, i] = hh(n, o)
+                    [r[t], o[t]] = [s, e], [n, i] = sd(n, o)
                 }
-                return new fh(n, i)
+                return new ad(n, i)
             }
             select(t) {
                 const e = this.schema.fields.reduce(((t, e, n) => t.set(e.name, n)), new Map);
                 return this.selectAt(t.map((t => e.get(t))).filter((t => t > -1)))
             }
             selectAt(t) {
                 const e = this.schema.selectAt(t),
                     n = this.batches.map((e => e.selectAt(t)));
-                return new fh(e, n)
+                return new ad(e, n)
             }
             assign(t) {
                 const e = this.schema.fields,
                     [n, i] = t.schema.fields.reduce(((t, n, i) => {
                         const [r, s] = t, o = e.findIndex((t => t.name === n.name));
                         return ~o ? s[o] = i : r.push(i), t
                     }), [
@@ -20737,19 +21464,19 @@
                         []
                     ]),
                     r = this.schema.assign(t.schema),
                     s = [...e.map(((t, e) => [e, i[e]])).map((e => {
                         let [n, i] = e;
                         return void 0 === i ? this.getChildAt(n) : t.getChildAt(i)
                     })), ...n.map((e => t.getChildAt(e)))].filter(Boolean);
-                return new fh(...hh(r, s))
+                return new ad(...sd(r, s))
             }
         }
-        oh = Symbol.toStringTag, fh[oh] = (t => (t.schema = null, t.batches = [], t._offsets = new Uint32Array([0]), t._nullCount = -1, t[Symbol.isConcatSpreadable] = !0, t.isValid = du(hu), t.get = du(Xc.getVisitFn(ia.Struct)), t.set = fu(xc.getVisitFn(ia.Struct)), t.indexOf = pu(ku.getVisitFn(ia.Struct)), t.getByteLength = du(Fu.getVisitFn(ia.Struct)), "Table"))(fh.prototype);
-        class ph {
+        td = Symbol.toStringTag, ad[td] = (t => (t.schema = null, t.batches = [], t._offsets = new Uint32Array([0]), t._nullCount = -1, t[Symbol.isConcatSpreadable] = !0, t.isValid = oh(sh), t.get = oh(ju.getVisitFn(Za.Struct)), t.set = ah(gu.getVisitFn(Za.Struct)), t.indexOf = lh(vh.getVisitFn(Za.Struct)), t.getByteLength = oh(Eh.getVisitFn(Za.Struct)), "Table"))(ad.prototype);
+        class ld {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             offset() {
@@ -20764,43 +21491,43 @@
             static sizeOf() {
                 return 24
             }
             static createBlock(t, e, n, i) {
                 return t.prep(8, 24), t.writeInt64(i), t.pad(4), t.writeInt32(n), t.writeInt64(e), t.offset()
             }
         }
-        const gh = new Int32Array(2),
-            mh = new Float32Array(gh.buffer),
-            yh = new Float64Array(gh.buffer),
-            bh = 1 === new Uint16Array(new Uint8Array([1, 0]).buffer)[0];
-        class vh {
+        const cd = new Int32Array(2),
+            ud = new Float32Array(cd.buffer),
+            hd = new Float64Array(cd.buffer),
+            dd = 1 === new Uint16Array(new Uint8Array([1, 0]).buffer)[0];
+        class fd {
             constructor(t, e) {
                 this.low = 0 | t, this.high = 0 | e
             }
             static create(t, e) {
-                return 0 == t && 0 == e ? vh.ZERO : new vh(t, e)
+                return 0 == t && 0 == e ? fd.ZERO : new fd(t, e)
             }
             toFloat64() {
                 return (this.low >>> 0) + 4294967296 * this.high
             }
             equals(t) {
                 return this.low == t.low && this.high == t.high
             }
         }
-        var _h, xh, wh, Sh, Th;
-        vh.ZERO = new vh(0, 0),
+        var pd, gd, md, yd, bd;
+        fd.ZERO = new fd(0, 0),
             function(t) {
                 t[t.UTF8_BYTES = 1] = "UTF8_BYTES", t[t.UTF16_STRING = 2] = "UTF16_STRING"
-            }(_h || (_h = {}));
-        class kh {
+            }(pd || (pd = {}));
+        class vd {
             constructor(t) {
                 this.bytes_ = t, this.position_ = 0
             }
             static allocate(t) {
-                return new kh(new Uint8Array(t))
+                return new vd(new Uint8Array(t))
             }
             clear() {
                 this.position_ = 0
             }
             bytes() {
                 return this.bytes_
             }
@@ -20828,24 +21555,24 @@
             readInt32(t) {
                 return this.bytes_[t] | this.bytes_[t + 1] << 8 | this.bytes_[t + 2] << 16 | this.bytes_[t + 3] << 24
             }
             readUint32(t) {
                 return this.readInt32(t) >>> 0
             }
             readInt64(t) {
-                return new vh(this.readInt32(t), this.readInt32(t + 4))
+                return new fd(this.readInt32(t), this.readInt32(t + 4))
             }
             readUint64(t) {
-                return new vh(this.readUint32(t), this.readUint32(t + 4))
+                return new fd(this.readUint32(t), this.readUint32(t + 4))
             }
             readFloat32(t) {
-                return gh[0] = this.readInt32(t), mh[0]
+                return cd[0] = this.readInt32(t), ud[0]
             }
             readFloat64(t) {
-                return gh[bh ? 0 : 1] = this.readInt32(t), gh[bh ? 1 : 0] = this.readInt32(t + 4), yh[0]
+                return cd[dd ? 0 : 1] = this.readInt32(t), cd[dd ? 1 : 0] = this.readInt32(t + 4), hd[0]
             }
             writeInt8(t, e) {
                 this.bytes_[t] = e
             }
             writeUint8(t, e) {
                 this.bytes_[t] = e
             }
@@ -20864,18 +21591,18 @@
             writeInt64(t, e) {
                 this.writeInt32(t, e.low), this.writeInt32(t + 4, e.high)
             }
             writeUint64(t, e) {
                 this.writeUint32(t, e.low), this.writeUint32(t + 4, e.high)
             }
             writeFloat32(t, e) {
-                mh[0] = e, this.writeInt32(t, gh[0])
+                ud[0] = e, this.writeInt32(t, cd[0])
             }
             writeFloat64(t, e) {
-                yh[0] = e, this.writeInt32(t, gh[bh ? 0 : 1]), this.writeInt32(t + 4, gh[bh ? 1 : 0])
+                hd[0] = e, this.writeInt32(t, cd[dd ? 0 : 1]), this.writeInt32(t + 4, cd[dd ? 1 : 0])
             }
             getBufferIdentifier() {
                 if (this.bytes_.length < this.position_ + 4 + 4) throw new Error("FlatBuffers: ByteBuffer is too short to contain an identifier.");
                 let t = "";
                 for (let e = 0; e < 4; e++) t += String.fromCharCode(this.readInt8(this.position_ + 4 + e));
                 return t
             }
@@ -20887,15 +21614,15 @@
                 return t.bb_pos = e + this.readInt32(e), t.bb = this, t
             }
             __string(t, e) {
                 t += this.readInt32(t);
                 const n = this.readInt32(t);
                 let i = "",
                     r = 0;
-                if (t += 4, e === _h.UTF8_BYTES) return this.bytes_.subarray(t, t + n);
+                if (t += 4, e === pd.UTF8_BYTES) return this.bytes_.subarray(t, t + n);
                 for (; r < n;) {
                     let e;
                     const n = this.readUint8(t + r++);
                     if (n < 192) e = n;
                     else {
                         const i = this.readUint8(t + r++);
                         if (n < 224) e = (31 & n) << 6 | 63 & i;
@@ -20926,15 +21653,15 @@
             __has_identifier(t) {
                 if (4 != t.length) throw new Error("FlatBuffers: file identifier must be length 4");
                 for (let e = 0; e < 4; e++)
                     if (t.charCodeAt(e) != this.readInt8(this.position() + 4 + e)) return !1;
                 return !0
             }
             createLong(t, e) {
-                return vh.create(t, e)
+                return fd.create(t, e)
             }
             createScalarList(t, e) {
                 const n = [];
                 for (let i = 0; i < e; ++i) null !== t(i) && n.push(t(i));
                 return n
             }
             createObjList(t, e) {
@@ -20942,18 +21669,18 @@
                 for (let i = 0; i < e; ++i) {
                     const e = t(i);
                     null !== e && n.push(e.unpack())
                 }
                 return n
             }
         }
-        class Mh {
+        class _d {
             constructor(t) {
                 let e;
-                this.minalign = 1, this.vtable = null, this.vtable_in_use = 0, this.isNested = !1, this.object_start = 0, this.vtables = [], this.vector_num_elems = 0, this.force_defaults = !1, this.string_maps = null, e = t || 1024, this.bb = kh.allocate(e), this.space = e
+                this.minalign = 1, this.vtable = null, this.vtable_in_use = 0, this.isNested = !1, this.object_start = 0, this.vtables = [], this.vector_num_elems = 0, this.force_defaults = !1, this.string_maps = null, e = t || 1024, this.bb = vd.allocate(e), this.space = e
             }
             clear() {
                 this.bb.clear(), this.space = this.bb.capacity(), this.minalign = 1, this.vtable = null, this.vtable_in_use = 0, this.isNested = !1, this.object_start = 0, this.vtables = [], this.vector_num_elems = 0, this.force_defaults = !1, this.string_maps = null
             }
             forceDefaults(t) {
                 this.force_defaults = t
             }
@@ -20964,15 +21691,15 @@
                 return this.bb.bytes().subarray(this.bb.position(), this.bb.position() + this.offset())
             }
             prep(t, e) {
                 t > this.minalign && (this.minalign = t);
                 const n = 1 + ~(this.bb.capacity() - this.space + e) & t - 1;
                 for (; this.space < n + t + e;) {
                     const t = this.bb.capacity();
-                    this.bb = Mh.growByteBuffer(this.bb), this.space += this.bb.capacity() - t
+                    this.bb = _d.growByteBuffer(this.bb), this.space += this.bb.capacity() - t
                 }
                 this.pad(n)
             }
             pad(t) {
                 for (let e = 0; e < t; e++) this.bb.writeInt8(--this.space, 0)
             }
             writeInt8(t) {
@@ -21047,15 +21774,15 @@
             offset() {
                 return this.bb.capacity() - this.space
             }
             static growByteBuffer(t) {
                 const e = t.capacity();
                 if (3221225472 & e) throw new Error("FlatBuffers: cannot grow buffer beyond 2 gigabytes.");
                 const n = e << 1,
-                    i = kh.allocate(n);
+                    i = vd.allocate(n);
                 return i.setPosition(n - e), i.bytes().set(t.bytes(), n - e), i
             }
             addOffset(t) {
                 this.prep(4, 0), this.writeInt32(this.offset() - t + 4)
             }
             startObject(t) {
                 this.notNested(), null == this.vtable && (this.vtable = []), this.vtable_in_use = t;
@@ -21133,15 +21860,15 @@
                     }
                 }
                 this.addInt8(0), this.startVector(1, e.length, 1), this.bb.setPosition(this.space -= e.length);
                 for (let n = 0, i = this.space, r = this.bb.bytes(); n < e.length; n++) r[i++] = e[n];
                 return this.endVector()
             }
             createLong(t, e) {
-                return vh.create(t, e)
+                return fd.create(t, e)
             }
             createObjectOffset(t) {
                 return null === t ? 0 : "string" === typeof t ? this.createString(t) : t.pack(this)
             }
             createObjectOffsetList(t) {
                 const e = [];
                 for (let n = 0; n < t.length; ++n) {
@@ -21151,26 +21878,26 @@
                 }
                 return e
             }
             createStructOffsetList(t, e) {
                 return e(this, t.length), this.createObjectOffsetList(t), this.endVector()
             }
         }
-        class Ih {
+        class xd {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsKeyValue(t, e) {
-                return (e || new Ih).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new xd).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsKeyValue(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Ih).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new xd).__init(t.readInt32(t.position()) + t.position(), t)
             }
             key(t) {
                 const e = this.bb.__offset(this.bb_pos, 4);
                 return e ? this.bb.__string(this.bb_pos + e, t) : null
             }
             value(t) {
                 const e = this.bb.__offset(this.bb_pos, 6);
@@ -21185,37 +21912,37 @@
             static addValue(t, e) {
                 t.addFieldOffset(1, e, 0)
             }
             static endKeyValue(t) {
                 return t.endObject()
             }
             static createKeyValue(t, e, n) {
-                return Ih.startKeyValue(t), Ih.addKey(t, e), Ih.addValue(t, n), Ih.endKeyValue(t)
+                return xd.startKeyValue(t), xd.addKey(t, e), xd.addValue(t, n), xd.endKeyValue(t)
             }
         }! function(t) {
             t[t.V1 = 0] = "V1", t[t.V2 = 1] = "V2", t[t.V3 = 2] = "V3", t[t.V4 = 3] = "V4", t[t.V5 = 4] = "V5"
-        }(xh || (xh = {})),
+        }(gd || (gd = {})),
         function(t) {
             t[t.Little = 0] = "Little", t[t.Big = 1] = "Big"
-        }(wh || (wh = {})),
+        }(md || (md = {})),
         function(t) {
             t[t.DenseArray = 0] = "DenseArray"
-        }(Sh || (Sh = {}));
-        class Eh {
+        }(yd || (yd = {}));
+        class wd {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsInt(t, e) {
-                return (e || new Eh).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new wd).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsInt(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Eh).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new wd).__init(t.readInt32(t.position()) + t.position(), t)
             }
             bitWidth() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return t ? this.bb.readInt32(this.bb_pos + t) : 0
             }
             isSigned() {
                 const t = this.bb.__offset(this.bb_pos, 6);
@@ -21230,111 +21957,111 @@
             static addIsSigned(t, e) {
                 t.addFieldInt8(1, +e, 0)
             }
             static endInt(t) {
                 return t.endObject()
             }
             static createInt(t, e, n) {
-                return Eh.startInt(t), Eh.addBitWidth(t, e), Eh.addIsSigned(t, n), Eh.endInt(t)
+                return wd.startInt(t), wd.addBitWidth(t, e), wd.addIsSigned(t, n), wd.endInt(t)
             }
         }
-        class Oh {
+        class Sd {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsDictionaryEncoding(t, e) {
-                return (e || new Oh).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Sd).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsDictionaryEncoding(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Oh).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Sd).__init(t.readInt32(t.position()) + t.position(), t)
             }
             id() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return t ? this.bb.readInt64(this.bb_pos + t) : this.bb.createLong(0, 0)
             }
             indexType(t) {
                 const e = this.bb.__offset(this.bb_pos, 6);
-                return e ? (t || new Eh).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
+                return e ? (t || new wd).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
             }
             isOrdered() {
                 const t = this.bb.__offset(this.bb_pos, 8);
                 return !!t && !!this.bb.readInt8(this.bb_pos + t)
             }
             dictionaryKind() {
                 const t = this.bb.__offset(this.bb_pos, 10);
-                return t ? this.bb.readInt16(this.bb_pos + t) : Sh.DenseArray
+                return t ? this.bb.readInt16(this.bb_pos + t) : yd.DenseArray
             }
             static startDictionaryEncoding(t) {
                 t.startObject(4)
             }
             static addId(t, e) {
                 t.addFieldInt64(0, e, t.createLong(0, 0))
             }
             static addIndexType(t, e) {
                 t.addFieldOffset(1, e, 0)
             }
             static addIsOrdered(t, e) {
                 t.addFieldInt8(2, +e, 0)
             }
             static addDictionaryKind(t, e) {
-                t.addFieldInt16(3, e, Sh.DenseArray)
+                t.addFieldInt16(3, e, yd.DenseArray)
             }
             static endDictionaryEncoding(t) {
                 return t.endObject()
             }
         }! function(t) {
             t[t.NONE = 0] = "NONE", t[t.Null = 1] = "Null", t[t.Int = 2] = "Int", t[t.FloatingPoint = 3] = "FloatingPoint", t[t.Binary = 4] = "Binary", t[t.Utf8 = 5] = "Utf8", t[t.Bool = 6] = "Bool", t[t.Decimal = 7] = "Decimal", t[t.Date = 8] = "Date", t[t.Time = 9] = "Time", t[t.Timestamp = 10] = "Timestamp", t[t.Interval = 11] = "Interval", t[t.List = 12] = "List", t[t.Struct_ = 13] = "Struct_", t[t.Union = 14] = "Union", t[t.FixedSizeBinary = 15] = "FixedSizeBinary", t[t.FixedSizeList = 16] = "FixedSizeList", t[t.Map = 17] = "Map", t[t.Duration = 18] = "Duration", t[t.LargeBinary = 19] = "LargeBinary", t[t.LargeUtf8 = 20] = "LargeUtf8", t[t.LargeList = 21] = "LargeList"
-        }(Th || (Th = {}));
-        class Dh {
+        }(bd || (bd = {}));
+        class Td {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsField(t, e) {
-                return (e || new Dh).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Td).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsField(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Dh).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Td).__init(t.readInt32(t.position()) + t.position(), t)
             }
             name(t) {
                 const e = this.bb.__offset(this.bb_pos, 4);
                 return e ? this.bb.__string(this.bb_pos + e, t) : null
             }
             nullable() {
                 const t = this.bb.__offset(this.bb_pos, 6);
                 return !!t && !!this.bb.readInt8(this.bb_pos + t)
             }
             typeType() {
                 const t = this.bb.__offset(this.bb_pos, 8);
-                return t ? this.bb.readUint8(this.bb_pos + t) : Th.NONE
+                return t ? this.bb.readUint8(this.bb_pos + t) : bd.NONE
             }
             type(t) {
                 const e = this.bb.__offset(this.bb_pos, 10);
                 return e ? this.bb.__union(t, this.bb_pos + e) : null
             }
             dictionary(t) {
                 const e = this.bb.__offset(this.bb_pos, 12);
-                return e ? (t || new Oh).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
+                return e ? (t || new Sd).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
             }
             children(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 14);
-                return n ? (e || new Dh).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
+                return n ? (e || new Td).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
             }
             childrenLength() {
                 const t = this.bb.__offset(this.bb_pos, 14);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             customMetadata(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 16);
-                return n ? (e || new Ih).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
+                return n ? (e || new xd).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
             }
             customMetadataLength() {
                 const t = this.bb.__offset(this.bb_pos, 16);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             static startField(t) {
                 t.startObject(7)
@@ -21342,15 +22069,15 @@
             static addName(t, e) {
                 t.addFieldOffset(0, e, 0)
             }
             static addNullable(t, e) {
                 t.addFieldInt8(1, +e, 0)
             }
             static addTypeType(t, e) {
-                t.addFieldInt8(2, e, Th.NONE)
+                t.addFieldInt8(2, e, bd.NONE)
             }
             static addType(t, e) {
                 t.addFieldOffset(3, e, 0)
             }
             static addDictionary(t, e) {
                 t.addFieldOffset(4, e, 0)
             }
@@ -21376,42 +22103,42 @@
             static startCustomMetadataVector(t, e) {
                 t.startVector(4, e, 4)
             }
             static endField(t) {
                 return t.endObject()
             }
         }
-        class Ah {
+        class kd {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsSchema(t, e) {
-                return (e || new Ah).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new kd).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsSchema(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Ah).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new kd).__init(t.readInt32(t.position()) + t.position(), t)
             }
             endianness() {
                 const t = this.bb.__offset(this.bb_pos, 4);
-                return t ? this.bb.readInt16(this.bb_pos + t) : wh.Little
+                return t ? this.bb.readInt16(this.bb_pos + t) : md.Little
             }
             fields(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 6);
-                return n ? (e || new Dh).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
+                return n ? (e || new Td).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
             }
             fieldsLength() {
                 const t = this.bb.__offset(this.bb_pos, 6);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             customMetadata(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 8);
-                return n ? (e || new Ih).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
+                return n ? (e || new xd).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
             }
             customMetadataLength() {
                 const t = this.bb.__offset(this.bb_pos, 8);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             features(t) {
                 const e = this.bb.__offset(this.bb_pos, 10);
@@ -21421,15 +22148,15 @@
                 const t = this.bb.__offset(this.bb_pos, 10);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             static startSchema(t) {
                 t.startObject(4)
             }
             static addEndianness(t, e) {
-                t.addFieldInt16(0, e, wh.Little)
+                t.addFieldInt16(0, e, md.Little)
             }
             static addFields(t, e) {
                 t.addFieldOffset(1, e, 0)
             }
             static createFieldsVector(t, e) {
                 t.startVector(4, e.length, 4);
                 for (let n = e.length - 1; n >= 0; n--) t.addOffset(e[n]);
@@ -21466,67 +22193,67 @@
             static finishSchemaBuffer(t, e) {
                 t.finish(e)
             }
             static finishSizePrefixedSchemaBuffer(t, e) {
                 t.finish(e, void 0, !0)
             }
             static createSchema(t, e, n, i, r) {
-                return Ah.startSchema(t), Ah.addEndianness(t, e), Ah.addFields(t, n), Ah.addCustomMetadata(t, i), Ah.addFeatures(t, r), Ah.endSchema(t)
+                return kd.startSchema(t), kd.addEndianness(t, e), kd.addFields(t, n), kd.addCustomMetadata(t, i), kd.addFeatures(t, r), kd.endSchema(t)
             }
         }
-        class Ch {
+        class Md {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsFooter(t, e) {
-                return (e || new Ch).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Md).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsFooter(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Ch).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Md).__init(t.readInt32(t.position()) + t.position(), t)
             }
             version() {
                 const t = this.bb.__offset(this.bb_pos, 4);
-                return t ? this.bb.readInt16(this.bb_pos + t) : xh.V1
+                return t ? this.bb.readInt16(this.bb_pos + t) : gd.V1
             }
             schema(t) {
                 const e = this.bb.__offset(this.bb_pos, 6);
-                return e ? (t || new Ah).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
+                return e ? (t || new kd).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
             }
             dictionaries(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 8);
-                return n ? (e || new ph).__init(this.bb.__vector(this.bb_pos + n) + 24 * t, this.bb) : null
+                return n ? (e || new ld).__init(this.bb.__vector(this.bb_pos + n) + 24 * t, this.bb) : null
             }
             dictionariesLength() {
                 const t = this.bb.__offset(this.bb_pos, 8);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             recordBatches(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 10);
-                return n ? (e || new ph).__init(this.bb.__vector(this.bb_pos + n) + 24 * t, this.bb) : null
+                return n ? (e || new ld).__init(this.bb.__vector(this.bb_pos + n) + 24 * t, this.bb) : null
             }
             recordBatchesLength() {
                 const t = this.bb.__offset(this.bb_pos, 10);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             customMetadata(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 12);
-                return n ? (e || new Ih).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
+                return n ? (e || new xd).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
             }
             customMetadataLength() {
                 const t = this.bb.__offset(this.bb_pos, 12);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             static startFooter(t) {
                 t.startObject(5)
             }
             static addVersion(t, e) {
-                t.addFieldInt16(0, e, xh.V1)
+                t.addFieldInt16(0, e, gd.V1)
             }
             static addSchema(t, e) {
                 t.addFieldOffset(1, e, 0)
             }
             static addDictionaries(t, e) {
                 t.addFieldOffset(2, e, 0)
             }
@@ -21556,40 +22283,40 @@
             static finishFooterBuffer(t, e) {
                 t.finish(e)
             }
             static finishSizePrefixedFooterBuffer(t, e) {
                 t.finish(e, void 0, !0)
             }
         }
-        var Ph = vh,
-            Fh = Mh,
-            Lh = kh;
-        class Nh {
+        var Id = fd,
+            Ed = _d,
+            Od = vd;
+        class Dd {
             constructor(t) {
-                let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Qo.V4,
+                let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Ha.V4,
                     n = arguments.length > 2 ? arguments[2] : void 0,
                     i = arguments.length > 3 ? arguments[3] : void 0;
                 this.schema = t, this.version = e, n && (this._recordBatches = n), i && (this._dictionaryBatches = i)
             }
             static decode(t) {
-                t = new Lh(Ha(t));
-                const e = Ch.getRootAsFooter(t),
-                    n = Wu.decode(e.schema());
-                return new Bh(n, e)
+                t = new Od(Rl(t));
+                const e = Md.getRootAsFooter(t),
+                    n = Bh.decode(e.schema());
+                return new Ad(n, e)
             }
             static encode(t) {
-                const e = new Fh,
-                    n = Wu.encode(e, t.schema);
-                Ch.startRecordBatchesVector(e, t.numRecordBatches);
-                for (const s of [...t.recordBatches()].slice().reverse()) Rh.encode(e, s);
+                const e = new Ed,
+                    n = Bh.encode(e, t.schema);
+                Md.startRecordBatchesVector(e, t.numRecordBatches);
+                for (const s of [...t.recordBatches()].slice().reverse()) Cd.encode(e, s);
                 const i = e.endVector();
-                Ch.startDictionariesVector(e, t.numDictionaries);
-                for (const s of [...t.dictionaryBatches()].slice().reverse()) Rh.encode(e, s);
+                Md.startDictionariesVector(e, t.numDictionaries);
+                for (const s of [...t.dictionaryBatches()].slice().reverse()) Cd.encode(e, s);
                 const r = e.endVector();
-                return Ch.startFooter(e), Ch.addSchema(e, n), Ch.addVersion(e, Qo.V4), Ch.addRecordBatches(e, i), Ch.addDictionaries(e, r), Ch.finishFooterBuffer(e, Ch.endFooter(e)), e.asUint8Array()
+                return Md.startFooter(e), Md.addSchema(e, n), Md.addVersion(e, Ha.V4), Md.addRecordBatches(e, i), Md.addDictionaries(e, r), Md.finishFooterBuffer(e, Md.endFooter(e)), e.asUint8Array()
             }
             get numRecordBatches() {
                 return this._recordBatches.length
             }
             get numDictionaries() {
                 return this._dictionaryBatches.length
             }* recordBatches() {
@@ -21600,66 +22327,66 @@
             getRecordBatch(t) {
                 return t >= 0 && t < this.numRecordBatches && this._recordBatches[t] || null
             }
             getDictionaryBatch(t) {
                 return t >= 0 && t < this.numDictionaries && this._dictionaryBatches[t] || null
             }
         }
-        class Bh extends Nh {
+        class Ad extends Dd {
             constructor(t, e) {
                 super(t, e.version()), this._footer = e
             }
             get numRecordBatches() {
                 return this._footer.recordBatchesLength()
             }
             get numDictionaries() {
                 return this._footer.dictionariesLength()
             }
             getRecordBatch(t) {
                 if (t >= 0 && t < this.numRecordBatches) {
                     const e = this._footer.recordBatches(t);
-                    if (e) return Rh.decode(e)
+                    if (e) return Cd.decode(e)
                 }
                 return null
             }
             getDictionaryBatch(t) {
                 if (t >= 0 && t < this.numDictionaries) {
                     const e = this._footer.dictionaries(t);
-                    if (e) return Rh.decode(e)
+                    if (e) return Cd.decode(e)
                 }
                 return null
             }
         }
-        class Rh {
+        class Cd {
             constructor(t, e, n) {
                 this.metaDataLength = t, this.offset = "number" === typeof n ? n : n.low, this.bodyLength = "number" === typeof e ? e : e.low
             }
             static decode(t) {
-                return new Rh(t.metaDataLength(), t.bodyLength(), t.offset())
+                return new Cd(t.metaDataLength(), t.bodyLength(), t.offset())
             }
             static encode(t, e) {
                 const {
                     metaDataLength: n
-                } = e, i = new Ph(e.offset, 0), r = new Ph(e.bodyLength, 0);
-                return ph.createBlock(t, i, n, r)
+                } = e, i = new Id(e.offset, 0), r = new Id(e.bodyLength, 0);
+                return ld.createBlock(t, i, n, r)
             }
         }
-        const zh = {
-                fromIterable: t => Uh(function*(t) {
+        const Pd = {
+                fromIterable: t => Fd(function*(t) {
                     let e, n, i, r, s = !1,
                         o = [],
                         a = 0;
 
                     function l() {
-                        return "peek" === i ? Va(o, r)[0] : ([n, o, a] = Va(o, r), n)
+                        return "peek" === i ? Ll(o, r)[0] : ([n, o, a] = Ll(o, r), n)
                     }({
                         cmd: i,
                         size: r
                     } = yield null);
-                    const c = (u = t, $a(Uint8Array, u))[Symbol.iterator]();
+                    const c = (u = t, Ul(Uint8Array, u))[Symbol.iterator]();
                     var u;
                     try {
                         do {
                             if (({
                                     done: e,
                                     value: n
                                 } = Number.isNaN(r - a) ? c.next() : c.next(r - a)), !e && n.byteLength > 0 && (o.push(n), a += n.byteLength), e || r <= a)
@@ -21673,116 +22400,116 @@
                     } catch (h) {
                         (s = !0) && "function" === typeof c.throw && c.throw(h)
                     } finally {
                         !1 === s && "function" === typeof c.return && c.return(null)
                     }
                     return null
                 }(t)),
-                fromAsyncIterable: t => Uh(function(t) {
-                    return Ca(this, arguments, (function*() {
+                fromAsyncIterable: t => Fd(function(t) {
+                    return Ml(this, arguments, (function*() {
                         let e, n, i, r, s = !1,
                             o = [],
                             a = 0;
 
                         function l() {
-                            return "peek" === i ? Va(o, r)[0] : ([n, o, a] = Va(o, r), n)
+                            return "peek" === i ? Ll(o, r)[0] : ([n, o, a] = Ll(o, r), n)
                         }({
                             cmd: i,
                             size: r
-                        } = yield yield Aa(null));
-                        const c = (u = t, Ka(Uint8Array, u))[Symbol.asyncIterator]();
+                        } = yield yield kl(null));
+                        const c = (u = t, Vl(Uint8Array, u))[Symbol.asyncIterator]();
                         var u;
                         try {
                             do {
                                 if (({
                                         done: e,
                                         value: n
-                                    } = Number.isNaN(r - a) ? yield Aa(c.next()): yield Aa(c.next(r - a))), !e && n.byteLength > 0 && (o.push(n), a += n.byteLength), e || r <= a)
+                                    } = Number.isNaN(r - a) ? yield kl(c.next()): yield kl(c.next(r - a))), !e && n.byteLength > 0 && (o.push(n), a += n.byteLength), e || r <= a)
                                     do {
                                         ({
                                             cmd: i,
                                             size: r
-                                        } = yield yield Aa(l()))
+                                        } = yield yield kl(l()))
                                     } while (r < a)
                             } while (!e)
                         } catch (h) {
-                            (s = !0) && "function" === typeof c.throw && (yield Aa(c.throw(h)))
+                            (s = !0) && "function" === typeof c.throw && (yield kl(c.throw(h)))
                         } finally {
-                            !1 === s && "function" === typeof c.return && (yield Aa(c.return(new Uint8Array(0))))
+                            !1 === s && "function" === typeof c.return && (yield kl(c.return(new Uint8Array(0))))
                         }
-                        return yield Aa(null)
+                        return yield kl(null)
                     }))
                 }(t)),
-                fromDOMStream: t => Uh(function(t) {
-                    return Ca(this, arguments, (function*() {
+                fromDOMStream: t => Fd(function(t) {
+                    return Ml(this, arguments, (function*() {
                         let e, n, i, r = !1,
                             s = !1,
                             o = [],
                             a = 0;
 
                         function l() {
-                            return "peek" === n ? Va(o, i)[0] : ([e, o, a] = Va(o, i), e)
+                            return "peek" === n ? Ll(o, i)[0] : ([e, o, a] = Ll(o, i), e)
                         }({
                             cmd: n,
                             size: i
-                        } = yield yield Aa(null));
-                        const c = new Vh(t);
+                        } = yield yield kl(null));
+                        const c = new Ld(t);
                         try {
                             do {
                                 if (({
                                         done: r,
                                         value: e
-                                    } = Number.isNaN(i - a) ? yield Aa(c.read()): yield Aa(c.read(i - a))), !r && e.byteLength > 0 && (o.push(Ha(e)), a += e.byteLength), r || i <= a)
+                                    } = Number.isNaN(i - a) ? yield kl(c.read()): yield kl(c.read(i - a))), !r && e.byteLength > 0 && (o.push(Rl(e)), a += e.byteLength), r || i <= a)
                                     do {
                                         ({
                                             cmd: n,
                                             size: i
-                                        } = yield yield Aa(l()))
+                                        } = yield yield kl(l()))
                                     } while (i < a)
                             } while (!r)
                         } catch (u) {
-                            (s = !0) && (yield Aa(c.cancel(u)))
+                            (s = !0) && (yield kl(c.cancel(u)))
                         } finally {
-                            !1 === s ? yield Aa(c.cancel()): t.locked && c.releaseLock()
+                            !1 === s ? yield kl(c.cancel()): t.locked && c.releaseLock()
                         }
-                        return yield Aa(null)
+                        return yield kl(null)
                     }))
                 }(t)),
-                fromNodeStream: t => Uh(function(t) {
-                    return Ca(this, arguments, (function*() {
+                fromNodeStream: t => Fd(function(t) {
+                    return Ml(this, arguments, (function*() {
                         const e = [];
                         let n, i, r, s = "error",
                             o = !1,
                             a = null,
                             l = 0,
                             c = [];
 
                         function u() {
-                            return "peek" === n ? Va(c, i)[0] : ([r, c, l] = Va(c, i), r)
+                            return "peek" === n ? Ll(c, i)[0] : ([r, c, l] = Ll(c, i), r)
                         }
                         if (({
                                 cmd: n,
                                 size: i
-                            } = yield yield Aa(null)), t.isTTY) return yield yield Aa(new Uint8Array(0)), yield Aa(null);
+                            } = yield yield kl(null)), t.isTTY) return yield yield kl(new Uint8Array(0)), yield kl(null);
                         try {
-                            e[0] = jh(t, "end"), e[1] = jh(t, "error");
+                            e[0] = Nd(t, "end"), e[1] = Nd(t, "error");
                             do {
-                                if (e[2] = jh(t, "readable"), [s, a] = yield Aa(Promise.race(e.map((t => t[2])))), "error" === s) break;
-                                if ((o = "end" === s) || (Number.isFinite(i - l) ? (r = Ha(t.read(i - l)), r.byteLength < i - l && (r = Ha(t.read()))) : r = Ha(t.read()), r.byteLength > 0 && (c.push(r), l += r.byteLength)), o || i <= l)
+                                if (e[2] = Nd(t, "readable"), [s, a] = yield kl(Promise.race(e.map((t => t[2])))), "error" === s) break;
+                                if ((o = "end" === s) || (Number.isFinite(i - l) ? (r = Rl(t.read(i - l)), r.byteLength < i - l && (r = Rl(t.read()))) : r = Rl(t.read()), r.byteLength > 0 && (c.push(r), l += r.byteLength)), o || i <= l)
                                     do {
                                         ({
                                             cmd: n,
                                             size: i
-                                        } = yield yield Aa(u()))
+                                        } = yield yield kl(u()))
                                     } while (i < l)
                             } while (!o)
                         } finally {
-                            yield Aa(h(e, "error" === s ? a : null))
+                            yield kl(h(e, "error" === s ? a : null))
                         }
-                        return yield Aa(null);
+                        return yield kl(null);
 
                         function h(e, n) {
                             return r = c = null, new Promise(((i, r) => {
                                 for (const [n, o] of e) t.off(n, o);
                                 try {
                                     const e = t.destroy;
                                     e && e.call(t, n), n = void 0
@@ -21798,69 +22525,69 @@
                 toDOMStream(t, e) {
                     throw new Error('"toDOMStream" not available in this environment')
                 },
                 toNodeStream(t, e) {
                     throw new Error('"toNodeStream" not available in this environment')
                 }
             },
-            Uh = t => (t.next(), t);
-        class Vh {
+            Fd = t => (t.next(), t);
+        class Ld {
             constructor(t) {
                 this.source = t, this.reader = null, this.reader = this.source.getReader(), this.reader.closed.catch((() => {}))
             }
             get closed() {
                 return this.reader ? this.reader.closed.catch((() => {})) : Promise.resolve()
             }
             releaseLock() {
                 this.reader && this.reader.releaseLock(), this.reader = null
             }
             cancel(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     const {
                         reader: e,
                         source: n
                     } = this;
                     e && (yield e.cancel(t).catch((() => {}))), n && n.locked && this.releaseLock()
                 }))
             }
             read(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     if (0 === t) return {
                         done: null == this.reader,
                         value: new Uint8Array(0)
                     };
                     const e = yield this.reader.read();
-                    return !e.done && (e.value = Ha(e)), e
+                    return !e.done && (e.value = Rl(e)), e
                 }))
             }
         }
-        const jh = (t, e) => {
+        const Nd = (t, e) => {
             const n = t => i([e, t]);
             let i;
             return [e, n, new Promise((r => (i = r) && t.once(e, n)))]
         };
-        const Wh = Object.freeze({
+        const Bd = Object.freeze({
             done: !0,
             value: void 0
         });
-        class Hh {
+        class Rd {
             constructor(t) {
                 this._json = t
             }
             get schema() {
                 return this._json.schema
             }
             get batches() {
                 return this._json.batches || []
             }
             get dictionaries() {
                 return this._json.dictionaries || []
             }
         }
-        class Yh {
+        class zd {
             tee() {
                 return this._getDOMStream().tee()
             }
             pipe(t, e) {
                 return this._getNodeStream().pipe(t, e)
             }
             pipeTo(t, e) {
@@ -21872,23 +22599,23 @@
             _getDOMStream() {
                 return this._DOMStream || (this._DOMStream = this.toDOMStream())
             }
             _getNodeStream() {
                 return this._nodeStream || (this._nodeStream = this.toNodeStream())
             }
         }
-        class $h extends Yh {
+        class Ud extends zd {
             constructor() {
                 super(), this._values = [], this.resolvers = [], this._closedPromise = new Promise((t => this._closedPromiseResolve = t))
             }
             get closed() {
                 return this._closedPromise
             }
             cancel(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     yield this.return(t)
                 }))
             }
             write(t) {
                 this._ensureOpen() && (this.resolvers.length <= 0 ? this._values.push(t) : this.resolvers.shift().resolve({
                     done: !1,
                     value: t
@@ -21903,43 +22630,43 @@
                 }))
             }
             close() {
                 if (this._closedPromiseResolve) {
                     const {
                         resolvers: t
                     } = this;
-                    for (; t.length > 0;) t.shift().resolve(Wh);
+                    for (; t.length > 0;) t.shift().resolve(Bd);
                     this._closedPromiseResolve(), this._closedPromiseResolve = void 0
                 }
             } [Symbol.asyncIterator]() {
                 return this
             }
             toDOMStream(t) {
-                return zh.toDOMStream(this._closedPromiseResolve || this._error ? this : this._values, t)
+                return Pd.toDOMStream(this._closedPromiseResolve || this._error ? this : this._values, t)
             }
             toNodeStream(t) {
-                return zh.toNodeStream(this._closedPromiseResolve || this._error ? this : this._values, t)
+                return Pd.toNodeStream(this._closedPromiseResolve || this._error ? this : this._values, t)
             }
             throw (t) {
-                return Oa(this, void 0, void 0, (function*() {
-                    return yield this.abort(t), Wh
+                return Sl(this, void 0, void 0, (function*() {
+                    return yield this.abort(t), Bd
                 }))
             }
             return (t) {
-                return Oa(this, void 0, void 0, (function*() {
-                    return yield this.close(), Wh
+                return Sl(this, void 0, void 0, (function*() {
+                    return yield this.close(), Bd
                 }))
             }
             read(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     return (yield this.next(t, "read")).value
                 }))
             }
             peek(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     return (yield this.next(t, "peek")).value
                 }))
             }
             next() {
                 return this._values.length > 0 ? Promise.resolve({
                     done: !1,
                     value: this._values.shift()
@@ -21947,56 +22674,56 @@
                     done: !0,
                     value: this._error.error
                 }) : this._closedPromiseResolve ? new Promise(((t, e) => {
                     this.resolvers.push({
                         resolve: t,
                         reject: e
                     })
-                })) : Promise.resolve(Wh)
+                })) : Promise.resolve(Bd)
             }
             _ensureOpen() {
                 if (this._closedPromiseResolve) return !0;
                 throw new Error("AsyncQueue is closed")
             }
         }
-        class Kh extends $h {
+        class Vd extends Ud {
             write(t) {
-                if ((t = Ha(t)).byteLength > 0) return super.write(t)
+                if ((t = Rl(t)).byteLength > 0) return super.write(t)
             }
             toString() {
-                return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? Na(this.toUint8Array(!0)) : this.toUint8Array(!1).then(Na)
+                return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? Dl(this.toUint8Array(!0)) : this.toUint8Array(!1).then(Dl)
             }
             toUint8Array() {
-                return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? Va(this._values)[0] : (() => Oa(this, void 0, void 0, (function*() {
+                return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? Ll(this._values)[0] : (() => Sl(this, void 0, void 0, (function*() {
                     var t, e;
                     const n = [];
                     let i = 0;
                     try {
-                        for (var r, s = Fa(this); !(r = yield s.next()).done;) {
+                        for (var r, s = El(this); !(r = yield s.next()).done;) {
                             const t = r.value;
                             n.push(t), i += t.byteLength
                         }
                     } catch (o) {
                         t = {
                             error: o
                         }
                     } finally {
                         try {
                             r && !r.done && (e = s.return) && (yield e.call(s))
                         } finally {
                             if (t) throw t.error
                         }
                     }
-                    return Va(n, i)[0]
+                    return Ll(n, i)[0]
                 })))()
             }
         }
-        class Xh {
+        class jd {
             constructor(t) {
-                t && (this.source = new Qh(zh.fromIterable(t)))
+                t && (this.source = new Hd(Pd.fromIterable(t)))
             } [Symbol.iterator]() {
                 return this
             }
             next(t) {
                 return this.source.next(t)
             }
             throw (t) {
@@ -22008,17 +22735,17 @@
             peek(t) {
                 return this.source.peek(t)
             }
             read(t) {
                 return this.source.read(t)
             }
         }
-        class qh {
+        class Wd {
             constructor(t) {
-                t instanceof qh ? this.source = t.source : t instanceof Kh ? this.source = new Zh(zh.fromAsyncIterable(t)) : Ma(t) ? this.source = new Zh(zh.fromNodeStream(t)) : ka(t) ? this.source = new Zh(zh.fromDOMStream(t)) : Sa(t) ? this.source = new Zh(zh.fromDOMStream(t.body)) : ba(t) ? this.source = new Zh(zh.fromIterable(t)) : (ya(t) || va(t)) && (this.source = new Zh(zh.fromAsyncIterable(t)))
+                t instanceof Wd ? this.source = t.source : t instanceof Vd ? this.source = new Yd(Pd.fromAsyncIterable(t)) : _l(t) ? this.source = new Yd(Pd.fromNodeStream(t)) : vl(t) ? this.source = new Yd(Pd.fromDOMStream(t)) : yl(t) ? this.source = new Yd(Pd.fromDOMStream(t.body)) : dl(t) ? this.source = new Yd(Pd.fromIterable(t)) : (hl(t) || fl(t)) && (this.source = new Yd(Pd.fromAsyncIterable(t)))
             } [Symbol.asyncIterator]() {
                 return this
             }
             next(t) {
                 return this.source.next(t)
             }
             throw (t) {
@@ -22036,15 +22763,15 @@
             peek(t) {
                 return this.source.peek(t)
             }
             read(t) {
                 return this.source.read(t)
             }
         }
-        class Qh {
+        class Hd {
             constructor(t) {
                 this.source = t
             }
             cancel(t) {
                 this.return(t)
             }
             peek(t) {
@@ -22057,67 +22784,67 @@
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "read";
                 return this.source.next({
                     cmd: e,
                     size: t
                 })
             }
             throw (t) {
-                return Object.create(this.source.throw && this.source.throw(t) || Wh)
+                return Object.create(this.source.throw && this.source.throw(t) || Bd)
             }
             return (t) {
-                return Object.create(this.source.return && this.source.return(t) || Wh)
+                return Object.create(this.source.return && this.source.return(t) || Bd)
             }
         }
-        class Zh {
+        class Yd {
             constructor(t) {
                 this.source = t, this._closedPromise = new Promise((t => this._closedPromiseResolve = t))
             }
             cancel(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     yield this.return(t)
                 }))
             }
             get closed() {
                 return this._closedPromise
             }
             read(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     return (yield this.next(t, "read")).value
                 }))
             }
             peek(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     return (yield this.next(t, "peek")).value
                 }))
             }
             next(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "read";
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     return yield this.source.next({
                         cmd: e,
                         size: t
                     })
                 }))
             }
             throw (t) {
-                return Oa(this, void 0, void 0, (function*() {
-                    const e = this.source.throw && (yield this.source.throw(t)) || Wh;
+                return Sl(this, void 0, void 0, (function*() {
+                    const e = this.source.throw && (yield this.source.throw(t)) || Bd;
                     return this._closedPromiseResolve && this._closedPromiseResolve(), this._closedPromiseResolve = void 0, Object.create(e)
                 }))
             }
             return (t) {
-                return Oa(this, void 0, void 0, (function*() {
-                    const e = this.source.return && (yield this.source.return(t)) || Wh;
+                return Sl(this, void 0, void 0, (function*() {
+                    const e = this.source.return && (yield this.source.return(t)) || Bd;
                     return this._closedPromiseResolve && this._closedPromiseResolve(), this._closedPromiseResolve = void 0, Object.create(e)
                 }))
             }
         }
-        class Gh extends Xh {
+        class $d extends jd {
             constructor(t, e) {
-                super(), this.position = 0, this.buffer = Ha(t), this.size = "undefined" === typeof e ? this.buffer.byteLength : e
+                super(), this.position = 0, this.buffer = Rl(t), this.size = "undefined" === typeof e ? this.buffer.byteLength : e
             }
             readInt32(t) {
                 const {
                     buffer: e,
                     byteOffset: n
                 } = this.readAt(t, 4);
                 return new DataView(e, n).getInt32(0, !0)
@@ -22150,36 +22877,36 @@
             return (t) {
                 return this.close(), {
                     done: !0,
                     value: t
                 }
             }
         }
-        class Jh extends qh {
+        class Kd extends Wd {
             constructor(t, e) {
-                super(), this.position = 0, this._handle = t, "number" === typeof e ? this.size = e : this._pending = (() => Oa(this, void 0, void 0, (function*() {
+                super(), this.position = 0, this._handle = t, "number" === typeof e ? this.size = e : this._pending = (() => Sl(this, void 0, void 0, (function*() {
                     this.size = (yield t.stat()).size, delete this._pending
                 })))()
             }
             readInt32(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     const {
                         buffer: e,
                         byteOffset: n
                     } = yield this.readAt(t, 4);
                     return new DataView(e, n).getInt32(0, !0)
                 }))
             }
             seek(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     return this._pending && (yield this._pending), this.position = Math.min(t, this.size), t < this.size
                 }))
             }
             read(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     this._pending && (yield this._pending);
                     const {
                         _handle: e,
                         size: n,
                         position: i
                     } = this;
                     if (e && i < n) {
@@ -22195,57 +22922,57 @@
                         } = yield e.read(l, s, l.byteLength - s, r));
                         return l
                     }
                     return null
                 }))
             }
             readAt(t, e) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     this._pending && (yield this._pending);
                     const {
                         _handle: n,
                         size: i
                     } = this;
                     if (n && t + e < i) {
                         const r = Math.min(i, t + e),
                             s = new Uint8Array(r - t);
                         return (yield n.read(s, 0, e, t)).buffer
                     }
                     return new Uint8Array(e)
                 }))
             }
             close() {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     const t = this._handle;
                     this._handle = null, t && (yield t.close())
                 }))
             }
             throw (t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     return yield this.close(), {
                         done: !0,
                         value: t
                     }
                 }))
             }
             return (t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     return yield this.close(), {
                         done: !0,
                         value: t
                     }
                 }))
             }
         }
 
-        function td(t) {
+        function Xd(t) {
             return t < 0 && (t = 4294967295 + t + 1), "0x".concat(t.toString(16))
         }
-        const ed = [1, 10, 100, 1e3, 1e4, 1e5, 1e6, 1e7, 1e8];
-        class nd {
+        const qd = [1, 10, 100, 1e3, 1e4, 1e5, 1e6, 1e7, 1e8];
+        class Qd {
             constructor(t) {
                 this.buffer = t
             }
             high() {
                 return this.buffer[1]
             }
             low() {
@@ -22269,57 +22996,57 @@
             equals(t) {
                 return this.buffer[1] === t.buffer[1] && this.buffer[0] == t.buffer[0]
             }
             greaterThan(t) {
                 return t.lessThan(this)
             }
             hex() {
-                return "".concat(td(this.buffer[1]), " ").concat(td(this.buffer[0]))
+                return "".concat(Xd(this.buffer[1]), " ").concat(Xd(this.buffer[0]))
             }
         }
-        class id extends nd {
+        class Zd extends Qd {
             times(t) {
                 return this._times(t), this
             }
             plus(t) {
                 return this._plus(t), this
             }
             static from(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(2);
-                return id.fromString("string" === typeof t ? t : t.toString(), e)
+                return Zd.fromString("string" === typeof t ? t : t.toString(), e)
             }
             static fromNumber(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(2);
-                return id.fromString(t.toString(), e)
+                return Zd.fromString(t.toString(), e)
             }
             static fromString(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(2);
                 const n = t.length,
-                    i = new id(e);
+                    i = new Zd(e);
                 for (let r = 0; r < n;) {
                     const e = 8 < n - r ? 8 : n - r,
-                        s = new id(new Uint32Array([Number.parseInt(t.slice(r, r + e), 10), 0])),
-                        o = new id(new Uint32Array([ed[e], 0]));
+                        s = new Zd(new Uint32Array([Number.parseInt(t.slice(r, r + e), 10), 0])),
+                        o = new Zd(new Uint32Array([qd[e], 0]));
                     i.times(o), i.plus(s), r += e
                 }
                 return i
             }
             static convertArray(t) {
                 const e = new Uint32Array(2 * t.length);
-                for (let n = -1, i = t.length; ++n < i;) id.from(t[n], new Uint32Array(e.buffer, e.byteOffset + 2 * n * 4, 2));
+                for (let n = -1, i = t.length; ++n < i;) Zd.from(t[n], new Uint32Array(e.buffer, e.byteOffset + 2 * n * 4, 2));
                 return e
             }
             static multiply(t, e) {
-                return new id(new Uint32Array(t.buffer)).times(e)
+                return new Zd(new Uint32Array(t.buffer)).times(e)
             }
             static add(t, e) {
-                return new id(new Uint32Array(t.buffer)).plus(e)
+                return new Zd(new Uint32Array(t.buffer)).plus(e)
             }
         }
-        class rd extends nd {
+        class Gd extends Qd {
             negate() {
                 return this.buffer[0] = 1 + ~this.buffer[0], this.buffer[1] = ~this.buffer[1], 0 == this.buffer[0] && ++this.buffer[1], this
             }
             times(t) {
                 return this._times(t), this
             }
             plus(t) {
@@ -22328,366 +23055,366 @@
             lessThan(t) {
                 const e = this.buffer[1] | 0,
                     n = t.buffer[1] | 0;
                 return e < n || e === n && this.buffer[0] < t.buffer[0]
             }
             static from(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(2);
-                return rd.fromString("string" === typeof t ? t : t.toString(), e)
+                return Gd.fromString("string" === typeof t ? t : t.toString(), e)
             }
             static fromNumber(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(2);
-                return rd.fromString(t.toString(), e)
+                return Gd.fromString(t.toString(), e)
             }
             static fromString(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(2);
                 const n = t.startsWith("-"),
                     i = t.length,
-                    r = new rd(e);
+                    r = new Gd(e);
                 for (let s = n ? 1 : 0; s < i;) {
                     const e = 8 < i - s ? 8 : i - s,
-                        n = new rd(new Uint32Array([Number.parseInt(t.slice(s, s + e), 10), 0])),
-                        o = new rd(new Uint32Array([ed[e], 0]));
+                        n = new Gd(new Uint32Array([Number.parseInt(t.slice(s, s + e), 10), 0])),
+                        o = new Gd(new Uint32Array([qd[e], 0]));
                     r.times(o), r.plus(n), s += e
                 }
                 return n ? r.negate() : r
             }
             static convertArray(t) {
                 const e = new Uint32Array(2 * t.length);
-                for (let n = -1, i = t.length; ++n < i;) rd.from(t[n], new Uint32Array(e.buffer, e.byteOffset + 2 * n * 4, 2));
+                for (let n = -1, i = t.length; ++n < i;) Gd.from(t[n], new Uint32Array(e.buffer, e.byteOffset + 2 * n * 4, 2));
                 return e
             }
             static multiply(t, e) {
-                return new rd(new Uint32Array(t.buffer)).times(e)
+                return new Gd(new Uint32Array(t.buffer)).times(e)
             }
             static add(t, e) {
-                return new rd(new Uint32Array(t.buffer)).plus(e)
+                return new Gd(new Uint32Array(t.buffer)).plus(e)
             }
         }
-        class sd {
+        class Jd {
             constructor(t) {
                 this.buffer = t
             }
             high() {
-                return new rd(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2))
+                return new Gd(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2))
             }
             low() {
-                return new rd(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset, 2))
+                return new Gd(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset, 2))
             }
             negate() {
                 return this.buffer[0] = 1 + ~this.buffer[0], this.buffer[1] = ~this.buffer[1], this.buffer[2] = ~this.buffer[2], this.buffer[3] = ~this.buffer[3], 0 == this.buffer[0] && ++this.buffer[1], 0 == this.buffer[1] && ++this.buffer[2], 0 == this.buffer[2] && ++this.buffer[3], this
             }
             times(t) {
-                const e = new id(new Uint32Array([this.buffer[3], 0])),
-                    n = new id(new Uint32Array([this.buffer[2], 0])),
-                    i = new id(new Uint32Array([this.buffer[1], 0])),
-                    r = new id(new Uint32Array([this.buffer[0], 0])),
-                    s = new id(new Uint32Array([t.buffer[3], 0])),
-                    o = new id(new Uint32Array([t.buffer[2], 0])),
-                    a = new id(new Uint32Array([t.buffer[1], 0])),
-                    l = new id(new Uint32Array([t.buffer[0], 0]));
-                let c = id.multiply(r, l);
+                const e = new Zd(new Uint32Array([this.buffer[3], 0])),
+                    n = new Zd(new Uint32Array([this.buffer[2], 0])),
+                    i = new Zd(new Uint32Array([this.buffer[1], 0])),
+                    r = new Zd(new Uint32Array([this.buffer[0], 0])),
+                    s = new Zd(new Uint32Array([t.buffer[3], 0])),
+                    o = new Zd(new Uint32Array([t.buffer[2], 0])),
+                    a = new Zd(new Uint32Array([t.buffer[1], 0])),
+                    l = new Zd(new Uint32Array([t.buffer[0], 0]));
+                let c = Zd.multiply(r, l);
                 this.buffer[0] = c.low();
-                const u = new id(new Uint32Array([c.high(), 0]));
-                c = id.multiply(i, l), u.plus(c), c = id.multiply(r, a), u.plus(c), this.buffer[1] = u.low(), this.buffer[3] = u.lessThan(c) ? 1 : 0, this.buffer[2] = u.high();
-                return new id(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2)).plus(id.multiply(n, l)).plus(id.multiply(i, a)).plus(id.multiply(r, o)), this.buffer[3] += id.multiply(e, l).plus(id.multiply(n, a)).plus(id.multiply(i, o)).plus(id.multiply(r, s)).low(), this
+                const u = new Zd(new Uint32Array([c.high(), 0]));
+                c = Zd.multiply(i, l), u.plus(c), c = Zd.multiply(r, a), u.plus(c), this.buffer[1] = u.low(), this.buffer[3] = u.lessThan(c) ? 1 : 0, this.buffer[2] = u.high();
+                return new Zd(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2)).plus(Zd.multiply(n, l)).plus(Zd.multiply(i, a)).plus(Zd.multiply(r, o)), this.buffer[3] += Zd.multiply(e, l).plus(Zd.multiply(n, a)).plus(Zd.multiply(i, o)).plus(Zd.multiply(r, s)).low(), this
             }
             plus(t) {
                 const e = new Uint32Array(4);
                 return e[3] = this.buffer[3] + t.buffer[3] >>> 0, e[2] = this.buffer[2] + t.buffer[2] >>> 0, e[1] = this.buffer[1] + t.buffer[1] >>> 0, e[0] = this.buffer[0] + t.buffer[0] >>> 0, e[0] < this.buffer[0] >>> 0 && ++e[1], e[1] < this.buffer[1] >>> 0 && ++e[2], e[2] < this.buffer[2] >>> 0 && ++e[3], this.buffer[3] = e[3], this.buffer[2] = e[2], this.buffer[1] = e[1], this.buffer[0] = e[0], this
             }
             hex() {
-                return "".concat(td(this.buffer[3]), " ").concat(td(this.buffer[2]), " ").concat(td(this.buffer[1]), " ").concat(td(this.buffer[0]))
+                return "".concat(Xd(this.buffer[3]), " ").concat(Xd(this.buffer[2]), " ").concat(Xd(this.buffer[1]), " ").concat(Xd(this.buffer[0]))
             }
             static multiply(t, e) {
-                return new sd(new Uint32Array(t.buffer)).times(e)
+                return new Jd(new Uint32Array(t.buffer)).times(e)
             }
             static add(t, e) {
-                return new sd(new Uint32Array(t.buffer)).plus(e)
+                return new Jd(new Uint32Array(t.buffer)).plus(e)
             }
             static from(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(4);
-                return sd.fromString("string" === typeof t ? t : t.toString(), e)
+                return Jd.fromString("string" === typeof t ? t : t.toString(), e)
             }
             static fromNumber(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(4);
-                return sd.fromString(t.toString(), e)
+                return Jd.fromString(t.toString(), e)
             }
             static fromString(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(4);
                 const n = t.startsWith("-"),
                     i = t.length,
-                    r = new sd(e);
+                    r = new Jd(e);
                 for (let s = n ? 1 : 0; s < i;) {
                     const e = 8 < i - s ? 8 : i - s,
-                        n = new sd(new Uint32Array([Number.parseInt(t.slice(s, s + e), 10), 0, 0, 0])),
-                        o = new sd(new Uint32Array([ed[e], 0, 0, 0]));
+                        n = new Jd(new Uint32Array([Number.parseInt(t.slice(s, s + e), 10), 0, 0, 0])),
+                        o = new Jd(new Uint32Array([qd[e], 0, 0, 0]));
                     r.times(o), r.plus(n), s += e
                 }
                 return n ? r.negate() : r
             }
             static convertArray(t) {
                 const e = new Uint32Array(4 * t.length);
-                for (let n = -1, i = t.length; ++n < i;) sd.from(t[n], new Uint32Array(e.buffer, e.byteOffset + 16 * n, 4));
+                for (let n = -1, i = t.length; ++n < i;) Jd.from(t[n], new Uint32Array(e.buffer, e.byteOffset + 16 * n, 4));
                 return e
             }
         }
-        class od extends Xl {
+        class tf extends jc {
             constructor(t, e, n, i) {
                 super(), this.nodesIndex = -1, this.buffersIndex = -1, this.bytes = t, this.nodes = e, this.buffers = n, this.dictionaries = i
             }
             visit(t) {
-                return super.visit(t instanceof Hu ? t.type : t)
+                return super.visit(t instanceof Rh ? t.type : t)
             }
             visitNull(t) {
                 let {
                     length: e
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e
                 })
             }
             visitBool(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     data: this.readData(t)
                 })
             }
             visitInt(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     data: this.readData(t)
                 })
             }
             visitFloat(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     data: this.readData(t)
                 })
             }
             visitUtf8(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     valueOffsets: this.readOffsets(t),
                     data: this.readData(t)
                 })
             }
             visitBinary(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     valueOffsets: this.readOffsets(t),
                     data: this.readData(t)
                 })
             }
             visitFixedSizeBinary(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     data: this.readData(t)
                 })
             }
             visitDate(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     data: this.readData(t)
                 })
             }
             visitTimestamp(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     data: this.readData(t)
                 })
             }
             visitTime(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     data: this.readData(t)
                 })
             }
             visitDecimal(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     data: this.readData(t)
                 })
             }
             visitList(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     valueOffsets: this.readOffsets(t),
                     child: this.visit(t.children[0])
                 })
             }
             visitStruct(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     children: this.visitMany(t.children)
                 })
             }
             visitUnion(t) {
-                return t.mode === Zo.Sparse ? this.visitSparseUnion(t) : this.visitDenseUnion(t)
+                return t.mode === Ya.Sparse ? this.visitSparseUnion(t) : this.visitDenseUnion(t)
             }
             visitDenseUnion(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     typeIds: this.readTypeIds(t),
                     valueOffsets: this.readOffsets(t),
                     children: this.visitMany(t.children)
                 })
             }
             visitSparseUnion(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     typeIds: this.readTypeIds(t),
                     children: this.visitMany(t.children)
                 })
             }
             visitDictionary(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     data: this.readData(t.indices),
                     dictionary: this.readDictionary(t)
                 })
             }
             visitInterval(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     data: this.readData(t)
                 })
             }
             visitFixedSizeList(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     child: this.visit(t.children[0])
                 })
             }
             visitMap(t) {
                 let {
                     length: e,
                     nullCount: n
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode();
-                return ju({
+                return Nh({
                     type: t,
                     length: e,
                     nullCount: n,
                     nullBitmap: this.readNullBitmap(t, n),
                     valueOffsets: this.readOffsets(t),
                     child: this.visit(t.children[0])
                 })
@@ -22715,96 +23442,96 @@
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange();
                 return this.bytes.subarray(n, n + e)
             }
             readDictionary(t) {
                 return this.dictionaries.get(t.id)
             }
         }
-        class ad extends od {
+        class ef extends tf {
             constructor(t, e, n, i) {
                 super(new Uint8Array(0), e, n, i), this.sources = t
             }
             readNullBitmap(t, e) {
                 let {
                     offset: n
                 } = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : this.nextBufferRange();
-                return e <= 0 ? new Uint8Array(0) : bu(this.sources[n])
+                return e <= 0 ? new Uint8Array(0) : dh(this.sources[n])
             }
             readOffsets(t) {
                 let {
                     offset: e
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange();
-                return ja(Uint8Array, ja(Int32Array, this.sources[e]))
+                return Nl(Uint8Array, Nl(Int32Array, this.sources[e]))
             }
             readTypeIds(t) {
                 let {
                     offset: e
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange();
-                return ja(Uint8Array, ja(t.ArrayType, this.sources[e]))
+                return Nl(Uint8Array, Nl(t.ArrayType, this.sources[e]))
             }
             readData(t) {
                 let {
                     offset: e
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange();
                 const {
                     sources: n
                 } = this;
-                return kl.isTimestamp(t) || (kl.isInt(t) || kl.isTime(t)) && 64 === t.bitWidth || kl.isDate(t) && t.unit === Jo.MILLISECOND ? ja(Uint8Array, rd.convertArray(n[e])) : kl.isDecimal(t) ? ja(Uint8Array, sd.convertArray(n[e])) : kl.isBinary(t) || kl.isFixedSizeBinary(t) ? function(t) {
+                return vc.isTimestamp(t) || (vc.isInt(t) || vc.isTime(t)) && 64 === t.bitWidth || vc.isDate(t) && t.unit === Ka.MILLISECOND ? Nl(Uint8Array, Gd.convertArray(n[e])) : vc.isDecimal(t) ? Nl(Uint8Array, Jd.convertArray(n[e])) : vc.isBinary(t) || vc.isFixedSizeBinary(t) ? function(t) {
                     const e = t.join(""),
                         n = new Uint8Array(e.length / 2);
                     for (let i = 0; i < e.length; i += 2) n[i >> 1] = Number.parseInt(e.slice(i, i + 2), 16);
                     return n
-                }(n[e]) : kl.isBool(t) ? bu(n[e]) : kl.isUtf8(t) ? Ra(n[e].join("")) : ja(Uint8Array, ja(t.ArrayType, n[e].map((t => +t))))
+                }(n[e]) : vc.isBool(t) ? dh(n[e]) : vc.isUtf8(t) ? Cl(n[e].join("")) : Nl(Uint8Array, Nl(t.ArrayType, n[e].map((t => +t))))
             }
         }
-        var ld, cd, ud, hd, dd, fd, pd, gd;
+        var nf, rf, sf, of, af, lf, cf, uf;
         ! function(t) {
             t[t.BUFFER = 0] = "BUFFER"
-        }(ld || (ld = {})),
+        }(nf || (nf = {})),
         function(t) {
             t[t.LZ4_FRAME = 0] = "LZ4_FRAME", t[t.ZSTD = 1] = "ZSTD"
-        }(cd || (cd = {}));
-        class md {
+        }(rf || (rf = {}));
+        class hf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsBodyCompression(t, e) {
-                return (e || new md).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new hf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsBodyCompression(t, e) {
-                return t.setPosition(t.position() + 4), (e || new md).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new hf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             codec() {
                 const t = this.bb.__offset(this.bb_pos, 4);
-                return t ? this.bb.readInt8(this.bb_pos + t) : cd.LZ4_FRAME
+                return t ? this.bb.readInt8(this.bb_pos + t) : rf.LZ4_FRAME
             }
             method() {
                 const t = this.bb.__offset(this.bb_pos, 6);
-                return t ? this.bb.readInt8(this.bb_pos + t) : ld.BUFFER
+                return t ? this.bb.readInt8(this.bb_pos + t) : nf.BUFFER
             }
             static startBodyCompression(t) {
                 t.startObject(2)
             }
             static addCodec(t, e) {
-                t.addFieldInt8(0, e, cd.LZ4_FRAME)
+                t.addFieldInt8(0, e, rf.LZ4_FRAME)
             }
             static addMethod(t, e) {
-                t.addFieldInt8(1, e, ld.BUFFER)
+                t.addFieldInt8(1, e, nf.BUFFER)
             }
             static endBodyCompression(t) {
                 return t.endObject()
             }
             static createBodyCompression(t, e, n) {
-                return md.startBodyCompression(t), md.addCodec(t, e), md.addMethod(t, n), md.endBodyCompression(t)
+                return hf.startBodyCompression(t), hf.addCodec(t, e), hf.addMethod(t, n), hf.endBodyCompression(t)
             }
         }
-        class yd {
+        class df {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             offset() {
@@ -22816,15 +23543,15 @@
             static sizeOf() {
                 return 16
             }
             static createBuffer(t, e, n) {
                 return t.prep(8, 16), t.writeInt64(n), t.writeInt64(e), t.offset()
             }
         }
-        class bd {
+        class ff {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             length() {
@@ -22836,50 +23563,50 @@
             static sizeOf() {
                 return 16
             }
             static createFieldNode(t, e, n) {
                 return t.prep(8, 16), t.writeInt64(n), t.writeInt64(e), t.offset()
             }
         }
-        class vd {
+        class pf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsRecordBatch(t, e) {
-                return (e || new vd).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new pf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsRecordBatch(t, e) {
-                return t.setPosition(t.position() + 4), (e || new vd).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new pf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             length() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return t ? this.bb.readInt64(this.bb_pos + t) : this.bb.createLong(0, 0)
             }
             nodes(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 6);
-                return n ? (e || new bd).__init(this.bb.__vector(this.bb_pos + n) + 16 * t, this.bb) : null
+                return n ? (e || new ff).__init(this.bb.__vector(this.bb_pos + n) + 16 * t, this.bb) : null
             }
             nodesLength() {
                 const t = this.bb.__offset(this.bb_pos, 6);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             buffers(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 8);
-                return n ? (e || new yd).__init(this.bb.__vector(this.bb_pos + n) + 16 * t, this.bb) : null
+                return n ? (e || new df).__init(this.bb.__vector(this.bb_pos + n) + 16 * t, this.bb) : null
             }
             buffersLength() {
                 const t = this.bb.__offset(this.bb_pos, 8);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             compression(t) {
                 const e = this.bb.__offset(this.bb_pos, 10);
-                return e ? (t || new md).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
+                return e ? (t || new hf).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
             }
             static startRecordBatch(t) {
                 t.startObject(4)
             }
             static addLength(t, e) {
                 t.addFieldInt64(0, e, t.createLong(0, 0))
             }
@@ -22898,34 +23625,34 @@
             static addCompression(t, e) {
                 t.addFieldOffset(3, e, 0)
             }
             static endRecordBatch(t) {
                 return t.endObject()
             }
         }
-        class _d {
+        class gf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsDictionaryBatch(t, e) {
-                return (e || new _d).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new gf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsDictionaryBatch(t, e) {
-                return t.setPosition(t.position() + 4), (e || new _d).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new gf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             id() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return t ? this.bb.readInt64(this.bb_pos + t) : this.bb.createLong(0, 0)
             }
             data(t) {
                 const e = this.bb.__offset(this.bb_pos, 6);
-                return e ? (t || new vd).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
+                return e ? (t || new pf).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
             }
             isDelta() {
                 const t = this.bb.__offset(this.bb_pos, 8);
                 return !!t && !!this.bb.readInt8(this.bb_pos + t)
             }
             static startDictionaryBatch(t) {
                 t.startObject(3)
@@ -22940,57 +23667,57 @@
                 t.addFieldInt8(2, +e, 0)
             }
             static endDictionaryBatch(t) {
                 return t.endObject()
             }
         }! function(t) {
             t[t.HALF = 0] = "HALF", t[t.SINGLE = 1] = "SINGLE", t[t.DOUBLE = 2] = "DOUBLE"
-        }(ud || (ud = {}));
-        class xd {
+        }(sf || (sf = {}));
+        class mf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsFloatingPoint(t, e) {
-                return (e || new xd).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new mf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsFloatingPoint(t, e) {
-                return t.setPosition(t.position() + 4), (e || new xd).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new mf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             precision() {
                 const t = this.bb.__offset(this.bb_pos, 4);
-                return t ? this.bb.readInt16(this.bb_pos + t) : ud.HALF
+                return t ? this.bb.readInt16(this.bb_pos + t) : sf.HALF
             }
             static startFloatingPoint(t) {
                 t.startObject(1)
             }
             static addPrecision(t, e) {
-                t.addFieldInt16(0, e, ud.HALF)
+                t.addFieldInt16(0, e, sf.HALF)
             }
             static endFloatingPoint(t) {
                 return t.endObject()
             }
             static createFloatingPoint(t, e) {
-                return xd.startFloatingPoint(t), xd.addPrecision(t, e), xd.endFloatingPoint(t)
+                return mf.startFloatingPoint(t), mf.addPrecision(t, e), mf.endFloatingPoint(t)
             }
         }
-        class wd {
+        class yf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsDecimal(t, e) {
-                return (e || new wd).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new yf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsDecimal(t, e) {
-                return t.setPosition(t.position() + 4), (e || new wd).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new yf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             precision() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return t ? this.bb.readInt32(this.bb_pos + t) : 0
             }
             scale() {
                 const t = this.bb.__offset(this.bb_pos, 6);
@@ -23012,175 +23739,175 @@
             static addBitWidth(t, e) {
                 t.addFieldInt32(2, e, 128)
             }
             static endDecimal(t) {
                 return t.endObject()
             }
             static createDecimal(t, e, n, i) {
-                return wd.startDecimal(t), wd.addPrecision(t, e), wd.addScale(t, n), wd.addBitWidth(t, i), wd.endDecimal(t)
+                return yf.startDecimal(t), yf.addPrecision(t, e), yf.addScale(t, n), yf.addBitWidth(t, i), yf.endDecimal(t)
             }
         }! function(t) {
             t[t.DAY = 0] = "DAY", t[t.MILLISECOND = 1] = "MILLISECOND"
-        }(hd || (hd = {}));
-        class Sd {
+        }(of || (of = {}));
+        class bf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsDate(t, e) {
-                return (e || new Sd).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new bf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsDate(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Sd).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new bf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             unit() {
                 const t = this.bb.__offset(this.bb_pos, 4);
-                return t ? this.bb.readInt16(this.bb_pos + t) : hd.MILLISECOND
+                return t ? this.bb.readInt16(this.bb_pos + t) : of.MILLISECOND
             }
             static startDate(t) {
                 t.startObject(1)
             }
             static addUnit(t, e) {
-                t.addFieldInt16(0, e, hd.MILLISECOND)
+                t.addFieldInt16(0, e, of.MILLISECOND)
             }
             static endDate(t) {
                 return t.endObject()
             }
             static createDate(t, e) {
-                return Sd.startDate(t), Sd.addUnit(t, e), Sd.endDate(t)
+                return bf.startDate(t), bf.addUnit(t, e), bf.endDate(t)
             }
         }! function(t) {
             t[t.SECOND = 0] = "SECOND", t[t.MILLISECOND = 1] = "MILLISECOND", t[t.MICROSECOND = 2] = "MICROSECOND", t[t.NANOSECOND = 3] = "NANOSECOND"
-        }(dd || (dd = {}));
-        class Td {
+        }(af || (af = {}));
+        class vf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsTime(t, e) {
-                return (e || new Td).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new vf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsTime(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Td).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new vf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             unit() {
                 const t = this.bb.__offset(this.bb_pos, 4);
-                return t ? this.bb.readInt16(this.bb_pos + t) : dd.MILLISECOND
+                return t ? this.bb.readInt16(this.bb_pos + t) : af.MILLISECOND
             }
             bitWidth() {
                 const t = this.bb.__offset(this.bb_pos, 6);
                 return t ? this.bb.readInt32(this.bb_pos + t) : 32
             }
             static startTime(t) {
                 t.startObject(2)
             }
             static addUnit(t, e) {
-                t.addFieldInt16(0, e, dd.MILLISECOND)
+                t.addFieldInt16(0, e, af.MILLISECOND)
             }
             static addBitWidth(t, e) {
                 t.addFieldInt32(1, e, 32)
             }
             static endTime(t) {
                 return t.endObject()
             }
             static createTime(t, e, n) {
-                return Td.startTime(t), Td.addUnit(t, e), Td.addBitWidth(t, n), Td.endTime(t)
+                return vf.startTime(t), vf.addUnit(t, e), vf.addBitWidth(t, n), vf.endTime(t)
             }
         }
-        class kd {
+        class _f {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsTimestamp(t, e) {
-                return (e || new kd).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new _f).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsTimestamp(t, e) {
-                return t.setPosition(t.position() + 4), (e || new kd).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new _f).__init(t.readInt32(t.position()) + t.position(), t)
             }
             unit() {
                 const t = this.bb.__offset(this.bb_pos, 4);
-                return t ? this.bb.readInt16(this.bb_pos + t) : dd.SECOND
+                return t ? this.bb.readInt16(this.bb_pos + t) : af.SECOND
             }
             timezone(t) {
                 const e = this.bb.__offset(this.bb_pos, 6);
                 return e ? this.bb.__string(this.bb_pos + e, t) : null
             }
             static startTimestamp(t) {
                 t.startObject(2)
             }
             static addUnit(t, e) {
-                t.addFieldInt16(0, e, dd.SECOND)
+                t.addFieldInt16(0, e, af.SECOND)
             }
             static addTimezone(t, e) {
                 t.addFieldOffset(1, e, 0)
             }
             static endTimestamp(t) {
                 return t.endObject()
             }
             static createTimestamp(t, e, n) {
-                return kd.startTimestamp(t), kd.addUnit(t, e), kd.addTimezone(t, n), kd.endTimestamp(t)
+                return _f.startTimestamp(t), _f.addUnit(t, e), _f.addTimezone(t, n), _f.endTimestamp(t)
             }
         }! function(t) {
             t[t.YEAR_MONTH = 0] = "YEAR_MONTH", t[t.DAY_TIME = 1] = "DAY_TIME", t[t.MONTH_DAY_NANO = 2] = "MONTH_DAY_NANO"
-        }(fd || (fd = {}));
-        class Md {
+        }(lf || (lf = {}));
+        class xf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsInterval(t, e) {
-                return (e || new Md).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new xf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsInterval(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Md).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new xf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             unit() {
                 const t = this.bb.__offset(this.bb_pos, 4);
-                return t ? this.bb.readInt16(this.bb_pos + t) : fd.YEAR_MONTH
+                return t ? this.bb.readInt16(this.bb_pos + t) : lf.YEAR_MONTH
             }
             static startInterval(t) {
                 t.startObject(1)
             }
             static addUnit(t, e) {
-                t.addFieldInt16(0, e, fd.YEAR_MONTH)
+                t.addFieldInt16(0, e, lf.YEAR_MONTH)
             }
             static endInterval(t) {
                 return t.endObject()
             }
             static createInterval(t, e) {
-                return Md.startInterval(t), Md.addUnit(t, e), Md.endInterval(t)
+                return xf.startInterval(t), xf.addUnit(t, e), xf.endInterval(t)
             }
         }! function(t) {
             t[t.Sparse = 0] = "Sparse", t[t.Dense = 1] = "Dense"
-        }(pd || (pd = {}));
-        class Id {
+        }(cf || (cf = {}));
+        class wf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsUnion(t, e) {
-                return (e || new Id).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new wf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsUnion(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Id).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new wf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             mode() {
                 const t = this.bb.__offset(this.bb_pos, 4);
-                return t ? this.bb.readInt16(this.bb_pos + t) : pd.Sparse
+                return t ? this.bb.readInt16(this.bb_pos + t) : cf.Sparse
             }
             typeIds(t) {
                 const e = this.bb.__offset(this.bb_pos, 6);
                 return e ? this.bb.readInt32(this.bb.__vector(this.bb_pos + e) + 4 * t) : 0
             }
             typeIdsLength() {
                 const t = this.bb.__offset(this.bb_pos, 6);
@@ -23190,15 +23917,15 @@
                 const t = this.bb.__offset(this.bb_pos, 6);
                 return t ? new Int32Array(this.bb.bytes().buffer, this.bb.bytes().byteOffset + this.bb.__vector(this.bb_pos + t), this.bb.__vector_len(this.bb_pos + t)) : null
             }
             static startUnion(t) {
                 t.startObject(2)
             }
             static addMode(t, e) {
-                t.addFieldInt16(0, e, pd.Sparse)
+                t.addFieldInt16(0, e, cf.Sparse)
             }
             static addTypeIds(t, e) {
                 t.addFieldOffset(1, e, 0)
             }
             static createTypeIdsVector(t, e) {
                 t.startVector(4, e.length, 4);
                 for (let n = e.length - 1; n >= 0; n--) t.addInt32(e[n]);
@@ -23207,29 +23934,29 @@
             static startTypeIdsVector(t, e) {
                 t.startVector(4, e, 4)
             }
             static endUnion(t) {
                 return t.endObject()
             }
             static createUnion(t, e, n) {
-                return Id.startUnion(t), Id.addMode(t, e), Id.addTypeIds(t, n), Id.endUnion(t)
+                return wf.startUnion(t), wf.addMode(t, e), wf.addTypeIds(t, n), wf.endUnion(t)
             }
         }
-        class Ed {
+        class Sf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsFixedSizeBinary(t, e) {
-                return (e || new Ed).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Sf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsFixedSizeBinary(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Ed).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Sf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             byteWidth() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return t ? this.bb.readInt32(this.bb_pos + t) : 0
             }
             static startFixedSizeBinary(t) {
                 t.startObject(1)
@@ -23237,29 +23964,29 @@
             static addByteWidth(t, e) {
                 t.addFieldInt32(0, e, 0)
             }
             static endFixedSizeBinary(t) {
                 return t.endObject()
             }
             static createFixedSizeBinary(t, e) {
-                return Ed.startFixedSizeBinary(t), Ed.addByteWidth(t, e), Ed.endFixedSizeBinary(t)
+                return Sf.startFixedSizeBinary(t), Sf.addByteWidth(t, e), Sf.endFixedSizeBinary(t)
             }
         }
-        class Od {
+        class Tf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsFixedSizeList(t, e) {
-                return (e || new Od).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Tf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsFixedSizeList(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Od).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Tf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             listSize() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return t ? this.bb.readInt32(this.bb_pos + t) : 0
             }
             static startFixedSizeList(t) {
                 t.startObject(1)
@@ -23267,29 +23994,29 @@
             static addListSize(t, e) {
                 t.addFieldInt32(0, e, 0)
             }
             static endFixedSizeList(t) {
                 return t.endObject()
             }
             static createFixedSizeList(t, e) {
-                return Od.startFixedSizeList(t), Od.addListSize(t, e), Od.endFixedSizeList(t)
+                return Tf.startFixedSizeList(t), Tf.addListSize(t, e), Tf.endFixedSizeList(t)
             }
         }
-        class Dd {
+        class kf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsMap(t, e) {
-                return (e || new Dd).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new kf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsMap(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Dd).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new kf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             keysSorted() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return !!t && !!this.bb.readInt8(this.bb_pos + t)
             }
             static startMap(t) {
                 t.startObject(1)
@@ -23297,64 +24024,64 @@
             static addKeysSorted(t, e) {
                 t.addFieldInt8(0, +e, 0)
             }
             static endMap(t) {
                 return t.endObject()
             }
             static createMap(t, e) {
-                return Dd.startMap(t), Dd.addKeysSorted(t, e), Dd.endMap(t)
+                return kf.startMap(t), kf.addKeysSorted(t, e), kf.endMap(t)
             }
         }! function(t) {
             t[t.NONE = 0] = "NONE", t[t.Schema = 1] = "Schema", t[t.DictionaryBatch = 2] = "DictionaryBatch", t[t.RecordBatch = 3] = "RecordBatch", t[t.Tensor = 4] = "Tensor", t[t.SparseTensor = 5] = "SparseTensor"
-        }(gd || (gd = {}));
-        class Ad {
+        }(uf || (uf = {}));
+        class Mf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsMessage(t, e) {
-                return (e || new Ad).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Mf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsMessage(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Ad).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Mf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             version() {
                 const t = this.bb.__offset(this.bb_pos, 4);
-                return t ? this.bb.readInt16(this.bb_pos + t) : xh.V1
+                return t ? this.bb.readInt16(this.bb_pos + t) : gd.V1
             }
             headerType() {
                 const t = this.bb.__offset(this.bb_pos, 6);
-                return t ? this.bb.readUint8(this.bb_pos + t) : gd.NONE
+                return t ? this.bb.readUint8(this.bb_pos + t) : uf.NONE
             }
             header(t) {
                 const e = this.bb.__offset(this.bb_pos, 8);
                 return e ? this.bb.__union(t, this.bb_pos + e) : null
             }
             bodyLength() {
                 const t = this.bb.__offset(this.bb_pos, 10);
                 return t ? this.bb.readInt64(this.bb_pos + t) : this.bb.createLong(0, 0)
             }
             customMetadata(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 12);
-                return n ? (e || new Ih).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
+                return n ? (e || new xd).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
             }
             customMetadataLength() {
                 const t = this.bb.__offset(this.bb_pos, 12);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             static startMessage(t) {
                 t.startObject(5)
             }
             static addVersion(t, e) {
-                t.addFieldInt16(0, e, xh.V1)
+                t.addFieldInt16(0, e, gd.V1)
             }
             static addHeaderType(t, e) {
-                t.addFieldInt8(1, e, gd.NONE)
+                t.addFieldInt8(1, e, uf.NONE)
             }
             static addHeader(t, e) {
                 t.addFieldOffset(2, e, 0)
             }
             static addBodyLength(t, e) {
                 t.addFieldInt64(3, e, t.createLong(0, 0))
             }
@@ -23375,372 +24102,372 @@
             static finishMessageBuffer(t, e) {
                 t.finish(e)
             }
             static finishSizePrefixedMessageBuffer(t, e) {
                 t.finish(e, void 0, !0)
             }
             static createMessage(t, e, n, i, r, s) {
-                return Ad.startMessage(t), Ad.addVersion(t, e), Ad.addHeaderType(t, n), Ad.addHeader(t, i), Ad.addBodyLength(t, r), Ad.addCustomMetadata(t, s), Ad.endMessage(t)
+                return Mf.startMessage(t), Mf.addVersion(t, e), Mf.addHeaderType(t, n), Mf.addHeader(t, i), Mf.addBodyLength(t, r), Mf.addCustomMetadata(t, s), Mf.endMessage(t)
             }
         }
-        class Cd {
+        class If {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsNull(t, e) {
-                return (e || new Cd).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new If).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsNull(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Cd).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new If).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static startNull(t) {
                 t.startObject(0)
             }
             static endNull(t) {
                 return t.endObject()
             }
             static createNull(t) {
-                return Cd.startNull(t), Cd.endNull(t)
+                return If.startNull(t), If.endNull(t)
             }
         }
-        class Pd {
+        class Ef {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsBinary(t, e) {
-                return (e || new Pd).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Ef).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsBinary(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Pd).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Ef).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static startBinary(t) {
                 t.startObject(0)
             }
             static endBinary(t) {
                 return t.endObject()
             }
             static createBinary(t) {
-                return Pd.startBinary(t), Pd.endBinary(t)
+                return Ef.startBinary(t), Ef.endBinary(t)
             }
         }
-        class Fd {
+        class Of {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsBool(t, e) {
-                return (e || new Fd).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Of).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsBool(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Fd).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Of).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static startBool(t) {
                 t.startObject(0)
             }
             static endBool(t) {
                 return t.endObject()
             }
             static createBool(t) {
-                return Fd.startBool(t), Fd.endBool(t)
+                return Of.startBool(t), Of.endBool(t)
             }
         }
-        class Ld {
+        class Df {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsUtf8(t, e) {
-                return (e || new Ld).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Df).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsUtf8(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Ld).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Df).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static startUtf8(t) {
                 t.startObject(0)
             }
             static endUtf8(t) {
                 return t.endObject()
             }
             static createUtf8(t) {
-                return Ld.startUtf8(t), Ld.endUtf8(t)
+                return Df.startUtf8(t), Df.endUtf8(t)
             }
         }
-        class Nd {
+        class Af {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsList(t, e) {
-                return (e || new Nd).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Af).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsList(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Nd).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Af).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static startList(t) {
                 t.startObject(0)
             }
             static endList(t) {
                 return t.endObject()
             }
             static createList(t) {
-                return Nd.startList(t), Nd.endList(t)
+                return Af.startList(t), Af.endList(t)
             }
         }
-        class Bd {
+        class Cf {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsStruct_(t, e) {
-                return (e || new Bd).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Cf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsStruct_(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Bd).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Cf).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static startStruct_(t) {
                 t.startObject(0)
             }
             static endStruct_(t) {
                 return t.endObject()
             }
             static createStruct_(t) {
-                return Bd.startStruct_(t), Bd.endStruct_(t)
+                return Cf.startStruct_(t), Cf.endStruct_(t)
             }
         }
-        var Rd = vh;
-        const zd = new class extends Xl {
+        var Pf = fd;
+        const Ff = new class extends jc {
             visit(t, e) {
                 return null == t || null == e ? void 0 : super.visit(t, e)
             }
             visitNull(t, e) {
-                return Cd.startNull(e), Cd.endNull(e)
+                return If.startNull(e), If.endNull(e)
             }
             visitInt(t, e) {
-                return Eh.startInt(e), Eh.addBitWidth(e, t.bitWidth), Eh.addIsSigned(e, t.isSigned), Eh.endInt(e)
+                return wd.startInt(e), wd.addBitWidth(e, t.bitWidth), wd.addIsSigned(e, t.isSigned), wd.endInt(e)
             }
             visitFloat(t, e) {
-                return xd.startFloatingPoint(e), xd.addPrecision(e, t.precision), xd.endFloatingPoint(e)
+                return mf.startFloatingPoint(e), mf.addPrecision(e, t.precision), mf.endFloatingPoint(e)
             }
             visitBinary(t, e) {
-                return Pd.startBinary(e), Pd.endBinary(e)
+                return Ef.startBinary(e), Ef.endBinary(e)
             }
             visitBool(t, e) {
-                return Fd.startBool(e), Fd.endBool(e)
+                return Of.startBool(e), Of.endBool(e)
             }
             visitUtf8(t, e) {
-                return Ld.startUtf8(e), Ld.endUtf8(e)
+                return Df.startUtf8(e), Df.endUtf8(e)
             }
             visitDecimal(t, e) {
-                return wd.startDecimal(e), wd.addScale(e, t.scale), wd.addPrecision(e, t.precision), wd.addBitWidth(e, t.bitWidth), wd.endDecimal(e)
+                return yf.startDecimal(e), yf.addScale(e, t.scale), yf.addPrecision(e, t.precision), yf.addBitWidth(e, t.bitWidth), yf.endDecimal(e)
             }
             visitDate(t, e) {
-                return Sd.startDate(e), Sd.addUnit(e, t.unit), Sd.endDate(e)
+                return bf.startDate(e), bf.addUnit(e, t.unit), bf.endDate(e)
             }
             visitTime(t, e) {
-                return Td.startTime(e), Td.addUnit(e, t.unit), Td.addBitWidth(e, t.bitWidth), Td.endTime(e)
+                return vf.startTime(e), vf.addUnit(e, t.unit), vf.addBitWidth(e, t.bitWidth), vf.endTime(e)
             }
             visitTimestamp(t, e) {
                 const n = t.timezone && e.createString(t.timezone) || void 0;
-                return kd.startTimestamp(e), kd.addUnit(e, t.unit), void 0 !== n && kd.addTimezone(e, n), kd.endTimestamp(e)
+                return _f.startTimestamp(e), _f.addUnit(e, t.unit), void 0 !== n && _f.addTimezone(e, n), _f.endTimestamp(e)
             }
             visitInterval(t, e) {
-                return Md.startInterval(e), Md.addUnit(e, t.unit), Md.endInterval(e)
+                return xf.startInterval(e), xf.addUnit(e, t.unit), xf.endInterval(e)
             }
             visitList(t, e) {
-                return Nd.startList(e), Nd.endList(e)
+                return Af.startList(e), Af.endList(e)
             }
             visitStruct(t, e) {
-                return Bd.startStruct_(e), Bd.endStruct_(e)
+                return Cf.startStruct_(e), Cf.endStruct_(e)
             }
             visitUnion(t, e) {
-                Id.startTypeIdsVector(e, t.typeIds.length);
-                const n = Id.createTypeIdsVector(e, t.typeIds);
-                return Id.startUnion(e), Id.addMode(e, t.mode), Id.addTypeIds(e, n), Id.endUnion(e)
+                wf.startTypeIdsVector(e, t.typeIds.length);
+                const n = wf.createTypeIdsVector(e, t.typeIds);
+                return wf.startUnion(e), wf.addMode(e, t.mode), wf.addTypeIds(e, n), wf.endUnion(e)
             }
             visitDictionary(t, e) {
                 const n = this.visit(t.indices, e);
-                return Oh.startDictionaryEncoding(e), Oh.addId(e, new Rd(t.id, 0)), Oh.addIsOrdered(e, t.isOrdered), void 0 !== n && Oh.addIndexType(e, n), Oh.endDictionaryEncoding(e)
+                return Sd.startDictionaryEncoding(e), Sd.addId(e, new Pf(t.id, 0)), Sd.addIsOrdered(e, t.isOrdered), void 0 !== n && Sd.addIndexType(e, n), Sd.endDictionaryEncoding(e)
             }
             visitFixedSizeBinary(t, e) {
-                return Ed.startFixedSizeBinary(e), Ed.addByteWidth(e, t.byteWidth), Ed.endFixedSizeBinary(e)
+                return Sf.startFixedSizeBinary(e), Sf.addByteWidth(e, t.byteWidth), Sf.endFixedSizeBinary(e)
             }
             visitFixedSizeList(t, e) {
-                return Od.startFixedSizeList(e), Od.addListSize(e, t.listSize), Od.endFixedSizeList(e)
+                return Tf.startFixedSizeList(e), Tf.addListSize(e, t.listSize), Tf.endFixedSizeList(e)
             }
             visitMap(t, e) {
-                return Dd.startMap(e), Dd.addKeysSorted(e, t.keysSorted), Dd.endMap(e)
+                return kf.startMap(e), kf.addKeysSorted(e, t.keysSorted), kf.endMap(e)
             }
         };
 
-        function Ud(t) {
-            return new Zd(t.count, jd(t.columns), Wd(t.columns))
+        function Lf(t) {
+            return new $f(t.count, Bf(t.columns), Rf(t.columns))
         }
 
-        function Vd(t, e) {
-            return (t.children || []).filter(Boolean).map((t => Hu.fromJSON(t, e)))
+        function Nf(t, e) {
+            return (t.children || []).filter(Boolean).map((t => Rh.fromJSON(t, e)))
         }
 
-        function jd(t) {
+        function Bf(t) {
             return (t || []).reduce(((t, e) => {
-                return [...t, new tf(e.count, (n = e.VALIDITY, (n || []).reduce(((t, e) => t + +(0 === e)), 0))), ...jd(e.children)];
+                return [...t, new qf(e.count, (n = e.VALIDITY, (n || []).reduce(((t, e) => t + +(0 === e)), 0))), ...Bf(e.children)];
                 var n
             }), [])
         }
 
-        function Wd(t) {
+        function Rf(t) {
             let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : [];
             for (let n = -1, i = (t || []).length; ++n < i;) {
                 const i = t[n];
-                i.VALIDITY && e.push(new Jd(e.length, i.VALIDITY.length)), i.TYPE && e.push(new Jd(e.length, i.TYPE.length)), i.OFFSET && e.push(new Jd(e.length, i.OFFSET.length)), i.DATA && e.push(new Jd(e.length, i.DATA.length)), e = Wd(i.children, e)
+                i.VALIDITY && e.push(new Xf(e.length, i.VALIDITY.length)), i.TYPE && e.push(new Xf(e.length, i.TYPE.length)), i.OFFSET && e.push(new Xf(e.length, i.OFFSET.length)), i.DATA && e.push(new Xf(e.length, i.DATA.length)), e = Rf(i.children, e)
             }
             return e
         }
 
-        function Hd(t) {
+        function zf(t) {
             return new Map(Object.entries(t || {}))
         }
 
-        function Yd(t) {
-            return new Il(t.isSigned, t.bitWidth)
+        function Uf(t) {
+            return new xc(t.isSigned, t.bitWidth)
         }
 
-        function $d(t, e) {
+        function Vf(t, e) {
             const n = t.type.name;
             switch (n) {
                 case "NONE":
                 case "null":
-                    return new Ml;
+                    return new _c;
                 case "binary":
-                    return new Dl;
+                    return new Tc;
                 case "utf8":
-                    return new Al;
+                    return new kc;
                 case "bool":
-                    return new Cl;
+                    return new Mc;
                 case "list":
-                    return new Rl((e || [])[0]);
+                    return new Cc((e || [])[0]);
                 case "struct":
                 case "struct_":
-                    return new zl(e || [])
+                    return new Pc(e || [])
             }
             switch (n) {
                 case "int": {
                     const e = t.type;
-                    return new Il(e.isSigned, e.bitWidth)
+                    return new xc(e.isSigned, e.bitWidth)
                 }
                 case "floatingpoint": {
                     const e = t.type;
-                    return new Ol(Go[e.precision])
+                    return new Sc($a[e.precision])
                 }
                 case "decimal": {
                     const e = t.type;
-                    return new Pl(e.scale, e.precision, e.bitWidth)
+                    return new Ic(e.scale, e.precision, e.bitWidth)
                 }
                 case "date": {
                     const e = t.type;
-                    return new Fl(Jo[e.unit])
+                    return new Ec(Ka[e.unit])
                 }
                 case "time": {
                     const e = t.type;
-                    return new Ll(ta[e.unit], e.bitWidth)
+                    return new Oc(Xa[e.unit], e.bitWidth)
                 }
                 case "timestamp": {
                     const e = t.type;
-                    return new Nl(ta[e.unit], e.timezone)
+                    return new Dc(Xa[e.unit], e.timezone)
                 }
                 case "interval": {
                     const e = t.type;
-                    return new Bl(ea[e.unit])
+                    return new Ac(qa[e.unit])
                 }
                 case "union": {
                     const n = t.type;
-                    return new Ul(Zo[n.mode], n.typeIds || [], e || [])
+                    return new Fc(Ya[n.mode], n.typeIds || [], e || [])
                 }
                 case "fixedsizebinary": {
                     const e = t.type;
-                    return new Vl(e.byteWidth)
+                    return new Lc(e.byteWidth)
                 }
                 case "fixedsizelist": {
                     const n = t.type;
-                    return new jl(n.listSize, (e || [])[0])
+                    return new Nc(n.listSize, (e || [])[0])
                 }
                 case "map": {
                     const n = t.type;
-                    return new Wl((e || [])[0], n.keysSorted)
+                    return new Bc((e || [])[0], n.keysSorted)
                 }
             }
             throw new Error('Unrecognized type: "'.concat(n, '"'))
         }
-        var Kd = vh,
-            Xd = Mh,
-            qd = kh;
-        class Qd {
+        var jf = fd,
+            Wf = _d,
+            Hf = vd;
+        class Yf {
             constructor(t, e, n, i) {
                 this._version = e, this._headerType = n, this.body = new Uint8Array(0), i && (this._createHeader = () => i), this._bodyLength = "number" === typeof t ? t : t.low
             }
             static fromJSON(t, e) {
-                const n = new Qd(0, Qo.V4, e);
+                const n = new Yf(0, Ha.V4, e);
                 return n._createHeader = function(t, e) {
                     return () => {
                         switch (e) {
-                            case na.Schema:
-                                return Wu.fromJSON(t);
-                            case na.RecordBatch:
-                                return Zd.fromJSON(t);
-                            case na.DictionaryBatch:
-                                return Gd.fromJSON(t)
+                            case Qa.Schema:
+                                return Bh.fromJSON(t);
+                            case Qa.RecordBatch:
+                                return $f.fromJSON(t);
+                            case Qa.DictionaryBatch:
+                                return Kf.fromJSON(t)
                         }
-                        throw new Error("Unrecognized Message type: { name: ".concat(na[e], ", type: ").concat(e, " }"))
+                        throw new Error("Unrecognized Message type: { name: ".concat(Qa[e], ", type: ").concat(e, " }"))
                     }
                 }(t, e), n
             }
             static decode(t) {
-                t = new qd(Ha(t));
-                const e = Ad.getRootAsMessage(t),
+                t = new Hf(Rl(t));
+                const e = Mf.getRootAsMessage(t),
                     n = e.bodyLength(),
                     i = e.version(),
                     r = e.headerType(),
-                    s = new Qd(n, i, r);
+                    s = new Yf(n, i, r);
                 return s._createHeader = function(t, e) {
                     return () => {
                         switch (e) {
-                            case na.Schema:
-                                return Wu.decode(t.header(new Ah));
-                            case na.RecordBatch:
-                                return Zd.decode(t.header(new vd), t.version());
-                            case na.DictionaryBatch:
-                                return Gd.decode(t.header(new _d), t.version())
+                            case Qa.Schema:
+                                return Bh.decode(t.header(new kd));
+                            case Qa.RecordBatch:
+                                return $f.decode(t.header(new pf), t.version());
+                            case Qa.DictionaryBatch:
+                                return Kf.decode(t.header(new gf), t.version())
                         }
-                        throw new Error("Unrecognized Message type: { name: ".concat(na[e], ", type: ").concat(e, " }"))
+                        throw new Error("Unrecognized Message type: { name: ".concat(Qa[e], ", type: ").concat(e, " }"))
                     }
                 }(e, r), s
             }
             static encode(t) {
-                const e = new Xd;
+                const e = new Wf;
                 let n = -1;
-                return t.isSchema() ? n = Wu.encode(e, t.header()) : t.isRecordBatch() ? n = Zd.encode(e, t.header()) : t.isDictionaryBatch() && (n = Gd.encode(e, t.header())), Ad.startMessage(e), Ad.addVersion(e, Qo.V4), Ad.addHeader(e, n), Ad.addHeaderType(e, t.headerType), Ad.addBodyLength(e, new Kd(t.bodyLength, 0)), Ad.finishMessageBuffer(e, Ad.endMessage(e)), e.asUint8Array()
+                return t.isSchema() ? n = Bh.encode(e, t.header()) : t.isRecordBatch() ? n = $f.encode(e, t.header()) : t.isDictionaryBatch() && (n = Kf.encode(e, t.header())), Mf.startMessage(e), Mf.addVersion(e, Ha.V4), Mf.addHeader(e, n), Mf.addHeaderType(e, t.headerType), Mf.addBodyLength(e, new jf(t.bodyLength, 0)), Mf.finishMessageBuffer(e, Mf.endMessage(e)), e.asUint8Array()
             }
             static from(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0;
-                if (t instanceof Wu) return new Qd(0, Qo.V4, na.Schema, t);
-                if (t instanceof Zd) return new Qd(e, Qo.V4, na.RecordBatch, t);
-                if (t instanceof Gd) return new Qd(e, Qo.V4, na.DictionaryBatch, t);
+                if (t instanceof Bh) return new Yf(0, Ha.V4, Qa.Schema, t);
+                if (t instanceof $f) return new Yf(e, Ha.V4, Qa.RecordBatch, t);
+                if (t instanceof Kf) return new Yf(e, Ha.V4, Qa.DictionaryBatch, t);
                 throw new Error("Unrecognized Message header: ".concat(t))
             }
             get type() {
                 return this.headerType
             }
             get version() {
                 return this._version
@@ -23751,38 +24478,38 @@
             get bodyLength() {
                 return this._bodyLength
             }
             header() {
                 return this._createHeader()
             }
             isSchema() {
-                return this.headerType === na.Schema
+                return this.headerType === Qa.Schema
             }
             isRecordBatch() {
-                return this.headerType === na.RecordBatch
+                return this.headerType === Qa.RecordBatch
             }
             isDictionaryBatch() {
-                return this.headerType === na.DictionaryBatch
+                return this.headerType === Qa.DictionaryBatch
             }
         }
-        class Zd {
+        class $f {
             constructor(t, e, n) {
                 this._nodes = e, this._buffers = n, this._length = "number" === typeof t ? t : t.low
             }
             get nodes() {
                 return this._nodes
             }
             get length() {
                 return this._length
             }
             get buffers() {
                 return this._buffers
             }
         }
-        class Gd {
+        class Kf {
             constructor(t, e) {
                 let n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2];
                 this._data = t, this._isDelta = n, this._id = "number" === typeof e ? e : e.low
             }
             get id() {
                 return this._id
             }
@@ -23798,390 +24525,394 @@
             get nodes() {
                 return this.data.nodes
             }
             get buffers() {
                 return this.data.buffers
             }
         }
-        class Jd {
+        class Xf {
             constructor(t, e) {
                 this.offset = "number" === typeof t ? t : t.low, this.length = "number" === typeof e ? e : e.low
             }
         }
-        class tf {
+        class qf {
             constructor(t, e) {
                 this.length = "number" === typeof t ? t : t.low, this.nullCount = "number" === typeof e ? e : e.low
             }
         }
 
-        function ef(t, e) {
+        function Qf(t, e) {
             const n = [];
-            for (let i, r = -1, s = -1, o = t.childrenLength(); ++r < o;)(i = t.children(r)) && (n[++s] = Hu.decode(i, e));
+            for (let i, r = -1, s = -1, o = t.childrenLength(); ++r < o;)(i = t.children(r)) && (n[++s] = Rh.decode(i, e));
             return n
         }
 
-        function nf(t) {
+        function Zf(t) {
             const e = new Map;
             if (t)
                 for (let n, i, r = -1, s = Math.trunc(t.customMetadataLength()); ++r < s;)(n = t.customMetadata(r)) && null != (i = n.key()) && e.set(i, n.value());
             return e
         }
 
-        function rf(t) {
-            return new Il(t.isSigned(), t.bitWidth())
+        function Gf(t) {
+            return new xc(t.isSigned(), t.bitWidth())
         }
 
-        function sf(t, e) {
+        function Jf(t, e) {
             const n = t.typeType();
             switch (n) {
-                case Th.NONE:
-                case Th.Null:
-                    return new Ml;
-                case Th.Binary:
-                    return new Dl;
-                case Th.Utf8:
-                    return new Al;
-                case Th.Bool:
-                    return new Cl;
-                case Th.List:
-                    return new Rl((e || [])[0]);
-                case Th.Struct_:
-                    return new zl(e || [])
+                case bd.NONE:
+                case bd.Null:
+                    return new _c;
+                case bd.Binary:
+                    return new Tc;
+                case bd.Utf8:
+                    return new kc;
+                case bd.Bool:
+                    return new Mc;
+                case bd.List:
+                    return new Cc((e || [])[0]);
+                case bd.Struct_:
+                    return new Pc(e || [])
             }
             switch (n) {
-                case Th.Int: {
-                    const e = t.type(new Eh);
-                    return new Il(e.isSigned(), e.bitWidth())
-                }
-                case Th.FloatingPoint: {
-                    const e = t.type(new xd);
-                    return new Ol(e.precision())
-                }
-                case Th.Decimal: {
+                case bd.Int: {
                     const e = t.type(new wd);
-                    return new Pl(e.scale(), e.precision(), e.bitWidth())
+                    return new xc(e.isSigned(), e.bitWidth())
                 }
-                case Th.Date: {
-                    const e = t.type(new Sd);
-                    return new Fl(e.unit())
+                case bd.FloatingPoint: {
+                    const e = t.type(new mf);
+                    return new Sc(e.precision())
                 }
-                case Th.Time: {
-                    const e = t.type(new Td);
-                    return new Ll(e.unit(), e.bitWidth())
+                case bd.Decimal: {
+                    const e = t.type(new yf);
+                    return new Ic(e.scale(), e.precision(), e.bitWidth())
                 }
-                case Th.Timestamp: {
-                    const e = t.type(new kd);
-                    return new Nl(e.unit(), e.timezone())
+                case bd.Date: {
+                    const e = t.type(new bf);
+                    return new Ec(e.unit())
                 }
-                case Th.Interval: {
-                    const e = t.type(new Md);
-                    return new Bl(e.unit())
+                case bd.Time: {
+                    const e = t.type(new vf);
+                    return new Oc(e.unit(), e.bitWidth())
                 }
-                case Th.Union: {
-                    const n = t.type(new Id);
-                    return new Ul(n.mode(), n.typeIdsArray() || [], e || [])
+                case bd.Timestamp: {
+                    const e = t.type(new _f);
+                    return new Dc(e.unit(), e.timezone())
                 }
-                case Th.FixedSizeBinary: {
-                    const e = t.type(new Ed);
-                    return new Vl(e.byteWidth())
+                case bd.Interval: {
+                    const e = t.type(new xf);
+                    return new Ac(e.unit())
                 }
-                case Th.FixedSizeList: {
-                    const n = t.type(new Od);
-                    return new jl(n.listSize(), (e || [])[0])
+                case bd.Union: {
+                    const n = t.type(new wf);
+                    return new Fc(n.mode(), n.typeIdsArray() || [], e || [])
                 }
-                case Th.Map: {
-                    const n = t.type(new Dd);
-                    return new Wl((e || [])[0], n.keysSorted())
+                case bd.FixedSizeBinary: {
+                    const e = t.type(new Sf);
+                    return new Lc(e.byteWidth())
+                }
+                case bd.FixedSizeList: {
+                    const n = t.type(new Tf);
+                    return new Nc(n.listSize(), (e || [])[0])
+                }
+                case bd.Map: {
+                    const n = t.type(new kf);
+                    return new Bc((e || [])[0], n.keysSorted())
                 }
             }
-            throw new Error('Unrecognized type: "'.concat(Th[n], '" (').concat(n, ")"))
+            throw new Error('Unrecognized type: "'.concat(bd[n], '" (').concat(n, ")"))
         }
-        Hu.encode = function(t, e) {
+        Rh.encode = function(t, e) {
             let n = -1,
                 i = -1,
                 r = -1;
             const s = e.type;
             let o = e.typeId;
-            kl.isDictionary(s) ? (o = s.dictionary.typeId, r = zd.visit(s, t), i = zd.visit(s.dictionary, t)) : i = zd.visit(s, t);
-            const a = (s.children || []).map((e => Hu.encode(t, e))),
-                l = Dh.createChildrenVector(t, a),
-                c = e.metadata && e.metadata.size > 0 ? Dh.createCustomMetadataVector(t, [...e.metadata].map((e => {
+            vc.isDictionary(s) ? (o = s.dictionary.typeId, r = Ff.visit(s, t), i = Ff.visit(s.dictionary, t)) : i = Ff.visit(s, t);
+            const a = (s.children || []).map((e => Rh.encode(t, e))),
+                l = Td.createChildrenVector(t, a),
+                c = e.metadata && e.metadata.size > 0 ? Td.createCustomMetadataVector(t, [...e.metadata].map((e => {
                     let [n, i] = e;
                     const r = t.createString("".concat(n)),
                         s = t.createString("".concat(i));
-                    return Ih.startKeyValue(t), Ih.addKey(t, r), Ih.addValue(t, s), Ih.endKeyValue(t)
+                    return xd.startKeyValue(t), xd.addKey(t, r), xd.addValue(t, s), xd.endKeyValue(t)
                 }))) : -1;
             e.name && (n = t.createString(e.name));
-            Dh.startField(t), Dh.addType(t, i), Dh.addTypeType(t, o), Dh.addChildren(t, l), Dh.addNullable(t, !!e.nullable), -1 !== n && Dh.addName(t, n); - 1 !== r && Dh.addDictionary(t, r); - 1 !== c && Dh.addCustomMetadata(t, c);
-            return Dh.endField(t)
-        }, Hu.decode = function(t, e) {
+            Td.startField(t), Td.addType(t, i), Td.addTypeType(t, o), Td.addChildren(t, l), Td.addNullable(t, !!e.nullable), -1 !== n && Td.addName(t, n); - 1 !== r && Td.addDictionary(t, r); - 1 !== c && Td.addCustomMetadata(t, c);
+            return Td.endField(t)
+        }, Rh.decode = function(t, e) {
             let n, i, r, s, o, a;
-            e && (a = t.dictionary()) ? e.has(n = a.id().low) ? (s = (s = a.indexType()) ? rf(s) : new El, o = new $l(e.get(n), s, n, a.isOrdered()), i = new Hu(t.name(), o, t.nullable(), nf(t))) : (s = (s = a.indexType()) ? rf(s) : new El, e.set(n, r = sf(t, ef(t, e))), o = new $l(r, s, n, a.isOrdered()), i = new Hu(t.name(), o, t.nullable(), nf(t))) : (r = sf(t, ef(t, e)), i = new Hu(t.name(), r, t.nullable(), nf(t)));
+            e && (a = t.dictionary()) ? e.has(n = a.id().low) ? (s = (s = a.indexType()) ? Gf(s) : new wc, o = new Uc(e.get(n), s, n, a.isOrdered()), i = new Rh(t.name(), o, t.nullable(), Zf(t))) : (s = (s = a.indexType()) ? Gf(s) : new wc, e.set(n, r = Jf(t, Qf(t, e))), o = new Uc(r, s, n, a.isOrdered()), i = new Rh(t.name(), o, t.nullable(), Zf(t))) : (r = Jf(t, Qf(t, e)), i = new Rh(t.name(), r, t.nullable(), Zf(t)));
             return i || null
-        }, Hu.fromJSON = function(t, e) {
+        }, Rh.fromJSON = function(t, e) {
             let n, i, r, s, o, a;
-            return e && (s = t.dictionary) ? e.has(n = s.id) ? (i = (i = s.indexType) ? Yd(i) : new El, a = new $l(e.get(n), i, n, s.isOrdered), r = new Hu(t.name, a, t.nullable, Hd(t.customMetadata))) : (i = (i = s.indexType) ? Yd(i) : new El, e.set(n, o = $d(t, Vd(t, e))), a = new $l(o, i, n, s.isOrdered), r = new Hu(t.name, a, t.nullable, Hd(t.customMetadata))) : (o = $d(t, Vd(t, e)), r = new Hu(t.name, o, t.nullable, Hd(t.customMetadata))), r || null
-        }, Wu.encode = function(t, e) {
-            const n = e.fields.map((e => Hu.encode(t, e)));
-            Ah.startFieldsVector(t, n.length);
-            const i = Ah.createFieldsVector(t, n),
-                r = e.metadata && e.metadata.size > 0 ? Ah.createCustomMetadataVector(t, [...e.metadata].map((e => {
+            return e && (s = t.dictionary) ? e.has(n = s.id) ? (i = (i = s.indexType) ? Uf(i) : new wc, a = new Uc(e.get(n), i, n, s.isOrdered), r = new Rh(t.name, a, t.nullable, zf(t.customMetadata))) : (i = (i = s.indexType) ? Uf(i) : new wc, e.set(n, o = Vf(t, Nf(t, e))), a = new Uc(o, i, n, s.isOrdered), r = new Rh(t.name, a, t.nullable, zf(t.customMetadata))) : (o = Vf(t, Nf(t, e)), r = new Rh(t.name, o, t.nullable, zf(t.customMetadata))), r || null
+        }, Bh.encode = function(t, e) {
+            const n = e.fields.map((e => Rh.encode(t, e)));
+            kd.startFieldsVector(t, n.length);
+            const i = kd.createFieldsVector(t, n),
+                r = e.metadata && e.metadata.size > 0 ? kd.createCustomMetadataVector(t, [...e.metadata].map((e => {
                     let [n, i] = e;
                     const r = t.createString("".concat(n)),
                         s = t.createString("".concat(i));
-                    return Ih.startKeyValue(t), Ih.addKey(t, r), Ih.addValue(t, s), Ih.endKeyValue(t)
+                    return xd.startKeyValue(t), xd.addKey(t, r), xd.addValue(t, s), xd.endKeyValue(t)
                 }))) : -1;
-            Ah.startSchema(t), Ah.addFields(t, i), Ah.addEndianness(t, of ? wh.Little : wh.Big), -1 !== r && Ah.addCustomMetadata(t, r);
-            return Ah.endSchema(t)
-        }, Wu.decode = function(t) {
+            kd.startSchema(t), kd.addFields(t, i), kd.addEndianness(t, tp ? md.Little : md.Big), -1 !== r && kd.addCustomMetadata(t, r);
+            return kd.endSchema(t)
+        }, Bh.decode = function(t) {
             let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Map;
             const n = function(t, e) {
                 const n = [];
-                for (let i, r = -1, s = -1, o = t.fieldsLength(); ++r < o;)(i = t.fields(r)) && (n[++s] = Hu.decode(i, e));
+                for (let i, r = -1, s = -1, o = t.fieldsLength(); ++r < o;)(i = t.fields(r)) && (n[++s] = Rh.decode(i, e));
                 return n
             }(t, e);
-            return new Wu(n, nf(t), e)
-        }, Wu.fromJSON = function(t) {
+            return new Bh(n, Zf(t), e)
+        }, Bh.fromJSON = function(t) {
             let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Map;
-            return new Wu(function(t, e) {
-                return (t.fields || []).filter(Boolean).map((t => Hu.fromJSON(t, e)))
-            }(t, e), Hd(t.customMetadata), e)
-        }, Zd.encode = function(t, e) {
+            return new Bh(function(t, e) {
+                return (t.fields || []).filter(Boolean).map((t => Rh.fromJSON(t, e)))
+            }(t, e), zf(t.customMetadata), e)
+        }, $f.encode = function(t, e) {
             const n = e.nodes || [],
                 i = e.buffers || [];
-            vd.startNodesVector(t, n.length);
-            for (const o of n.slice().reverse()) tf.encode(t, o);
+            pf.startNodesVector(t, n.length);
+            for (const o of n.slice().reverse()) qf.encode(t, o);
             const r = t.endVector();
-            vd.startBuffersVector(t, i.length);
-            for (const o of i.slice().reverse()) Jd.encode(t, o);
+            pf.startBuffersVector(t, i.length);
+            for (const o of i.slice().reverse()) Xf.encode(t, o);
             const s = t.endVector();
-            return vd.startRecordBatch(t), vd.addLength(t, new Kd(e.length, 0)), vd.addNodes(t, r), vd.addBuffers(t, s), vd.endRecordBatch(t)
-        }, Zd.decode = function(t) {
-            let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Qo.V4;
+            return pf.startRecordBatch(t), pf.addLength(t, new jf(e.length, 0)), pf.addNodes(t, r), pf.addBuffers(t, s), pf.endRecordBatch(t)
+        }, $f.decode = function(t) {
+            let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Ha.V4;
             if (null !== t.compression()) throw new Error("Record batch compression not implemented");
-            return new Zd(t.length(), function(t) {
+            return new $f(t.length(), function(t) {
                 const e = [];
-                for (let n, i = -1, r = -1, s = t.nodesLength(); ++i < s;)(n = t.nodes(i)) && (e[++r] = tf.decode(n));
+                for (let n, i = -1, r = -1, s = t.nodesLength(); ++i < s;)(n = t.nodes(i)) && (e[++r] = qf.decode(n));
                 return e
             }(t), function(t, e) {
                 const n = [];
-                for (let i, r = -1, s = -1, o = t.buffersLength(); ++r < o;)(i = t.buffers(r)) && (e < Qo.V4 && (i.bb_pos += 8 * (r + 1)), n[++s] = Jd.decode(i));
+                for (let i, r = -1, s = -1, o = t.buffersLength(); ++r < o;)(i = t.buffers(r)) && (e < Ha.V4 && (i.bb_pos += 8 * (r + 1)), n[++s] = Xf.decode(i));
                 return n
             }(t, e))
-        }, Zd.fromJSON = Ud, Gd.encode = function(t, e) {
-            const n = Zd.encode(t, e.data);
-            return _d.startDictionaryBatch(t), _d.addId(t, new Kd(e.id, 0)), _d.addIsDelta(t, e.isDelta), _d.addData(t, n), _d.endDictionaryBatch(t)
-        }, Gd.decode = function(t) {
-            let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Qo.V4;
-            return new Gd(Zd.decode(t.data(), e), t.id(), t.isDelta())
-        }, Gd.fromJSON = function(t) {
-            return new Gd(Ud(t.data), t.id, t.isDelta)
-        }, tf.encode = function(t, e) {
-            return bd.createFieldNode(t, new Kd(e.length, 0), new Kd(e.nullCount, 0))
-        }, tf.decode = function(t) {
-            return new tf(t.length(), t.nullCount())
-        }, Jd.encode = function(t, e) {
-            return yd.createBuffer(t, new Kd(e.offset, 0), new Kd(e.length, 0))
-        }, Jd.decode = function(t) {
-            return new Jd(t.offset(), t.length())
+        }, $f.fromJSON = Lf, Kf.encode = function(t, e) {
+            const n = $f.encode(t, e.data);
+            return gf.startDictionaryBatch(t), gf.addId(t, new jf(e.id, 0)), gf.addIsDelta(t, e.isDelta), gf.addData(t, n), gf.endDictionaryBatch(t)
+        }, Kf.decode = function(t) {
+            let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Ha.V4;
+            return new Kf($f.decode(t.data(), e), t.id(), t.isDelta())
+        }, Kf.fromJSON = function(t) {
+            return new Kf(Lf(t.data), t.id, t.isDelta)
+        }, qf.encode = function(t, e) {
+            return ff.createFieldNode(t, new jf(e.length, 0), new jf(e.nullCount, 0))
+        }, qf.decode = function(t) {
+            return new qf(t.length(), t.nullCount())
+        }, Xf.encode = function(t, e) {
+            return df.createBuffer(t, new jf(e.offset, 0), new jf(e.length, 0))
+        }, Xf.decode = function(t) {
+            return new Xf(t.offset(), t.length())
         };
-        const of = (() => {
-            const t = new ArrayBuffer(2);
-            return new DataView(t).setInt16(0, 256, !0), 256 === new Int16Array(t)[0]
-        })(), af = t => "Expected ".concat(na[t], " Message in stream, but was null or length 0."), lf = t => "Header pointer of flatbuffer-encoded ".concat(na[t], " Message is null or length 0."), cf = (t, e) => "Expected to read ".concat(t, " metadata bytes, but only read ").concat(e, "."), uf = (t, e) => "Expected to read ".concat(t, " bytes for message body, but only read ").concat(e, ".");
-        class hf {
+        const tp = (() => {
+                const t = new ArrayBuffer(2);
+                return new DataView(t).setInt16(0, 256, !0), 256 === new Int16Array(t)[0]
+            })(),
+            ep = t => "Expected ".concat(Qa[t], " Message in stream, but was null or length 0."),
+            np = t => "Header pointer of flatbuffer-encoded ".concat(Qa[t], " Message is null or length 0."),
+            ip = (t, e) => "Expected to read ".concat(t, " metadata bytes, but only read ").concat(e, "."),
+            rp = (t, e) => "Expected to read ".concat(t, " bytes for message body, but only read ").concat(e, ".");
+        class sp {
             constructor(t) {
-                this.source = t instanceof Xh ? t : new Xh(t)
+                this.source = t instanceof jd ? t : new jd(t)
             } [Symbol.iterator]() {
                 return this
             }
             next() {
                 let t;
-                return (t = this.readMetadataLength()).done || -1 === t.value && (t = this.readMetadataLength()).done || (t = this.readMetadata(t.value)).done ? Wh : t
+                return (t = this.readMetadataLength()).done || -1 === t.value && (t = this.readMetadataLength()).done || (t = this.readMetadata(t.value)).done ? Bd : t
             }
             throw (t) {
                 return this.source.throw(t)
             }
             return (t) {
                 return this.source.return(t)
             }
             readMessage(t) {
                 let e;
                 if ((e = this.next()).done) return null;
-                if (null != t && e.value.headerType !== t) throw new Error(af(t));
+                if (null != t && e.value.headerType !== t) throw new Error(ep(t));
                 return e.value
             }
             readMessageBody(t) {
                 if (t <= 0) return new Uint8Array(0);
-                const e = Ha(this.source.read(t));
-                if (e.byteLength < t) throw new Error(uf(t, e.byteLength));
+                const e = Rl(this.source.read(t));
+                if (e.byteLength < t) throw new Error(rp(t, e.byteLength));
                 return e.byteOffset % 8 === 0 && e.byteOffset + e.byteLength <= e.buffer.byteLength ? e : e.slice()
             }
             readSchema() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
-                const e = na.Schema,
+                const e = Qa.Schema,
                     n = this.readMessage(e),
                     i = null === n || void 0 === n ? void 0 : n.header();
-                if (t && !i) throw new Error(lf(e));
+                if (t && !i) throw new Error(np(e));
                 return i
             }
             readMetadataLength() {
-                const t = this.source.read(pf),
-                    e = t && new kh(t),
+                const t = this.source.read(lp),
+                    e = t && new vd(t),
                     n = (null === e || void 0 === e ? void 0 : e.readInt32(0)) || 0;
                 return {
                     done: 0 === n,
                     value: n
                 }
             }
             readMetadata(t) {
                 const e = this.source.read(t);
-                if (!e) return Wh;
-                if (e.byteLength < t) throw new Error(cf(t, e.byteLength));
+                if (!e) return Bd;
+                if (e.byteLength < t) throw new Error(ip(t, e.byteLength));
                 return {
                     done: !1,
-                    value: Qd.decode(e)
+                    value: Yf.decode(e)
                 }
             }
         }
-        class df {
+        class op {
             constructor(t, e) {
-                this.source = t instanceof qh ? t : wa(t) ? new Jh(t, e) : new qh(t)
+                this.source = t instanceof Wd ? t : ml(t) ? new Kd(t, e) : new Wd(t)
             } [Symbol.asyncIterator]() {
                 return this
             }
             next() {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     let t;
-                    return (t = yield this.readMetadataLength()).done || -1 === t.value && (t = yield this.readMetadataLength()).done || (t = yield this.readMetadata(t.value)).done ? Wh : t
+                    return (t = yield this.readMetadataLength()).done || -1 === t.value && (t = yield this.readMetadataLength()).done || (t = yield this.readMetadata(t.value)).done ? Bd : t
                 }))
             }
             throw (t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     return yield this.source.throw(t)
                 }))
             }
             return (t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     return yield this.source.return(t)
                 }))
             }
             readMessage(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     let e;
                     if ((e = yield this.next()).done) return null;
-                    if (null != t && e.value.headerType !== t) throw new Error(af(t));
+                    if (null != t && e.value.headerType !== t) throw new Error(ep(t));
                     return e.value
                 }))
             }
             readMessageBody(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     if (t <= 0) return new Uint8Array(0);
-                    const e = Ha(yield this.source.read(t));
-                    if (e.byteLength < t) throw new Error(uf(t, e.byteLength));
+                    const e = Rl(yield this.source.read(t));
+                    if (e.byteLength < t) throw new Error(rp(t, e.byteLength));
                     return e.byteOffset % 8 === 0 && e.byteOffset + e.byteLength <= e.buffer.byteLength ? e : e.slice()
                 }))
             }
             readSchema() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
-                return Oa(this, void 0, void 0, (function*() {
-                    const e = na.Schema,
+                return Sl(this, void 0, void 0, (function*() {
+                    const e = Qa.Schema,
                         n = yield this.readMessage(e), i = null === n || void 0 === n ? void 0 : n.header();
-                    if (t && !i) throw new Error(lf(e));
+                    if (t && !i) throw new Error(np(e));
                     return i
                 }))
             }
             readMetadataLength() {
-                return Oa(this, void 0, void 0, (function*() {
-                    const t = yield this.source.read(pf), e = t && new kh(t), n = (null === e || void 0 === e ? void 0 : e.readInt32(0)) || 0;
+                return Sl(this, void 0, void 0, (function*() {
+                    const t = yield this.source.read(lp), e = t && new vd(t), n = (null === e || void 0 === e ? void 0 : e.readInt32(0)) || 0;
                     return {
                         done: 0 === n,
                         value: n
                     }
                 }))
             }
             readMetadata(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     const e = yield this.source.read(t);
-                    if (!e) return Wh;
-                    if (e.byteLength < t) throw new Error(cf(t, e.byteLength));
+                    if (!e) return Bd;
+                    if (e.byteLength < t) throw new Error(ip(t, e.byteLength));
                     return {
                         done: !1,
-                        value: Qd.decode(e)
+                        value: Yf.decode(e)
                     }
                 }))
             }
         }
-        class ff extends hf {
+        class ap extends sp {
             constructor(t) {
-                super(new Uint8Array(0)), this._schema = !1, this._body = [], this._batchIndex = 0, this._dictionaryIndex = 0, this._json = t instanceof Hh ? t : new Hh(t)
+                super(new Uint8Array(0)), this._schema = !1, this._body = [], this._batchIndex = 0, this._dictionaryIndex = 0, this._json = t instanceof Rd ? t : new Rd(t)
             }
             next() {
                 const {
                     _json: t
                 } = this;
                 if (!this._schema) {
                     this._schema = !0;
                     return {
                         done: !1,
-                        value: Qd.fromJSON(t.schema, na.Schema)
+                        value: Yf.fromJSON(t.schema, Qa.Schema)
                     }
                 }
                 if (this._dictionaryIndex < t.dictionaries.length) {
                     const e = t.dictionaries[this._dictionaryIndex++];
                     this._body = e.data.columns;
                     return {
                         done: !1,
-                        value: Qd.fromJSON(e, na.DictionaryBatch)
+                        value: Yf.fromJSON(e, Qa.DictionaryBatch)
                     }
                 }
                 if (this._batchIndex < t.batches.length) {
                     const e = t.batches[this._batchIndex++];
                     this._body = e.columns;
                     return {
                         done: !1,
-                        value: Qd.fromJSON(e, na.RecordBatch)
+                        value: Yf.fromJSON(e, Qa.RecordBatch)
                     }
                 }
-                return this._body = [], Wh
+                return this._body = [], Bd
             }
             readMessageBody(t) {
                 return function t(e) {
                     return (e || []).reduce(((e, n) => [...e, ...n.VALIDITY && [n.VALIDITY] || [], ...n.TYPE && [n.TYPE] || [], ...n.OFFSET && [n.OFFSET] || [], ...n.DATA && [n.DATA] || [], ...t(n.children)]), [])
                 }(this._body)
             }
             readMessage(t) {
                 let e;
                 if ((e = this.next()).done) return null;
-                if (null != t && e.value.headerType !== t) throw new Error(af(t));
+                if (null != t && e.value.headerType !== t) throw new Error(ep(t));
                 return e.value
             }
             readSchema() {
-                const t = na.Schema,
+                const t = Qa.Schema,
                     e = this.readMessage(t),
                     n = null === e || void 0 === e ? void 0 : e.header();
-                if (!e || !n) throw new Error(lf(t));
+                if (!e || !n) throw new Error(np(t));
                 return n
             }
         }
-        const pf = 4,
-            gf = "ARROW1",
-            mf = new Uint8Array(6);
-        for (let n = 0; n < 6; n += 1) mf[n] = gf.codePointAt(n);
+        const lp = 4,
+            cp = "ARROW1",
+            up = new Uint8Array(6);
+        for (let n = 0; n < 6; n += 1) up[n] = cp.codePointAt(n);
 
-        function yf(t) {
+        function hp(t) {
             let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0;
-            for (let n = -1, i = mf.length; ++n < i;)
-                if (mf[n] !== t[e + n]) return !1;
+            for (let n = -1, i = up.length; ++n < i;)
+                if (up[n] !== t[e + n]) return !1;
             return !0
         }
-        const bf = mf.length,
-            vf = bf + pf,
-            _f = 2 * bf + pf;
-        class xf extends Yh {
+        const dp = up.length,
+            fp = dp + lp,
+            pp = 2 * dp + lp;
+        class gp extends zd {
             constructor(t) {
                 super(), this._impl = t
             }
             get closed() {
                 return this._impl.closed
             }
             get schema() {
@@ -24227,97 +24958,97 @@
                 return this._impl.cancel()
             }
             reset(t) {
                 return this._impl.reset(t), this._DOMStream = void 0, this._nodeStream = void 0, this
             }
             open(t) {
                 const e = this._impl.open(t);
-                return ya(e) ? e.then((() => this)) : this
+                return hl(e) ? e.then((() => this)) : this
             }
             readRecordBatch(t) {
                 return this._impl.isFile() ? this._impl.readRecordBatch(t) : null
             } [Symbol.iterator]() {
                 return this._impl[Symbol.iterator]()
             } [Symbol.asyncIterator]() {
                 return this._impl[Symbol.asyncIterator]()
             }
             toDOMStream() {
-                return zh.toDOMStream(this.isSync() ? {
+                return Pd.toDOMStream(this.isSync() ? {
                     [Symbol.iterator]: () => this
                 } : {
                     [Symbol.asyncIterator]: () => this
                 })
             }
             toNodeStream() {
-                return zh.toNodeStream(this.isSync() ? {
+                return Pd.toNodeStream(this.isSync() ? {
                     [Symbol.iterator]: () => this
                 } : {
                     [Symbol.asyncIterator]: () => this
                 }, {
                     objectMode: !0
                 })
             }
             static throughNode(t) {
                 throw new Error('"throughNode" not available in this environment')
             }
             static throughDOM(t, e) {
                 throw new Error('"throughDOM" not available in this environment')
             }
             static from(t) {
-                return t instanceof xf ? t : _a(t) ? function(t) {
-                    return new wf(new Af(t))
-                }(t) : wa(t) ? function(t) {
-                    return Oa(this, void 0, void 0, (function*() {
+                return t instanceof gp ? t : pl(t) ? function(t) {
+                    return new mp(new kp(t))
+                }(t) : ml(t) ? function(t) {
+                    return Sl(this, void 0, void 0, (function*() {
                         const {
                             size: e
-                        } = yield t.stat(), n = new Jh(t, e);
-                        return e >= _f && yf(yield n.readAt(0, bf + 7 & -8)) ? new kf(new Df(n)) : new Sf(new Ef(n))
+                        } = yield t.stat(), n = new Kd(t, e);
+                        return e >= pp && hp(yield n.readAt(0, dp + 7 & -8)) ? new vp(new Tp(n)) : new yp(new wp(n))
                     }))
-                }(t) : ya(t) ? (() => Oa(this, void 0, void 0, (function*() {
-                    return yield xf.from(yield t)
-                })))() : Sa(t) || ka(t) || Ma(t) || va(t) ? function(t) {
-                    return Oa(this, void 0, void 0, (function*() {
-                        const e = yield t.peek(bf + 7 & -8);
-                        return e && e.byteLength >= 4 ? yf(e) ? new Tf(new Of(yield t.read())) : new Sf(new Ef(t)) : new Sf(new Ef(function() {
-                            return Ca(this, arguments, (function*() {}))
+                }(t) : hl(t) ? (() => Sl(this, void 0, void 0, (function*() {
+                    return yield gp.from(yield t)
+                })))() : yl(t) || vl(t) || _l(t) || fl(t) ? function(t) {
+                    return Sl(this, void 0, void 0, (function*() {
+                        const e = yield t.peek(dp + 7 & -8);
+                        return e && e.byteLength >= 4 ? hp(e) ? new bp(new Sp(yield t.read())) : new yp(new wp(t)) : new yp(new wp(function() {
+                            return Ml(this, arguments, (function*() {}))
                         }()))
                     }))
-                }(new qh(t)) : function(t) {
-                    const e = t.peek(bf + 7 & -8);
-                    return e && e.byteLength >= 4 ? yf(e) ? new Tf(new Of(t.read())) : new wf(new If(t)) : new wf(new If(function*() {}()))
-                }(new Xh(t))
+                }(new Wd(t)) : function(t) {
+                    const e = t.peek(dp + 7 & -8);
+                    return e && e.byteLength >= 4 ? hp(e) ? new bp(new Sp(t.read())) : new mp(new xp(t)) : new mp(new xp(function*() {}()))
+                }(new jd(t))
             }
             static readAll(t) {
-                return t instanceof xf ? t.isSync() ? Pf(t) : Ff(t) : _a(t) || ArrayBuffer.isView(t) || ba(t) || xa(t) ? Pf(t) : Ff(t)
+                return t instanceof gp ? t.isSync() ? Ip(t) : Ep(t) : pl(t) || ArrayBuffer.isView(t) || dl(t) || gl(t) ? Ip(t) : Ep(t)
             }
         }
-        class wf extends xf {
+        class mp extends gp {
             constructor(t) {
                 super(t), this._impl = t
             }
             readAll() {
                 return [...this]
             } [Symbol.iterator]() {
                 return this._impl[Symbol.iterator]()
             } [Symbol.asyncIterator]() {
-                return Ca(this, arguments, (function*() {
-                    yield Aa(yield* Pa(Fa(this[Symbol.iterator]())))
+                return Ml(this, arguments, (function*() {
+                    yield kl(yield* Il(El(this[Symbol.iterator]())))
                 }))
             }
         }
-        class Sf extends xf {
+        class yp extends gp {
             constructor(t) {
                 super(t), this._impl = t
             }
             readAll() {
                 var t, e;
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     const n = new Array;
                     try {
-                        for (var i, r = Fa(this); !(i = yield r.next()).done;) {
+                        for (var i, r = El(this); !(i = yield r.next()).done;) {
                             const t = i.value;
                             n.push(t)
                         }
                     } catch (s) {
                         t = {
                             error: s
                         }
@@ -24332,25 +25063,25 @@
                 }))
             } [Symbol.iterator]() {
                 throw new Error("AsyncRecordBatchStreamReader is not Iterable")
             } [Symbol.asyncIterator]() {
                 return this._impl[Symbol.asyncIterator]()
             }
         }
-        class Tf extends wf {
+        class bp extends mp {
             constructor(t) {
                 super(t), this._impl = t
             }
         }
-        class kf extends Sf {
+        class vp extends yp {
             constructor(t) {
                 super(t), this._impl = t
             }
         }
-        class Mf {
+        class _p {
             constructor() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : new Map;
                 this.closed = !1, this.autoDestroy = !0, this._dictionaryIndex = 0, this._recordBatchIndex = 0, this.dictionaries = t
             }
             get numDictionaries() {
                 return this._dictionaryIndex
             }
@@ -24370,66 +25101,66 @@
                 return !1
             }
             reset(t) {
                 return this._dictionaryIndex = 0, this._recordBatchIndex = 0, this.schema = t, this.dictionaries = new Map, this
             }
             _loadRecordBatch(t, e) {
                 const n = this._loadVectors(t, e, this.schema.fields),
-                    i = ju({
-                        type: new zl(this.schema.fields),
+                    i = Nh({
+                        type: new Pc(this.schema.fields),
                         length: t.length,
                         children: n
                     });
-                return new ah(this.schema, i)
+                return new ed(this.schema, i)
             }
             _loadDictionaryBatch(t, e) {
                 const {
                     id: n,
                     isDelta: i
                 } = t, {
                     dictionaries: r,
                     schema: s
                 } = this, o = r.get(n);
                 if (i || !o) {
                     const r = s.dictionaries.get(n),
                         a = this._loadVectors(t.data, e, [r]);
-                    return (o && i ? o.concat(new Ru(a)) : new Ru(a)).memoize()
+                    return (o && i ? o.concat(new Ch(a)) : new Ch(a)).memoize()
                 }
                 return o.memoize()
             }
             _loadVectors(t, e, n) {
-                return new od(e, t.nodes, t.buffers, this.dictionaries).visitMany(n)
+                return new tf(e, t.nodes, t.buffers, this.dictionaries).visitMany(n)
             }
         }
-        class If extends Mf {
+        class xp extends _p {
             constructor(t, e) {
-                super(e), this._reader = _a(t) ? new ff(this._handle = t) : new hf(this._handle = t)
+                super(e), this._reader = pl(t) ? new ap(this._handle = t) : new sp(this._handle = t)
             }
             isSync() {
                 return !0
             }
             isStream() {
                 return !0
             } [Symbol.iterator]() {
                 return this
             }
             cancel() {
                 !this.closed && (this.closed = !0) && (this.reset()._reader.return(), this._reader = null, this.dictionaries = null)
             }
             open(t) {
-                return this.closed || (this.autoDestroy = Cf(this, t), this.schema || (this.schema = this._reader.readSchema()) || this.cancel()), this
+                return this.closed || (this.autoDestroy = Mp(this, t), this.schema || (this.schema = this._reader.readSchema()) || this.cancel()), this
             }
             throw (t) {
-                return !this.closed && this.autoDestroy && (this.closed = !0) ? this.reset()._reader.throw(t) : Wh
+                return !this.closed && this.autoDestroy && (this.closed = !0) ? this.reset()._reader.throw(t) : Bd
             }
             return (t) {
-                return !this.closed && this.autoDestroy && (this.closed = !0) ? this.reset()._reader.return(t) : Wh
+                return !this.closed && this.autoDestroy && (this.closed = !0) ? this.reset()._reader.return(t) : Bd
             }
             next() {
-                if (this.closed) return Wh;
+                if (this.closed) return Bd;
                 let t;
                 const {
                     _reader: e
                 } = this;
                 for (; t = this._readNextMessageAndValidate();)
                     if (t.isSchema()) this.reset(t.header());
                     else {
@@ -24447,56 +25178,56 @@
                             const n = t.header(),
                                 i = e.readMessageBody(t.bodyLength),
                                 r = this._loadDictionaryBatch(n, i);
                             this.dictionaries.set(n.id, r)
                         }
                     } return this.schema && 0 === this._recordBatchIndex ? (this._recordBatchIndex++, {
                     done: !1,
-                    value: new uh(this.schema)
+                    value: new rd(this.schema)
                 }) : this.return()
             }
             _readNextMessageAndValidate(t) {
                 return this._reader.readMessage(t)
             }
         }
-        class Ef extends Mf {
+        class wp extends _p {
             constructor(t, e) {
-                super(e), this._reader = new df(this._handle = t)
+                super(e), this._reader = new op(this._handle = t)
             }
             isAsync() {
                 return !0
             }
             isStream() {
                 return !0
             } [Symbol.asyncIterator]() {
                 return this
             }
             cancel() {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     !this.closed && (this.closed = !0) && (yield this.reset()._reader.return(), this._reader = null, this.dictionaries = null)
                 }))
             }
             open(t) {
-                return Oa(this, void 0, void 0, (function*() {
-                    return this.closed || (this.autoDestroy = Cf(this, t), this.schema || (this.schema = yield this._reader.readSchema()) || (yield this.cancel())), this
+                return Sl(this, void 0, void 0, (function*() {
+                    return this.closed || (this.autoDestroy = Mp(this, t), this.schema || (this.schema = yield this._reader.readSchema()) || (yield this.cancel())), this
                 }))
             }
             throw (t) {
-                return Oa(this, void 0, void 0, (function*() {
-                    return !this.closed && this.autoDestroy && (this.closed = !0) ? yield this.reset()._reader.throw(t): Wh
+                return Sl(this, void 0, void 0, (function*() {
+                    return !this.closed && this.autoDestroy && (this.closed = !0) ? yield this.reset()._reader.throw(t): Bd
                 }))
             }
             return (t) {
-                return Oa(this, void 0, void 0, (function*() {
-                    return !this.closed && this.autoDestroy && (this.closed = !0) ? yield this.reset()._reader.return(t): Wh
+                return Sl(this, void 0, void 0, (function*() {
+                    return !this.closed && this.autoDestroy && (this.closed = !0) ? yield this.reset()._reader.return(t): Bd
                 }))
             }
             next() {
-                return Oa(this, void 0, void 0, (function*() {
-                    if (this.closed) return Wh;
+                return Sl(this, void 0, void 0, (function*() {
+                    if (this.closed) return Bd;
                     let t;
                     const {
                         _reader: e
                     } = this;
                     for (; t = yield this._readNextMessageAndValidate();)
                         if (t.isSchema()) yield this.reset(t.header());
                         else {
@@ -24513,27 +25244,27 @@
                                 this._dictionaryIndex++;
                                 const n = t.header(),
                                     i = yield e.readMessageBody(t.bodyLength), r = this._loadDictionaryBatch(n, i);
                                 this.dictionaries.set(n.id, r)
                             }
                         } return this.schema && 0 === this._recordBatchIndex ? (this._recordBatchIndex++, {
                         done: !1,
-                        value: new uh(this.schema)
+                        value: new rd(this.schema)
                     }) : yield this.return()
                 }))
             }
             _readNextMessageAndValidate(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     return yield this._reader.readMessage(t)
                 }))
             }
         }
-        class Of extends If {
+        class Sp extends xp {
             constructor(t, e) {
-                super(t instanceof Gh ? t : new Gh(t), e)
+                super(t instanceof $d ? t : new $d(t), e)
             }
             get footer() {
                 return this._footer
             }
             get numDictionaries() {
                 return this._footer ? this._footer.numDictionaries : 0
             }
@@ -24555,57 +25286,57 @@
             }
             readRecordBatch(t) {
                 var e;
                 if (this.closed) return null;
                 this._footer || this.open();
                 const n = null === (e = this._footer) || void 0 === e ? void 0 : e.getRecordBatch(t);
                 if (n && this._handle.seek(n.offset)) {
-                    const t = this._reader.readMessage(na.RecordBatch);
+                    const t = this._reader.readMessage(Qa.RecordBatch);
                     if (null === t || void 0 === t ? void 0 : t.isRecordBatch()) {
                         const e = t.header(),
                             n = this._reader.readMessageBody(t.bodyLength);
                         return this._loadRecordBatch(e, n)
                     }
                 }
                 return null
             }
             _readDictionaryBatch(t) {
                 var e;
                 const n = null === (e = this._footer) || void 0 === e ? void 0 : e.getDictionaryBatch(t);
                 if (n && this._handle.seek(n.offset)) {
-                    const t = this._reader.readMessage(na.DictionaryBatch);
+                    const t = this._reader.readMessage(Qa.DictionaryBatch);
                     if (null === t || void 0 === t ? void 0 : t.isDictionaryBatch()) {
                         const e = t.header(),
                             n = this._reader.readMessageBody(t.bodyLength),
                             i = this._loadDictionaryBatch(e, n);
                         this.dictionaries.set(e.id, i)
                     }
                 }
             }
             _readFooter() {
                 const {
                     _handle: t
-                } = this, e = t.size - vf, n = t.readInt32(e), i = t.readAt(e - n, n);
-                return Nh.decode(i)
+                } = this, e = t.size - fp, n = t.readInt32(e), i = t.readAt(e - n, n);
+                return Dd.decode(i)
             }
             _readNextMessageAndValidate(t) {
                 var e;
                 if (this._footer || this.open(), this._footer && this._recordBatchIndex < this.numRecordBatches) {
                     const n = null === (e = this._footer) || void 0 === e ? void 0 : e.getRecordBatch(this._recordBatchIndex);
                     if (n && this._handle.seek(n.offset)) return this._reader.readMessage(t)
                 }
                 return null
             }
         }
-        class Df extends Ef {
+        class Tp extends wp {
             constructor(t) {
                 for (var e = arguments.length, n = new Array(e > 1 ? e - 1 : 0), i = 1; i < e; i++) n[i - 1] = arguments[i];
                 const r = "number" !== typeof n[0] ? n.shift() : void 0,
                     s = n[0] instanceof Map ? n.shift() : void 0;
-                super(t instanceof Jh ? t : new Jh(t, r), s)
+                super(t instanceof Kd ? t : new Kd(t, r), s)
             }
             get footer() {
                 return this._footer
             }
             get numDictionaries() {
                 return this._footer ? this._footer.numDictionaries : 0
             }
@@ -24620,138 +25351,138 @@
             }
             open(t) {
                 const e = Object.create(null, {
                     open: {
                         get: () => super.open
                     }
                 });
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     if (!this.closed && !this._footer) {
                         this.schema = (this._footer = yield this._readFooter()).schema;
                         for (const t of this._footer.dictionaryBatches()) t && (yield this._readDictionaryBatch(this._dictionaryIndex++))
                     }
                     return yield e.open.call(this, t)
                 }))
             }
             readRecordBatch(t) {
                 var e;
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     if (this.closed) return null;
                     this._footer || (yield this.open());
                     const n = null === (e = this._footer) || void 0 === e ? void 0 : e.getRecordBatch(t);
                     if (n && (yield this._handle.seek(n.offset))) {
-                        const t = yield this._reader.readMessage(na.RecordBatch);
+                        const t = yield this._reader.readMessage(Qa.RecordBatch);
                         if (null === t || void 0 === t ? void 0 : t.isRecordBatch()) {
                             const e = t.header(),
                                 n = yield this._reader.readMessageBody(t.bodyLength);
                             return this._loadRecordBatch(e, n)
                         }
                     }
                     return null
                 }))
             }
             _readDictionaryBatch(t) {
                 var e;
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     const n = null === (e = this._footer) || void 0 === e ? void 0 : e.getDictionaryBatch(t);
                     if (n && (yield this._handle.seek(n.offset))) {
-                        const t = yield this._reader.readMessage(na.DictionaryBatch);
+                        const t = yield this._reader.readMessage(Qa.DictionaryBatch);
                         if (null === t || void 0 === t ? void 0 : t.isDictionaryBatch()) {
                             const e = t.header(),
                                 n = yield this._reader.readMessageBody(t.bodyLength), i = this._loadDictionaryBatch(e, n);
                             this.dictionaries.set(e.id, i)
                         }
                     }
                 }))
             }
             _readFooter() {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     const {
                         _handle: t
                     } = this;
                     t._pending && (yield t._pending);
-                    const e = t.size - vf,
+                    const e = t.size - fp,
                         n = yield t.readInt32(e), i = yield t.readAt(e - n, n);
-                    return Nh.decode(i)
+                    return Dd.decode(i)
                 }))
             }
             _readNextMessageAndValidate(t) {
-                return Oa(this, void 0, void 0, (function*() {
+                return Sl(this, void 0, void 0, (function*() {
                     if (this._footer || (yield this.open()), this._footer && this._recordBatchIndex < this.numRecordBatches) {
                         const e = this._footer.getRecordBatch(this._recordBatchIndex);
                         if (e && (yield this._handle.seek(e.offset))) return yield this._reader.readMessage(t)
                     }
                     return null
                 }))
             }
         }
-        class Af extends If {
+        class kp extends xp {
             constructor(t, e) {
                 super(t, e)
             }
             _loadVectors(t, e, n) {
-                return new ad(e, t.nodes, t.buffers, this.dictionaries).visitMany(n)
+                return new ef(e, t.nodes, t.buffers, this.dictionaries).visitMany(n)
             }
         }
 
-        function Cf(t, e) {
+        function Mp(t, e) {
             return e && "boolean" === typeof e.autoDestroy ? e.autoDestroy : t.autoDestroy
         }
 
-        function* Pf(t) {
-            const e = xf.from(t);
+        function* Ip(t) {
+            const e = gp.from(t);
             try {
                 if (!e.open({
                         autoDestroy: !1
                     }).closed)
                     do {
                         yield e
                     } while (!e.reset().open().closed)
             } finally {
                 e.cancel()
             }
         }
 
-        function Ff(t) {
-            return Ca(this, arguments, (function*() {
-                const e = yield Aa(xf.from(t));
+        function Ep(t) {
+            return Ml(this, arguments, (function*() {
+                const e = yield kl(gp.from(t));
                 try {
-                    if (!(yield Aa(e.open({
+                    if (!(yield kl(e.open({
                             autoDestroy: !1
                         }))).closed)
                         do {
-                            yield yield Aa(e)
-                        } while (!(yield Aa(e.reset().open())).closed)
+                            yield yield kl(e)
+                        } while (!(yield kl(e.reset().open())).closed)
                 } finally {
-                    yield Aa(e.cancel())
+                    yield kl(e.cancel())
                 }
             }))
         }
-        class Lf extends Xl {
+        class Op extends jc {
             constructor() {
                 super(), this._byteLength = 0, this._nodes = [], this._buffers = [], this._bufferRegions = []
             }
             static assemble() {
-                const t = e => e.flatMap((e => Array.isArray(e) ? t(e) : e instanceof ah ? e.data.children : e.data)),
-                    e = new Lf;
+                const t = e => e.flatMap((e => Array.isArray(e) ? t(e) : e instanceof ed ? e.data.children : e.data)),
+                    e = new Op;
                 for (var n = arguments.length, i = new Array(n), r = 0; r < n; r++) i[r] = arguments[r];
                 return e.visitMany(t(i)), e
             }
             visit(t) {
-                if (t instanceof Ru) return this.visitMany(t.data), this;
+                if (t instanceof Ch) return this.visitMany(t.data), this;
                 const {
                     type: e
                 } = t;
-                if (!kl.isDictionary(e)) {
+                if (!vc.isDictionary(e)) {
                     const {
                         length: n,
                         nullCount: i
                     } = t;
                     if (n > 2147483647) throw new RangeError("Cannot write arrays larger than 2^31 - 1 in length");
-                    kl.isNull(e) || Nf.call(this, i <= 0 ? new Uint8Array(0) : yu(t.offset, n, t.nullBitmap)), this.nodes.push(new tf(n, i))
+                    vc.isNull(e) || Dp.call(this, i <= 0 ? new Uint8Array(0) : hh(t.offset, n, t.nullBitmap)), this.nodes.push(new qf(n, i))
                 }
                 return super.visit(t)
             }
             visitNull(t) {
                 return this
             }
             visitDictionary(t) {
@@ -24767,77 +25498,77 @@
                 return this._byteLength
             }
             get bufferRegions() {
                 return this._bufferRegions
             }
         }
 
-        function Nf(t) {
+        function Dp(t) {
             const e = t.byteLength + 7 & -8;
-            return this.buffers.push(t), this.bufferRegions.push(new Jd(this._byteLength, e)), this._byteLength += e, this
+            return this.buffers.push(t), this.bufferRegions.push(new Xf(this._byteLength, e)), this._byteLength += e, this
         }
 
-        function Bf(t) {
-            return Nf.call(this, t.values.subarray(0, t.length * t.stride))
+        function Ap(t) {
+            return Dp.call(this, t.values.subarray(0, t.length * t.stride))
         }
 
-        function Rf(t) {
+        function Cp(t) {
             const {
                 length: e,
                 values: n,
                 valueOffsets: i
             } = t, r = i[0], s = i[e], o = Math.min(s - r, n.byteLength - r);
-            return Nf.call(this, Xa(-i[0], e, i)), Nf.call(this, n.subarray(r, r + o)), this
+            return Dp.call(this, jl(-i[0], e, i)), Dp.call(this, n.subarray(r, r + o)), this
         }
 
-        function zf(t) {
+        function Pp(t) {
             const {
                 length: e,
                 valueOffsets: n
             } = t;
-            return n && Nf.call(this, Xa(n[0], e, n)), this.visit(t.children[0])
+            return n && Dp.call(this, jl(n[0], e, n)), this.visit(t.children[0])
         }
 
-        function Uf(t) {
+        function Fp(t) {
             return this.visitMany(t.type.children.map(((e, n) => t.children[n])).filter(Boolean))[0]
         }
-        Lf.prototype.visitBool = function(t) {
+        Op.prototype.visitBool = function(t) {
             let e;
-            return t.nullCount >= t.length ? Nf.call(this, new Uint8Array(0)) : (e = t.values) instanceof Uint8Array ? Nf.call(this, yu(t.offset, t.length, e)) : Nf.call(this, bu(t.values))
-        }, Lf.prototype.visitInt = Bf, Lf.prototype.visitFloat = Bf, Lf.prototype.visitUtf8 = Rf, Lf.prototype.visitBinary = Rf, Lf.prototype.visitFixedSizeBinary = Bf, Lf.prototype.visitDate = Bf, Lf.prototype.visitTimestamp = Bf, Lf.prototype.visitTime = Bf, Lf.prototype.visitDecimal = Bf, Lf.prototype.visitList = zf, Lf.prototype.visitStruct = Uf, Lf.prototype.visitUnion = function(t) {
+            return t.nullCount >= t.length ? Dp.call(this, new Uint8Array(0)) : (e = t.values) instanceof Uint8Array ? Dp.call(this, hh(t.offset, t.length, e)) : Dp.call(this, dh(t.values))
+        }, Op.prototype.visitInt = Ap, Op.prototype.visitFloat = Ap, Op.prototype.visitUtf8 = Cp, Op.prototype.visitBinary = Cp, Op.prototype.visitFixedSizeBinary = Ap, Op.prototype.visitDate = Ap, Op.prototype.visitTimestamp = Ap, Op.prototype.visitTime = Ap, Op.prototype.visitDecimal = Ap, Op.prototype.visitList = Pp, Op.prototype.visitStruct = Fp, Op.prototype.visitUnion = function(t) {
             const {
                 type: e,
                 length: n,
                 typeIds: i,
                 valueOffsets: r
             } = t;
-            if (Nf.call(this, i), e.mode === Zo.Sparse) return Uf.call(this, t);
-            if (e.mode === Zo.Dense) {
-                if (t.offset <= 0) return Nf.call(this, r), Uf.call(this, t);
+            if (Dp.call(this, i), e.mode === Ya.Sparse) return Fp.call(this, t);
+            if (e.mode === Ya.Dense) {
+                if (t.offset <= 0) return Dp.call(this, r), Fp.call(this, t);
                 {
                     const s = i.reduce(((t, e) => Math.max(t, e)), i[0]),
                         o = new Int32Array(s + 1),
                         a = new Int32Array(s + 1).fill(-1),
                         l = new Int32Array(n),
-                        c = Xa(-r[0], n, r);
+                        c = jl(-r[0], n, r);
                     for (let t, e, r = -1; ++r < n;) - 1 === (e = a[t = i[r]]) && (e = a[t] = c[t]), l[r] = c[r] - e, ++o[t];
-                    Nf.call(this, l);
+                    Dp.call(this, l);
                     for (let i, r = -1, u = e.children.length; ++r < u;)
                         if (i = t.children[r]) {
                             const t = e.typeIds[r],
                                 s = Math.min(n, o[t]);
                             this.visit(i.slice(a[t], s))
                         }
                 }
             }
             return this
-        }, Lf.prototype.visitInterval = Bf, Lf.prototype.visitFixedSizeList = zf, Lf.prototype.visitMap = zf;
-        class Vf extends Yh {
+        }, Op.prototype.visitInterval = Ap, Op.prototype.visitFixedSizeList = Pp, Op.prototype.visitMap = Pp;
+        class Lp extends zd {
             constructor(t) {
-                super(), this._position = 0, this._started = !1, this._sink = new Kh, this._schema = null, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, ma(t) || (t = {
+                super(), this._position = 0, this._started = !1, this._sink = new Vd, this._schema = null, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, ul(t) || (t = {
                     autoDestroy: !0,
                     writeLegacyIpcFormat: !1
                 }), this._autoDestroy = "boolean" !== typeof t.autoDestroy || t.autoDestroy, this._writeLegacyIpcFormat = "boolean" === typeof t.writeLegacyIpcFormat && t.writeLegacyIpcFormat
             }
             static throughNode(t) {
                 throw new Error('"throughNode" not available in this environment')
             }
@@ -24849,15 +25580,15 @@
                 return this._sink.toString(t)
             }
             toUint8Array() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
                 return this._sink.toUint8Array(t)
             }
             writeAll(t) {
-                return ya(t) ? t.then((t => this.writeAll(t))) : va(t) ? Yf(this, t) : Hf(this, t)
+                return hl(t) ? t.then((t => this.writeAll(t))) : fl(t) ? zp(this, t) : Rp(this, t)
             }
             get closed() {
                 return this._sink.closed
             } [Symbol.asyncIterator]() {
                 return this._sink[Symbol.asyncIterator]()
             }
             toDOMStream(t) {
@@ -24875,78 +25606,78 @@
             finish() {
                 return this._autoDestroy ? this.close() : this.reset(this._sink, this._schema), this
             }
             reset() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this._sink,
                     e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null;
                 var n;
-                return t === this._sink || t instanceof Kh ? this._sink = t : (this._sink = new Kh, t && (ma(n = t) && ga(n.abort) && ga(n.getWriter) && !Ta(n)) ? this.toDOMStream({
+                return t === this._sink || t instanceof Vd ? this._sink = t : (this._sink = new Vd, t && (ul(n = t) && cl(n.abort) && cl(n.getWriter) && !bl(n)) ? this.toDOMStream({
                     type: "bytes"
-                }).pipeTo(t) : t && (t => ma(t) && ga(t.end) && ga(t.write) && pa(t.writable) && !Ta(t))(t) && this.toNodeStream({
+                }).pipeTo(t) : t && (t => ul(t) && cl(t.end) && cl(t.write) && ll(t.writable) && !bl(t))(t) && this.toNodeStream({
                     objectMode: !1
-                }).pipe(t)), this._started && this._schema && this._writeFooter(this._schema), this._started = !1, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, e && rh(e, this._schema) || (null == e ? (this._position = 0, this._schema = null) : (this._started = !0, this._schema = e, this._writeSchema(e))), this
+                }).pipe(t)), this._started && this._schema && this._writeFooter(this._schema), this._started = !1, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, e && Gh(e, this._schema) || (null == e ? (this._position = 0, this._schema = null) : (this._started = !0, this._schema = e, this._writeSchema(e))), this
             }
             write(t) {
                 let e = null;
                 if (!this._sink) throw new Error("RecordBatchWriter is closed");
                 if (null == t) return this.finish() && void 0;
-                if (t instanceof fh && !(e = t.schema)) return this.finish() && void 0;
-                if (t instanceof ah && !(e = t.schema)) return this.finish() && void 0;
-                if (e && !rh(e, this._schema)) {
+                if (t instanceof ad && !(e = t.schema)) return this.finish() && void 0;
+                if (t instanceof ed && !(e = t.schema)) return this.finish() && void 0;
+                if (e && !Gh(e, this._schema)) {
                     if (this._started && this._autoDestroy) return this.close();
                     this.reset(this._sink, e)
                 }
-                t instanceof ah ? t instanceof uh || this._writeRecordBatch(t) : t instanceof fh ? this.writeAll(t.batches) : ba(t) && this.writeAll(t)
+                t instanceof ed ? t instanceof rd || this._writeRecordBatch(t) : t instanceof ad ? this.writeAll(t.batches) : dl(t) && this.writeAll(t)
             }
             _writeMessage(t) {
                 const e = (arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 8) - 1,
-                    n = Qd.encode(t),
+                    n = Yf.encode(t),
                     i = n.byteLength,
                     r = this._writeLegacyIpcFormat ? 4 : 8,
                     s = i + r + e & ~e,
                     o = s - i - r;
-                return t.headerType === na.RecordBatch ? this._recordBatchBlocks.push(new Rh(s, t.bodyLength, this._position)) : t.headerType === na.DictionaryBatch && this._dictionaryBlocks.push(new Rh(s, t.bodyLength, this._position)), this._writeLegacyIpcFormat || this._write(Int32Array.of(-1)), this._write(Int32Array.of(s - r)), i > 0 && this._write(n), this._writePadding(o)
+                return t.headerType === Qa.RecordBatch ? this._recordBatchBlocks.push(new Cd(s, t.bodyLength, this._position)) : t.headerType === Qa.DictionaryBatch && this._dictionaryBlocks.push(new Cd(s, t.bodyLength, this._position)), this._writeLegacyIpcFormat || this._write(Int32Array.of(-1)), this._write(Int32Array.of(s - r)), i > 0 && this._write(n), this._writePadding(o)
             }
             _write(t) {
                 if (this._started) {
-                    const e = Ha(t);
+                    const e = Rl(t);
                     e && e.byteLength > 0 && (this._sink.write(e), this._position += e.byteLength)
                 }
                 return this
             }
             _writeSchema(t) {
-                return this._writeMessage(Qd.from(t))
+                return this._writeMessage(Yf.from(t))
             }
             _writeFooter(t) {
                 return this._writeLegacyIpcFormat ? this._write(Int32Array.of(0)) : this._write(Int32Array.of(-1, 0))
             }
             _writeMagic() {
-                return this._write(mf)
+                return this._write(up)
             }
             _writePadding(t) {
                 return t > 0 ? this._write(new Uint8Array(t)) : this
             }
             _writeRecordBatch(t) {
                 const {
                     byteLength: e,
                     nodes: n,
                     bufferRegions: i,
                     buffers: r
-                } = Lf.assemble(t), s = new Zd(t.numRows, n, i), o = Qd.from(s, e);
+                } = Op.assemble(t), s = new $f(t.numRows, n, i), o = Yf.from(s, e);
                 return this._writeDictionaries(t)._writeMessage(o)._writeBodyBuffers(r)
             }
             _writeDictionaryBatch(t, e) {
                 let n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2];
                 this._dictionaryDeltaOffsets.set(e, t.length + (this._dictionaryDeltaOffsets.get(e) || 0));
                 const {
                     byteLength: i,
                     nodes: r,
                     bufferRegions: s,
                     buffers: o
-                } = Lf.assemble(new Ru([t])), a = new Zd(t.length, r, s), l = new Gd(a, e, n), c = Qd.from(l, i);
+                } = Op.assemble(new Ch([t])), a = new $f(t.length, r, s), l = new Kf(a, e, n), c = Yf.from(l, i);
                 return this._writeMessage(c)._writeBodyBuffers(o)
             }
             _writeBodyBuffers(t) {
                 let e, n, i;
                 for (let r = -1, s = t.length; ++r < s;)(e = t[r]) && (n = e.byteLength) > 0 && (this._write(e), (i = (n + 7 & -8) - n) > 0 && this._writePadding(i));
                 return this
             }
@@ -24955,49 +25686,49 @@
                     let t = this._dictionaryDeltaOffsets.get(e) || 0;
                     if (0 === t || (n = null === n || void 0 === n ? void 0 : n.slice(t)).length > 0)
                         for (const i of n.data) this._writeDictionaryBatch(i, e, t > 0), t += i.length
                 }
                 return this
             }
         }
-        class jf extends Vf {
+        class Np extends Lp {
             static writeAll(t, e) {
-                const n = new jf(e);
-                return ya(t) ? t.then((t => n.writeAll(t))) : va(t) ? Yf(n, t) : Hf(n, t)
+                const n = new Np(e);
+                return hl(t) ? t.then((t => n.writeAll(t))) : fl(t) ? zp(n, t) : Rp(n, t)
             }
         }
-        class Wf extends Vf {
+        class Bp extends Lp {
             static writeAll(t) {
-                const e = new Wf;
-                return ya(t) ? t.then((t => e.writeAll(t))) : va(t) ? Yf(e, t) : Hf(e, t)
+                const e = new Bp;
+                return hl(t) ? t.then((t => e.writeAll(t))) : fl(t) ? zp(e, t) : Rp(e, t)
             }
             constructor() {
                 super(), this._autoDestroy = !0
             }
             _writeSchema(t) {
                 return this._writeMagic()._writePadding(2)
             }
             _writeFooter(t) {
-                const e = Nh.encode(new Nh(t, Qo.V4, this._recordBatchBlocks, this._dictionaryBlocks));
+                const e = Dd.encode(new Dd(t, Ha.V4, this._recordBatchBlocks, this._dictionaryBlocks));
                 return super._writeFooter(t)._write(e)._write(Int32Array.of(e.byteLength))._writeMagic()
             }
         }
 
-        function Hf(t, e) {
+        function Rp(t, e) {
             let n = e;
-            e instanceof fh && (n = e.batches, t.reset(void 0, e.schema));
+            e instanceof ad && (n = e.batches, t.reset(void 0, e.schema));
             for (const i of n) t.write(i);
             return t.finish()
         }
 
-        function Yf(t, e) {
+        function zp(t, e) {
             var n, i, r, s;
-            return Oa(this, void 0, void 0, (function*() {
+            return Sl(this, void 0, void 0, (function*() {
                 try {
-                    for (n = Fa(e); !(i = yield n.next()).done;) {
+                    for (n = El(e); !(i = yield n.next()).done;) {
                         const e = i.value;
                         t.write(e)
                     }
                 } catch (o) {
                     r = {
                         error: o
                     }
@@ -25008,23 +25739,23 @@
                         if (r) throw r.error
                     }
                 }
                 return t.finish()
             }))
         }
 
-        function $f(t) {
-            const e = xf.from(t);
-            return ya(e) ? e.then((t => $f(t))) : e.isAsync() ? e.readAll().then((t => new fh(t))) : new fh(e.readAll())
+        function Up(t) {
+            const e = gp.from(t);
+            return hl(e) ? e.then((t => Up(t))) : e.isAsync() ? e.readAll().then((t => new ad(t))) : new ad(e.readAll())
         }
 
-        function Kf(t) {
-            return ("stream" === (arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "stream") ? jf : Wf).writeAll(t).toUint8Array(!0)
+        function Vp(t) {
+            return ("stream" === (arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "stream") ? Np : Bp).writeAll(t).toUint8Array(!0)
         }
-        var Xf, qf = function() {
+        var jp, Wp = function() {
                 function t(t, e, n, i) {
                     var r = this;
                     this.getCell = function(t, e) {
                         var n = t < r.headerRows && e < r.headerColumns,
                             i = t >= r.headerRows && e < r.headerColumns,
                             s = t < r.headerRows && e >= r.headerColumns;
                         if (n) {
@@ -25055,18 +25786,18 @@
                             type: "data",
                             id: "T_".concat(r.uuid, "row").concat(a, "_col").concat(l),
                             classNames: o.join(" "),
                             content: c
                         }
                     }, this.getContent = function(t, e, n) {
                         var i = t.getChildAt(n);
-                        return null === i ? "" : r.getColumnTypeId(t, n) === ia.Timestamp ? r.nanosToDate(i.get(e)) : i.get(e)
-                    }, this.dataTable = $f(t), this.indexTable = $f(e), this.columnsTable = $f(n), this.styler = i ? {
+                        return null === i ? "" : r.getColumnTypeId(t, n) === Za.Timestamp ? r.nanosToDate(i.get(e)) : i.get(e)
+                    }, this.dataTable = Up(t), this.indexTable = Up(e), this.columnsTable = Up(n), this.styler = i ? {
                         caption: i.caption,
-                        displayValuesTable: $f(i.displayValues),
+                        displayValuesTable: Up(i.displayValues),
                         styles: i.styles,
                         uuid: i.uuid
                     } : void 0
                 }
                 return Object.defineProperty(t.prototype, "rows", {
                     get: function() {
                         return this.indexTable.numRows + this.columnsTable.numCols
@@ -25137,66 +25868,66 @@
                     get: function() {
                         return this.columnsTable
                     },
                     enumerable: !1,
                     configurable: !0
                 }), t.prototype.serialize = function() {
                     return {
-                        data: Kf(this.dataTable),
-                        index: Kf(this.indexTable),
-                        columns: Kf(this.columnsTable)
+                        data: Vp(this.dataTable),
+                        index: Vp(this.indexTable),
+                        columns: Vp(this.columnsTable)
                     }
                 }, t.prototype.getColumnTypeId = function(t, e) {
                     return t.schema.fields[e].type.typeId
                 }, t.prototype.nanosToDate = function(t) {
                     return new Date(t / 1e6)
                 }, t
             }(),
-            Qf = function() {
-                return Qf = Object.assign || function(t) {
+            Hp = function() {
+                return Hp = Object.assign || function(t) {
                     for (var e, n = 1, i = arguments.length; n < i; n++)
                         for (var r in e = arguments[n]) Object.prototype.hasOwnProperty.call(e, r) && (t[r] = e[r]);
                     return t
-                }, Qf.apply(this, arguments)
+                }, Hp.apply(this, arguments)
             };
         ! function(t) {
             t.COMPONENT_READY = "streamlit:componentReady", t.SET_COMPONENT_VALUE = "streamlit:setComponentValue", t.SET_FRAME_HEIGHT = "streamlit:setFrameHeight"
-        }(Xf || (Xf = {}));
-        var Zf = function() {
+        }(jp || (jp = {}));
+        var Yp = function() {
                 function t() {}
                 return t.API_VERSION = 1, t.RENDER_EVENT = "streamlit:render", t.events = new EventTarget, t.registeredMessageListener = !1, t.setComponentReady = function() {
-                    t.registeredMessageListener || (window.addEventListener("message", t.onMessageEvent), t.registeredMessageListener = !0), t.sendBackMsg(Xf.COMPONENT_READY, {
+                    t.registeredMessageListener || (window.addEventListener("message", t.onMessageEvent), t.registeredMessageListener = !0), t.sendBackMsg(jp.COMPONENT_READY, {
                         apiVersion: t.API_VERSION
                     })
                 }, t.setFrameHeight = function(e) {
-                    void 0 === e && (e = document.body.scrollHeight), e !== t.lastFrameHeight && (t.lastFrameHeight = e, t.sendBackMsg(Xf.SET_FRAME_HEIGHT, {
+                    void 0 === e && (e = document.body.scrollHeight), e !== t.lastFrameHeight && (t.lastFrameHeight = e, t.sendBackMsg(jp.SET_FRAME_HEIGHT, {
                         height: e
                     }))
                 }, t.setComponentValue = function(e) {
                     var n;
-                    e instanceof qf ? (n = "dataframe", e = e.serialize()) : ! function(t) {
+                    e instanceof Wp ? (n = "dataframe", e = e.serialize()) : ! function(t) {
                         var e = !1;
                         try {
                             e = t instanceof BigInt64Array || t instanceof BigUint64Array
                         } catch (n) {}
                         return t instanceof Int8Array || t instanceof Uint8Array || t instanceof Uint8ClampedArray || t instanceof Int16Array || t instanceof Uint16Array || t instanceof Int32Array || t instanceof Uint32Array || t instanceof Float32Array || t instanceof Float64Array || e
-                    }(e) ? e instanceof ArrayBuffer ? (n = "bytes", e = new Uint8Array(e)) : n = "json" : (n = "bytes", e = new Uint8Array(e.buffer)), t.sendBackMsg(Xf.SET_COMPONENT_VALUE, {
+                    }(e) ? e instanceof ArrayBuffer ? (n = "bytes", e = new Uint8Array(e)) : n = "json" : (n = "bytes", e = new Uint8Array(e.buffer)), t.sendBackMsg(jp.SET_COMPONENT_VALUE, {
                         value: e,
                         dataType: n
                     })
                 }, t.onMessageEvent = function(e) {
                     if (e.data.type === t.RENDER_EVENT) t.onRenderMessage(e.data)
                 }, t.onRenderMessage = function(e) {
                     var n = e.args;
                     null == n && (console.error("Got null args in onRenderMessage. This should never happen"), n = {});
                     var i = e.dfs && e.dfs.length > 0 ? t.argsDataframeToObject(e.dfs) : {};
-                    n = Qf(Qf({}, n), i);
+                    n = Hp(Hp({}, n), i);
                     var r = Boolean(e.disabled),
                         s = e.theme;
-                    s && Gf(s);
+                    s && $p(s);
                     var o = {
                             disabled: r,
                             args: n,
                             theme: s
                         },
                         a = new CustomEvent(t.RENDER_EVENT, {
                             detail: o
@@ -25210,27 +25941,27 @@
                     }));
                     return Object.fromEntries(n)
                 }, t.toArrowTable = function(t) {
                     var e, n = (e = t.data).data,
                         i = e.index,
                         r = e.columns,
                         s = e.styler;
-                    return new qf(n, i, r, s)
+                    return new Wp(n, i, r, s)
                 }, t.sendBackMsg = function(t, e) {
-                    window.parent.postMessage(Qf({
+                    window.parent.postMessage(Hp({
                         isStreamlitMessage: !0,
                         type: t
                     }, e), "*")
                 }, t
             }(),
-            Gf = function(t) {
+            $p = function(t) {
                 var e = document.createElement("style");
                 document.head.appendChild(e), e.innerHTML = "\n    :root {\n      --primary-color: ".concat(t.primaryColor, ";\n      --background-color: ").concat(t.backgroundColor, ";\n      --secondary-background-color: ").concat(t.secondaryBackgroundColor, ";\n      --text-color: ").concat(t.textColor, ";\n      --font: ").concat(t.font, ";\n    }\n\n    body {\n      background-color: var(--background-color);\n      color: var(--text-color);\n    }\n  ")
             };
-        var Jf = function() {
+        var Kp = function() {
                 var t = function(e, n) {
                     return t = Object.setPrototypeOf || {
                         __proto__: []
                     }
                     instanceof Array && function(t, e) {
                         t.__proto__ = e
                     } || function(t, e) {
@@ -25242,787 +25973,148 @@
 
                     function i() {
                         this.constructor = e
                     }
                     t(e, n), e.prototype = null === n ? Object.create(n) : (i.prototype = n.prototype, new i)
                 }
             }(),
-            tp = function(t) {
+            Xp = function(t) {
                 function e() {
                     return null !== t && t.apply(this, arguments) || this
                 }
-                return Jf(e, t), e.prototype.componentDidMount = function() {
-                    Zf.setFrameHeight()
+                return Kp(e, t), e.prototype.componentDidMount = function() {
+                    Yp.setFrameHeight()
                 }, e.prototype.componentDidUpdate = function() {
-                    Zf.setFrameHeight()
+                    Yp.setFrameHeight()
                 }, e
             }(t.PureComponent);
-        var ep = n(895),
-            np = n.n(ep);
-        const ip = t => t && t.enabled && t.modifierKey,
-            rp = (t, e) => t && e[t + "Key"],
-            sp = (t, e) => t && !e[t + "Key"];
-
-        function op(t, e, n) {
-            return void 0 === t || ("string" === typeof t ? -1 !== t.indexOf(e) : "function" === typeof t && -1 !== t({
-                chart: n
-            }).indexOf(e))
-        }
 
-        function ap(t, e) {
-            return "function" === typeof t && (t = t({
-                chart: e
-            })), "string" === typeof t ? {
-                x: -1 !== t.indexOf("x"),
-                y: -1 !== t.indexOf("y")
-            } : {
-                x: !1,
-                y: !1
-            }
-        }
-
-        function lp(t, e, n) {
-            const {
-                mode: i = "xy",
-                scaleMode: r,
-                overScaleMode: s
-            } = t || {}, o = function(t, e) {
-                let {
-                    x: n,
-                    y: i
-                } = t;
-                const r = e.scales,
-                    s = Object.keys(r);
-                for (let o = 0; o < s.length; o++) {
-                    const t = r[s[o]];
-                    if (i >= t.top && i <= t.bottom && n >= t.left && n <= t.right) return t
+        function qp(t, e) {
+            const n = Object.entries(t).map(((t, e) => {
+                let [n, i] = t;
+                return {
+                    data: Object.values(i),
+                    label: n,
+                    fill: !1,
+                    lineTension: .3,
+                    cubicInterpolationMode: "monotone"
                 }
-                return null
-            }(e, n), a = ap(i, n), l = ap(r, n);
-            if (s) {
-                const t = ap(s, n);
-                for (const e of ["x", "y"]) t[e] && (l[e] = a[e], a[e] = !1)
+            }));
+            return e && e.colors && n.forEach(((t, n) => {
+                t.backgroundColor = e.colors[n], t.borderColor = e.colors[n]
+            })), {
+                labels: Object.keys(t.Col1),
+                datasets: n
             }
-            if (o && l[o.axis]) return [o];
-            const c = [];
-            return q(n.scales, (function(t) {
-                a[t.axis] && c.push(t)
-            })), c
-        }
-        const cp = new WeakMap;
-
-        function up(t) {
-            let e = cp.get(t);
-            return e || (e = {
-                originalScaleLimits: {},
-                updatedScaleLimits: {},
-                handlers: {},
-                panDelta: {}
-            }, cp.set(t, e)), e
         }
 
-        function hp(t, e, n) {
-            const i = t.max - t.min,
-                r = i * (e - 1),
-                s = t.isHorizontal() ? n.x : n.y,
-                o = Math.max(0, Math.min(1, (t.getValueForPixel(s) - t.min) / i || 0));
+        function Qp(t, e) {
             return {
-                min: r * o,
-                max: r * (1 - o)
-            }
-        }
-
-        function dp(t, e, n, i, r) {
-            let s = n[i];
-            if ("original" === s) {
-                const n = t.originalScaleLimits[e.id][i];
-                s = $(n.options, n.scale)
-            }
-            return $(s, r)
-        }
-
-        function fp(t, e, n) {
-            let {
-                min: i,
-                max: r
-            } = e, s = arguments.length > 3 && void 0 !== arguments[3] && arguments[3];
-            const o = up(t.chart),
-                {
-                    id: a,
-                    axis: l,
-                    options: c
-                } = t,
-                u = n && (n[a] || n[l]) || {},
-                {
-                    minRange: h = 0
-                } = u,
-                d = dp(o, t, u, "min", -1 / 0),
-                f = dp(o, t, u, "max", 1 / 0),
-                p = s ? Math.max(r - i, h) : t.max - t.min,
-                g = (p - r + i) / 2;
-            return i -= g, r += g, i < d ? (i = d, r = Math.min(d + p, f)) : r > f && (r = f, i = Math.max(f - p, d)), c.min = i, c.max = r, o.updatedScaleLimits[t.id] = {
-                min: i,
-                max: r
-            }, t.parse(i) !== t.min || t.parse(r) !== t.max
-        }
-        const pp = t => 0 === t || isNaN(t) ? 0 : t < 0 ? Math.min(Math.round(t), -1) : Math.max(Math.round(t), 1);
-        const gp = {
-            second: 500,
-            minute: 3e4,
-            hour: 18e5,
-            day: 432e5,
-            week: 3024e5,
-            month: 1296e6,
-            quarter: 5184e6,
-            year: 157248e5
-        };
-
-        function mp(t, e, n) {
-            let i = arguments.length > 3 && void 0 !== arguments[3] && arguments[3];
-            const {
-                min: r,
-                max: s,
-                options: o
-            } = t, a = o.time && o.time.round, l = gp[a] || 0, c = t.getValueForPixel(t.getPixelForValue(r + l) - e), u = t.getValueForPixel(t.getPixelForValue(s + l) - e), {
-                min: h = -1 / 0,
-                max: d = 1 / 0
-            } = i && n && n[t.axis] || {};
-            return !!(isNaN(c) || isNaN(u) || c < h || u > d) || fp(t, {
-                min: c,
-                max: u
-            }, n, i)
-        }
-
-        function yp(t, e, n) {
-            return mp(t, e, n, !0)
-        }
-        const bp = {
-                category: function(t, e, n, i) {
-                    const r = hp(t, e, n);
-                    return t.min === t.max && e < 1 && function(t) {
-                        const e = t.getLabels().length - 1;
-                        t.min > 0 && (t.min -= 1), t.max < e && (t.max += 1)
-                    }(t), fp(t, {
-                        min: t.min + pp(r.min),
-                        max: t.max - pp(r.max)
-                    }, i, !0)
+                responsive: !0,
+                animation: {
+                    duration: 0
                 },
-                default: function(t, e, n, i) {
-                    const r = hp(t, e, n);
-                    return fp(t, {
-                        min: t.min + r.min,
-                        max: t.max - r.max
-                    }, i, !0)
-                }
-            },
-            vp = {
-                default: function(t, e, n, i) {
-                    fp(t, function(t, e, n) {
-                        const i = t.getValueForPixel(e),
-                            r = t.getValueForPixel(n);
-                        return {
-                            min: Math.min(i, r),
-                            max: Math.max(i, r)
-                        }
-                    }(t, e, n), i, !0)
-                }
-            },
-            _p = {
-                category: function(t, e, n) {
-                    const i = t.getLabels().length - 1;
-                    let {
-                        min: r,
-                        max: s
-                    } = t;
-                    const o = Math.max(s - r, 1),
-                        a = Math.round(function(t) {
-                            return t.isHorizontal() ? t.width : t.height
-                        }(t) / Math.max(o, 10)),
-                        l = Math.round(Math.abs(e / a));
-                    let c;
-                    return e < -a ? (s = Math.min(s + l, i), r = 1 === o ? s : s - o, c = s === i) : e > a && (r = Math.max(0, r - l), s = 1 === o ? r : r + o, c = 0 === r), fp(t, {
-                        min: r,
-                        max: s
-                    }, n) || c
+                tooltips: {
+                    mode: "nearest"
                 },
-                default: mp,
-                logarithmic: yp,
-                timeseries: yp
-            };
-
-        function xp(t, e) {
-            q(t, ((n, i) => {
-                e[i] || delete t[i]
-            }))
-        }
-
-        function wp(t, e) {
-            const {
-                scales: n
-            } = t, {
-                originalScaleLimits: i,
-                updatedScaleLimits: r
-            } = e;
-            return q(n, (function(t) {
-                (function(t, e, n) {
-                    const {
-                        id: i,
-                        options: {
-                            min: r,
-                            max: s
+                onHover: (t, e) => {
+                    e.length > 0 ? t.native.target.style.cursor = "crosshair" : t.native.target.style.cursor = "default"
+                },
+                plugins: {
+                    zoom: {
+                        zoom: {
+                            wheel: {
+                                enabled: !0
+                            },
+                            mode: "x"
+                        },
+                        pan: {
+                            enabled: !1
                         }
-                    } = t;
-                    if (!e[i] || !n[i]) return !0;
-                    const o = n[i];
-                    return o.min !== r || o.max !== s
-                })(t, i, r) && (i[t.id] = {
-                    min: {
-                        scale: t.min,
-                        options: t.options.min
                     },
-                    max: {
-                        scale: t.max,
-                        options: t.options.max
-                    }
-                })
-            })), xp(i, n), xp(r, n), i
-        }
-
-        function Sp(t, e, n, i) {
-            X(bp[t.type] || bp.default, [t, e, n, i])
-        }
-
-        function Tp(t, e, n, i, r) {
-            X(vp[t.type] || vp.default, [t, e, n, i, r])
-        }
-
-        function kp(t) {
-            const e = t.chartArea;
-            return {
-                x: (e.left + e.right) / 2,
-                y: (e.top + e.bottom) / 2
-            }
-        }
-
-        function Mp(t, e) {
-            let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "none";
-            const {
-                x: i = 1,
-                y: r = 1,
-                focalPoint: s = kp(t)
-            } = "number" === typeof e ? {
-                x: e,
-                y: e
-            } : e, o = up(t), {
-                options: {
-                    limits: a,
-                    zoom: l
-                }
-            } = o;
-            wp(t, o);
-            const c = 1 !== i,
-                u = 1 !== r;
-            q(lp(l, s, t) || t.scales, (function(t) {
-                t.isHorizontal() && c ? Sp(t, i, s, a) : !t.isHorizontal() && u && Sp(t, r, s, a)
-            })), t.update(n), X(l.onZoom, [{
-                chart: t
-            }])
-        }
-
-        function Ip(t, e, n) {
-            let i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : "none";
-            const r = up(t),
-                {
-                    options: {
-                        limits: s,
-                        zoom: o
+                    title: Zp(t),
+                    legend: {
+                        onHover: (t, e, n) => {
+                            t.native.target.style.cursor = e ? "pointer" : "default"
+                        }
                     }
-                } = r,
-                {
-                    mode: a = "xy"
-                } = o;
-            wp(t, r);
-            const l = op(a, "x", t),
-                c = op(a, "y", t);
-            q(t.scales, (function(t) {
-                t.isHorizontal() && l ? Tp(t, e.x, n.x, s) : !t.isHorizontal() && c && Tp(t, e.y, n.y, s)
-            })), t.update(i), X(o.onZoom, [{
-                chart: t
-            }])
-        }
-
-        function Ep(t) {
-            const e = up(t);
-            let n = 1,
-                i = 1;
-            return q(t.scales, (function(t) {
-                const r = function(t, e) {
-                    const n = t.originalScaleLimits[e];
-                    if (!n) return;
-                    const {
-                        min: i,
-                        max: r
-                    } = n;
-                    return $(r.options, r.scale) - $(i.options, i.scale)
-                }(e, t.id);
-                if (r) {
-                    const e = Math.round(r / (t.max - t.min) * 100) / 100;
-                    n = Math.min(n, e), i = Math.max(i, e)
-                }
-            })), n < 1 ? n : i
-        }
-
-        function Op(t, e, n, i) {
-            const {
-                panDelta: r
-            } = i, s = r[t.id] || 0;
-            bt(s) === bt(e) && (e += s);
-            X(_p[t.type] || _p.default, [t, e, n]) ? r[t.id] = 0 : r[t.id] = e
-        }
-
-        function Dp(t, e, n) {
-            let i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : "none";
-            const {
-                x: r = 0,
-                y: s = 0
-            } = "number" === typeof e ? {
-                x: e,
-                y: e
-            } : e, o = up(t), {
-                options: {
-                    pan: a,
-                    limits: l
-                }
-            } = o, {
-                onPan: c
-            } = a || {};
-            wp(t, o);
-            const u = 0 !== r,
-                h = 0 !== s;
-            q(n || t.scales, (function(t) {
-                t.isHorizontal() && u ? Op(t, r, l, o) : !t.isHorizontal() && h && Op(t, s, l, o)
-            })), t.update(i), X(c, [{
-                chart: t
-            }])
-        }
-
-        function Ap(t) {
-            const e = up(t);
-            wp(t, e);
-            const n = {};
-            for (const i of Object.keys(t.scales)) {
-                const {
-                    min: t,
-                    max: r
-                } = e.originalScaleLimits[i] || {
-                    min: {},
-                    max: {}
-                };
-                n[i] = {
-                    min: t.scale,
-                    max: r.scale
-                }
-            }
-            return n
-        }
-
-        function Cp(t, e) {
-            const {
-                handlers: n
-            } = up(t), i = n[e];
-            i && i.target && (i.target.removeEventListener(e, i), delete n[e])
-        }
-
-        function Pp(t, e, n, i) {
-            const {
-                handlers: r,
-                options: s
-            } = up(t), o = r[n];
-            o && o.target === e || (Cp(t, n), r[n] = e => i(t, e, s), r[n].target = e, e.addEventListener(n, r[n]))
-        }
-
-        function Fp(t, e) {
-            const n = up(t);
-            n.dragStart && (n.dragging = !0, n.dragEnd = e, t.update("none"))
-        }
-
-        function Lp(t, e) {
-            const n = up(t);
-            n.dragStart && "Escape" === e.key && (Cp(t, "keydown"), n.dragging = !1, n.dragStart = n.dragEnd = null, t.update("none"))
-        }
-
-        function Np(t, e, n) {
-            const {
-                onZoomStart: i,
-                onZoomRejected: r
-            } = n;
-            if (i) {
-                if (!1 === X(i, [{
-                        chart: t,
-                        event: e,
-                        point: hn(e, t)
-                    }])) return X(r, [{
-                    chart: t,
-                    event: e
-                }]), !1
+                },
+                scales: Gp(t, e)
             }
         }
 
-        function Bp(t, e) {
-            const n = up(t),
-                {
-                    pan: i,
-                    zoom: r = {}
-                } = n.options;
-            if (0 !== e.button || rp(ip(i), e) || sp(ip(r.drag), e)) return X(r.onZoomRejected, [{
-                chart: t,
-                event: e
-            }]);
-            !1 !== Np(t, e, r) && (n.dragStart = e, Pp(t, t.canvas, "mousemove", Fp), Pp(t, window.document, "keydown", Lp))
-        }
-
-        function Rp(t, e, n, i) {
-            const r = op(e, "x", t),
-                s = op(e, "y", t);
-            let {
-                top: o,
-                left: a,
-                right: l,
-                bottom: c,
-                width: u,
-                height: h
-            } = t.chartArea;
-            const d = hn(n, t),
-                f = hn(i, t);
-            r && (a = Math.min(d.x, f.x), l = Math.max(d.x, f.x)), s && (o = Math.min(d.y, f.y), c = Math.max(d.y, f.y));
-            const p = l - a,
-                g = c - o;
+        function Zp(t) {
             return {
-                left: a,
-                top: o,
-                right: l,
-                bottom: c,
-                width: p,
-                height: g,
-                zoomX: r && p ? 1 + (u - p) / u : 1,
-                zoomY: s && g ? 1 + (h - g) / h : 1
-            }
-        }
-
-        function zp(t, e) {
-            const n = up(t);
-            if (!n.dragStart) return;
-            Cp(t, "mousemove");
-            const {
-                mode: i,
-                onZoomComplete: r,
-                drag: {
-                    threshold: s = 0
-                }
-            } = n.options.zoom, o = Rp(t, i, n.dragStart, e), a = op(i, "x", t) ? o.width : 0, l = op(i, "y", t) ? o.height : 0, c = Math.sqrt(a * a + l * l);
-            if (n.dragStart = n.dragEnd = null, c <= s) return n.dragging = !1, void t.update("none");
-            Ip(t, {
-                x: o.left,
-                y: o.top
-            }, {
-                x: o.right,
-                y: o.bottom
-            }, "zoom"), setTimeout((() => n.dragging = !1), 500), X(r, [{
-                chart: t
-            }])
-        }
-
-        function Up(t, e) {
-            const {
-                handlers: {
-                    onZoomComplete: n
-                },
-                options: {
-                    zoom: i
-                }
-            } = up(t);
-            if (! function(t, e, n) {
-                    if (sp(ip(n.wheel), e)) X(n.onZoomRejected, [{
-                        chart: t,
-                        event: e
-                    }]);
-                    else if (!1 !== Np(t, e, n) && (e.cancelable && e.preventDefault(), void 0 !== e.deltaY)) return !0
-                }(t, e, i)) return;
-            const r = e.target.getBoundingClientRect(),
-                s = 1 + (e.deltaY >= 0 ? -i.wheel.speed : i.wheel.speed);
-            Mp(t, {
-                x: s,
-                y: s,
-                focalPoint: {
-                    x: e.clientX - r.left,
-                    y: e.clientY - r.top
-                }
-            }), n && n()
-        }
-
-        function Vp(t, e, n, i) {
-            n && (up(t).handlers[e] = function(t, e) {
-                let n;
-                return function() {
-                    return clearTimeout(n), n = setTimeout(t, e), e
-                }
-            }((() => X(n, [{
-                chart: t
-            }])), i))
-        }
-
-        function jp(t, e) {
-            return function(n, i) {
-                const {
-                    pan: r,
-                    zoom: s = {}
-                } = e.options;
-                if (!r || !r.enabled) return !1;
-                const o = i && i.srcEvent;
-                return !o || (!(!e.panning && "mouse" === i.pointerType && (sp(ip(r), o) || rp(ip(s.drag), o))) || (X(r.onPanRejected, [{
-                    chart: t,
-                    event: i
-                }]), !1))
+                display: !0,
+                text: t.title
             }
         }
 
-        function Wp(t, e, n) {
-            if (e.scale) {
-                const {
-                    center: i,
-                    pointers: r
-                } = n, s = 1 / e.scale * n.scale, o = n.target.getBoundingClientRect(), a = function(t, e) {
-                    const n = Math.abs(t.clientX - e.clientX),
-                        i = Math.abs(t.clientY - e.clientY),
-                        r = n / i;
-                    let s, o;
-                    return r > .3 && r < 1.7 ? s = o = !0 : n > i ? s = !0 : o = !0, {
-                        x: s,
-                        y: o
+        function Gp(t, e) {
+            return {
+                x: {
+                    display: !0,
+                    title: {
+                        display: !0,
+                        text: t.x_label
+                    },
+                    grid: {
+                        display: t.x_grid,
+                        color: e.fadedText05
                     }
-                }(r[0], r[1]), l = e.options.zoom.mode;
-                Mp(t, {
-                    x: a.x && op(l, "x", t) ? s : 1,
-                    y: a.y && op(l, "y", t) ? s : 1,
-                    focalPoint: {
-                        x: i.x - o.left,
-                        y: i.y - o.top
+                },
+                y: {
+                    display: !0,
+                    title: {
+                        display: !0,
+                        text: t.y_label
+                    },
+                    grid: {
+                        display: t.y_grid,
+                        color: e.fadedText05
                     }
-                }), e.scale = n.scale
+                }
             }
         }
-
-        function Hp(t, e, n) {
-            const i = e.delta;
-            i && (e.panning = !0, Dp(t, {
-                x: n.deltaX - i.x,
-                y: n.deltaY - i.y
-            }, e.panScales), e.delta = {
-                x: n.deltaX,
-                y: n.deltaY
-            })
-        }
-        const Yp = new WeakMap;
-
-        function $p(t, e) {
-            const n = up(t),
-                i = t.canvas,
-                {
-                    pan: r,
-                    zoom: s
-                } = e,
-                o = new(np().Manager)(i);
-            s && s.pinch.enabled && (o.add(new(np().Pinch)), o.on("pinchstart", (() => function(t, e) {
-                e.options.zoom.pinch.enabled && (e.scale = 1)
-            }(0, n))), o.on("pinch", (e => Wp(t, n, e))), o.on("pinchend", (e => function(t, e, n) {
-                e.scale && (Wp(t, e, n), e.scale = null, X(e.options.zoom.onZoomComplete, [{
-                    chart: t
-                }]))
-            }(t, n, e)))), r && r.enabled && (o.add(new(np().Pan)({
-                threshold: r.threshold,
-                enable: jp(t, n)
-            })), o.on("panstart", (e => function(t, e, n) {
-                const {
-                    enabled: i,
-                    onPanStart: r,
-                    onPanRejected: s
-                } = e.options.pan;
-                if (!i) return;
-                const o = n.target.getBoundingClientRect(),
-                    a = {
-                        x: n.center.x - o.left,
-                        y: n.center.y - o.top
-                    };
-                if (!1 === X(r, [{
-                        chart: t,
-                        event: n,
-                        point: a
-                    }])) return X(s, [{
-                    chart: t,
-                    event: n
-                }]);
-                e.panScales = lp(e.options.pan, a, t), e.delta = {
-                    x: 0,
-                    y: 0
-                }, clearTimeout(e.panEndTimeout), Hp(t, e, n)
-            }(t, n, e))), o.on("panmove", (e => Hp(t, n, e))), o.on("panend", (() => function(t, e) {
-                e.delta = null, e.panning && (e.panEndTimeout = setTimeout((() => e.panning = !1), 500), X(e.options.pan.onPanComplete, [{
-                    chart: t
-                }]))
-            }(t, n)))), Yp.set(t, o)
-        }
-
-        function Kp(t, e, n) {
-            const i = n.zoom.drag,
-                {
-                    dragStart: r,
-                    dragEnd: s
-                } = up(t);
-            if (i.drawTime !== e || !s) return;
-            const {
-                left: o,
-                top: a,
-                width: l,
-                height: c
-            } = Rp(t, n.zoom.mode, r, s), u = t.ctx;
-            u.save(), u.beginPath(), u.fillStyle = i.backgroundColor || "rgba(225,225,225,0.3)", u.fillRect(o, a, l, c), i.borderWidth > 0 && (u.lineWidth = i.borderWidth, u.strokeStyle = i.borderColor || "rgba(225,225,225)", u.strokeRect(o, a, l, c)), u.restore()
-        }
-        var Xp = {
-                id: "zoom",
-                version: "2.0.1",
-                defaults: {
-                    pan: {
-                        enabled: !1,
-                        mode: "xy",
-                        threshold: 10,
-                        modifierKey: null
-                    },
-                    zoom: {
-                        wheel: {
-                            enabled: !1,
-                            speed: .1,
-                            modifierKey: null
-                        },
-                        drag: {
-                            enabled: !1,
-                            drawTime: "beforeDatasetsDraw",
-                            modifierKey: null
-                        },
-                        pinch: {
-                            enabled: !1
-                        },
-                        mode: "xy"
-                    }
-                },
-                start: function(t, e, n) {
-                    up(t).options = n, Object.prototype.hasOwnProperty.call(n.zoom, "enabled") && console.warn("The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`."), (Object.prototype.hasOwnProperty.call(n.zoom, "overScaleMode") || Object.prototype.hasOwnProperty.call(n.pan, "overScaleMode")) && console.warn("The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired)."), np() && $p(t, n), t.pan = (e, n, i) => Dp(t, e, n, i), t.zoom = (e, n) => Mp(t, e, n), t.zoomRect = (e, n, i) => Ip(t, e, n, i), t.zoomScale = (e, n, i) => function(t, e, n) {
-                        let i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : "none";
-                        wp(t, up(t)), fp(t.scales[e], n, void 0, !0), t.update(i)
-                    }(t, e, n, i), t.resetZoom = e => function(t) {
-                        let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "default";
-                        const n = up(t),
-                            i = wp(t, n);
-                        q(t.scales, (function(t) {
-                            const e = t.options;
-                            i[t.id] ? (e.min = i[t.id].min.options, e.max = i[t.id].max.options) : (delete e.min, delete e.max)
-                        })), t.update(e), X(n.options.zoom.onZoomComplete, [{
-                            chart: t
-                        }])
-                    }(t, e), t.getZoomLevel = () => Ep(t), t.getInitialScaleBounds = () => Ap(t), t.isZoomedOrPanned = () => function(t) {
-                        const e = Ap(t);
-                        for (const n of Object.keys(t.scales)) {
-                            const {
-                                min: i,
-                                max: r
-                            } = e[n];
-                            if (void 0 !== i && t.scales[n].min !== i) return !0;
-                            if (void 0 !== r && t.scales[n].max !== r) return !0
-                        }
-                        return !1
-                    }(t)
-                },
-                beforeEvent(t) {
-                    const e = up(t);
-                    if (e.panning || e.dragging) return !1
-                },
-                beforeUpdate: function(t, e, n) {
-                    up(t).options = n,
-                        function(t, e) {
-                            const n = t.canvas,
-                                {
-                                    wheel: i,
-                                    drag: r,
-                                    onZoomComplete: s
-                                } = e.zoom;
-                            i.enabled ? (Pp(t, n, "wheel", Up), Vp(t, "onZoomComplete", s, 250)) : Cp(t, "wheel"), r.enabled ? (Pp(t, n, "mousedown", Bp), Pp(t, n.ownerDocument, "mouseup", zp)) : (Cp(t, "mousedown"), Cp(t, "mousemove"), Cp(t, "mouseup"), Cp(t, "keydown"))
-                        }(t, n)
-                },
-                beforeDatasetsDraw(t, e, n) {
-                    Kp(t, "beforeDatasetsDraw", n)
-                },
-                afterDatasetsDraw(t, e, n) {
-                    Kp(t, "afterDatasetsDraw", n)
-                },
-                beforeDraw(t, e, n) {
-                    Kp(t, "beforeDraw", n)
-                },
-                afterDraw(t, e, n) {
-                    Kp(t, "afterDraw", n)
-                },
-                stop: function(t) {
-                    ! function(t) {
-                        Cp(t, "mousedown"), Cp(t, "mousemove"), Cp(t, "mouseup"), Cp(t, "wheel"), Cp(t, "click"), Cp(t, "keydown")
-                    }(t), np() && function(t) {
-                            const e = Yp.get(t);
-                            e && (e.remove("pinchstart"), e.remove("pinch"), e.remove("pinchend"), e.remove("panstart"), e.remove("pan"), e.remove("panend"), e.destroy(), Yp.delete(t))
-                        }(t),
-                        function(t) {
-                            cp.delete(t)
-                        }(t)
-                },
-                panFunctions: _p,
-                zoomFunctions: bp,
-                zoomRectFunctions: vp
-            },
-            qp = n(579);
-        Rr.register(...Uo, Xp);
-        const Qp = function(e) {
+        var Jp = n(579);
+        Rr.register(...Uo, Fa);
+        const tg = function(e) {
             var n = function(n) {
                 function i(t) {
                     var e = n.call(this, t) || this;
                     return e.componentDidMount = function() {
-                        Zf.events.addEventListener(Zf.RENDER_EVENT, e.onRenderEvent), Zf.setComponentReady()
+                        Yp.events.addEventListener(Yp.RENDER_EVENT, e.onRenderEvent), Yp.setComponentReady()
                     }, e.componentDidUpdate = function() {
-                        null != e.state.componentError && Zf.setFrameHeight()
+                        null != e.state.componentError && Yp.setFrameHeight()
                     }, e.componentWillUnmount = function() {
-                        Zf.events.removeEventListener(Zf.RENDER_EVENT, e.onRenderEvent)
+                        Yp.events.removeEventListener(Yp.RENDER_EVENT, e.onRenderEvent)
                     }, e.onRenderEvent = function(t) {
                         e.setState({
                             renderData: t.detail
                         })
                     }, e.state = {
                         renderData: void 0,
                         componentError: void 0
                     }, e
                 }
-                return Jf(i, n), i.prototype.render = function() {
+                return Kp(i, n), i.prototype.render = function() {
                     return null != this.state.componentError ? t.createElement("div", null, t.createElement("h1", null, "Component Error"), t.createElement("span", null, this.state.componentError.message)) : null == this.state.renderData ? null : t.createElement(e, {
                         width: window.innerWidth,
                         disabled: this.state.renderData.disabled,
                         args: this.state.renderData.args,
                         theme: this.state.renderData.theme
                     })
                 }, i.getDerivedStateFromError = function(t) {
                     return {
                         componentError: t
                     }
                 }, i
             }(t.PureComponent);
-            return oa()(n, e)
-        }(class extends tp {
+            return tl()(n, e)
+        }(class extends Xp {
             constructor(e) {
                 super(e), this.downHandler = t => {
                     const e = function(t, e) {
                         return t.getElementsAtEventForMode(e.nativeEvent, "nearest", {
                             intersect: !0
                         }, !1)
                     }(this.chartRef.current, t);
@@ -26031,15 +26123,15 @@
                     })
                 }, this.upHandler = t => {
                     if (this.state.activePoint) {
                         const t = this.chartRef.current.data.datasets.reduce(((t, e) => {
                             const n = e.data.reduce(((t, e, n) => (t[this.state.chartData.labels[n]] = e, t)), {});
                             return t[e.label] = n, t
                         }), {});
-                        Zf.setComponentValue(t)
+                        Yp.setComponentValue(t)
                     }
                     this.setState({
                         activePoint: null
                     })
                 }, this.moveHandler = t => {
                     if (this.state.activePoint) {
                         const e = this.chartRef.current,
@@ -26047,104 +26139,34 @@
                             i = e.chartArea,
                             r = e.scales.y,
                             s = this.map(n.y, i.bottom, i.top, r.min, r.max);
                         e.data.datasets[this.state.activePoint.datasetIndex].data[this.state.activePoint.index] = s, e.update()
                     }
                 }, this.map = (t, e, n, i, r) => i + (t - e) / (n - e) * (r - i), this.chartRef = t.createRef(), this.state = {
                     activePoint: null,
-                    chartData: this.createChartData(e.args.data, e.args.options.colors),
-                    options: this.createOptions(e.args.options)
+                    chartData: qp(e.args.data, e.args.options.colors),
+                    options: Qp(e.args.options, e.theme)
                 }
             }
             componentDidUpdate(t) {
-                Zf.setFrameHeight(), this.props.args !== t.args && this.setState({
-                    chartData: this.createChartData(this.props.args.data, this.props.args.options),
-                    options: this.createOptions(this.props.args.options)
+                Yp.setFrameHeight(), this.props.args !== t.args && this.setState({
+                    chartData: qp(this.props.args.data, this.props.args.options),
+                    options: Qp(this.props.args.options, this.props.theme)
                 })
             }
-            createChartData(t, e) {
-                const n = Object.entries(t).map(((t, e) => {
-                    let [n, i] = t;
-                    return {
-                        data: Object.values(i),
-                        label: n,
-                        fill: !1,
-                        lineTension: .3,
-                        cubicInterpolationMode: "monotone"
-                    }
-                }));
-                return e.colors && n.forEach(((t, n) => {
-                    t.backgroundColor = e.colors[n], t.borderColor = e.colors[n]
-                })), {
-                    labels: Object.keys(t.Col1),
-                    datasets: n
-                }
-            }
-            createOptions(t) {
-                return {
-                    responsive: !0,
-                    animation: {
-                        duration: 0
-                    },
-                    tooltips: {
-                        mode: "nearest"
-                    },
-                    onHover: (t, e) => {
-                        e.length > 0 ? t.native.target.style.cursor = "crosshair" : t.native.target.style.cursor = "default"
-                    },
-                    plugins: {
-                        zoom: {
-                            zoom: {
-                                wheel: {
-                                    enabled: !0
-                                },
-                                mode: "x"
-                            },
-                            pan: {
-                                enabled: !1
-                            }
-                        },
-                        title: {
-                            display: !0,
-                            text: t.title
-                        },
-                        legend: {
-                            onHover: (t, e, n) => {
-                                t.native.target.style.cursor = e ? "pointer" : "default"
-                            }
-                        }
-                    },
-                    scales: {
-                        x: {
-                            display: !0,
-                            title: {
-                                display: !0,
-                                text: t.x_label
-                            }
-                        },
-                        y: {
-                            display: !0,
-                            title: {
-                                display: !0,
-                                text: t.y_label
-                            }
-                        }
-                    }
-                }
-            }
             render() {
-                return (0, qp.jsx)(qo, {
+                return (0, Jp.jsx)(Wa, {
                     ref: this.chartRef,
                     data: this.state.chartData,
                     options: this.state.options,
                     onPointerDown: this.downHandler,
                     onPointerUp: this.upHandler,
                     onPointerMove: this.moveHandler
                 })
             }
         });
-        e.render((0, qp.jsx)(t.StrictMode, {
-            children: (0, qp.jsx)(Qp, {})
+        e.render((0, Jp.jsx)(t.StrictMode, {
+            children: (0, Jp.jsx)(tg, {})
         }), document.getElementById("root"))
     })()
 })();
-//# sourceMappingURL=main.a519b502.js.map
+//# sourceMappingURL=main.8e0bbc33.js.map
```

### Comparing `draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/static/js/main.a519b502.js.LICENSE.txt` & `draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/static/js/main.8e0bbc33.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `draggable-line-chart-0.1.0/draggable_line_chart/frontend/build/static/js/main.a519b502.js.map` & `draggable-line-chart-0.2.0/draggable_line_chart/frontend/build/static/js/main.8e0bbc33.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8498557250537182%*

 * *Differences: {"'file'": "'static/js/main.8e0bbc33.js'",*

 * * "'mappings'": "';2BAAA,OAKA,SAAUA,EAAQC,EAAUC,EAAYC,GACtC,aAEF,IA+FIC,EA/FAC,EAAkB,CAAC,GAAI,SAAU,MAAO,KAAM,KAAM,KACpDC,EAAeL,EAASM,cAAc,OAEtCC,EAAgB,WAEhBC,EAAQC,KAAKD,MACbE,EAAMD,KAAKC,IACXC,EAAMC,KAAKD,IASf,SAASE,EAAkBC,EAAIC,EAASC,GACpC,OAAOC,WAAWC,EAAOJ,EAAIE,GAAUD,EAC3C,CAWA,SAASI,EAAeC,EAAKN,EAAIE,GAC7B,QAAIK,MAAMC,QAAQF,KACdG,EAAKH,EAAKJ,EAAQF,GAAKE,IAChB,EAGf,CAQA,SAASO,EAAKC,EAAKC,EAAUT,GACzB,IAAIU,EAEJ,GAAKF,EAIL,GAAIA,EAAIG,QACJH,EAAIG,QAAQF,EAAUT,QACn […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.a519b502.js",
+    "file": "static/js/main.8e0bbc33.js",
     "names": [
         "window",
         "document",
         "exportName",
         "undefined",
         "assign",
         "VENDOR_PREFIXES",
@@ -4073,14 +4073,151 @@
         "TimeSeriesScale",
         "_table",
         "_minPos",
         "_tableRange",
         "_getTimestampsForTable",
         "buildLookupTable",
         "registerables",
+        "getModifierKey",
+        "modifierKey",
+        "keyPressed",
+        "keyNotPressed",
+        "directionEnabled",
+        "directionsEnabled",
+        "getEnabledScalesByPoint",
+        "scaleMode",
+        "overScaleMode",
+        "scaleIds",
+        "getScaleUnderPoint",
+        "scaleEnabled",
+        "overScaleEnabled",
+        "enabledScales",
+        "scaleItem",
+        "chartStates",
+        "getState",
+        "originalScaleLimits",
+        "updatedScaleLimits",
+        "panDelta",
+        "zoomDelta",
+        "newRange",
+        "centerPoint",
+        "minPercent",
+        "getLimit",
+        "scaleLimits",
+        "updateRange",
+        "minRange",
+        "minLimit",
+        "maxLimit",
+        "integerChange",
+        "OFFSETS",
+        "panNumericalScale",
+        "canZoom",
+        "prevStart",
+        "prevEnd",
+        "newMin",
+        "newMax",
+        "panNonLinearScale",
+        "zoomFunctions",
+        "category",
+        "existCategoryFromMaxZoom",
+        "zoomRectFunctions",
+        "pixel0",
+        "pixel1",
+        "panFunctions",
+        "lastLabelIndex",
+        "stepDelta",
+        "scaleLength",
+        "applied",
+        "timeseries",
+        "removeMissingScales",
+        "opt",
+        "storeOriginalScaleLimits",
+        "shouldUpdateScaleLimits",
+        "doZoom",
+        "doZoomRect",
+        "focalPoint",
+        "zoomOptions",
+        "xEnabled",
+        "yEnabled",
+        "onZoom",
+        "zoomRect",
+        "getZoomLevel",
+        "origRange",
+        "scaleId",
+        "getOriginalRange",
+        "level",
+        "panScale",
+        "storedDelta",
+        "pan",
+        "panOptions",
+        "onPan",
+        "getInitialScaleBounds",
+        "scaleBounds",
+        "removeHandler",
+        "addHandler",
+        "oldHandler",
+        "mouseMove",
+        "dragStart",
+        "dragging",
+        "dragEnd",
+        "keyDown",
+        "zoomStart",
+        "onZoomStart",
+        "onZoomRejected",
+        "mouseDown",
+        "drag",
+        "computeDragRect",
+        "beginPointEvent",
+        "endPointEvent",
+        "chartHeight",
+        "beginPoint",
+        "endPoint",
+        "zoomX",
+        "zoomY",
+        "mouseUp",
+        "onZoomComplete",
+        "distanceX",
+        "distanceY",
+        "wheel",
+        "wheelPreconditions",
+        "speed",
+        "addDebouncedHandler",
+        "createEnabler",
+        "panning",
+        "onPanRejected",
+        "handlePinch",
+        "zoomPercent",
+        "pinch",
+        "pinchX",
+        "pinchY",
+        "pinchAxes",
+        "handlePan",
+        "panScales",
+        "hammers",
+        "startHammer",
+        "startPinch",
+        "endPinch",
+        "onPanStart",
+        "panEndTimeout",
+        "startPan",
+        "onPanComplete",
+        "endPan",
+        "dragOptions",
+        "zoomScale",
+        "resetZoom",
+        "isZoomedOrPanned",
+        "originalMin",
+        "originalMax",
+        "beforeEvent",
+        "wheelOptions",
+        "addListeners",
+        "afterDatasetsDraw",
+        "removeListeners",
+        "stopHammer",
+        "removeState",
         "defaultDatasetIdKey",
         "reforwardRef",
         "setLabels",
         "currentData",
         "nextLabels",
         "setDatasets",
         "nextDatasets",
@@ -5517,182 +5654,50 @@
         "primaryColor",
         "secondaryBackgroundColor",
         "__extends",
         "extendStatics",
         "__proto__",
         "__",
         "StreamlitComponentBase",
-        "getModifierKey",
-        "modifierKey",
-        "keyPressed",
-        "keyNotPressed",
-        "directionEnabled",
-        "directionsEnabled",
-        "getEnabledScalesByPoint",
-        "scaleMode",
-        "overScaleMode",
-        "scaleIds",
-        "getScaleUnderPoint",
-        "scaleEnabled",
-        "overScaleEnabled",
-        "enabledScales",
-        "scaleItem",
-        "chartStates",
-        "getState",
-        "originalScaleLimits",
-        "updatedScaleLimits",
-        "panDelta",
-        "zoomDelta",
-        "newRange",
-        "centerPoint",
-        "minPercent",
-        "getLimit",
-        "scaleLimits",
-        "updateRange",
-        "minRange",
-        "minLimit",
-        "maxLimit",
-        "integerChange",
-        "OFFSETS",
-        "panNumericalScale",
-        "canZoom",
-        "prevStart",
-        "prevEnd",
-        "newMin",
-        "newMax",
-        "panNonLinearScale",
-        "zoomFunctions",
-        "category",
-        "existCategoryFromMaxZoom",
-        "zoomRectFunctions",
-        "pixel0",
-        "pixel1",
-        "panFunctions",
-        "lastLabelIndex",
-        "stepDelta",
-        "scaleLength",
-        "applied",
-        "timeseries",
-        "removeMissingScales",
-        "opt",
-        "storeOriginalScaleLimits",
-        "shouldUpdateScaleLimits",
-        "doZoom",
-        "doZoomRect",
-        "focalPoint",
-        "zoomOptions",
-        "xEnabled",
-        "yEnabled",
-        "onZoom",
-        "zoomRect",
-        "getZoomLevel",
-        "origRange",
-        "scaleId",
-        "getOriginalRange",
-        "level",
-        "panScale",
-        "storedDelta",
-        "pan",
-        "panOptions",
-        "onPan",
-        "getInitialScaleBounds",
-        "scaleBounds",
-        "removeHandler",
-        "addHandler",
-        "oldHandler",
-        "mouseMove",
-        "dragStart",
-        "dragging",
-        "dragEnd",
-        "keyDown",
-        "zoomStart",
-        "onZoomStart",
-        "onZoomRejected",
-        "mouseDown",
-        "drag",
-        "computeDragRect",
-        "beginPointEvent",
-        "endPointEvent",
-        "chartHeight",
-        "beginPoint",
-        "endPoint",
-        "zoomX",
-        "zoomY",
-        "mouseUp",
-        "onZoomComplete",
-        "distanceX",
-        "distanceY",
-        "wheel",
-        "wheelPreconditions",
-        "speed",
-        "addDebouncedHandler",
-        "createEnabler",
-        "panning",
-        "onPanRejected",
-        "handlePinch",
-        "zoomPercent",
-        "pinch",
-        "pinchX",
-        "pinchY",
-        "pinchAxes",
-        "handlePan",
-        "panScales",
-        "hammers",
-        "startHammer",
-        "startPinch",
-        "endPinch",
-        "onPanStart",
-        "panEndTimeout",
-        "startPan",
-        "onPanComplete",
-        "endPan",
-        "dragOptions",
-        "zoomScale",
-        "resetZoom",
-        "isZoomedOrPanned",
-        "originalMin",
-        "originalMax",
-        "beforeEvent",
-        "wheelOptions",
-        "addListeners",
-        "afterDatasetsDraw",
-        "removeListeners",
-        "stopHammer",
-        "removeState",
+        "createChartData",
+        "colName",
+        "colData",
+        "lineTension",
+        "Col1",
+        "createOptions",
+        "tooltips",
+        "chartElement",
+        "createTitleOptions",
+        "createScalesOptions",
+        "x_label",
+        "x_grid",
+        "fadedText05",
+        "y_label",
+        "y_grid",
         "zoomPlugin",
         "WrappedComponent",
         "ComponentWrapper",
         "onRenderEvent",
         "componentError",
         "renderData",
         "innerWidth",
         "downHandler",
         "getElementAtEvent",
         "activePoint",
         "upHandler",
-        "colData",
         "colAcc",
         "chartData",
         "moveHandler",
         "yAxis",
         "yValue",
         "start1",
         "stop1",
         "start2",
         "stop2",
-        "createChartData",
-        "createOptions",
         "prevProps",
-        "colName",
-        "lineTension",
-        "Col1",
-        "tooltips",
-        "chartElement",
-        "x_label",
-        "y_label",
         "_jsx",
         "onPointerDown",
         "onPointerUp",
         "onPointerMove",
         "ReactDOM",
         "DraggableLinechart"
     ],
@@ -5789,14 +5794,15 @@
         "../node_modules/chart.js/src/scales/scale.linearbase.js",
         "../node_modules/chart.js/src/scales/scale.linear.js",
         "../node_modules/chart.js/src/scales/scale.logarithmic.js",
         "../node_modules/chart.js/src/scales/scale.radialLinear.js",
         "../node_modules/chart.js/src/scales/scale.time.js",
         "../node_modules/chart.js/src/scales/scale.timeseries.js",
         "../node_modules/chart.js/src/index.ts",
+        "../node_modules/chartjs-plugin-zoom/dist/chartjs-plugin-zoom.esm.js",
         "../node_modules/react-chartjs-2/src/utils.ts",
         "../node_modules/react-chartjs-2/src/chart.tsx",
         "../node_modules/react-chartjs-2/src/typedCharts.tsx",
         "../node_modules/apache-arrow/src/enum.ts",
         "../node_modules/apache-arrow/src/util/compat.ts",
         "../node_modules/apache-arrow/src/util/pretty.ts",
         "../node_modules/tslib/tslib.es6.mjs",
@@ -5884,15 +5890,16 @@
         "../node_modules/apache-arrow/src/ipc/reader.ts",
         "../node_modules/apache-arrow/src/visitor/vectorassembler.ts",
         "../node_modules/apache-arrow/src/ipc/writer.ts",
         "../node_modules/apache-arrow/src/ipc/serialization.ts",
         "../node_modules/streamlit-component-lib/dist/ArrowTable.js",
         "../node_modules/streamlit-component-lib/dist/streamlit.js",
         "../node_modules/streamlit-component-lib/dist/StreamlitReact.js",
-        "../node_modules/chartjs-plugin-zoom/dist/chartjs-plugin-zoom.esm.js",
+        "chartData.jsx",
+        "chartOptions.jsx",
         "DraggableLineChart.jsx",
         "index.tsx"
     ],
     "sourcesContent": [
         "/*! Hammer.JS - v2.0.7 - 2016-04-22\n * http://hammerjs.github.io/\n *\n * Copyright (c) 2016 Jorik Tangelder;\n * Licensed under the MIT license */\n(function(window, document, exportName, undefined) {\n  'use strict';\n\nvar VENDOR_PREFIXES = ['', 'webkit', 'Moz', 'MS', 'ms', 'o'];\nvar TEST_ELEMENT = document.createElement('div');\n\nvar TYPE_FUNCTION = 'function';\n\nvar round = Math.round;\nvar abs = Math.abs;\nvar now = Date.now;\n\n/**\n * set a timeout with a given scope\n * @param {Function} fn\n * @param {Number} timeout\n * @param {Object} context\n * @returns {number}\n */\nfunction setTimeoutContext(fn, timeout, context) {\n    return setTimeout(bindFn(fn, context), timeout);\n}\n\n/**\n * if the argument is an array, we want to execute the fn on each entry\n * if it aint an array we don't want to do a thing.\n * this is used by all the methods that accept a single and array argument.\n * @param {*|Array} arg\n * @param {String} fn\n * @param {Object} [context]\n * @returns {Boolean}\n */\nfunction invokeArrayArg(arg, fn, context) {\n    if (Array.isArray(arg)) {\n        each(arg, context[fn], context);\n        return true;\n    }\n    return false;\n}\n\n/**\n * walk objects and arrays\n * @param {Object} obj\n * @param {Function} iterator\n * @param {Object} context\n */\nfunction each(obj, iterator, context) {\n    var i;\n\n    if (!obj) {\n        return;\n    }\n\n    if (obj.forEach) {\n        obj.forEach(iterator, context);\n    } else if (obj.length !== undefined) {\n        i = 0;\n        while (i < obj.length) {\n            iterator.call(context, obj[i], i, obj);\n            i++;\n        }\n    } else {\n        for (i in obj) {\n            obj.hasOwnProperty(i) && iterator.call(context, obj[i], i, obj);\n        }\n    }\n}\n\n/**\n * wrap a method with a deprecation warning and stack trace\n * @param {Function} method\n * @param {String} name\n * @param {String} message\n * @returns {Function} A new function wrapping the supplied method.\n */\nfunction deprecate(method, name, message) {\n    var deprecationMessage = 'DEPRECATED METHOD: ' + name + '\\n' + message + ' AT \\n';\n    return function() {\n        var e = new Error('get-stack-trace');\n        var stack = e && e.stack ? e.stack.replace(/^[^\\(]+?[\\n$]/gm, '')\n            .replace(/^\\s+at\\s+/gm, '')\n            .replace(/^Object.<anonymous>\\s*\\(/gm, '{anonymous}()@') : 'Unknown Stack Trace';\n\n        var log = window.console && (window.console.warn || window.console.log);\n        if (log) {\n            log.call(window.console, deprecationMessage, stack);\n        }\n        return method.apply(this, arguments);\n    };\n}\n\n/**\n * extend object.\n * means that properties in dest will be overwritten by the ones in src.\n * @param {Object} target\n * @param {...Object} objects_to_assign\n * @returns {Object} target\n */\nvar assign;\nif (typeof Object.assign !== 'function') {\n    assign = function assign(target) {\n        if (target === undefined || target === null) {\n            throw new TypeError('Cannot convert undefined or null to object');\n        }\n\n        var output = Object(target);\n        for (var index = 1; index < arguments.length; index++) {\n            var source = arguments[index];\n            if (source !== undefined && source !== null) {\n                for (var nextKey in source) {\n                    if (source.hasOwnProperty(nextKey)) {\n                        output[nextKey] = source[nextKey];\n                    }\n                }\n            }\n        }\n        return output;\n    };\n} else {\n    assign = Object.assign;\n}\n\n/**\n * extend object.\n * means that properties in dest will be overwritten by the ones in src.\n * @param {Object} dest\n * @param {Object} src\n * @param {Boolean} [merge=false]\n * @returns {Object} dest\n */\nvar extend = deprecate(function extend(dest, src, merge) {\n    var keys = Object.keys(src);\n    var i = 0;\n    while (i < keys.length) {\n        if (!merge || (merge && dest[keys[i]] === undefined)) {\n            dest[keys[i]] = src[keys[i]];\n        }\n        i++;\n    }\n    return dest;\n}, 'extend', 'Use `assign`.');\n\n/**\n * merge the values from src in the dest.\n * means that properties that exist in dest will not be overwritten by src\n * @param {Object} dest\n * @param {Object} src\n * @returns {Object} dest\n */\nvar merge = deprecate(function merge(dest, src) {\n    return extend(dest, src, true);\n}, 'merge', 'Use `assign`.');\n\n/**\n * simple class inheritance\n * @param {Function} child\n * @param {Function} base\n * @param {Object} [properties]\n */\nfunction inherit(child, base, properties) {\n    var baseP = base.prototype,\n        childP;\n\n    childP = child.prototype = Object.create(baseP);\n    childP.constructor = child;\n    childP._super = baseP;\n\n    if (properties) {\n        assign(childP, properties);\n    }\n}\n\n/**\n * simple function bind\n * @param {Function} fn\n * @param {Object} context\n * @returns {Function}\n */\nfunction bindFn(fn, context) {\n    return function boundFn() {\n        return fn.apply(context, arguments);\n    };\n}\n\n/**\n * let a boolean value also be a function that must return a boolean\n * this first item in args will be used as the context\n * @param {Boolean|Function} val\n * @param {Array} [args]\n * @returns {Boolean}\n */\nfunction boolOrFn(val, args) {\n    if (typeof val == TYPE_FUNCTION) {\n        return val.apply(args ? args[0] || undefined : undefined, args);\n    }\n    return val;\n}\n\n/**\n * use the val2 when val1 is undefined\n * @param {*} val1\n * @param {*} val2\n * @returns {*}\n */\nfunction ifUndefined(val1, val2) {\n    return (val1 === undefined) ? val2 : val1;\n}\n\n/**\n * addEventListener with multiple events at once\n * @param {EventTarget} target\n * @param {String} types\n * @param {Function} handler\n */\nfunction addEventListeners(target, types, handler) {\n    each(splitStr(types), function(type) {\n        target.addEventListener(type, handler, false);\n    });\n}\n\n/**\n * removeEventListener with multiple events at once\n * @param {EventTarget} target\n * @param {String} types\n * @param {Function} handler\n */\nfunction removeEventListeners(target, types, handler) {\n    each(splitStr(types), function(type) {\n        target.removeEventListener(type, handler, false);\n    });\n}\n\n/**\n * find if a node is in the given parent\n * @method hasParent\n * @param {HTMLElement} node\n * @param {HTMLElement} parent\n * @return {Boolean} found\n */\nfunction hasParent(node, parent) {\n    while (node) {\n        if (node == parent) {\n            return true;\n        }\n        node = node.parentNode;\n    }\n    return false;\n}\n\n/**\n * small indexOf wrapper\n * @param {String} str\n * @param {String} find\n * @returns {Boolean} found\n */\nfunction inStr(str, find) {\n    return str.indexOf(find) > -1;\n}\n\n/**\n * split string on whitespace\n * @param {String} str\n * @returns {Array} words\n */\nfunction splitStr(str) {\n    return str.trim().split(/\\s+/g);\n}\n\n/**\n * find if a array contains the object using indexOf or a simple polyFill\n * @param {Array} src\n * @param {String} find\n * @param {String} [findByKey]\n * @return {Boolean|Number} false when not found, or the index\n */\nfunction inArray(src, find, findByKey) {\n    if (src.indexOf && !findByKey) {\n        return src.indexOf(find);\n    } else {\n        var i = 0;\n        while (i < src.length) {\n            if ((findByKey && src[i][findByKey] == find) || (!findByKey && src[i] === find)) {\n                return i;\n            }\n            i++;\n        }\n        return -1;\n    }\n}\n\n/**\n * convert array-like objects to real arrays\n * @param {Object} obj\n * @returns {Array}\n */\nfunction toArray(obj) {\n    return Array.prototype.slice.call(obj, 0);\n}\n\n/**\n * unique array with objects based on a key (like 'id') or just by the array's value\n * @param {Array} src [{id:1},{id:2},{id:1}]\n * @param {String} [key]\n * @param {Boolean} [sort=False]\n * @returns {Array} [{id:1},{id:2}]\n */\nfunction uniqueArray(src, key, sort) {\n    var results = [];\n    var values = [];\n    var i = 0;\n\n    while (i < src.length) {\n        var val = key ? src[i][key] : src[i];\n        if (inArray(values, val) < 0) {\n            results.push(src[i]);\n        }\n        values[i] = val;\n        i++;\n    }\n\n    if (sort) {\n        if (!key) {\n            results = results.sort();\n        } else {\n            results = results.sort(function sortUniqueArray(a, b) {\n                return a[key] > b[key];\n            });\n        }\n    }\n\n    return results;\n}\n\n/**\n * get the prefixed property\n * @param {Object} obj\n * @param {String} property\n * @returns {String|Undefined} prefixed\n */\nfunction prefixed(obj, property) {\n    var prefix, prop;\n    var camelProp = property[0].toUpperCase() + property.slice(1);\n\n    var i = 0;\n    while (i < VENDOR_PREFIXES.length) {\n        prefix = VENDOR_PREFIXES[i];\n        prop = (prefix) ? prefix + camelProp : property;\n\n        if (prop in obj) {\n            return prop;\n        }\n        i++;\n    }\n    return undefined;\n}\n\n/**\n * get a unique id\n * @returns {number} uniqueId\n */\nvar _uniqueId = 1;\nfunction uniqueId() {\n    return _uniqueId++;\n}\n\n/**\n * get the window object of an element\n * @param {HTMLElement} element\n * @returns {DocumentView|Window}\n */\nfunction getWindowForElement(element) {\n    var doc = element.ownerDocument || element;\n    return (doc.defaultView || doc.parentWindow || window);\n}\n\nvar MOBILE_REGEX = /mobile|tablet|ip(ad|hone|od)|android/i;\n\nvar SUPPORT_TOUCH = ('ontouchstart' in window);\nvar SUPPORT_POINTER_EVENTS = prefixed(window, 'PointerEvent') !== undefined;\nvar SUPPORT_ONLY_TOUCH = SUPPORT_TOUCH && MOBILE_REGEX.test(navigator.userAgent);\n\nvar INPUT_TYPE_TOUCH = 'touch';\nvar INPUT_TYPE_PEN = 'pen';\nvar INPUT_TYPE_MOUSE = 'mouse';\nvar INPUT_TYPE_KINECT = 'kinect';\n\nvar COMPUTE_INTERVAL = 25;\n\nvar INPUT_START = 1;\nvar INPUT_MOVE = 2;\nvar INPUT_END = 4;\nvar INPUT_CANCEL = 8;\n\nvar DIRECTION_NONE = 1;\nvar DIRECTION_LEFT = 2;\nvar DIRECTION_RIGHT = 4;\nvar DIRECTION_UP = 8;\nvar DIRECTION_DOWN = 16;\n\nvar DIRECTION_HORIZONTAL = DIRECTION_LEFT | DIRECTION_RIGHT;\nvar DIRECTION_VERTICAL = DIRECTION_UP | DIRECTION_DOWN;\nvar DIRECTION_ALL = DIRECTION_HORIZONTAL | DIRECTION_VERTICAL;\n\nvar PROPS_XY = ['x', 'y'];\nvar PROPS_CLIENT_XY = ['clientX', 'clientY'];\n\n/**\n * create new input type manager\n * @param {Manager} manager\n * @param {Function} callback\n * @returns {Input}\n * @constructor\n */\nfunction Input(manager, callback) {\n    var self = this;\n    this.manager = manager;\n    this.callback = callback;\n    this.element = manager.element;\n    this.target = manager.options.inputTarget;\n\n    // smaller wrapper around the handler, for the scope and the enabled state of the manager,\n    // so when disabled the input events are completely bypassed.\n    this.domHandler = function(ev) {\n        if (boolOrFn(manager.options.enable, [manager])) {\n            self.handler(ev);\n        }\n    };\n\n    this.init();\n\n}\n\nInput.prototype = {\n    /**\n     * should handle the inputEvent data and trigger the callback\n     * @virtual\n     */\n    handler: function() { },\n\n    /**\n     * bind the events\n     */\n    init: function() {\n        this.evEl && addEventListeners(this.element, this.evEl, this.domHandler);\n        this.evTarget && addEventListeners(this.target, this.evTarget, this.domHandler);\n        this.evWin && addEventListeners(getWindowForElement(this.element), this.evWin, this.domHandler);\n    },\n\n    /**\n     * unbind the events\n     */\n    destroy: function() {\n        this.evEl && removeEventListeners(this.element, this.evEl, this.domHandler);\n        this.evTarget && removeEventListeners(this.target, this.evTarget, this.domHandler);\n        this.evWin && removeEventListeners(getWindowForElement(this.element), this.evWin, this.domHandler);\n    }\n};\n\n/**\n * create new input type manager\n * called by the Manager constructor\n * @param {Hammer} manager\n * @returns {Input}\n */\nfunction createInputInstance(manager) {\n    var Type;\n    var inputClass = manager.options.inputClass;\n\n    if (inputClass) {\n        Type = inputClass;\n    } else if (SUPPORT_POINTER_EVENTS) {\n        Type = PointerEventInput;\n    } else if (SUPPORT_ONLY_TOUCH) {\n        Type = TouchInput;\n    } else if (!SUPPORT_TOUCH) {\n        Type = MouseInput;\n    } else {\n        Type = TouchMouseInput;\n    }\n    return new (Type)(manager, inputHandler);\n}\n\n/**\n * handle input events\n * @param {Manager} manager\n * @param {String} eventType\n * @param {Object} input\n */\nfunction inputHandler(manager, eventType, input) {\n    var pointersLen = input.pointers.length;\n    var changedPointersLen = input.changedPointers.length;\n    var isFirst = (eventType & INPUT_START && (pointersLen - changedPointersLen === 0));\n    var isFinal = (eventType & (INPUT_END | INPUT_CANCEL) && (pointersLen - changedPointersLen === 0));\n\n    input.isFirst = !!isFirst;\n    input.isFinal = !!isFinal;\n\n    if (isFirst) {\n        manager.session = {};\n    }\n\n    // source event is the normalized value of the domEvents\n    // like 'touchstart, mouseup, pointerdown'\n    input.eventType = eventType;\n\n    // compute scale, rotation etc\n    computeInputData(manager, input);\n\n    // emit secret event\n    manager.emit('hammer.input', input);\n\n    manager.recognize(input);\n    manager.session.prevInput = input;\n}\n\n/**\n * extend the data with some usable properties like scale, rotate, velocity etc\n * @param {Object} manager\n * @param {Object} input\n */\nfunction computeInputData(manager, input) {\n    var session = manager.session;\n    var pointers = input.pointers;\n    var pointersLength = pointers.length;\n\n    // store the first input to calculate the distance and direction\n    if (!session.firstInput) {\n        session.firstInput = simpleCloneInputData(input);\n    }\n\n    // to compute scale and rotation we need to store the multiple touches\n    if (pointersLength > 1 && !session.firstMultiple) {\n        session.firstMultiple = simpleCloneInputData(input);\n    } else if (pointersLength === 1) {\n        session.firstMultiple = false;\n    }\n\n    var firstInput = session.firstInput;\n    var firstMultiple = session.firstMultiple;\n    var offsetCenter = firstMultiple ? firstMultiple.center : firstInput.center;\n\n    var center = input.center = getCenter(pointers);\n    input.timeStamp = now();\n    input.deltaTime = input.timeStamp - firstInput.timeStamp;\n\n    input.angle = getAngle(offsetCenter, center);\n    input.distance = getDistance(offsetCenter, center);\n\n    computeDeltaXY(session, input);\n    input.offsetDirection = getDirection(input.deltaX, input.deltaY);\n\n    var overallVelocity = getVelocity(input.deltaTime, input.deltaX, input.deltaY);\n    input.overallVelocityX = overallVelocity.x;\n    input.overallVelocityY = overallVelocity.y;\n    input.overallVelocity = (abs(overallVelocity.x) > abs(overallVelocity.y)) ? overallVelocity.x : overallVelocity.y;\n\n    input.scale = firstMultiple ? getScale(firstMultiple.pointers, pointers) : 1;\n    input.rotation = firstMultiple ? getRotation(firstMultiple.pointers, pointers) : 0;\n\n    input.maxPointers = !session.prevInput ? input.pointers.length : ((input.pointers.length >\n        session.prevInput.maxPointers) ? input.pointers.length : session.prevInput.maxPointers);\n\n    computeIntervalInputData(session, input);\n\n    // find the correct target\n    var target = manager.element;\n    if (hasParent(input.srcEvent.target, target)) {\n        target = input.srcEvent.target;\n    }\n    input.target = target;\n}\n\nfunction computeDeltaXY(session, input) {\n    var center = input.center;\n    var offset = session.offsetDelta || {};\n    var prevDelta = session.prevDelta || {};\n    var prevInput = session.prevInput || {};\n\n    if (input.eventType === INPUT_START || prevInput.eventType === INPUT_END) {\n        prevDelta = session.prevDelta = {\n            x: prevInput.deltaX || 0,\n            y: prevInput.deltaY || 0\n        };\n\n        offset = session.offsetDelta = {\n            x: center.x,\n            y: center.y\n        };\n    }\n\n    input.deltaX = prevDelta.x + (center.x - offset.x);\n    input.deltaY = prevDelta.y + (center.y - offset.y);\n}\n\n/**\n * velocity is calculated every x ms\n * @param {Object} session\n * @param {Object} input\n */\nfunction computeIntervalInputData(session, input) {\n    var last = session.lastInterval || input,\n        deltaTime = input.timeStamp - last.timeStamp,\n        velocity, velocityX, velocityY, direction;\n\n    if (input.eventType != INPUT_CANCEL && (deltaTime > COMPUTE_INTERVAL || last.velocity === undefined)) {\n        var deltaX = input.deltaX - last.deltaX;\n        var deltaY = input.deltaY - last.deltaY;\n\n        var v = getVelocity(deltaTime, deltaX, deltaY);\n        velocityX = v.x;\n        velocityY = v.y;\n        velocity = (abs(v.x) > abs(v.y)) ? v.x : v.y;\n        direction = getDirection(deltaX, deltaY);\n\n        session.lastInterval = input;\n    } else {\n        // use latest velocity info if it doesn't overtake a minimum period\n        velocity = last.velocity;\n        velocityX = last.velocityX;\n        velocityY = last.velocityY;\n        direction = last.direction;\n    }\n\n    input.velocity = velocity;\n    input.velocityX = velocityX;\n    input.velocityY = velocityY;\n    input.direction = direction;\n}\n\n/**\n * create a simple clone from the input used for storage of firstInput and firstMultiple\n * @param {Object} input\n * @returns {Object} clonedInputData\n */\nfunction simpleCloneInputData(input) {\n    // make a simple copy of the pointers because we will get a reference if we don't\n    // we only need clientXY for the calculations\n    var pointers = [];\n    var i = 0;\n    while (i < input.pointers.length) {\n        pointers[i] = {\n            clientX: round(input.pointers[i].clientX),\n            clientY: round(input.pointers[i].clientY)\n        };\n        i++;\n    }\n\n    return {\n        timeStamp: now(),\n        pointers: pointers,\n        center: getCenter(pointers),\n        deltaX: input.deltaX,\n        deltaY: input.deltaY\n    };\n}\n\n/**\n * get the center of all the pointers\n * @param {Array} pointers\n * @return {Object} center contains `x` and `y` properties\n */\nfunction getCenter(pointers) {\n    var pointersLength = pointers.length;\n\n    // no need to loop when only one touch\n    if (pointersLength === 1) {\n        return {\n            x: round(pointers[0].clientX),\n            y: round(pointers[0].clientY)\n        };\n    }\n\n    var x = 0, y = 0, i = 0;\n    while (i < pointersLength) {\n        x += pointers[i].clientX;\n        y += pointers[i].clientY;\n        i++;\n    }\n\n    return {\n        x: round(x / pointersLength),\n        y: round(y / pointersLength)\n    };\n}\n\n/**\n * calculate the velocity between two points. unit is in px per ms.\n * @param {Number} deltaTime\n * @param {Number} x\n * @param {Number} y\n * @return {Object} velocity `x` and `y`\n */\nfunction getVelocity(deltaTime, x, y) {\n    return {\n        x: x / deltaTime || 0,\n        y: y / deltaTime || 0\n    };\n}\n\n/**\n * get the direction between two points\n * @param {Number} x\n * @param {Number} y\n * @return {Number} direction\n */\nfunction getDirection(x, y) {\n    if (x === y) {\n        return DIRECTION_NONE;\n    }\n\n    if (abs(x) >= abs(y)) {\n        return x < 0 ? DIRECTION_LEFT : DIRECTION_RIGHT;\n    }\n    return y < 0 ? DIRECTION_UP : DIRECTION_DOWN;\n}\n\n/**\n * calculate the absolute distance between two points\n * @param {Object} p1 {x, y}\n * @param {Object} p2 {x, y}\n * @param {Array} [props] containing x and y keys\n * @return {Number} distance\n */\nfunction getDistance(p1, p2, props) {\n    if (!props) {\n        props = PROPS_XY;\n    }\n    var x = p2[props[0]] - p1[props[0]],\n        y = p2[props[1]] - p1[props[1]];\n\n    return Math.sqrt((x * x) + (y * y));\n}\n\n/**\n * calculate the angle between two coordinates\n * @param {Object} p1\n * @param {Object} p2\n * @param {Array} [props] containing x and y keys\n * @return {Number} angle\n */\nfunction getAngle(p1, p2, props) {\n    if (!props) {\n        props = PROPS_XY;\n    }\n    var x = p2[props[0]] - p1[props[0]],\n        y = p2[props[1]] - p1[props[1]];\n    return Math.atan2(y, x) * 180 / Math.PI;\n}\n\n/**\n * calculate the rotation degrees between two pointersets\n * @param {Array} start array of pointers\n * @param {Array} end array of pointers\n * @return {Number} rotation\n */\nfunction getRotation(start, end) {\n    return getAngle(end[1], end[0], PROPS_CLIENT_XY) + getAngle(start[1], start[0], PROPS_CLIENT_XY);\n}\n\n/**\n * calculate the scale factor between two pointersets\n * no scale is 1, and goes down to 0 when pinched together, and bigger when pinched out\n * @param {Array} start array of pointers\n * @param {Array} end array of pointers\n * @return {Number} scale\n */\nfunction getScale(start, end) {\n    return getDistance(end[0], end[1], PROPS_CLIENT_XY) / getDistance(start[0], start[1], PROPS_CLIENT_XY);\n}\n\nvar MOUSE_INPUT_MAP = {\n    mousedown: INPUT_START,\n    mousemove: INPUT_MOVE,\n    mouseup: INPUT_END\n};\n\nvar MOUSE_ELEMENT_EVENTS = 'mousedown';\nvar MOUSE_WINDOW_EVENTS = 'mousemove mouseup';\n\n/**\n * Mouse events input\n * @constructor\n * @extends Input\n */\nfunction MouseInput() {\n    this.evEl = MOUSE_ELEMENT_EVENTS;\n    this.evWin = MOUSE_WINDOW_EVENTS;\n\n    this.pressed = false; // mousedown state\n\n    Input.apply(this, arguments);\n}\n\ninherit(MouseInput, Input, {\n    /**\n     * handle mouse events\n     * @param {Object} ev\n     */\n    handler: function MEhandler(ev) {\n        var eventType = MOUSE_INPUT_MAP[ev.type];\n\n        // on start we want to have the left mouse button down\n        if (eventType & INPUT_START && ev.button === 0) {\n            this.pressed = true;\n        }\n\n        if (eventType & INPUT_MOVE && ev.which !== 1) {\n            eventType = INPUT_END;\n        }\n\n        // mouse must be down\n        if (!this.pressed) {\n            return;\n        }\n\n        if (eventType & INPUT_END) {\n            this.pressed = false;\n        }\n\n        this.callback(this.manager, eventType, {\n            pointers: [ev],\n            changedPointers: [ev],\n            pointerType: INPUT_TYPE_MOUSE,\n            srcEvent: ev\n        });\n    }\n});\n\nvar POINTER_INPUT_MAP = {\n    pointerdown: INPUT_START,\n    pointermove: INPUT_MOVE,\n    pointerup: INPUT_END,\n    pointercancel: INPUT_CANCEL,\n    pointerout: INPUT_CANCEL\n};\n\n// in IE10 the pointer types is defined as an enum\nvar IE10_POINTER_TYPE_ENUM = {\n    2: INPUT_TYPE_TOUCH,\n    3: INPUT_TYPE_PEN,\n    4: INPUT_TYPE_MOUSE,\n    5: INPUT_TYPE_KINECT // see https://twitter.com/jacobrossi/status/480596438489890816\n};\n\nvar POINTER_ELEMENT_EVENTS = 'pointerdown';\nvar POINTER_WINDOW_EVENTS = 'pointermove pointerup pointercancel';\n\n// IE10 has prefixed support, and case-sensitive\nif (window.MSPointerEvent && !window.PointerEvent) {\n    POINTER_ELEMENT_EVENTS = 'MSPointerDown';\n    POINTER_WINDOW_EVENTS = 'MSPointerMove MSPointerUp MSPointerCancel';\n}\n\n/**\n * Pointer events input\n * @constructor\n * @extends Input\n */\nfunction PointerEventInput() {\n    this.evEl = POINTER_ELEMENT_EVENTS;\n    this.evWin = POINTER_WINDOW_EVENTS;\n\n    Input.apply(this, arguments);\n\n    this.store = (this.manager.session.pointerEvents = []);\n}\n\ninherit(PointerEventInput, Input, {\n    /**\n     * handle mouse events\n     * @param {Object} ev\n     */\n    handler: function PEhandler(ev) {\n        var store = this.store;\n        var removePointer = false;\n\n        var eventTypeNormalized = ev.type.toLowerCase().replace('ms', '');\n        var eventType = POINTER_INPUT_MAP[eventTypeNormalized];\n        var pointerType = IE10_POINTER_TYPE_ENUM[ev.pointerType] || ev.pointerType;\n\n        var isTouch = (pointerType == INPUT_TYPE_TOUCH);\n\n        // get index of the event in the store\n        var storeIndex = inArray(store, ev.pointerId, 'pointerId');\n\n        // start and mouse must be down\n        if (eventType & INPUT_START && (ev.button === 0 || isTouch)) {\n            if (storeIndex < 0) {\n                store.push(ev);\n                storeIndex = store.length - 1;\n            }\n        } else if (eventType & (INPUT_END | INPUT_CANCEL)) {\n            removePointer = true;\n        }\n\n        // it not found, so the pointer hasn't been down (so it's probably a hover)\n        if (storeIndex < 0) {\n            return;\n        }\n\n        // update the event in the store\n        store[storeIndex] = ev;\n\n        this.callback(this.manager, eventType, {\n            pointers: store,\n            changedPointers: [ev],\n            pointerType: pointerType,\n            srcEvent: ev\n        });\n\n        if (removePointer) {\n            // remove from the store\n            store.splice(storeIndex, 1);\n        }\n    }\n});\n\nvar SINGLE_TOUCH_INPUT_MAP = {\n    touchstart: INPUT_START,\n    touchmove: INPUT_MOVE,\n    touchend: INPUT_END,\n    touchcancel: INPUT_CANCEL\n};\n\nvar SINGLE_TOUCH_TARGET_EVENTS = 'touchstart';\nvar SINGLE_TOUCH_WINDOW_EVENTS = 'touchstart touchmove touchend touchcancel';\n\n/**\n * Touch events input\n * @constructor\n * @extends Input\n */\nfunction SingleTouchInput() {\n    this.evTarget = SINGLE_TOUCH_TARGET_EVENTS;\n    this.evWin = SINGLE_TOUCH_WINDOW_EVENTS;\n    this.started = false;\n\n    Input.apply(this, arguments);\n}\n\ninherit(SingleTouchInput, Input, {\n    handler: function TEhandler(ev) {\n        var type = SINGLE_TOUCH_INPUT_MAP[ev.type];\n\n        // should we handle the touch events?\n        if (type === INPUT_START) {\n            this.started = true;\n        }\n\n        if (!this.started) {\n            return;\n        }\n\n        var touches = normalizeSingleTouches.call(this, ev, type);\n\n        // when done, reset the started state\n        if (type & (INPUT_END | INPUT_CANCEL) && touches[0].length - touches[1].length === 0) {\n            this.started = false;\n        }\n\n        this.callback(this.manager, type, {\n            pointers: touches[0],\n            changedPointers: touches[1],\n            pointerType: INPUT_TYPE_TOUCH,\n            srcEvent: ev\n        });\n    }\n});\n\n/**\n * @this {TouchInput}\n * @param {Object} ev\n * @param {Number} type flag\n * @returns {undefined|Array} [all, changed]\n */\nfunction normalizeSingleTouches(ev, type) {\n    var all = toArray(ev.touches);\n    var changed = toArray(ev.changedTouches);\n\n    if (type & (INPUT_END | INPUT_CANCEL)) {\n        all = uniqueArray(all.concat(changed), 'identifier', true);\n    }\n\n    return [all, changed];\n}\n\nvar TOUCH_INPUT_MAP = {\n    touchstart: INPUT_START,\n    touchmove: INPUT_MOVE,\n    touchend: INPUT_END,\n    touchcancel: INPUT_CANCEL\n};\n\nvar TOUCH_TARGET_EVENTS = 'touchstart touchmove touchend touchcancel';\n\n/**\n * Multi-user touch events input\n * @constructor\n * @extends Input\n */\nfunction TouchInput() {\n    this.evTarget = TOUCH_TARGET_EVENTS;\n    this.targetIds = {};\n\n    Input.apply(this, arguments);\n}\n\ninherit(TouchInput, Input, {\n    handler: function MTEhandler(ev) {\n        var type = TOUCH_INPUT_MAP[ev.type];\n        var touches = getTouches.call(this, ev, type);\n        if (!touches) {\n            return;\n        }\n\n        this.callback(this.manager, type, {\n            pointers: touches[0],\n            changedPointers: touches[1],\n            pointerType: INPUT_TYPE_TOUCH,\n            srcEvent: ev\n        });\n    }\n});\n\n/**\n * @this {TouchInput}\n * @param {Object} ev\n * @param {Number} type flag\n * @returns {undefined|Array} [all, changed]\n */\nfunction getTouches(ev, type) {\n    var allTouches = toArray(ev.touches);\n    var targetIds = this.targetIds;\n\n    // when there is only one touch, the process can be simplified\n    if (type & (INPUT_START | INPUT_MOVE) && allTouches.length === 1) {\n        targetIds[allTouches[0].identifier] = true;\n        return [allTouches, allTouches];\n    }\n\n    var i,\n        targetTouches,\n        changedTouches = toArray(ev.changedTouches),\n        changedTargetTouches = [],\n        target = this.target;\n\n    // get target touches from touches\n    targetTouches = allTouches.filter(function(touch) {\n        return hasParent(touch.target, target);\n    });\n\n    // collect touches\n    if (type === INPUT_START) {\n        i = 0;\n        while (i < targetTouches.length) {\n            targetIds[targetTouches[i].identifier] = true;\n            i++;\n        }\n    }\n\n    // filter changed touches to only contain touches that exist in the collected target ids\n    i = 0;\n    while (i < changedTouches.length) {\n        if (targetIds[changedTouches[i].identifier]) {\n            changedTargetTouches.push(changedTouches[i]);\n        }\n\n        // cleanup removed touches\n        if (type & (INPUT_END | INPUT_CANCEL)) {\n            delete targetIds[changedTouches[i].identifier];\n        }\n        i++;\n    }\n\n    if (!changedTargetTouches.length) {\n        return;\n    }\n\n    return [\n        // merge targetTouches with changedTargetTouches so it contains ALL touches, including 'end' and 'cancel'\n        uniqueArray(targetTouches.concat(changedTargetTouches), 'identifier', true),\n        changedTargetTouches\n    ];\n}\n\n/**\n * Combined touch and mouse input\n *\n * Touch has a higher priority then mouse, and while touching no mouse events are allowed.\n * This because touch devices also emit mouse events while doing a touch.\n *\n * @constructor\n * @extends Input\n */\n\nvar DEDUP_TIMEOUT = 2500;\nvar DEDUP_DISTANCE = 25;\n\nfunction TouchMouseInput() {\n    Input.apply(this, arguments);\n\n    var handler = bindFn(this.handler, this);\n    this.touch = new TouchInput(this.manager, handler);\n    this.mouse = new MouseInput(this.manager, handler);\n\n    this.primaryTouch = null;\n    this.lastTouches = [];\n}\n\ninherit(TouchMouseInput, Input, {\n    /**\n     * handle mouse and touch events\n     * @param {Hammer} manager\n     * @param {String} inputEvent\n     * @param {Object} inputData\n     */\n    handler: function TMEhandler(manager, inputEvent, inputData) {\n        var isTouch = (inputData.pointerType == INPUT_TYPE_TOUCH),\n            isMouse = (inputData.pointerType == INPUT_TYPE_MOUSE);\n\n        if (isMouse && inputData.sourceCapabilities && inputData.sourceCapabilities.firesTouchEvents) {\n            return;\n        }\n\n        // when we're in a touch event, record touches to  de-dupe synthetic mouse event\n        if (isTouch) {\n            recordTouches.call(this, inputEvent, inputData);\n        } else if (isMouse && isSyntheticEvent.call(this, inputData)) {\n            return;\n        }\n\n        this.callback(manager, inputEvent, inputData);\n    },\n\n    /**\n     * remove the event listeners\n     */\n    destroy: function destroy() {\n        this.touch.destroy();\n        this.mouse.destroy();\n    }\n});\n\nfunction recordTouches(eventType, eventData) {\n    if (eventType & INPUT_START) {\n        this.primaryTouch = eventData.changedPointers[0].identifier;\n        setLastTouch.call(this, eventData);\n    } else if (eventType & (INPUT_END | INPUT_CANCEL)) {\n        setLastTouch.call(this, eventData);\n    }\n}\n\nfunction setLastTouch(eventData) {\n    var touch = eventData.changedPointers[0];\n\n    if (touch.identifier === this.primaryTouch) {\n        var lastTouch = {x: touch.clientX, y: touch.clientY};\n        this.lastTouches.push(lastTouch);\n        var lts = this.lastTouches;\n        var removeLastTouch = function() {\n            var i = lts.indexOf(lastTouch);\n            if (i > -1) {\n                lts.splice(i, 1);\n            }\n        };\n        setTimeout(removeLastTouch, DEDUP_TIMEOUT);\n    }\n}\n\nfunction isSyntheticEvent(eventData) {\n    var x = eventData.srcEvent.clientX, y = eventData.srcEvent.clientY;\n    for (var i = 0; i < this.lastTouches.length; i++) {\n        var t = this.lastTouches[i];\n        var dx = Math.abs(x - t.x), dy = Math.abs(y - t.y);\n        if (dx <= DEDUP_DISTANCE && dy <= DEDUP_DISTANCE) {\n            return true;\n        }\n    }\n    return false;\n}\n\nvar PREFIXED_TOUCH_ACTION = prefixed(TEST_ELEMENT.style, 'touchAction');\nvar NATIVE_TOUCH_ACTION = PREFIXED_TOUCH_ACTION !== undefined;\n\n// magical touchAction value\nvar TOUCH_ACTION_COMPUTE = 'compute';\nvar TOUCH_ACTION_AUTO = 'auto';\nvar TOUCH_ACTION_MANIPULATION = 'manipulation'; // not implemented\nvar TOUCH_ACTION_NONE = 'none';\nvar TOUCH_ACTION_PAN_X = 'pan-x';\nvar TOUCH_ACTION_PAN_Y = 'pan-y';\nvar TOUCH_ACTION_MAP = getTouchActionProps();\n\n/**\n * Touch Action\n * sets the touchAction property or uses the js alternative\n * @param {Manager} manager\n * @param {String} value\n * @constructor\n */\nfunction TouchAction(manager, value) {\n    this.manager = manager;\n    this.set(value);\n}\n\nTouchAction.prototype = {\n    /**\n     * set the touchAction value on the element or enable the polyfill\n     * @param {String} value\n     */\n    set: function(value) {\n        // find out the touch-action by the event handlers\n        if (value == TOUCH_ACTION_COMPUTE) {\n            value = this.compute();\n        }\n\n        if (NATIVE_TOUCH_ACTION && this.manager.element.style && TOUCH_ACTION_MAP[value]) {\n            this.manager.element.style[PREFIXED_TOUCH_ACTION] = value;\n        }\n        this.actions = value.toLowerCase().trim();\n    },\n\n    /**\n     * just re-set the touchAction value\n     */\n    update: function() {\n        this.set(this.manager.options.touchAction);\n    },\n\n    /**\n     * compute the value for the touchAction property based on the recognizer's settings\n     * @returns {String} value\n     */\n    compute: function() {\n        var actions = [];\n        each(this.manager.recognizers, function(recognizer) {\n            if (boolOrFn(recognizer.options.enable, [recognizer])) {\n                actions = actions.concat(recognizer.getTouchAction());\n            }\n        });\n        return cleanTouchActions(actions.join(' '));\n    },\n\n    /**\n     * this method is called on each input cycle and provides the preventing of the browser behavior\n     * @param {Object} input\n     */\n    preventDefaults: function(input) {\n        var srcEvent = input.srcEvent;\n        var direction = input.offsetDirection;\n\n        // if the touch action did prevented once this session\n        if (this.manager.session.prevented) {\n            srcEvent.preventDefault();\n            return;\n        }\n\n        var actions = this.actions;\n        var hasNone = inStr(actions, TOUCH_ACTION_NONE) && !TOUCH_ACTION_MAP[TOUCH_ACTION_NONE];\n        var hasPanY = inStr(actions, TOUCH_ACTION_PAN_Y) && !TOUCH_ACTION_MAP[TOUCH_ACTION_PAN_Y];\n        var hasPanX = inStr(actions, TOUCH_ACTION_PAN_X) && !TOUCH_ACTION_MAP[TOUCH_ACTION_PAN_X];\n\n        if (hasNone) {\n            //do not prevent defaults if this is a tap gesture\n\n            var isTapPointer = input.pointers.length === 1;\n            var isTapMovement = input.distance < 2;\n            var isTapTouchTime = input.deltaTime < 250;\n\n            if (isTapPointer && isTapMovement && isTapTouchTime) {\n                return;\n            }\n        }\n\n        if (hasPanX && hasPanY) {\n            // `pan-x pan-y` means browser handles all scrolling/panning, do not prevent\n            return;\n        }\n\n        if (hasNone ||\n            (hasPanY && direction & DIRECTION_HORIZONTAL) ||\n            (hasPanX && direction & DIRECTION_VERTICAL)) {\n            return this.preventSrc(srcEvent);\n        }\n    },\n\n    /**\n     * call preventDefault to prevent the browser's default behavior (scrolling in most cases)\n     * @param {Object} srcEvent\n     */\n    preventSrc: function(srcEvent) {\n        this.manager.session.prevented = true;\n        srcEvent.preventDefault();\n    }\n};\n\n/**\n * when the touchActions are collected they are not a valid value, so we need to clean things up. *\n * @param {String} actions\n * @returns {*}\n */\nfunction cleanTouchActions(actions) {\n    // none\n    if (inStr(actions, TOUCH_ACTION_NONE)) {\n        return TOUCH_ACTION_NONE;\n    }\n\n    var hasPanX = inStr(actions, TOUCH_ACTION_PAN_X);\n    var hasPanY = inStr(actions, TOUCH_ACTION_PAN_Y);\n\n    // if both pan-x and pan-y are set (different recognizers\n    // for different directions, e.g. horizontal pan but vertical swipe?)\n    // we need none (as otherwise with pan-x pan-y combined none of these\n    // recognizers will work, since the browser would handle all panning\n    if (hasPanX && hasPanY) {\n        return TOUCH_ACTION_NONE;\n    }\n\n    // pan-x OR pan-y\n    if (hasPanX || hasPanY) {\n        return hasPanX ? TOUCH_ACTION_PAN_X : TOUCH_ACTION_PAN_Y;\n    }\n\n    // manipulation\n    if (inStr(actions, TOUCH_ACTION_MANIPULATION)) {\n        return TOUCH_ACTION_MANIPULATION;\n    }\n\n    return TOUCH_ACTION_AUTO;\n}\n\nfunction getTouchActionProps() {\n    if (!NATIVE_TOUCH_ACTION) {\n        return false;\n    }\n    var touchMap = {};\n    var cssSupports = window.CSS && window.CSS.supports;\n    ['auto', 'manipulation', 'pan-y', 'pan-x', 'pan-x pan-y', 'none'].forEach(function(val) {\n\n        // If css.supports is not supported but there is native touch-action assume it supports\n        // all values. This is the case for IE 10 and 11.\n        touchMap[val] = cssSupports ? window.CSS.supports('touch-action', val) : true;\n    });\n    return touchMap;\n}\n\n/**\n * Recognizer flow explained; *\n * All recognizers have the initial state of POSSIBLE when a input session starts.\n * The definition of a input session is from the first input until the last input, with all it's movement in it. *\n * Example session for mouse-input: mousedown -> mousemove -> mouseup\n *\n * On each recognizing cycle (see Manager.recognize) the .recognize() method is executed\n * which determines with state it should be.\n *\n * If the recognizer has the state FAILED, CANCELLED or RECOGNIZED (equals ENDED), it is reset to\n * POSSIBLE to give it another change on the next cycle.\n *\n *               Possible\n *                  |\n *            +-----+---------------+\n *            |                     |\n *      +-----+-----+               |\n *      |           |               |\n *   Failed      Cancelled          |\n *                          +-------+------+\n *                          |              |\n *                      Recognized       Began\n *                                         |\n *                                      Changed\n *                                         |\n *                                  Ended/Recognized\n */\nvar STATE_POSSIBLE = 1;\nvar STATE_BEGAN = 2;\nvar STATE_CHANGED = 4;\nvar STATE_ENDED = 8;\nvar STATE_RECOGNIZED = STATE_ENDED;\nvar STATE_CANCELLED = 16;\nvar STATE_FAILED = 32;\n\n/**\n * Recognizer\n * Every recognizer needs to extend from this class.\n * @constructor\n * @param {Object} options\n */\nfunction Recognizer(options) {\n    this.options = assign({}, this.defaults, options || {});\n\n    this.id = uniqueId();\n\n    this.manager = null;\n\n    // default is enable true\n    this.options.enable = ifUndefined(this.options.enable, true);\n\n    this.state = STATE_POSSIBLE;\n\n    this.simultaneous = {};\n    this.requireFail = [];\n}\n\nRecognizer.prototype = {\n    /**\n     * @virtual\n     * @type {Object}\n     */\n    defaults: {},\n\n    /**\n     * set options\n     * @param {Object} options\n     * @return {Recognizer}\n     */\n    set: function(options) {\n        assign(this.options, options);\n\n        // also update the touchAction, in case something changed about the directions/enabled state\n        this.manager && this.manager.touchAction.update();\n        return this;\n    },\n\n    /**\n     * recognize simultaneous with an other recognizer.\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    recognizeWith: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'recognizeWith', this)) {\n            return this;\n        }\n\n        var simultaneous = this.simultaneous;\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        if (!simultaneous[otherRecognizer.id]) {\n            simultaneous[otherRecognizer.id] = otherRecognizer;\n            otherRecognizer.recognizeWith(this);\n        }\n        return this;\n    },\n\n    /**\n     * drop the simultaneous link. it doesnt remove the link on the other recognizer.\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    dropRecognizeWith: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'dropRecognizeWith', this)) {\n            return this;\n        }\n\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        delete this.simultaneous[otherRecognizer.id];\n        return this;\n    },\n\n    /**\n     * recognizer can only run when an other is failing\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    requireFailure: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'requireFailure', this)) {\n            return this;\n        }\n\n        var requireFail = this.requireFail;\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        if (inArray(requireFail, otherRecognizer) === -1) {\n            requireFail.push(otherRecognizer);\n            otherRecognizer.requireFailure(this);\n        }\n        return this;\n    },\n\n    /**\n     * drop the requireFailure link. it does not remove the link on the other recognizer.\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    dropRequireFailure: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'dropRequireFailure', this)) {\n            return this;\n        }\n\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        var index = inArray(this.requireFail, otherRecognizer);\n        if (index > -1) {\n            this.requireFail.splice(index, 1);\n        }\n        return this;\n    },\n\n    /**\n     * has require failures boolean\n     * @returns {boolean}\n     */\n    hasRequireFailures: function() {\n        return this.requireFail.length > 0;\n    },\n\n    /**\n     * if the recognizer can recognize simultaneous with an other recognizer\n     * @param {Recognizer} otherRecognizer\n     * @returns {Boolean}\n     */\n    canRecognizeWith: function(otherRecognizer) {\n        return !!this.simultaneous[otherRecognizer.id];\n    },\n\n    /**\n     * You should use `tryEmit` instead of `emit` directly to check\n     * that all the needed recognizers has failed before emitting.\n     * @param {Object} input\n     */\n    emit: function(input) {\n        var self = this;\n        var state = this.state;\n\n        function emit(event) {\n            self.manager.emit(event, input);\n        }\n\n        // 'panstart' and 'panmove'\n        if (state < STATE_ENDED) {\n            emit(self.options.event + stateStr(state));\n        }\n\n        emit(self.options.event); // simple 'eventName' events\n\n        if (input.additionalEvent) { // additional event(panleft, panright, pinchin, pinchout...)\n            emit(input.additionalEvent);\n        }\n\n        // panend and pancancel\n        if (state >= STATE_ENDED) {\n            emit(self.options.event + stateStr(state));\n        }\n    },\n\n    /**\n     * Check that all the require failure recognizers has failed,\n     * if true, it emits a gesture event,\n     * otherwise, setup the state to FAILED.\n     * @param {Object} input\n     */\n    tryEmit: function(input) {\n        if (this.canEmit()) {\n            return this.emit(input);\n        }\n        // it's failing anyway\n        this.state = STATE_FAILED;\n    },\n\n    /**\n     * can we emit?\n     * @returns {boolean}\n     */\n    canEmit: function() {\n        var i = 0;\n        while (i < this.requireFail.length) {\n            if (!(this.requireFail[i].state & (STATE_FAILED | STATE_POSSIBLE))) {\n                return false;\n            }\n            i++;\n        }\n        return true;\n    },\n\n    /**\n     * update the recognizer\n     * @param {Object} inputData\n     */\n    recognize: function(inputData) {\n        // make a new copy of the inputData\n        // so we can change the inputData without messing up the other recognizers\n        var inputDataClone = assign({}, inputData);\n\n        // is is enabled and allow recognizing?\n        if (!boolOrFn(this.options.enable, [this, inputDataClone])) {\n            this.reset();\n            this.state = STATE_FAILED;\n            return;\n        }\n\n        // reset when we've reached the end\n        if (this.state & (STATE_RECOGNIZED | STATE_CANCELLED | STATE_FAILED)) {\n            this.state = STATE_POSSIBLE;\n        }\n\n        this.state = this.process(inputDataClone);\n\n        // the recognizer has recognized a gesture\n        // so trigger an event\n        if (this.state & (STATE_BEGAN | STATE_CHANGED | STATE_ENDED | STATE_CANCELLED)) {\n            this.tryEmit(inputDataClone);\n        }\n    },\n\n    /**\n     * return the state of the recognizer\n     * the actual recognizing happens in this method\n     * @virtual\n     * @param {Object} inputData\n     * @returns {Const} STATE\n     */\n    process: function(inputData) { }, // jshint ignore:line\n\n    /**\n     * return the preferred touch-action\n     * @virtual\n     * @returns {Array}\n     */\n    getTouchAction: function() { },\n\n    /**\n     * called when the gesture isn't allowed to recognize\n     * like when another is being recognized or it is disabled\n     * @virtual\n     */\n    reset: function() { }\n};\n\n/**\n * get a usable string, used as event postfix\n * @param {Const} state\n * @returns {String} state\n */\nfunction stateStr(state) {\n    if (state & STATE_CANCELLED) {\n        return 'cancel';\n    } else if (state & STATE_ENDED) {\n        return 'end';\n    } else if (state & STATE_CHANGED) {\n        return 'move';\n    } else if (state & STATE_BEGAN) {\n        return 'start';\n    }\n    return '';\n}\n\n/**\n * direction cons to string\n * @param {Const} direction\n * @returns {String}\n */\nfunction directionStr(direction) {\n    if (direction == DIRECTION_DOWN) {\n        return 'down';\n    } else if (direction == DIRECTION_UP) {\n        return 'up';\n    } else if (direction == DIRECTION_LEFT) {\n        return 'left';\n    } else if (direction == DIRECTION_RIGHT) {\n        return 'right';\n    }\n    return '';\n}\n\n/**\n * get a recognizer by name if it is bound to a manager\n * @param {Recognizer|String} otherRecognizer\n * @param {Recognizer} recognizer\n * @returns {Recognizer}\n */\nfunction getRecognizerByNameIfManager(otherRecognizer, recognizer) {\n    var manager = recognizer.manager;\n    if (manager) {\n        return manager.get(otherRecognizer);\n    }\n    return otherRecognizer;\n}\n\n/**\n * This recognizer is just used as a base for the simple attribute recognizers.\n * @constructor\n * @extends Recognizer\n */\nfunction AttrRecognizer() {\n    Recognizer.apply(this, arguments);\n}\n\ninherit(AttrRecognizer, Recognizer, {\n    /**\n     * @namespace\n     * @memberof AttrRecognizer\n     */\n    defaults: {\n        /**\n         * @type {Number}\n         * @default 1\n         */\n        pointers: 1\n    },\n\n    /**\n     * Used to check if it the recognizer receives valid input, like input.distance > 10.\n     * @memberof AttrRecognizer\n     * @param {Object} input\n     * @returns {Boolean} recognized\n     */\n    attrTest: function(input) {\n        var optionPointers = this.options.pointers;\n        return optionPointers === 0 || input.pointers.length === optionPointers;\n    },\n\n    /**\n     * Process the input and return the state for the recognizer\n     * @memberof AttrRecognizer\n     * @param {Object} input\n     * @returns {*} State\n     */\n    process: function(input) {\n        var state = this.state;\n        var eventType = input.eventType;\n\n        var isRecognized = state & (STATE_BEGAN | STATE_CHANGED);\n        var isValid = this.attrTest(input);\n\n        // on cancel input and we've recognized before, return STATE_CANCELLED\n        if (isRecognized && (eventType & INPUT_CANCEL || !isValid)) {\n            return state | STATE_CANCELLED;\n        } else if (isRecognized || isValid) {\n            if (eventType & INPUT_END) {\n                return state | STATE_ENDED;\n            } else if (!(state & STATE_BEGAN)) {\n                return STATE_BEGAN;\n            }\n            return state | STATE_CHANGED;\n        }\n        return STATE_FAILED;\n    }\n});\n\n/**\n * Pan\n * Recognized when the pointer is down and moved in the allowed direction.\n * @constructor\n * @extends AttrRecognizer\n */\nfunction PanRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n\n    this.pX = null;\n    this.pY = null;\n}\n\ninherit(PanRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof PanRecognizer\n     */\n    defaults: {\n        event: 'pan',\n        threshold: 10,\n        pointers: 1,\n        direction: DIRECTION_ALL\n    },\n\n    getTouchAction: function() {\n        var direction = this.options.direction;\n        var actions = [];\n        if (direction & DIRECTION_HORIZONTAL) {\n            actions.push(TOUCH_ACTION_PAN_Y);\n        }\n        if (direction & DIRECTION_VERTICAL) {\n            actions.push(TOUCH_ACTION_PAN_X);\n        }\n        return actions;\n    },\n\n    directionTest: function(input) {\n        var options = this.options;\n        var hasMoved = true;\n        var distance = input.distance;\n        var direction = input.direction;\n        var x = input.deltaX;\n        var y = input.deltaY;\n\n        // lock to axis?\n        if (!(direction & options.direction)) {\n            if (options.direction & DIRECTION_HORIZONTAL) {\n                direction = (x === 0) ? DIRECTION_NONE : (x < 0) ? DIRECTION_LEFT : DIRECTION_RIGHT;\n                hasMoved = x != this.pX;\n                distance = Math.abs(input.deltaX);\n            } else {\n                direction = (y === 0) ? DIRECTION_NONE : (y < 0) ? DIRECTION_UP : DIRECTION_DOWN;\n                hasMoved = y != this.pY;\n                distance = Math.abs(input.deltaY);\n            }\n        }\n        input.direction = direction;\n        return hasMoved && distance > options.threshold && direction & options.direction;\n    },\n\n    attrTest: function(input) {\n        return AttrRecognizer.prototype.attrTest.call(this, input) &&\n            (this.state & STATE_BEGAN || (!(this.state & STATE_BEGAN) && this.directionTest(input)));\n    },\n\n    emit: function(input) {\n\n        this.pX = input.deltaX;\n        this.pY = input.deltaY;\n\n        var direction = directionStr(input.direction);\n\n        if (direction) {\n            input.additionalEvent = this.options.event + direction;\n        }\n        this._super.emit.call(this, input);\n    }\n});\n\n/**\n * Pinch\n * Recognized when two or more pointers are moving toward (zoom-in) or away from each other (zoom-out).\n * @constructor\n * @extends AttrRecognizer\n */\nfunction PinchRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n}\n\ninherit(PinchRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof PinchRecognizer\n     */\n    defaults: {\n        event: 'pinch',\n        threshold: 0,\n        pointers: 2\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_NONE];\n    },\n\n    attrTest: function(input) {\n        return this._super.attrTest.call(this, input) &&\n            (Math.abs(input.scale - 1) > this.options.threshold || this.state & STATE_BEGAN);\n    },\n\n    emit: function(input) {\n        if (input.scale !== 1) {\n            var inOut = input.scale < 1 ? 'in' : 'out';\n            input.additionalEvent = this.options.event + inOut;\n        }\n        this._super.emit.call(this, input);\n    }\n});\n\n/**\n * Press\n * Recognized when the pointer is down for x ms without any movement.\n * @constructor\n * @extends Recognizer\n */\nfunction PressRecognizer() {\n    Recognizer.apply(this, arguments);\n\n    this._timer = null;\n    this._input = null;\n}\n\ninherit(PressRecognizer, Recognizer, {\n    /**\n     * @namespace\n     * @memberof PressRecognizer\n     */\n    defaults: {\n        event: 'press',\n        pointers: 1,\n        time: 251, // minimal time of the pointer to be pressed\n        threshold: 9 // a minimal movement is ok, but keep it low\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_AUTO];\n    },\n\n    process: function(input) {\n        var options = this.options;\n        var validPointers = input.pointers.length === options.pointers;\n        var validMovement = input.distance < options.threshold;\n        var validTime = input.deltaTime > options.time;\n\n        this._input = input;\n\n        // we only allow little movement\n        // and we've reached an end event, so a tap is possible\n        if (!validMovement || !validPointers || (input.eventType & (INPUT_END | INPUT_CANCEL) && !validTime)) {\n            this.reset();\n        } else if (input.eventType & INPUT_START) {\n            this.reset();\n            this._timer = setTimeoutContext(function() {\n                this.state = STATE_RECOGNIZED;\n                this.tryEmit();\n            }, options.time, this);\n        } else if (input.eventType & INPUT_END) {\n            return STATE_RECOGNIZED;\n        }\n        return STATE_FAILED;\n    },\n\n    reset: function() {\n        clearTimeout(this._timer);\n    },\n\n    emit: function(input) {\n        if (this.state !== STATE_RECOGNIZED) {\n            return;\n        }\n\n        if (input && (input.eventType & INPUT_END)) {\n            this.manager.emit(this.options.event + 'up', input);\n        } else {\n            this._input.timeStamp = now();\n            this.manager.emit(this.options.event, this._input);\n        }\n    }\n});\n\n/**\n * Rotate\n * Recognized when two or more pointer are moving in a circular motion.\n * @constructor\n * @extends AttrRecognizer\n */\nfunction RotateRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n}\n\ninherit(RotateRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof RotateRecognizer\n     */\n    defaults: {\n        event: 'rotate',\n        threshold: 0,\n        pointers: 2\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_NONE];\n    },\n\n    attrTest: function(input) {\n        return this._super.attrTest.call(this, input) &&\n            (Math.abs(input.rotation) > this.options.threshold || this.state & STATE_BEGAN);\n    }\n});\n\n/**\n * Swipe\n * Recognized when the pointer is moving fast (velocity), with enough distance in the allowed direction.\n * @constructor\n * @extends AttrRecognizer\n */\nfunction SwipeRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n}\n\ninherit(SwipeRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof SwipeRecognizer\n     */\n    defaults: {\n        event: 'swipe',\n        threshold: 10,\n        velocity: 0.3,\n        direction: DIRECTION_HORIZONTAL | DIRECTION_VERTICAL,\n        pointers: 1\n    },\n\n    getTouchAction: function() {\n        return PanRecognizer.prototype.getTouchAction.call(this);\n    },\n\n    attrTest: function(input) {\n        var direction = this.options.direction;\n        var velocity;\n\n        if (direction & (DIRECTION_HORIZONTAL | DIRECTION_VERTICAL)) {\n            velocity = input.overallVelocity;\n        } else if (direction & DIRECTION_HORIZONTAL) {\n            velocity = input.overallVelocityX;\n        } else if (direction & DIRECTION_VERTICAL) {\n            velocity = input.overallVelocityY;\n        }\n\n        return this._super.attrTest.call(this, input) &&\n            direction & input.offsetDirection &&\n            input.distance > this.options.threshold &&\n            input.maxPointers == this.options.pointers &&\n            abs(velocity) > this.options.velocity && input.eventType & INPUT_END;\n    },\n\n    emit: function(input) {\n        var direction = directionStr(input.offsetDirection);\n        if (direction) {\n            this.manager.emit(this.options.event + direction, input);\n        }\n\n        this.manager.emit(this.options.event, input);\n    }\n});\n\n/**\n * A tap is ecognized when the pointer is doing a small tap/click. Multiple taps are recognized if they occur\n * between the given interval and position. The delay option can be used to recognize multi-taps without firing\n * a single tap.\n *\n * The eventData from the emitted event contains the property `tapCount`, which contains the amount of\n * multi-taps being recognized.\n * @constructor\n * @extends Recognizer\n */\nfunction TapRecognizer() {\n    Recognizer.apply(this, arguments);\n\n    // previous time and center,\n    // used for tap counting\n    this.pTime = false;\n    this.pCenter = false;\n\n    this._timer = null;\n    this._input = null;\n    this.count = 0;\n}\n\ninherit(TapRecognizer, Recognizer, {\n    /**\n     * @namespace\n     * @memberof PinchRecognizer\n     */\n    defaults: {\n        event: 'tap',\n        pointers: 1,\n        taps: 1,\n        interval: 300, // max time between the multi-tap taps\n        time: 250, // max time of the pointer to be down (like finger on the screen)\n        threshold: 9, // a minimal movement is ok, but keep it low\n        posThreshold: 10 // a multi-tap can be a bit off the initial position\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_MANIPULATION];\n    },\n\n    process: function(input) {\n        var options = this.options;\n\n        var validPointers = input.pointers.length === options.pointers;\n        var validMovement = input.distance < options.threshold;\n        var validTouchTime = input.deltaTime < options.time;\n\n        this.reset();\n\n        if ((input.eventType & INPUT_START) && (this.count === 0)) {\n            return this.failTimeout();\n        }\n\n        // we only allow little movement\n        // and we've reached an end event, so a tap is possible\n        if (validMovement && validTouchTime && validPointers) {\n            if (input.eventType != INPUT_END) {\n                return this.failTimeout();\n            }\n\n            var validInterval = this.pTime ? (input.timeStamp - this.pTime < options.interval) : true;\n            var validMultiTap = !this.pCenter || getDistance(this.pCenter, input.center) < options.posThreshold;\n\n            this.pTime = input.timeStamp;\n            this.pCenter = input.center;\n\n            if (!validMultiTap || !validInterval) {\n                this.count = 1;\n            } else {\n                this.count += 1;\n            }\n\n            this._input = input;\n\n            // if tap count matches we have recognized it,\n            // else it has began recognizing...\n            var tapCount = this.count % options.taps;\n            if (tapCount === 0) {\n                // no failing requirements, immediately trigger the tap event\n                // or wait as long as the multitap interval to trigger\n                if (!this.hasRequireFailures()) {\n                    return STATE_RECOGNIZED;\n                } else {\n                    this._timer = setTimeoutContext(function() {\n                        this.state = STATE_RECOGNIZED;\n                        this.tryEmit();\n                    }, options.interval, this);\n                    return STATE_BEGAN;\n                }\n            }\n        }\n        return STATE_FAILED;\n    },\n\n    failTimeout: function() {\n        this._timer = setTimeoutContext(function() {\n            this.state = STATE_FAILED;\n        }, this.options.interval, this);\n        return STATE_FAILED;\n    },\n\n    reset: function() {\n        clearTimeout(this._timer);\n    },\n\n    emit: function() {\n        if (this.state == STATE_RECOGNIZED) {\n            this._input.tapCount = this.count;\n            this.manager.emit(this.options.event, this._input);\n        }\n    }\n});\n\n/**\n * Simple way to create a manager with a default set of recognizers.\n * @param {HTMLElement} element\n * @param {Object} [options]\n * @constructor\n */\nfunction Hammer(element, options) {\n    options = options || {};\n    options.recognizers = ifUndefined(options.recognizers, Hammer.defaults.preset);\n    return new Manager(element, options);\n}\n\n/**\n * @const {string}\n */\nHammer.VERSION = '2.0.7';\n\n/**\n * default settings\n * @namespace\n */\nHammer.defaults = {\n    /**\n     * set if DOM events are being triggered.\n     * But this is slower and unused by simple implementations, so disabled by default.\n     * @type {Boolean}\n     * @default false\n     */\n    domEvents: false,\n\n    /**\n     * The value for the touchAction property/fallback.\n     * When set to `compute` it will magically set the correct value based on the added recognizers.\n     * @type {String}\n     * @default compute\n     */\n    touchAction: TOUCH_ACTION_COMPUTE,\n\n    /**\n     * @type {Boolean}\n     * @default true\n     */\n    enable: true,\n\n    /**\n     * EXPERIMENTAL FEATURE -- can be removed/changed\n     * Change the parent input target element.\n     * If Null, then it is being set the to main element.\n     * @type {Null|EventTarget}\n     * @default null\n     */\n    inputTarget: null,\n\n    /**\n     * force an input class\n     * @type {Null|Function}\n     * @default null\n     */\n    inputClass: null,\n\n    /**\n     * Default recognizer setup when calling `Hammer()`\n     * When creating a new Manager these will be skipped.\n     * @type {Array}\n     */\n    preset: [\n        // RecognizerClass, options, [recognizeWith, ...], [requireFailure, ...]\n        [RotateRecognizer, {enable: false}],\n        [PinchRecognizer, {enable: false}, ['rotate']],\n        [SwipeRecognizer, {direction: DIRECTION_HORIZONTAL}],\n        [PanRecognizer, {direction: DIRECTION_HORIZONTAL}, ['swipe']],\n        [TapRecognizer],\n        [TapRecognizer, {event: 'doubletap', taps: 2}, ['tap']],\n        [PressRecognizer]\n    ],\n\n    /**\n     * Some CSS properties can be used to improve the working of Hammer.\n     * Add them to this method and they will be set when creating a new Manager.\n     * @namespace\n     */\n    cssProps: {\n        /**\n         * Disables text selection to improve the dragging gesture. Mainly for desktop browsers.\n         * @type {String}\n         * @default 'none'\n         */\n        userSelect: 'none',\n\n        /**\n         * Disable the Windows Phone grippers when pressing an element.\n         * @type {String}\n         * @default 'none'\n         */\n        touchSelect: 'none',\n\n        /**\n         * Disables the default callout shown when you touch and hold a touch target.\n         * On iOS, when you touch and hold a touch target such as a link, Safari displays\n         * a callout containing information about the link. This property allows you to disable that callout.\n         * @type {String}\n         * @default 'none'\n         */\n        touchCallout: 'none',\n\n        /**\n         * Specifies whether zooming is enabled. Used by IE10>\n         * @type {String}\n         * @default 'none'\n         */\n        contentZooming: 'none',\n\n        /**\n         * Specifies that an entire element should be draggable instead of its contents. Mainly for desktop browsers.\n         * @type {String}\n         * @default 'none'\n         */\n        userDrag: 'none',\n\n        /**\n         * Overrides the highlight color shown when the user taps a link or a JavaScript\n         * clickable element in iOS. This property obeys the alpha value, if specified.\n         * @type {String}\n         * @default 'rgba(0,0,0,0)'\n         */\n        tapHighlightColor: 'rgba(0,0,0,0)'\n    }\n};\n\nvar STOP = 1;\nvar FORCED_STOP = 2;\n\n/**\n * Manager\n * @param {HTMLElement} element\n * @param {Object} [options]\n * @constructor\n */\nfunction Manager(element, options) {\n    this.options = assign({}, Hammer.defaults, options || {});\n\n    this.options.inputTarget = this.options.inputTarget || element;\n\n    this.handlers = {};\n    this.session = {};\n    this.recognizers = [];\n    this.oldCssProps = {};\n\n    this.element = element;\n    this.input = createInputInstance(this);\n    this.touchAction = new TouchAction(this, this.options.touchAction);\n\n    toggleCssProps(this, true);\n\n    each(this.options.recognizers, function(item) {\n        var recognizer = this.add(new (item[0])(item[1]));\n        item[2] && recognizer.recognizeWith(item[2]);\n        item[3] && recognizer.requireFailure(item[3]);\n    }, this);\n}\n\nManager.prototype = {\n    /**\n     * set options\n     * @param {Object} options\n     * @returns {Manager}\n     */\n    set: function(options) {\n        assign(this.options, options);\n\n        // Options that need a little more setup\n        if (options.touchAction) {\n            this.touchAction.update();\n        }\n        if (options.inputTarget) {\n            // Clean up existing event listeners and reinitialize\n            this.input.destroy();\n            this.input.target = options.inputTarget;\n            this.input.init();\n        }\n        return this;\n    },\n\n    /**\n     * stop recognizing for this session.\n     * This session will be discarded, when a new [input]start event is fired.\n     * When forced, the recognizer cycle is stopped immediately.\n     * @param {Boolean} [force]\n     */\n    stop: function(force) {\n        this.session.stopped = force ? FORCED_STOP : STOP;\n    },\n\n    /**\n     * run the recognizers!\n     * called by the inputHandler function on every movement of the pointers (touches)\n     * it walks through all the recognizers and tries to detect the gesture that is being made\n     * @param {Object} inputData\n     */\n    recognize: function(inputData) {\n        var session = this.session;\n        if (session.stopped) {\n            return;\n        }\n\n        // run the touch-action polyfill\n        this.touchAction.preventDefaults(inputData);\n\n        var recognizer;\n        var recognizers = this.recognizers;\n\n        // this holds the recognizer that is being recognized.\n        // so the recognizer's state needs to be BEGAN, CHANGED, ENDED or RECOGNIZED\n        // if no recognizer is detecting a thing, it is set to `null`\n        var curRecognizer = session.curRecognizer;\n\n        // reset when the last recognizer is recognized\n        // or when we're in a new session\n        if (!curRecognizer || (curRecognizer && curRecognizer.state & STATE_RECOGNIZED)) {\n            curRecognizer = session.curRecognizer = null;\n        }\n\n        var i = 0;\n        while (i < recognizers.length) {\n            recognizer = recognizers[i];\n\n            // find out if we are allowed try to recognize the input for this one.\n            // 1.   allow if the session is NOT forced stopped (see the .stop() method)\n            // 2.   allow if we still haven't recognized a gesture in this session, or the this recognizer is the one\n            //      that is being recognized.\n            // 3.   allow if the recognizer is allowed to run simultaneous with the current recognized recognizer.\n            //      this can be setup with the `recognizeWith()` method on the recognizer.\n            if (session.stopped !== FORCED_STOP && ( // 1\n                    !curRecognizer || recognizer == curRecognizer || // 2\n                    recognizer.canRecognizeWith(curRecognizer))) { // 3\n                recognizer.recognize(inputData);\n            } else {\n                recognizer.reset();\n            }\n\n            // if the recognizer has been recognizing the input as a valid gesture, we want to store this one as the\n            // current active recognizer. but only if we don't already have an active recognizer\n            if (!curRecognizer && recognizer.state & (STATE_BEGAN | STATE_CHANGED | STATE_ENDED)) {\n                curRecognizer = session.curRecognizer = recognizer;\n            }\n            i++;\n        }\n    },\n\n    /**\n     * get a recognizer by its event name.\n     * @param {Recognizer|String} recognizer\n     * @returns {Recognizer|Null}\n     */\n    get: function(recognizer) {\n        if (recognizer instanceof Recognizer) {\n            return recognizer;\n        }\n\n        var recognizers = this.recognizers;\n        for (var i = 0; i < recognizers.length; i++) {\n            if (recognizers[i].options.event == recognizer) {\n                return recognizers[i];\n            }\n        }\n        return null;\n    },\n\n    /**\n     * add a recognizer to the manager\n     * existing recognizers with the same event name will be removed\n     * @param {Recognizer} recognizer\n     * @returns {Recognizer|Manager}\n     */\n    add: function(recognizer) {\n        if (invokeArrayArg(recognizer, 'add', this)) {\n            return this;\n        }\n\n        // remove existing\n        var existing = this.get(recognizer.options.event);\n        if (existing) {\n            this.remove(existing);\n        }\n\n        this.recognizers.push(recognizer);\n        recognizer.manager = this;\n\n        this.touchAction.update();\n        return recognizer;\n    },\n\n    /**\n     * remove a recognizer by name or instance\n     * @param {Recognizer|String} recognizer\n     * @returns {Manager}\n     */\n    remove: function(recognizer) {\n        if (invokeArrayArg(recognizer, 'remove', this)) {\n            return this;\n        }\n\n        recognizer = this.get(recognizer);\n\n        // let's make sure this recognizer exists\n        if (recognizer) {\n            var recognizers = this.recognizers;\n            var index = inArray(recognizers, recognizer);\n\n            if (index !== -1) {\n                recognizers.splice(index, 1);\n                this.touchAction.update();\n            }\n        }\n\n        return this;\n    },\n\n    /**\n     * bind event\n     * @param {String} events\n     * @param {Function} handler\n     * @returns {EventEmitter} this\n     */\n    on: function(events, handler) {\n        if (events === undefined) {\n            return;\n        }\n        if (handler === undefined) {\n            return;\n        }\n\n        var handlers = this.handlers;\n        each(splitStr(events), function(event) {\n            handlers[event] = handlers[event] || [];\n            handlers[event].push(handler);\n        });\n        return this;\n    },\n\n    /**\n     * unbind event, leave emit blank to remove all handlers\n     * @param {String} events\n     * @param {Function} [handler]\n     * @returns {EventEmitter} this\n     */\n    off: function(events, handler) {\n        if (events === undefined) {\n            return;\n        }\n\n        var handlers = this.handlers;\n        each(splitStr(events), function(event) {\n            if (!handler) {\n                delete handlers[event];\n            } else {\n                handlers[event] && handlers[event].splice(inArray(handlers[event], handler), 1);\n            }\n        });\n        return this;\n    },\n\n    /**\n     * emit event to the listeners\n     * @param {String} event\n     * @param {Object} data\n     */\n    emit: function(event, data) {\n        // we also want to trigger dom events\n        if (this.options.domEvents) {\n            triggerDomEvent(event, data);\n        }\n\n        // no handlers, so skip it all\n        var handlers = this.handlers[event] && this.handlers[event].slice();\n        if (!handlers || !handlers.length) {\n            return;\n        }\n\n        data.type = event;\n        data.preventDefault = function() {\n            data.srcEvent.preventDefault();\n        };\n\n        var i = 0;\n        while (i < handlers.length) {\n            handlers[i](data);\n            i++;\n        }\n    },\n\n    /**\n     * destroy the manager and unbinds all events\n     * it doesn't unbind dom events, that is the user own responsibility\n     */\n    destroy: function() {\n        this.element && toggleCssProps(this, false);\n\n        this.handlers = {};\n        this.session = {};\n        this.input.destroy();\n        this.element = null;\n    }\n};\n\n/**\n * add/remove the css properties as defined in manager.options.cssProps\n * @param {Manager} manager\n * @param {Boolean} add\n */\nfunction toggleCssProps(manager, add) {\n    var element = manager.element;\n    if (!element.style) {\n        return;\n    }\n    var prop;\n    each(manager.options.cssProps, function(value, name) {\n        prop = prefixed(element.style, name);\n        if (add) {\n            manager.oldCssProps[prop] = element.style[prop];\n            element.style[prop] = value;\n        } else {\n            element.style[prop] = manager.oldCssProps[prop] || '';\n        }\n    });\n    if (!add) {\n        manager.oldCssProps = {};\n    }\n}\n\n/**\n * trigger dom event\n * @param {String} event\n * @param {Object} data\n */\nfunction triggerDomEvent(event, data) {\n    var gestureEvent = document.createEvent('Event');\n    gestureEvent.initEvent(event, true, true);\n    gestureEvent.gesture = data;\n    data.target.dispatchEvent(gestureEvent);\n}\n\nassign(Hammer, {\n    INPUT_START: INPUT_START,\n    INPUT_MOVE: INPUT_MOVE,\n    INPUT_END: INPUT_END,\n    INPUT_CANCEL: INPUT_CANCEL,\n\n    STATE_POSSIBLE: STATE_POSSIBLE,\n    STATE_BEGAN: STATE_BEGAN,\n    STATE_CHANGED: STATE_CHANGED,\n    STATE_ENDED: STATE_ENDED,\n    STATE_RECOGNIZED: STATE_RECOGNIZED,\n    STATE_CANCELLED: STATE_CANCELLED,\n    STATE_FAILED: STATE_FAILED,\n\n    DIRECTION_NONE: DIRECTION_NONE,\n    DIRECTION_LEFT: DIRECTION_LEFT,\n    DIRECTION_RIGHT: DIRECTION_RIGHT,\n    DIRECTION_UP: DIRECTION_UP,\n    DIRECTION_DOWN: DIRECTION_DOWN,\n    DIRECTION_HORIZONTAL: DIRECTION_HORIZONTAL,\n    DIRECTION_VERTICAL: DIRECTION_VERTICAL,\n    DIRECTION_ALL: DIRECTION_ALL,\n\n    Manager: Manager,\n    Input: Input,\n    TouchAction: TouchAction,\n\n    TouchInput: TouchInput,\n    MouseInput: MouseInput,\n    PointerEventInput: PointerEventInput,\n    TouchMouseInput: TouchMouseInput,\n    SingleTouchInput: SingleTouchInput,\n\n    Recognizer: Recognizer,\n    AttrRecognizer: AttrRecognizer,\n    Tap: TapRecognizer,\n    Pan: PanRecognizer,\n    Swipe: SwipeRecognizer,\n    Pinch: PinchRecognizer,\n    Rotate: RotateRecognizer,\n    Press: PressRecognizer,\n\n    on: addEventListeners,\n    off: removeEventListeners,\n    each: each,\n    merge: merge,\n    extend: extend,\n    assign: assign,\n    inherit: inherit,\n    bindFn: bindFn,\n    prefixed: prefixed\n});\n\n// this prevents errors when Hammer is loaded in the presence of an AMD\n//  style loader but by script tag, not by the loader.\nvar freeGlobal = (typeof window !== 'undefined' ? window : (typeof self !== 'undefined' ? self : {})); // jshint ignore:line\nfreeGlobal.Hammer = Hammer;\n\nif (typeof define === 'function' && define.amd) {\n    define(function() {\n        return Hammer;\n    });\n} else if (typeof module != 'undefined' && module.exports) {\n    module.exports = Hammer;\n} else {\n    window[exportName] = Hammer;\n}\n\n})(window, document, 'Hammer');\n",
         "'use strict';\n\nvar reactIs = require('react-is');\n\n/**\n * Copyright 2015, Yahoo! Inc.\n * Copyrights licensed under the New BSD License. See the accompanying LICENSE file for terms.\n */\nvar REACT_STATICS = {\n  childContextTypes: true,\n  contextType: true,\n  contextTypes: true,\n  defaultProps: true,\n  displayName: true,\n  getDefaultProps: true,\n  getDerivedStateFromError: true,\n  getDerivedStateFromProps: true,\n  mixins: true,\n  propTypes: true,\n  type: true\n};\nvar KNOWN_STATICS = {\n  name: true,\n  length: true,\n  prototype: true,\n  caller: true,\n  callee: true,\n  arguments: true,\n  arity: true\n};\nvar FORWARD_REF_STATICS = {\n  '$$typeof': true,\n  render: true,\n  defaultProps: true,\n  displayName: true,\n  propTypes: true\n};\nvar MEMO_STATICS = {\n  '$$typeof': true,\n  compare: true,\n  defaultProps: true,\n  displayName: true,\n  propTypes: true,\n  type: true\n};\nvar TYPE_STATICS = {};\nTYPE_STATICS[reactIs.ForwardRef] = FORWARD_REF_STATICS;\nTYPE_STATICS[reactIs.Memo] = MEMO_STATICS;\n\nfunction getStatics(component) {\n  // React v16.11 and below\n  if (reactIs.isMemo(component)) {\n    return MEMO_STATICS;\n  } // React v16.12 and above\n\n\n  return TYPE_STATICS[component['$$typeof']] || REACT_STATICS;\n}\n\nvar defineProperty = Object.defineProperty;\nvar getOwnPropertyNames = Object.getOwnPropertyNames;\nvar getOwnPropertySymbols = Object.getOwnPropertySymbols;\nvar getOwnPropertyDescriptor = Object.getOwnPropertyDescriptor;\nvar getPrototypeOf = Object.getPrototypeOf;\nvar objectPrototype = Object.prototype;\nfunction hoistNonReactStatics(targetComponent, sourceComponent, blacklist) {\n  if (typeof sourceComponent !== 'string') {\n    // don't hoist over string (html) components\n    if (objectPrototype) {\n      var inheritedComponent = getPrototypeOf(sourceComponent);\n\n      if (inheritedComponent && inheritedComponent !== objectPrototype) {\n        hoistNonReactStatics(targetComponent, inheritedComponent, blacklist);\n      }\n    }\n\n    var keys = getOwnPropertyNames(sourceComponent);\n\n    if (getOwnPropertySymbols) {\n      keys = keys.concat(getOwnPropertySymbols(sourceComponent));\n    }\n\n    var targetStatics = getStatics(targetComponent);\n    var sourceStatics = getStatics(sourceComponent);\n\n    for (var i = 0; i < keys.length; ++i) {\n      var key = keys[i];\n\n      if (!KNOWN_STATICS[key] && !(blacklist && blacklist[key]) && !(sourceStatics && sourceStatics[key]) && !(targetStatics && targetStatics[key])) {\n        var descriptor = getOwnPropertyDescriptor(sourceComponent, key);\n\n        try {\n          // Avoid failures from read-only properties\n          defineProperty(targetComponent, key, descriptor);\n        } catch (e) {}\n      }\n    }\n  }\n\n  return targetComponent;\n}\n\nmodule.exports = hoistNonReactStatics;\n",
         "/*\nobject-assign\n(c) Sindre Sorhus\n@license MIT\n*/\n\n'use strict';\n/* eslint-disable no-unused-vars */\nvar getOwnPropertySymbols = Object.getOwnPropertySymbols;\nvar hasOwnProperty = Object.prototype.hasOwnProperty;\nvar propIsEnumerable = Object.prototype.propertyIsEnumerable;\n\nfunction toObject(val) {\n\tif (val === null || val === undefined) {\n\t\tthrow new TypeError('Object.assign cannot be called with null or undefined');\n\t}\n\n\treturn Object(val);\n}\n\nfunction shouldUseNative() {\n\ttry {\n\t\tif (!Object.assign) {\n\t\t\treturn false;\n\t\t}\n\n\t\t// Detect buggy property enumeration order in older V8 versions.\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=4118\n\t\tvar test1 = new String('abc');  // eslint-disable-line no-new-wrappers\n\t\ttest1[5] = 'de';\n\t\tif (Object.getOwnPropertyNames(test1)[0] === '5') {\n\t\t\treturn false;\n\t\t}\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=3056\n\t\tvar test2 = {};\n\t\tfor (var i = 0; i < 10; i++) {\n\t\t\ttest2['_' + String.fromCharCode(i)] = i;\n\t\t}\n\t\tvar order2 = Object.getOwnPropertyNames(test2).map(function (n) {\n\t\t\treturn test2[n];\n\t\t});\n\t\tif (order2.join('') !== '0123456789') {\n\t\t\treturn false;\n\t\t}\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=3056\n\t\tvar test3 = {};\n\t\t'abcdefghijklmnopqrst'.split('').forEach(function (letter) {\n\t\t\ttest3[letter] = letter;\n\t\t});\n\t\tif (Object.keys(Object.assign({}, test3)).join('') !==\n\t\t\t\t'abcdefghijklmnopqrst') {\n\t\t\treturn false;\n\t\t}\n\n\t\treturn true;\n\t} catch (err) {\n\t\t// We don't expect any of the above to throw, but better to be safe.\n\t\treturn false;\n\t}\n}\n\nmodule.exports = shouldUseNative() ? Object.assign : function (target, source) {\n\tvar from;\n\tvar to = toObject(target);\n\tvar symbols;\n\n\tfor (var s = 1; s < arguments.length; s++) {\n\t\tfrom = Object(arguments[s]);\n\n\t\tfor (var key in from) {\n\t\t\tif (hasOwnProperty.call(from, key)) {\n\t\t\t\tto[key] = from[key];\n\t\t\t}\n\t\t}\n\n\t\tif (getOwnPropertySymbols) {\n\t\t\tsymbols = getOwnPropertySymbols(from);\n\t\t\tfor (var i = 0; i < symbols.length; i++) {\n\t\t\t\tif (propIsEnumerable.call(from, symbols[i])) {\n\t\t\t\t\tto[symbols[i]] = from[symbols[i]];\n\t\t\t\t}\n\t\t\t}\n\t\t}\n\t}\n\n\treturn to;\n};\n",
@@ -5984,14 +5991,15 @@
         "import {isNullOrUndef} from '../helpers/helpers.core.js';\nimport {almostEquals, almostWhole, niceNum, _decimalPlaces, _setMinAndMaxByKey, sign, toRadians} from '../helpers/helpers.math.js';\nimport Scale from '../core/core.scale.js';\nimport {formatNumber} from '../helpers/helpers.intl.js';\n\n/**\n * Generate a set of linear ticks for an axis\n * 1. If generationOptions.min, generationOptions.max, and generationOptions.step are defined:\n *    if (max - min) / step is an integer, ticks are generated as [min, min + step, ..., max]\n *    Note that the generationOptions.maxCount setting is respected in this scenario\n *\n * 2. If generationOptions.min, generationOptions.max, and generationOptions.count is defined\n *    spacing = (max - min) / count\n *    Ticks are generated as [min, min + spacing, ..., max]\n *\n * 3. If generationOptions.count is defined\n *    spacing = (niceMax - niceMin) / count\n *\n * 4. Compute optimal spacing of ticks using niceNum algorithm\n *\n * @param generationOptions the options used to generate the ticks\n * @param dataRange the range of the data\n * @returns {object[]} array of tick objects\n */\nfunction generateTicks(generationOptions, dataRange) {\n  const ticks = [];\n  // To get a \"nice\" value for the tick spacing, we will use the appropriately named\n  // \"nice number\" algorithm. See https://stackoverflow.com/questions/8506881/nice-label-algorithm-for-charts-with-minimum-ticks\n  // for details.\n\n  const MIN_SPACING = 1e-14;\n  const {bounds, step, min, max, precision, count, maxTicks, maxDigits, includeBounds} = generationOptions;\n  const unit = step || 1;\n  const maxSpaces = maxTicks - 1;\n  const {min: rmin, max: rmax} = dataRange;\n  const minDefined = !isNullOrUndef(min);\n  const maxDefined = !isNullOrUndef(max);\n  const countDefined = !isNullOrUndef(count);\n  const minSpacing = (rmax - rmin) / (maxDigits + 1);\n  let spacing = niceNum((rmax - rmin) / maxSpaces / unit) * unit;\n  let factor, niceMin, niceMax, numSpaces;\n\n  // Beyond MIN_SPACING floating point numbers being to lose precision\n  // such that we can't do the math necessary to generate ticks\n  if (spacing < MIN_SPACING && !minDefined && !maxDefined) {\n    return [{value: rmin}, {value: rmax}];\n  }\n\n  numSpaces = Math.ceil(rmax / spacing) - Math.floor(rmin / spacing);\n  if (numSpaces > maxSpaces) {\n    // If the calculated num of spaces exceeds maxNumSpaces, recalculate it\n    spacing = niceNum(numSpaces * spacing / maxSpaces / unit) * unit;\n  }\n\n  if (!isNullOrUndef(precision)) {\n    // If the user specified a precision, round to that number of decimal places\n    factor = Math.pow(10, precision);\n    spacing = Math.ceil(spacing * factor) / factor;\n  }\n\n  if (bounds === 'ticks') {\n    niceMin = Math.floor(rmin / spacing) * spacing;\n    niceMax = Math.ceil(rmax / spacing) * spacing;\n  } else {\n    niceMin = rmin;\n    niceMax = rmax;\n  }\n\n  if (minDefined && maxDefined && step && almostWhole((max - min) / step, spacing / 1000)) {\n    // Case 1: If min, max and stepSize are set and they make an evenly spaced scale use it.\n    // spacing = step;\n    // numSpaces = (max - min) / spacing;\n    // Note that we round here to handle the case where almostWhole translated an FP error\n    numSpaces = Math.round(Math.min((max - min) / spacing, maxTicks));\n    spacing = (max - min) / numSpaces;\n    niceMin = min;\n    niceMax = max;\n  } else if (countDefined) {\n    // Cases 2 & 3, we have a count specified. Handle optional user defined edges to the range.\n    // Sometimes these are no-ops, but it makes the code a lot clearer\n    // and when a user defined range is specified, we want the correct ticks\n    niceMin = minDefined ? min : niceMin;\n    niceMax = maxDefined ? max : niceMax;\n    numSpaces = count - 1;\n    spacing = (niceMax - niceMin) / numSpaces;\n  } else {\n    // Case 4\n    numSpaces = (niceMax - niceMin) / spacing;\n\n    // If very close to our rounded value, use it.\n    if (almostEquals(numSpaces, Math.round(numSpaces), spacing / 1000)) {\n      numSpaces = Math.round(numSpaces);\n    } else {\n      numSpaces = Math.ceil(numSpaces);\n    }\n  }\n\n  // The spacing will have changed in cases 1, 2, and 3 so the factor cannot be computed\n  // until this point\n  const decimalPlaces = Math.max(\n    _decimalPlaces(spacing),\n    _decimalPlaces(niceMin)\n  );\n  factor = Math.pow(10, isNullOrUndef(precision) ? decimalPlaces : precision);\n  niceMin = Math.round(niceMin * factor) / factor;\n  niceMax = Math.round(niceMax * factor) / factor;\n\n  let j = 0;\n  if (minDefined) {\n    if (includeBounds && niceMin !== min) {\n      ticks.push({value: min});\n\n      if (niceMin < min) {\n        j++; // Skip niceMin\n      }\n      // If the next nice tick is close to min, skip it\n      if (almostEquals(Math.round((niceMin + j * spacing) * factor) / factor, min, relativeLabelSize(min, minSpacing, generationOptions))) {\n        j++;\n      }\n    } else if (niceMin < min) {\n      j++;\n    }\n  }\n\n  for (; j < numSpaces; ++j) {\n    const tickValue = Math.round((niceMin + j * spacing) * factor) / factor;\n    if (maxDefined && tickValue > max) {\n      break;\n    }\n    ticks.push({value: tickValue});\n  }\n\n  if (maxDefined && includeBounds && niceMax !== max) {\n    // If the previous tick is too close to max, replace it with max, else add max\n    if (ticks.length && almostEquals(ticks[ticks.length - 1].value, max, relativeLabelSize(max, minSpacing, generationOptions))) {\n      ticks[ticks.length - 1].value = max;\n    } else {\n      ticks.push({value: max});\n    }\n  } else if (!maxDefined || niceMax === max) {\n    ticks.push({value: niceMax});\n  }\n\n  return ticks;\n}\n\nfunction relativeLabelSize(value, minSpacing, {horizontal, minRotation}) {\n  const rad = toRadians(minRotation);\n  const ratio = (horizontal ? Math.sin(rad) : Math.cos(rad)) || 0.001;\n  const length = 0.75 * minSpacing * ('' + value).length;\n  return Math.min(minSpacing / ratio, length);\n}\n\nexport default class LinearScaleBase extends Scale {\n\n  constructor(cfg) {\n    super(cfg);\n\n    /** @type {number} */\n    this.start = undefined;\n    /** @type {number} */\n    this.end = undefined;\n    /** @type {number} */\n    this._startValue = undefined;\n    /** @type {number} */\n    this._endValue = undefined;\n    this._valueRange = 0;\n  }\n\n  parse(raw, index) { // eslint-disable-line no-unused-vars\n    if (isNullOrUndef(raw)) {\n      return null;\n    }\n    if ((typeof raw === 'number' || raw instanceof Number) && !isFinite(+raw)) {\n      return null;\n    }\n\n    return +raw;\n  }\n\n  handleTickRangeOptions() {\n    const {beginAtZero} = this.options;\n    const {minDefined, maxDefined} = this.getUserBounds();\n    let {min, max} = this;\n\n    const setMin = v => (min = minDefined ? min : v);\n    const setMax = v => (max = maxDefined ? max : v);\n\n    if (beginAtZero) {\n      const minSign = sign(min);\n      const maxSign = sign(max);\n\n      if (minSign < 0 && maxSign < 0) {\n        setMax(0);\n      } else if (minSign > 0 && maxSign > 0) {\n        setMin(0);\n      }\n    }\n\n    if (min === max) {\n      let offset = max === 0 ? 1 : Math.abs(max * 0.05);\n\n      setMax(max + offset);\n\n      if (!beginAtZero) {\n        setMin(min - offset);\n      }\n    }\n    this.min = min;\n    this.max = max;\n  }\n\n  getTickLimit() {\n    const tickOpts = this.options.ticks;\n    // eslint-disable-next-line prefer-const\n    let {maxTicksLimit, stepSize} = tickOpts;\n    let maxTicks;\n\n    if (stepSize) {\n      maxTicks = Math.ceil(this.max / stepSize) - Math.floor(this.min / stepSize) + 1;\n      if (maxTicks > 1000) {\n        console.warn(`scales.${this.id}.ticks.stepSize: ${stepSize} would result generating up to ${maxTicks} ticks. Limiting to 1000.`);\n        maxTicks = 1000;\n      }\n    } else {\n      maxTicks = this.computeTickLimit();\n      maxTicksLimit = maxTicksLimit || 11;\n    }\n\n    if (maxTicksLimit) {\n      maxTicks = Math.min(maxTicksLimit, maxTicks);\n    }\n\n    return maxTicks;\n  }\n\n  /**\n\t * @protected\n\t */\n  computeTickLimit() {\n    return Number.POSITIVE_INFINITY;\n  }\n\n  buildTicks() {\n    const opts = this.options;\n    const tickOpts = opts.ticks;\n\n    // Figure out what the max number of ticks we can support it is based on the size of\n    // the axis area. For now, we say that the minimum tick spacing in pixels must be 40\n    // We also limit the maximum number of ticks to 11 which gives a nice 10 squares on\n    // the graph. Make sure we always have at least 2 ticks\n    let maxTicks = this.getTickLimit();\n    maxTicks = Math.max(2, maxTicks);\n\n    const numericGeneratorOptions = {\n      maxTicks,\n      bounds: opts.bounds,\n      min: opts.min,\n      max: opts.max,\n      precision: tickOpts.precision,\n      step: tickOpts.stepSize,\n      count: tickOpts.count,\n      maxDigits: this._maxDigits(),\n      horizontal: this.isHorizontal(),\n      minRotation: tickOpts.minRotation || 0,\n      includeBounds: tickOpts.includeBounds !== false\n    };\n    const dataRange = this._range || this;\n    const ticks = generateTicks(numericGeneratorOptions, dataRange);\n\n    // At this point, we need to update our max and min given the tick values,\n    // since we probably have expanded the range of the scale\n    if (opts.bounds === 'ticks') {\n      _setMinAndMaxByKey(ticks, this, 'value');\n    }\n\n    if (opts.reverse) {\n      ticks.reverse();\n\n      this.start = this.max;\n      this.end = this.min;\n    } else {\n      this.start = this.min;\n      this.end = this.max;\n    }\n\n    return ticks;\n  }\n\n  /**\n\t * @protected\n\t */\n  configure() {\n    const ticks = this.ticks;\n    let start = this.min;\n    let end = this.max;\n\n    super.configure();\n\n    if (this.options.offset && ticks.length) {\n      const offset = (end - start) / Math.max(ticks.length - 1, 1) / 2;\n      start -= offset;\n      end += offset;\n    }\n    this._startValue = start;\n    this._endValue = end;\n    this._valueRange = end - start;\n  }\n\n  getLabelForValue(value) {\n    return formatNumber(value, this.chart.options.locale, this.options.ticks.format);\n  }\n}\n",
         "import {isFinite} from '../helpers/helpers.core.js';\nimport LinearScaleBase from './scale.linearbase.js';\nimport Ticks from '../core/core.ticks.js';\nimport {toRadians} from '../helpers/index.js';\n\nexport default class LinearScale extends LinearScaleBase {\n\n  static id = 'linear';\n\n  /**\n   * @type {any}\n   */\n  static defaults = {\n    ticks: {\n      callback: Ticks.formatters.numeric\n    }\n  };\n\n\n  determineDataLimits() {\n    const {min, max} = this.getMinMax(true);\n\n    this.min = isFinite(min) ? min : 0;\n    this.max = isFinite(max) ? max : 1;\n\n    // Common base implementation to handle min, max, beginAtZero\n    this.handleTickRangeOptions();\n  }\n\n  /**\n\t * Returns the maximum number of ticks based on the scale dimension\n\t * @protected\n \t */\n  computeTickLimit() {\n    const horizontal = this.isHorizontal();\n    const length = horizontal ? this.width : this.height;\n    const minRotation = toRadians(this.options.ticks.minRotation);\n    const ratio = (horizontal ? Math.sin(minRotation) : Math.cos(minRotation)) || 0.001;\n    const tickFont = this._resolveTickFontOptions(0);\n    return Math.ceil(length / Math.min(40, tickFont.lineHeight / ratio));\n  }\n\n  // Utils\n  getPixelForValue(value) {\n    return value === null ? NaN : this.getPixelForDecimal((value - this._startValue) / this._valueRange);\n  }\n\n  getValueForPixel(pixel) {\n    return this._startValue + this.getDecimalForPixel(pixel) * this._valueRange;\n  }\n}\n",
         "import {finiteOrDefault, isFinite} from '../helpers/helpers.core.js';\nimport {formatNumber} from '../helpers/helpers.intl.js';\nimport {_setMinAndMaxByKey, log10} from '../helpers/helpers.math.js';\nimport Scale from '../core/core.scale.js';\nimport LinearScaleBase from './scale.linearbase.js';\nimport Ticks from '../core/core.ticks.js';\n\nconst log10Floor = v => Math.floor(log10(v));\nconst changeExponent = (v, m) => Math.pow(10, log10Floor(v) + m);\n\nfunction isMajor(tickVal) {\n  const remain = tickVal / (Math.pow(10, log10Floor(tickVal)));\n  return remain === 1;\n}\n\nfunction steps(min, max, rangeExp) {\n  const rangeStep = Math.pow(10, rangeExp);\n  const start = Math.floor(min / rangeStep);\n  const end = Math.ceil(max / rangeStep);\n  return end - start;\n}\n\nfunction startExp(min, max) {\n  const range = max - min;\n  let rangeExp = log10Floor(range);\n  while (steps(min, max, rangeExp) > 10) {\n    rangeExp++;\n  }\n  while (steps(min, max, rangeExp) < 10) {\n    rangeExp--;\n  }\n  return Math.min(rangeExp, log10Floor(min));\n}\n\n\n/**\n * Generate a set of logarithmic ticks\n * @param generationOptions the options used to generate the ticks\n * @param dataRange the range of the data\n * @returns {object[]} array of tick objects\n */\nfunction generateTicks(generationOptions, {min, max}) {\n  min = finiteOrDefault(generationOptions.min, min);\n  const ticks = [];\n  const minExp = log10Floor(min);\n  let exp = startExp(min, max);\n  let precision = exp < 0 ? Math.pow(10, Math.abs(exp)) : 1;\n  const stepSize = Math.pow(10, exp);\n  const base = minExp > exp ? Math.pow(10, minExp) : 0;\n  const start = Math.round((min - base) * precision) / precision;\n  const offset = Math.floor((min - base) / stepSize / 10) * stepSize * 10;\n  let significand = Math.floor((start - offset) / Math.pow(10, exp));\n  let value = finiteOrDefault(generationOptions.min, Math.round((base + offset + significand * Math.pow(10, exp)) * precision) / precision);\n  while (value < max) {\n    ticks.push({value, major: isMajor(value), significand});\n    if (significand >= 10) {\n      significand = significand < 15 ? 15 : 20;\n    } else {\n      significand++;\n    }\n    if (significand >= 20) {\n      exp++;\n      significand = 2;\n      precision = exp >= 0 ? 1 : precision;\n    }\n    value = Math.round((base + offset + significand * Math.pow(10, exp)) * precision) / precision;\n  }\n  const lastTick = finiteOrDefault(generationOptions.max, value);\n  ticks.push({value: lastTick, major: isMajor(lastTick), significand});\n\n  return ticks;\n}\n\nexport default class LogarithmicScale extends Scale {\n\n  static id = 'logarithmic';\n\n  /**\n   * @type {any}\n   */\n  static defaults = {\n    ticks: {\n      callback: Ticks.formatters.logarithmic,\n      major: {\n        enabled: true\n      }\n    }\n  };\n\n\n  constructor(cfg) {\n    super(cfg);\n\n    /** @type {number} */\n    this.start = undefined;\n    /** @type {number} */\n    this.end = undefined;\n    /** @type {number} */\n    this._startValue = undefined;\n    this._valueRange = 0;\n  }\n\n  parse(raw, index) {\n    const value = LinearScaleBase.prototype.parse.apply(this, [raw, index]);\n    if (value === 0) {\n      this._zero = true;\n      return undefined;\n    }\n    return isFinite(value) && value > 0 ? value : null;\n  }\n\n  determineDataLimits() {\n    const {min, max} = this.getMinMax(true);\n\n    this.min = isFinite(min) ? Math.max(0, min) : null;\n    this.max = isFinite(max) ? Math.max(0, max) : null;\n\n    if (this.options.beginAtZero) {\n      this._zero = true;\n    }\n\n    // if data has `0` in it or `beginAtZero` is true, min (non zero) value is at bottom\n    // of scale, and it does not equal suggestedMin, lower the min bound by one exp.\n    if (this._zero && this.min !== this._suggestedMin && !isFinite(this._userMin)) {\n      this.min = min === changeExponent(this.min, 0) ? changeExponent(this.min, -1) : changeExponent(this.min, 0);\n    }\n\n    this.handleTickRangeOptions();\n  }\n\n  handleTickRangeOptions() {\n    const {minDefined, maxDefined} = this.getUserBounds();\n    let min = this.min;\n    let max = this.max;\n\n    const setMin = v => (min = minDefined ? min : v);\n    const setMax = v => (max = maxDefined ? max : v);\n\n    if (min === max) {\n      if (min <= 0) { // includes null\n        setMin(1);\n        setMax(10);\n      } else {\n        setMin(changeExponent(min, -1));\n        setMax(changeExponent(max, +1));\n      }\n    }\n    if (min <= 0) {\n      setMin(changeExponent(max, -1));\n    }\n    if (max <= 0) {\n\n      setMax(changeExponent(min, +1));\n    }\n\n    this.min = min;\n    this.max = max;\n  }\n\n  buildTicks() {\n    const opts = this.options;\n\n    const generationOptions = {\n      min: this._userMin,\n      max: this._userMax\n    };\n    const ticks = generateTicks(generationOptions, this);\n\n    // At this point, we need to update our max and min given the tick values,\n    // since we probably have expanded the range of the scale\n    if (opts.bounds === 'ticks') {\n      _setMinAndMaxByKey(ticks, this, 'value');\n    }\n\n    if (opts.reverse) {\n      ticks.reverse();\n\n      this.start = this.max;\n      this.end = this.min;\n    } else {\n      this.start = this.min;\n      this.end = this.max;\n    }\n\n    return ticks;\n  }\n\n  /**\n\t * @param {number} value\n\t * @return {string}\n\t */\n  getLabelForValue(value) {\n    return value === undefined\n      ? '0'\n      : formatNumber(value, this.chart.options.locale, this.options.ticks.format);\n  }\n\n  /**\n\t * @protected\n\t */\n  configure() {\n    const start = this.min;\n\n    super.configure();\n\n    this._startValue = log10(start);\n    this._valueRange = log10(this.max) - log10(start);\n  }\n\n  getPixelForValue(value) {\n    if (value === undefined || value === 0) {\n      value = this.min;\n    }\n    if (value === null || isNaN(value)) {\n      return NaN;\n    }\n    return this.getPixelForDecimal(value === this.min\n      ? 0\n      : (log10(value) - this._startValue) / this._valueRange);\n  }\n\n  getValueForPixel(pixel) {\n    const decimal = this.getDecimalForPixel(pixel);\n    return Math.pow(10, this._startValue + decimal * this._valueRange);\n  }\n}\n",
         "import defaults from '../core/core.defaults.js';\nimport {_longestText, addRoundedRectPath, renderText, _isPointInArea} from '../helpers/helpers.canvas.js';\nimport {HALF_PI, TAU, toDegrees, toRadians, _normalizeAngle, PI} from '../helpers/helpers.math.js';\nimport LinearScaleBase from './scale.linearbase.js';\nimport Ticks from '../core/core.ticks.js';\nimport {valueOrDefault, isArray, isFinite, callback as callCallback, isNullOrUndef} from '../helpers/helpers.core.js';\nimport {createContext, toFont, toPadding, toTRBLCorners} from '../helpers/helpers.options.js';\n\nfunction getTickBackdropHeight(opts) {\n  const tickOpts = opts.ticks;\n\n  if (tickOpts.display && opts.display) {\n    const padding = toPadding(tickOpts.backdropPadding);\n    return valueOrDefault(tickOpts.font && tickOpts.font.size, defaults.font.size) + padding.height;\n  }\n  return 0;\n}\n\nfunction measureLabelSize(ctx, font, label) {\n  label = isArray(label) ? label : [label];\n  return {\n    w: _longestText(ctx, font.string, label),\n    h: label.length * font.lineHeight\n  };\n}\n\nfunction determineLimits(angle, pos, size, min, max) {\n  if (angle === min || angle === max) {\n    return {\n      start: pos - (size / 2),\n      end: pos + (size / 2)\n    };\n  } else if (angle < min || angle > max) {\n    return {\n      start: pos - size,\n      end: pos\n    };\n  }\n\n  return {\n    start: pos,\n    end: pos + size\n  };\n}\n\n/**\n * Helper function to fit a radial linear scale with point labels\n */\nfunction fitWithPointLabels(scale) {\n\n  // Right, this is really confusing and there is a lot of maths going on here\n  // The gist of the problem is here: https://gist.github.com/nnnick/696cc9c55f4b0beb8fe9\n  //\n  // Reaction: https://dl.dropboxusercontent.com/u/34601363/toomuchscience.gif\n  //\n  // Solution:\n  //\n  // We assume the radius of the polygon is half the size of the canvas at first\n  // at each index we check if the text overlaps.\n  //\n  // Where it does, we store that angle and that index.\n  //\n  // After finding the largest index and angle we calculate how much we need to remove\n  // from the shape radius to move the point inwards by that x.\n  //\n  // We average the left and right distances to get the maximum shape radius that can fit in the box\n  // along with labels.\n  //\n  // Once we have that, we can find the centre point for the chart, by taking the x text protrusion\n  // on each side, removing that from the size, halving it and adding the left x protrusion width.\n  //\n  // This will mean we have a shape fitted to the canvas, as large as it can be with the labels\n  // and position it in the most space efficient manner\n  //\n  // https://dl.dropboxusercontent.com/u/34601363/yeahscience.gif\n\n  // Get maximum radius of the polygon. Either half the height (minus the text width) or half the width.\n  // Use this to calculate the offset + change. - Make sure L/R protrusion is at least 0 to stop issues with centre points\n  const orig = {\n    l: scale.left + scale._padding.left,\n    r: scale.right - scale._padding.right,\n    t: scale.top + scale._padding.top,\n    b: scale.bottom - scale._padding.bottom\n  };\n  const limits = Object.assign({}, orig);\n  const labelSizes = [];\n  const padding = [];\n  const valueCount = scale._pointLabels.length;\n  const pointLabelOpts = scale.options.pointLabels;\n  const additionalAngle = pointLabelOpts.centerPointLabels ? PI / valueCount : 0;\n\n  for (let i = 0; i < valueCount; i++) {\n    const opts = pointLabelOpts.setContext(scale.getPointLabelContext(i));\n    padding[i] = opts.padding;\n    const pointPosition = scale.getPointPosition(i, scale.drawingArea + padding[i], additionalAngle);\n    const plFont = toFont(opts.font);\n    const textSize = measureLabelSize(scale.ctx, plFont, scale._pointLabels[i]);\n    labelSizes[i] = textSize;\n\n    const angleRadians = _normalizeAngle(scale.getIndexAngle(i) + additionalAngle);\n    const angle = Math.round(toDegrees(angleRadians));\n    const hLimits = determineLimits(angle, pointPosition.x, textSize.w, 0, 180);\n    const vLimits = determineLimits(angle, pointPosition.y, textSize.h, 90, 270);\n    updateLimits(limits, orig, angleRadians, hLimits, vLimits);\n  }\n\n  scale.setCenterPoint(\n    orig.l - limits.l,\n    limits.r - orig.r,\n    orig.t - limits.t,\n    limits.b - orig.b\n  );\n\n  // Now that text size is determined, compute the full positions\n  scale._pointLabelItems = buildPointLabelItems(scale, labelSizes, padding);\n}\n\nfunction updateLimits(limits, orig, angle, hLimits, vLimits) {\n  const sin = Math.abs(Math.sin(angle));\n  const cos = Math.abs(Math.cos(angle));\n  let x = 0;\n  let y = 0;\n  if (hLimits.start < orig.l) {\n    x = (orig.l - hLimits.start) / sin;\n    limits.l = Math.min(limits.l, orig.l - x);\n  } else if (hLimits.end > orig.r) {\n    x = (hLimits.end - orig.r) / sin;\n    limits.r = Math.max(limits.r, orig.r + x);\n  }\n  if (vLimits.start < orig.t) {\n    y = (orig.t - vLimits.start) / cos;\n    limits.t = Math.min(limits.t, orig.t - y);\n  } else if (vLimits.end > orig.b) {\n    y = (vLimits.end - orig.b) / cos;\n    limits.b = Math.max(limits.b, orig.b + y);\n  }\n}\n\nfunction createPointLabelItem(scale, index, itemOpts) {\n  const outerDistance = scale.drawingArea;\n  const {extra, additionalAngle, padding, size} = itemOpts;\n  const pointLabelPosition = scale.getPointPosition(index, outerDistance + extra + padding, additionalAngle);\n  const angle = Math.round(toDegrees(_normalizeAngle(pointLabelPosition.angle + HALF_PI)));\n  const y = yForAngle(pointLabelPosition.y, size.h, angle);\n  const textAlign = getTextAlignForAngle(angle);\n  const left = leftForTextAlign(pointLabelPosition.x, size.w, textAlign);\n  return {\n    // if to draw or overlapped\n    visible: true,\n\n    // Text position\n    x: pointLabelPosition.x,\n    y,\n\n    // Text rendering data\n    textAlign,\n\n    // Bounding box\n    left,\n    top: y,\n    right: left + size.w,\n    bottom: y + size.h\n  };\n}\n\nfunction isNotOverlapped(item, area) {\n  if (!area) {\n    return true;\n  }\n  const {left, top, right, bottom} = item;\n  const apexesInArea = _isPointInArea({x: left, y: top}, area) || _isPointInArea({x: left, y: bottom}, area) ||\n    _isPointInArea({x: right, y: top}, area) || _isPointInArea({x: right, y: bottom}, area);\n  return !apexesInArea;\n}\n\nfunction buildPointLabelItems(scale, labelSizes, padding) {\n  const items = [];\n  const valueCount = scale._pointLabels.length;\n  const opts = scale.options;\n  const {centerPointLabels, display} = opts.pointLabels;\n  const itemOpts = {\n    extra: getTickBackdropHeight(opts) / 2,\n    additionalAngle: centerPointLabels ? PI / valueCount : 0\n  };\n  let area;\n\n  for (let i = 0; i < valueCount; i++) {\n    itemOpts.padding = padding[i];\n    itemOpts.size = labelSizes[i];\n\n    const item = createPointLabelItem(scale, i, itemOpts);\n    items.push(item);\n    if (display === 'auto') {\n      item.visible = isNotOverlapped(item, area);\n      if (item.visible) {\n        area = item;\n      }\n    }\n  }\n  return items;\n}\n\nfunction getTextAlignForAngle(angle) {\n  if (angle === 0 || angle === 180) {\n    return 'center';\n  } else if (angle < 180) {\n    return 'left';\n  }\n\n  return 'right';\n}\n\nfunction leftForTextAlign(x, w, align) {\n  if (align === 'right') {\n    x -= w;\n  } else if (align === 'center') {\n    x -= (w / 2);\n  }\n  return x;\n}\n\nfunction yForAngle(y, h, angle) {\n  if (angle === 90 || angle === 270) {\n    y -= (h / 2);\n  } else if (angle > 270 || angle < 90) {\n    y -= h;\n  }\n  return y;\n}\n\nfunction drawPointLabelBox(ctx, opts, item) {\n  const {left, top, right, bottom} = item;\n  const {backdropColor} = opts;\n\n  if (!isNullOrUndef(backdropColor)) {\n    const borderRadius = toTRBLCorners(opts.borderRadius);\n    const padding = toPadding(opts.backdropPadding);\n    ctx.fillStyle = backdropColor;\n\n    const backdropLeft = left - padding.left;\n    const backdropTop = top - padding.top;\n    const backdropWidth = right - left + padding.width;\n    const backdropHeight = bottom - top + padding.height;\n\n    if (Object.values(borderRadius).some(v => v !== 0)) {\n      ctx.beginPath();\n      addRoundedRectPath(ctx, {\n        x: backdropLeft,\n        y: backdropTop,\n        w: backdropWidth,\n        h: backdropHeight,\n        radius: borderRadius,\n      });\n      ctx.fill();\n    } else {\n      ctx.fillRect(backdropLeft, backdropTop, backdropWidth, backdropHeight);\n    }\n  }\n}\n\nfunction drawPointLabels(scale, labelCount) {\n  const {ctx, options: {pointLabels}} = scale;\n\n  for (let i = labelCount - 1; i >= 0; i--) {\n    const item = scale._pointLabelItems[i];\n    if (!item.visible) {\n      // overlapping\n      continue;\n    }\n    const optsAtIndex = pointLabels.setContext(scale.getPointLabelContext(i));\n    drawPointLabelBox(ctx, optsAtIndex, item);\n    const plFont = toFont(optsAtIndex.font);\n    const {x, y, textAlign} = item;\n\n    renderText(\n      ctx,\n      scale._pointLabels[i],\n      x,\n      y + (plFont.lineHeight / 2),\n      plFont,\n      {\n        color: optsAtIndex.color,\n        textAlign: textAlign,\n        textBaseline: 'middle'\n      }\n    );\n  }\n}\n\nfunction pathRadiusLine(scale, radius, circular, labelCount) {\n  const {ctx} = scale;\n  if (circular) {\n    // Draw circular arcs between the points\n    ctx.arc(scale.xCenter, scale.yCenter, radius, 0, TAU);\n  } else {\n    // Draw straight lines connecting each index\n    let pointPosition = scale.getPointPosition(0, radius);\n    ctx.moveTo(pointPosition.x, pointPosition.y);\n\n    for (let i = 1; i < labelCount; i++) {\n      pointPosition = scale.getPointPosition(i, radius);\n      ctx.lineTo(pointPosition.x, pointPosition.y);\n    }\n  }\n}\n\nfunction drawRadiusLine(scale, gridLineOpts, radius, labelCount, borderOpts) {\n  const ctx = scale.ctx;\n  const circular = gridLineOpts.circular;\n\n  const {color, lineWidth} = gridLineOpts;\n\n  if ((!circular && !labelCount) || !color || !lineWidth || radius < 0) {\n    return;\n  }\n\n  ctx.save();\n  ctx.strokeStyle = color;\n  ctx.lineWidth = lineWidth;\n  ctx.setLineDash(borderOpts.dash);\n  ctx.lineDashOffset = borderOpts.dashOffset;\n\n  ctx.beginPath();\n  pathRadiusLine(scale, radius, circular, labelCount);\n  ctx.closePath();\n  ctx.stroke();\n  ctx.restore();\n}\n\nfunction createPointLabelContext(parent, index, label) {\n  return createContext(parent, {\n    label,\n    index,\n    type: 'pointLabel'\n  });\n}\n\nexport default class RadialLinearScale extends LinearScaleBase {\n\n  static id = 'radialLinear';\n\n  /**\n   * @type {any}\n   */\n  static defaults = {\n    display: true,\n\n    // Boolean - Whether to animate scaling the chart from the centre\n    animate: true,\n    position: 'chartArea',\n\n    angleLines: {\n      display: true,\n      lineWidth: 1,\n      borderDash: [],\n      borderDashOffset: 0.0\n    },\n\n    grid: {\n      circular: false\n    },\n\n    startAngle: 0,\n\n    // label settings\n    ticks: {\n      // Boolean - Show a backdrop to the scale label\n      showLabelBackdrop: true,\n\n      callback: Ticks.formatters.numeric\n    },\n\n    pointLabels: {\n      backdropColor: undefined,\n\n      // Number - The backdrop padding above & below the label in pixels\n      backdropPadding: 2,\n\n      // Boolean - if true, show point labels\n      display: true,\n\n      // Number - Point label font size in pixels\n      font: {\n        size: 10\n      },\n\n      // Function - Used to convert point labels\n      callback(label) {\n        return label;\n      },\n\n      // Number - Additionl padding between scale and pointLabel\n      padding: 5,\n\n      // Boolean - if true, center point labels to slices in polar chart\n      centerPointLabels: false\n    }\n  };\n\n  static defaultRoutes = {\n    'angleLines.color': 'borderColor',\n    'pointLabels.color': 'color',\n    'ticks.color': 'color'\n  };\n\n  static descriptors = {\n    angleLines: {\n      _fallback: 'grid'\n    }\n  };\n\n  constructor(cfg) {\n    super(cfg);\n\n    /** @type {number} */\n    this.xCenter = undefined;\n    /** @type {number} */\n    this.yCenter = undefined;\n    /** @type {number} */\n    this.drawingArea = undefined;\n    /** @type {string[]} */\n    this._pointLabels = [];\n    this._pointLabelItems = [];\n  }\n\n  setDimensions() {\n    // Set the unconstrained dimension before label rotation\n    const padding = this._padding = toPadding(getTickBackdropHeight(this.options) / 2);\n    const w = this.width = this.maxWidth - padding.width;\n    const h = this.height = this.maxHeight - padding.height;\n    this.xCenter = Math.floor(this.left + w / 2 + padding.left);\n    this.yCenter = Math.floor(this.top + h / 2 + padding.top);\n    this.drawingArea = Math.floor(Math.min(w, h) / 2);\n  }\n\n  determineDataLimits() {\n    const {min, max} = this.getMinMax(false);\n\n    this.min = isFinite(min) && !isNaN(min) ? min : 0;\n    this.max = isFinite(max) && !isNaN(max) ? max : 0;\n\n    // Common base implementation to handle min, max, beginAtZero\n    this.handleTickRangeOptions();\n  }\n\n  /**\n\t * Returns the maximum number of ticks based on the scale dimension\n\t * @protected\n\t */\n  computeTickLimit() {\n    return Math.ceil(this.drawingArea / getTickBackdropHeight(this.options));\n  }\n\n  generateTickLabels(ticks) {\n    LinearScaleBase.prototype.generateTickLabels.call(this, ticks);\n\n    // Point labels\n    this._pointLabels = this.getLabels()\n      .map((value, index) => {\n        const label = callCallback(this.options.pointLabels.callback, [value, index], this);\n        return label || label === 0 ? label : '';\n      })\n      .filter((v, i) => this.chart.getDataVisibility(i));\n  }\n\n  fit() {\n    const opts = this.options;\n\n    if (opts.display && opts.pointLabels.display) {\n      fitWithPointLabels(this);\n    } else {\n      this.setCenterPoint(0, 0, 0, 0);\n    }\n  }\n\n  setCenterPoint(leftMovement, rightMovement, topMovement, bottomMovement) {\n    this.xCenter += Math.floor((leftMovement - rightMovement) / 2);\n    this.yCenter += Math.floor((topMovement - bottomMovement) / 2);\n    this.drawingArea -= Math.min(this.drawingArea / 2, Math.max(leftMovement, rightMovement, topMovement, bottomMovement));\n  }\n\n  getIndexAngle(index) {\n    const angleMultiplier = TAU / (this._pointLabels.length || 1);\n    const startAngle = this.options.startAngle || 0;\n\n    return _normalizeAngle(index * angleMultiplier + toRadians(startAngle));\n  }\n\n  getDistanceFromCenterForValue(value) {\n    if (isNullOrUndef(value)) {\n      return NaN;\n    }\n\n    // Take into account half font size + the yPadding of the top value\n    const scalingFactor = this.drawingArea / (this.max - this.min);\n    if (this.options.reverse) {\n      return (this.max - value) * scalingFactor;\n    }\n    return (value - this.min) * scalingFactor;\n  }\n\n  getValueForDistanceFromCenter(distance) {\n    if (isNullOrUndef(distance)) {\n      return NaN;\n    }\n\n    const scaledDistance = distance / (this.drawingArea / (this.max - this.min));\n    return this.options.reverse ? this.max - scaledDistance : this.min + scaledDistance;\n  }\n\n  getPointLabelContext(index) {\n    const pointLabels = this._pointLabels || [];\n\n    if (index >= 0 && index < pointLabels.length) {\n      const pointLabel = pointLabels[index];\n      return createPointLabelContext(this.getContext(), index, pointLabel);\n    }\n  }\n\n  getPointPosition(index, distanceFromCenter, additionalAngle = 0) {\n    const angle = this.getIndexAngle(index) - HALF_PI + additionalAngle;\n    return {\n      x: Math.cos(angle) * distanceFromCenter + this.xCenter,\n      y: Math.sin(angle) * distanceFromCenter + this.yCenter,\n      angle\n    };\n  }\n\n  getPointPositionForValue(index, value) {\n    return this.getPointPosition(index, this.getDistanceFromCenterForValue(value));\n  }\n\n  getBasePosition(index) {\n    return this.getPointPositionForValue(index || 0, this.getBaseValue());\n  }\n\n  getPointLabelPosition(index) {\n    const {left, top, right, bottom} = this._pointLabelItems[index];\n    return {\n      left,\n      top,\n      right,\n      bottom,\n    };\n  }\n\n  /**\n\t * @protected\n\t */\n  drawBackground() {\n    const {backgroundColor, grid: {circular}} = this.options;\n    if (backgroundColor) {\n      const ctx = this.ctx;\n      ctx.save();\n      ctx.beginPath();\n      pathRadiusLine(this, this.getDistanceFromCenterForValue(this._endValue), circular, this._pointLabels.length);\n      ctx.closePath();\n      ctx.fillStyle = backgroundColor;\n      ctx.fill();\n      ctx.restore();\n    }\n  }\n\n  /**\n\t * @protected\n\t */\n  drawGrid() {\n    const ctx = this.ctx;\n    const opts = this.options;\n    const {angleLines, grid, border} = opts;\n    const labelCount = this._pointLabels.length;\n\n    let i, offset, position;\n\n    if (opts.pointLabels.display) {\n      drawPointLabels(this, labelCount);\n    }\n\n    if (grid.display) {\n      this.ticks.forEach((tick, index) => {\n        if (index !== 0 || (index === 0 && this.min < 0)) {\n          offset = this.getDistanceFromCenterForValue(tick.value);\n          const context = this.getContext(index);\n          const optsAtIndex = grid.setContext(context);\n          const optsAtIndexBorder = border.setContext(context);\n\n          drawRadiusLine(this, optsAtIndex, offset, labelCount, optsAtIndexBorder);\n        }\n      });\n    }\n\n    if (angleLines.display) {\n      ctx.save();\n\n      for (i = labelCount - 1; i >= 0; i--) {\n        const optsAtIndex = angleLines.setContext(this.getPointLabelContext(i));\n        const {color, lineWidth} = optsAtIndex;\n\n        if (!lineWidth || !color) {\n          continue;\n        }\n\n        ctx.lineWidth = lineWidth;\n        ctx.strokeStyle = color;\n\n        ctx.setLineDash(optsAtIndex.borderDash);\n        ctx.lineDashOffset = optsAtIndex.borderDashOffset;\n\n        offset = this.getDistanceFromCenterForValue(opts.ticks.reverse ? this.min : this.max);\n        position = this.getPointPosition(i, offset);\n        ctx.beginPath();\n        ctx.moveTo(this.xCenter, this.yCenter);\n        ctx.lineTo(position.x, position.y);\n        ctx.stroke();\n      }\n\n      ctx.restore();\n    }\n  }\n\n  /**\n\t * @protected\n\t */\n  drawBorder() {}\n\n  /**\n\t * @protected\n\t */\n  drawLabels() {\n    const ctx = this.ctx;\n    const opts = this.options;\n    const tickOpts = opts.ticks;\n\n    if (!tickOpts.display) {\n      return;\n    }\n\n    const startAngle = this.getIndexAngle(0);\n    let offset, width;\n\n    ctx.save();\n    ctx.translate(this.xCenter, this.yCenter);\n    ctx.rotate(startAngle);\n    ctx.textAlign = 'center';\n    ctx.textBaseline = 'middle';\n\n    this.ticks.forEach((tick, index) => {\n      if ((index === 0 && this.min >= 0) && !opts.reverse) {\n        return;\n      }\n\n      const optsAtIndex = tickOpts.setContext(this.getContext(index));\n      const tickFont = toFont(optsAtIndex.font);\n      offset = this.getDistanceFromCenterForValue(this.ticks[index].value);\n\n      if (optsAtIndex.showLabelBackdrop) {\n        ctx.font = tickFont.string;\n        width = ctx.measureText(tick.label).width;\n        ctx.fillStyle = optsAtIndex.backdropColor;\n\n        const padding = toPadding(optsAtIndex.backdropPadding);\n        ctx.fillRect(\n          -width / 2 - padding.left,\n          -offset - tickFont.size / 2 - padding.top,\n          width + padding.width,\n          tickFont.size + padding.height\n        );\n      }\n\n      renderText(ctx, tick.label, 0, -offset, tickFont, {\n        color: optsAtIndex.color,\n        strokeColor: optsAtIndex.textStrokeColor,\n        strokeWidth: optsAtIndex.textStrokeWidth,\n      });\n    });\n\n    ctx.restore();\n  }\n\n  /**\n\t * @protected\n\t */\n  drawTitle() {}\n}\n",
         "import adapters from '../core/core.adapters.js';\nimport {callback as call, isFinite, isNullOrUndef, mergeIf, valueOrDefault} from '../helpers/helpers.core.js';\nimport {toRadians, isNumber, _limitValue} from '../helpers/helpers.math.js';\nimport Scale from '../core/core.scale.js';\nimport {_arrayUnique, _filterBetween, _lookup} from '../helpers/helpers.collection.js';\n\n/**\n * @typedef { import('../core/core.adapters.js').TimeUnit } Unit\n * @typedef {{common: boolean, size: number, steps?: number}} Interval\n * @typedef { import('../core/core.adapters.js').DateAdapter } DateAdapter\n */\n\n/**\n * @type {Object<Unit, Interval>}\n */\nconst INTERVALS = {\n  millisecond: {common: true, size: 1, steps: 1000},\n  second: {common: true, size: 1000, steps: 60},\n  minute: {common: true, size: 60000, steps: 60},\n  hour: {common: true, size: 3600000, steps: 24},\n  day: {common: true, size: 86400000, steps: 30},\n  week: {common: false, size: 604800000, steps: 4},\n  month: {common: true, size: 2.628e9, steps: 12},\n  quarter: {common: false, size: 7.884e9, steps: 4},\n  year: {common: true, size: 3.154e10}\n};\n\n/**\n * @type {Unit[]}\n */\nconst UNITS = /** @type Unit[] */ /* #__PURE__ */ (Object.keys(INTERVALS));\n\n/**\n * @param {number} a\n * @param {number} b\n */\nfunction sorter(a, b) {\n  return a - b;\n}\n\n/**\n * @param {TimeScale} scale\n * @param {*} input\n * @return {number}\n */\nfunction parse(scale, input) {\n  if (isNullOrUndef(input)) {\n    return null;\n  }\n\n  const adapter = scale._adapter;\n  const {parser, round, isoWeekday} = scale._parseOpts;\n  let value = input;\n\n  if (typeof parser === 'function') {\n    value = parser(value);\n  }\n\n  // Only parse if it's not a timestamp already\n  if (!isFinite(value)) {\n    value = typeof parser === 'string'\n      ? adapter.parse(value, /** @type {Unit} */ (parser))\n      : adapter.parse(value);\n  }\n\n  if (value === null) {\n    return null;\n  }\n\n  if (round) {\n    value = round === 'week' && (isNumber(isoWeekday) || isoWeekday === true)\n      ? adapter.startOf(value, 'isoWeek', isoWeekday)\n      : adapter.startOf(value, round);\n  }\n\n  return +value;\n}\n\n/**\n * Figures out what unit results in an appropriate number of auto-generated ticks\n * @param {Unit} minUnit\n * @param {number} min\n * @param {number} max\n * @param {number} capacity\n * @return {object}\n */\nfunction determineUnitForAutoTicks(minUnit, min, max, capacity) {\n  const ilen = UNITS.length;\n\n  for (let i = UNITS.indexOf(minUnit); i < ilen - 1; ++i) {\n    const interval = INTERVALS[UNITS[i]];\n    const factor = interval.steps ? interval.steps : Number.MAX_SAFE_INTEGER;\n\n    if (interval.common && Math.ceil((max - min) / (factor * interval.size)) <= capacity) {\n      return UNITS[i];\n    }\n  }\n\n  return UNITS[ilen - 1];\n}\n\n/**\n * Figures out what unit to format a set of ticks with\n * @param {TimeScale} scale\n * @param {number} numTicks\n * @param {Unit} minUnit\n * @param {number} min\n * @param {number} max\n * @return {Unit}\n */\nfunction determineUnitForFormatting(scale, numTicks, minUnit, min, max) {\n  for (let i = UNITS.length - 1; i >= UNITS.indexOf(minUnit); i--) {\n    const unit = UNITS[i];\n    if (INTERVALS[unit].common && scale._adapter.diff(max, min, unit) >= numTicks - 1) {\n      return unit;\n    }\n  }\n\n  return UNITS[minUnit ? UNITS.indexOf(minUnit) : 0];\n}\n\n/**\n * @param {Unit} unit\n * @return {object}\n */\nfunction determineMajorUnit(unit) {\n  for (let i = UNITS.indexOf(unit) + 1, ilen = UNITS.length; i < ilen; ++i) {\n    if (INTERVALS[UNITS[i]].common) {\n      return UNITS[i];\n    }\n  }\n}\n\n/**\n * @param {object} ticks\n * @param {number} time\n * @param {number[]} [timestamps] - if defined, snap to these timestamps\n */\nfunction addTick(ticks, time, timestamps) {\n  if (!timestamps) {\n    ticks[time] = true;\n  } else if (timestamps.length) {\n    const {lo, hi} = _lookup(timestamps, time);\n    const timestamp = timestamps[lo] >= time ? timestamps[lo] : timestamps[hi];\n    ticks[timestamp] = true;\n  }\n}\n\n/**\n * @param {TimeScale} scale\n * @param {object[]} ticks\n * @param {object} map\n * @param {Unit} majorUnit\n * @return {object[]}\n */\nfunction setMajorTicks(scale, ticks, map, majorUnit) {\n  const adapter = scale._adapter;\n  const first = +adapter.startOf(ticks[0].value, majorUnit);\n  const last = ticks[ticks.length - 1].value;\n  let major, index;\n\n  for (major = first; major <= last; major = +adapter.add(major, 1, majorUnit)) {\n    index = map[major];\n    if (index >= 0) {\n      ticks[index].major = true;\n    }\n  }\n  return ticks;\n}\n\n/**\n * @param {TimeScale} scale\n * @param {number[]} values\n * @param {Unit|undefined} [majorUnit]\n * @return {object[]}\n */\nfunction ticksFromTimestamps(scale, values, majorUnit) {\n  const ticks = [];\n  /** @type {Object<number,object>} */\n  const map = {};\n  const ilen = values.length;\n  let i, value;\n\n  for (i = 0; i < ilen; ++i) {\n    value = values[i];\n    map[value] = i;\n\n    ticks.push({\n      value,\n      major: false\n    });\n  }\n\n  // We set the major ticks separately from the above loop because calling startOf for every tick\n  // is expensive when there is a large number of ticks\n  return (ilen === 0 || !majorUnit) ? ticks : setMajorTicks(scale, ticks, map, majorUnit);\n}\n\nexport default class TimeScale extends Scale {\n\n  static id = 'time';\n\n  /**\n   * @type {any}\n   */\n  static defaults = {\n    /**\n     * Scale boundary strategy (bypassed by min/max time options)\n     * - `data`: make sure data are fully visible, ticks outside are removed\n     * - `ticks`: make sure ticks are fully visible, data outside are truncated\n     * @see https://github.com/chartjs/Chart.js/pull/4556\n     * @since 2.7.0\n     */\n    bounds: 'data',\n\n    adapters: {},\n    time: {\n      parser: false, // false == a pattern string from or a custom callback that converts its argument to a timestamp\n      unit: false, // false == automatic or override with week, month, year, etc.\n      round: false, // none, or override with week, month, year, etc.\n      isoWeekday: false, // override week start day\n      minUnit: 'millisecond',\n      displayFormats: {}\n    },\n    ticks: {\n      /**\n       * Ticks generation input values:\n       * - 'auto': generates \"optimal\" ticks based on scale size and time options.\n       * - 'data': generates ticks from data (including labels from data {t|x|y} objects).\n       * - 'labels': generates ticks from user given `data.labels` values ONLY.\n       * @see https://github.com/chartjs/Chart.js/pull/4507\n       * @since 2.7.0\n       */\n      source: 'auto',\n\n      callback: false,\n\n      major: {\n        enabled: false\n      }\n    }\n  };\n\n  /**\n\t * @param {object} props\n\t */\n  constructor(props) {\n    super(props);\n\n    /** @type {{data: number[], labels: number[], all: number[]}} */\n    this._cache = {\n      data: [],\n      labels: [],\n      all: []\n    };\n\n    /** @type {Unit} */\n    this._unit = 'day';\n    /** @type {Unit=} */\n    this._majorUnit = undefined;\n    this._offsets = {};\n    this._normalized = false;\n    this._parseOpts = undefined;\n  }\n\n  init(scaleOpts, opts = {}) {\n    const time = scaleOpts.time || (scaleOpts.time = {});\n    /** @type {DateAdapter} */\n    const adapter = this._adapter = new adapters._date(scaleOpts.adapters.date);\n\n    adapter.init(opts);\n\n    // Backward compatibility: before introducing adapter, `displayFormats` was\n    // supposed to contain *all* unit/string pairs but this can't be resolved\n    // when loading the scale (adapters are loaded afterward), so let's populate\n    // missing formats on update\n    mergeIf(time.displayFormats, adapter.formats());\n\n    this._parseOpts = {\n      parser: time.parser,\n      round: time.round,\n      isoWeekday: time.isoWeekday\n    };\n\n    super.init(scaleOpts);\n\n    this._normalized = opts.normalized;\n  }\n\n  /**\n\t * @param {*} raw\n\t * @param {number?} [index]\n\t * @return {number}\n\t */\n  parse(raw, index) { // eslint-disable-line no-unused-vars\n    if (raw === undefined) {\n      return null;\n    }\n    return parse(this, raw);\n  }\n\n  beforeLayout() {\n    super.beforeLayout();\n    this._cache = {\n      data: [],\n      labels: [],\n      all: []\n    };\n  }\n\n  determineDataLimits() {\n    const options = this.options;\n    const adapter = this._adapter;\n    const unit = options.time.unit || 'day';\n    // eslint-disable-next-line prefer-const\n    let {min, max, minDefined, maxDefined} = this.getUserBounds();\n\n    /**\n\t\t * @param {object} bounds\n\t\t */\n    function _applyBounds(bounds) {\n      if (!minDefined && !isNaN(bounds.min)) {\n        min = Math.min(min, bounds.min);\n      }\n      if (!maxDefined && !isNaN(bounds.max)) {\n        max = Math.max(max, bounds.max);\n      }\n    }\n\n    // If we have user provided `min` and `max` labels / data bounds can be ignored\n    if (!minDefined || !maxDefined) {\n      // Labels are always considered, when user did not force bounds\n      _applyBounds(this._getLabelBounds());\n\n      // If `bounds` is `'ticks'` and `ticks.source` is `'labels'`,\n      // data bounds are ignored (and don't need to be determined)\n      if (options.bounds !== 'ticks' || options.ticks.source !== 'labels') {\n        _applyBounds(this.getMinMax(false));\n      }\n    }\n\n    min = isFinite(min) && !isNaN(min) ? min : +adapter.startOf(Date.now(), unit);\n    max = isFinite(max) && !isNaN(max) ? max : +adapter.endOf(Date.now(), unit) + 1;\n\n    // Make sure that max is strictly higher than min (required by the timeseries lookup table)\n    this.min = Math.min(min, max - 1);\n    this.max = Math.max(min + 1, max);\n  }\n\n  /**\n\t * @private\n\t */\n  _getLabelBounds() {\n    const arr = this.getLabelTimestamps();\n    let min = Number.POSITIVE_INFINITY;\n    let max = Number.NEGATIVE_INFINITY;\n\n    if (arr.length) {\n      min = arr[0];\n      max = arr[arr.length - 1];\n    }\n    return {min, max};\n  }\n\n  /**\n\t * @return {object[]}\n\t */\n  buildTicks() {\n    const options = this.options;\n    const timeOpts = options.time;\n    const tickOpts = options.ticks;\n    const timestamps = tickOpts.source === 'labels' ? this.getLabelTimestamps() : this._generate();\n\n    if (options.bounds === 'ticks' && timestamps.length) {\n      this.min = this._userMin || timestamps[0];\n      this.max = this._userMax || timestamps[timestamps.length - 1];\n    }\n\n    const min = this.min;\n    const max = this.max;\n\n    const ticks = _filterBetween(timestamps, min, max);\n\n    // PRIVATE\n    // determineUnitForFormatting relies on the number of ticks so we don't use it when\n    // autoSkip is enabled because we don't yet know what the final number of ticks will be\n    this._unit = timeOpts.unit || (tickOpts.autoSkip\n      ? determineUnitForAutoTicks(timeOpts.minUnit, this.min, this.max, this._getLabelCapacity(min))\n      : determineUnitForFormatting(this, ticks.length, timeOpts.minUnit, this.min, this.max));\n    this._majorUnit = !tickOpts.major.enabled || this._unit === 'year' ? undefined\n      : determineMajorUnit(this._unit);\n    this.initOffsets(timestamps);\n\n    if (options.reverse) {\n      ticks.reverse();\n    }\n\n    return ticksFromTimestamps(this, ticks, this._majorUnit);\n  }\n\n  afterAutoSkip() {\n    // Offsets for bar charts need to be handled with the auto skipped\n    // ticks. Once ticks have been skipped, we re-compute the offsets.\n    if (this.options.offsetAfterAutoskip) {\n      this.initOffsets(this.ticks.map(tick => +tick.value));\n    }\n  }\n\n  /**\n\t * Returns the start and end offsets from edges in the form of {start, end}\n\t * where each value is a relative width to the scale and ranges between 0 and 1.\n\t * They add extra margins on the both sides by scaling down the original scale.\n\t * Offsets are added when the `offset` option is true.\n\t * @param {number[]} timestamps\n\t * @protected\n\t */\n  initOffsets(timestamps = []) {\n    let start = 0;\n    let end = 0;\n    let first, last;\n\n    if (this.options.offset && timestamps.length) {\n      first = this.getDecimalForValue(timestamps[0]);\n      if (timestamps.length === 1) {\n        start = 1 - first;\n      } else {\n        start = (this.getDecimalForValue(timestamps[1]) - first) / 2;\n      }\n      last = this.getDecimalForValue(timestamps[timestamps.length - 1]);\n      if (timestamps.length === 1) {\n        end = last;\n      } else {\n        end = (last - this.getDecimalForValue(timestamps[timestamps.length - 2])) / 2;\n      }\n    }\n    const limit = timestamps.length < 3 ? 0.5 : 0.25;\n    start = _limitValue(start, 0, limit);\n    end = _limitValue(end, 0, limit);\n\n    this._offsets = {start, end, factor: 1 / (start + 1 + end)};\n  }\n\n  /**\n\t * Generates a maximum of `capacity` timestamps between min and max, rounded to the\n\t * `minor` unit using the given scale time `options`.\n\t * Important: this method can return ticks outside the min and max range, it's the\n\t * responsibility of the calling code to clamp values if needed.\n\t * @protected\n\t */\n  _generate() {\n    const adapter = this._adapter;\n    const min = this.min;\n    const max = this.max;\n    const options = this.options;\n    const timeOpts = options.time;\n    // @ts-ignore\n    const minor = timeOpts.unit || determineUnitForAutoTicks(timeOpts.minUnit, min, max, this._getLabelCapacity(min));\n    const stepSize = valueOrDefault(options.ticks.stepSize, 1);\n    const weekday = minor === 'week' ? timeOpts.isoWeekday : false;\n    const hasWeekday = isNumber(weekday) || weekday === true;\n    const ticks = {};\n    let first = min;\n    let time, count;\n\n    // For 'week' unit, handle the first day of week option\n    if (hasWeekday) {\n      first = +adapter.startOf(first, 'isoWeek', weekday);\n    }\n\n    // Align first ticks on unit\n    first = +adapter.startOf(first, hasWeekday ? 'day' : minor);\n\n    // Prevent browser from freezing in case user options request millions of milliseconds\n    if (adapter.diff(max, min, minor) > 100000 * stepSize) {\n      throw new Error(min + ' and ' + max + ' are too far apart with stepSize of ' + stepSize + ' ' + minor);\n    }\n\n    const timestamps = options.ticks.source === 'data' && this.getDataTimestamps();\n    for (time = first, count = 0; time < max; time = +adapter.add(time, stepSize, minor), count++) {\n      addTick(ticks, time, timestamps);\n    }\n\n    if (time === max || options.bounds === 'ticks' || count === 1) {\n      addTick(ticks, time, timestamps);\n    }\n\n    // @ts-ignore\n    return Object.keys(ticks).sort(sorter).map(x => +x);\n  }\n\n  /**\n\t * @param {number} value\n\t * @return {string}\n\t */\n  getLabelForValue(value) {\n    const adapter = this._adapter;\n    const timeOpts = this.options.time;\n\n    if (timeOpts.tooltipFormat) {\n      return adapter.format(value, timeOpts.tooltipFormat);\n    }\n    return adapter.format(value, timeOpts.displayFormats.datetime);\n  }\n\n  /**\n\t * @param {number} value\n\t * @param {string|undefined} format\n\t * @return {string}\n\t */\n  format(value, format) {\n    const options = this.options;\n    const formats = options.time.displayFormats;\n    const unit = this._unit;\n    const fmt = format || formats[unit];\n    return this._adapter.format(value, fmt);\n  }\n\n  /**\n\t * Function to format an individual tick mark\n\t * @param {number} time\n\t * @param {number} index\n\t * @param {object[]} ticks\n\t * @param {string|undefined} [format]\n\t * @return {string}\n\t * @private\n\t */\n  _tickFormatFunction(time, index, ticks, format) {\n    const options = this.options;\n    const formatter = options.ticks.callback;\n\n    if (formatter) {\n      return call(formatter, [time, index, ticks], this);\n    }\n\n    const formats = options.time.displayFormats;\n    const unit = this._unit;\n    const majorUnit = this._majorUnit;\n    const minorFormat = unit && formats[unit];\n    const majorFormat = majorUnit && formats[majorUnit];\n    const tick = ticks[index];\n    const major = majorUnit && majorFormat && tick && tick.major;\n\n    return this._adapter.format(time, format || (major ? majorFormat : minorFormat));\n  }\n\n  /**\n\t * @param {object[]} ticks\n\t */\n  generateTickLabels(ticks) {\n    let i, ilen, tick;\n\n    for (i = 0, ilen = ticks.length; i < ilen; ++i) {\n      tick = ticks[i];\n      tick.label = this._tickFormatFunction(tick.value, i, ticks);\n    }\n  }\n\n  /**\n\t * @param {number} value - Milliseconds since epoch (1 January 1970 00:00:00 UTC)\n\t * @return {number}\n\t */\n  getDecimalForValue(value) {\n    return value === null ? NaN : (value - this.min) / (this.max - this.min);\n  }\n\n  /**\n\t * @param {number} value - Milliseconds since epoch (1 January 1970 00:00:00 UTC)\n\t * @return {number}\n\t */\n  getPixelForValue(value) {\n    const offsets = this._offsets;\n    const pos = this.getDecimalForValue(value);\n    return this.getPixelForDecimal((offsets.start + pos) * offsets.factor);\n  }\n\n  /**\n\t * @param {number} pixel\n\t * @return {number}\n\t */\n  getValueForPixel(pixel) {\n    const offsets = this._offsets;\n    const pos = this.getDecimalForPixel(pixel) / offsets.factor - offsets.end;\n    return this.min + pos * (this.max - this.min);\n  }\n\n  /**\n\t * @param {string} label\n\t * @return {{w:number, h:number}}\n\t * @private\n\t */\n  _getLabelSize(label) {\n    const ticksOpts = this.options.ticks;\n    const tickLabelWidth = this.ctx.measureText(label).width;\n    const angle = toRadians(this.isHorizontal() ? ticksOpts.maxRotation : ticksOpts.minRotation);\n    const cosRotation = Math.cos(angle);\n    const sinRotation = Math.sin(angle);\n    const tickFontSize = this._resolveTickFontOptions(0).size;\n\n    return {\n      w: (tickLabelWidth * cosRotation) + (tickFontSize * sinRotation),\n      h: (tickLabelWidth * sinRotation) + (tickFontSize * cosRotation)\n    };\n  }\n\n  /**\n\t * @param {number} exampleTime\n\t * @return {number}\n\t * @private\n\t */\n  _getLabelCapacity(exampleTime) {\n    const timeOpts = this.options.time;\n    const displayFormats = timeOpts.displayFormats;\n\n    // pick the longest format (milliseconds) for guesstimation\n    const format = displayFormats[timeOpts.unit] || displayFormats.millisecond;\n    const exampleLabel = this._tickFormatFunction(exampleTime, 0, ticksFromTimestamps(this, [exampleTime], this._majorUnit), format);\n    const size = this._getLabelSize(exampleLabel);\n    // subtract 1 - if offset then there's one less label than tick\n    // if not offset then one half label padding is added to each end leaving room for one less label\n    const capacity = Math.floor(this.isHorizontal() ? this.width / size.w : this.height / size.h) - 1;\n    return capacity > 0 ? capacity : 1;\n  }\n\n  /**\n\t * @protected\n\t */\n  getDataTimestamps() {\n    let timestamps = this._cache.data || [];\n    let i, ilen;\n\n    if (timestamps.length) {\n      return timestamps;\n    }\n\n    const metas = this.getMatchingVisibleMetas();\n\n    if (this._normalized && metas.length) {\n      return (this._cache.data = metas[0].controller.getAllParsedValues(this));\n    }\n\n    for (i = 0, ilen = metas.length; i < ilen; ++i) {\n      timestamps = timestamps.concat(metas[i].controller.getAllParsedValues(this));\n    }\n\n    return (this._cache.data = this.normalize(timestamps));\n  }\n\n  /**\n\t * @protected\n\t */\n  getLabelTimestamps() {\n    const timestamps = this._cache.labels || [];\n    let i, ilen;\n\n    if (timestamps.length) {\n      return timestamps;\n    }\n\n    const labels = this.getLabels();\n    for (i = 0, ilen = labels.length; i < ilen; ++i) {\n      timestamps.push(parse(this, labels[i]));\n    }\n\n    return (this._cache.labels = this._normalized ? timestamps : this.normalize(timestamps));\n  }\n\n  /**\n\t * @param {number[]} values\n\t * @protected\n\t */\n  normalize(values) {\n    // It seems to be somewhat faster to do sorting first\n    return _arrayUnique(values.sort(sorter));\n  }\n}\n",
         "import TimeScale from './scale.time.js';\nimport {_lookupByKey} from '../helpers/helpers.collection.js';\n\n/**\n * Linearly interpolates the given source `val` using the table. If value is out of bounds, values\n * at edges are used for the interpolation.\n * @param {object} table\n * @param {number} val\n * @param {boolean} [reverse] lookup time based on position instead of vice versa\n * @return {object}\n */\nfunction interpolate(table, val, reverse) {\n  let lo = 0;\n  let hi = table.length - 1;\n  let prevSource, nextSource, prevTarget, nextTarget;\n  if (reverse) {\n    if (val >= table[lo].pos && val <= table[hi].pos) {\n      ({lo, hi} = _lookupByKey(table, 'pos', val));\n    }\n    ({pos: prevSource, time: prevTarget} = table[lo]);\n    ({pos: nextSource, time: nextTarget} = table[hi]);\n  } else {\n    if (val >= table[lo].time && val <= table[hi].time) {\n      ({lo, hi} = _lookupByKey(table, 'time', val));\n    }\n    ({time: prevSource, pos: prevTarget} = table[lo]);\n    ({time: nextSource, pos: nextTarget} = table[hi]);\n  }\n\n  const span = nextSource - prevSource;\n  return span ? prevTarget + (nextTarget - prevTarget) * (val - prevSource) / span : prevTarget;\n}\n\nclass TimeSeriesScale extends TimeScale {\n\n  static id = 'timeseries';\n\n  /**\n   * @type {any}\n   */\n  static defaults = TimeScale.defaults;\n\n  /**\n\t * @param {object} props\n\t */\n  constructor(props) {\n    super(props);\n\n    /** @type {object[]} */\n    this._table = [];\n    /** @type {number} */\n    this._minPos = undefined;\n    /** @type {number} */\n    this._tableRange = undefined;\n  }\n\n  /**\n\t * @protected\n\t */\n  initOffsets() {\n    const timestamps = this._getTimestampsForTable();\n    const table = this._table = this.buildLookupTable(timestamps);\n    this._minPos = interpolate(table, this.min);\n    this._tableRange = interpolate(table, this.max) - this._minPos;\n    super.initOffsets(timestamps);\n  }\n\n  /**\n\t * Returns an array of {time, pos} objects used to interpolate a specific `time` or position\n\t * (`pos`) on the scale, by searching entries before and after the requested value. `pos` is\n\t * a decimal between 0 and 1: 0 being the start of the scale (left or top) and 1 the other\n\t * extremity (left + width or top + height). Note that it would be more optimized to directly\n\t * store pre-computed pixels, but the scale dimensions are not guaranteed at the time we need\n\t * to create the lookup table. The table ALWAYS contains at least two items: min and max.\n\t * @param {number[]} timestamps\n\t * @return {object[]}\n\t * @protected\n\t */\n  buildLookupTable(timestamps) {\n    const {min, max} = this;\n    const items = [];\n    const table = [];\n    let i, ilen, prev, curr, next;\n\n    for (i = 0, ilen = timestamps.length; i < ilen; ++i) {\n      curr = timestamps[i];\n      if (curr >= min && curr <= max) {\n        items.push(curr);\n      }\n    }\n\n    if (items.length < 2) {\n      // In case there is less that 2 timestamps between min and max, the scale is defined by min and max\n      return [\n        {time: min, pos: 0},\n        {time: max, pos: 1}\n      ];\n    }\n\n    for (i = 0, ilen = items.length; i < ilen; ++i) {\n      next = items[i + 1];\n      prev = items[i - 1];\n      curr = items[i];\n\n      // only add points that breaks the scale linearity\n      if (Math.round((next + prev) / 2) !== curr) {\n        table.push({time: curr, pos: i / (ilen - 1)});\n      }\n    }\n    return table;\n  }\n\n  /**\n    * Generates all timestamps defined in the data.\n    * Important: this method can return ticks outside the min and max range, it's the\n    * responsibility of the calling code to clamp values if needed.\n    * @protected\n    */\n  _generate() {\n    const min = this.min;\n    const max = this.max;\n    let timestamps = super.getDataTimestamps();\n    if (!timestamps.includes(min) || !timestamps.length) {\n      timestamps.splice(0, 0, min);\n    }\n    if (!timestamps.includes(max) || timestamps.length === 1) {\n      timestamps.push(max);\n    }\n    return timestamps.sort((a, b) => a - b);\n  }\n\n  /**\n\t * Returns all timestamps\n\t * @return {number[]}\n\t * @private\n\t */\n  _getTimestampsForTable() {\n    let timestamps = this._cache.all || [];\n\n    if (timestamps.length) {\n      return timestamps;\n    }\n\n    const data = this.getDataTimestamps();\n    const label = this.getLabelTimestamps();\n    if (data.length && label.length) {\n      // If combining labels and data (data might not contain all labels),\n      // we need to recheck uniqueness and sort\n      timestamps = this.normalize(data.concat(label));\n    } else {\n      timestamps = data.length ? data : label;\n    }\n    timestamps = this._cache.all = timestamps;\n\n    return timestamps;\n  }\n\n  /**\n\t * @param {number} value - Milliseconds since epoch (1 January 1970 00:00:00 UTC)\n\t * @return {number}\n\t */\n  getDecimalForValue(value) {\n    return (interpolate(this._table, value) - this._minPos) / this._tableRange;\n  }\n\n  /**\n\t * @param {number} pixel\n\t * @return {number}\n\t */\n  getValueForPixel(pixel) {\n    const offsets = this._offsets;\n    const decimal = this.getDecimalForPixel(pixel) / offsets.factor - offsets.end;\n    return interpolate(this._table, decimal * this._tableRange + this._minPos, true);\n  }\n}\n\nexport default TimeSeriesScale;\n",
         "export * from './controllers/index.js';\nexport * from './core/index.js';\nexport * from './elements/index.js';\nexport * from './platform/index.js';\nexport * from './plugins/index.js';\nexport * from './scales/index.js';\n\nimport * as controllers from './controllers/index.js';\nimport * as elements from './elements/index.js';\nimport * as plugins from './plugins/index.js';\nimport * as scales from './scales/index.js';\n\nexport {\n  controllers,\n  elements,\n  plugins,\n  scales,\n};\n\nexport const registerables = [\n  controllers,\n  elements,\n  plugins,\n  scales,\n];\n",
+        "/*!\n* chartjs-plugin-zoom v2.0.1\n* undefined\n * (c) 2016-2023 chartjs-plugin-zoom Contributors\n * Released under the MIT License\n */\nimport Hammer from 'hammerjs';\nimport { each, valueOrDefault, callback, sign, getRelativePosition } from 'chart.js/helpers';\n\nconst getModifierKey = opts => opts && opts.enabled && opts.modifierKey;\nconst keyPressed = (key, event) => key && event[key + 'Key'];\nconst keyNotPressed = (key, event) => key && !event[key + 'Key'];\n\n/**\n * @param {string|function} mode can be 'x', 'y' or 'xy'\n * @param {string} dir can be 'x' or 'y'\n * @param {import('chart.js').Chart} chart instance of the chart in question\n * @returns {boolean}\n */\nfunction directionEnabled(mode, dir, chart) {\n  if (mode === undefined) {\n    return true;\n  } else if (typeof mode === 'string') {\n    return mode.indexOf(dir) !== -1;\n  } else if (typeof mode === 'function') {\n    return mode({chart}).indexOf(dir) !== -1;\n  }\n\n  return false;\n}\n\nfunction directionsEnabled(mode, chart) {\n  if (typeof mode === 'function') {\n    mode = mode({chart});\n  }\n  if (typeof mode === 'string') {\n    return {x: mode.indexOf('x') !== -1, y: mode.indexOf('y') !== -1};\n  }\n\n  return {x: false, y: false};\n}\n\n/**\n * Debounces calling `fn` for `delay` ms\n * @param {function} fn - Function to call. No arguments are passed.\n * @param {number} delay - Delay in ms. 0 = immediate invocation.\n * @returns {function}\n */\nfunction debounce(fn, delay) {\n  let timeout;\n  return function() {\n    clearTimeout(timeout);\n    timeout = setTimeout(fn, delay);\n    return delay;\n  };\n}\n\n/**\n * Checks which axis is under the mouse cursor.\n * @param {{x: number, y: number}} point - the mouse location\n * @param {import('chart.js').Chart} [chart] instance of the chart in question\n * @return {import('chart.js').Scale}\n */\nfunction getScaleUnderPoint({x, y}, chart) {\n  const scales = chart.scales;\n  const scaleIds = Object.keys(scales);\n  for (let i = 0; i < scaleIds.length; i++) {\n    const scale = scales[scaleIds[i]];\n    if (y >= scale.top && y <= scale.bottom && x >= scale.left && x <= scale.right) {\n      return scale;\n    }\n  }\n  return null;\n}\n\n/**\n * Evaluate the chart's mode, scaleMode, and overScaleMode properties to\n * determine which axes are eligible for scaling.\n * options.overScaleMode can be a function if user want zoom only one scale of many for example.\n * @param options - Zoom or pan options\n * @param {{x: number, y: number}} point - the mouse location\n * @param {import('chart.js').Chart} [chart] instance of the chart in question\n * @return {import('chart.js').Scale[]}\n */\nfunction getEnabledScalesByPoint(options, point, chart) {\n  const {mode = 'xy', scaleMode, overScaleMode} = options || {};\n  const scale = getScaleUnderPoint(point, chart);\n\n  const enabled = directionsEnabled(mode, chart);\n  const scaleEnabled = directionsEnabled(scaleMode, chart);\n\n  // Convert deprecated overScaleEnabled to new scaleEnabled.\n  if (overScaleMode) {\n    const overScaleEnabled = directionsEnabled(overScaleMode, chart);\n    for (const axis of ['x', 'y']) {\n      if (overScaleEnabled[axis]) {\n        scaleEnabled[axis] = enabled[axis];\n        enabled[axis] = false;\n      }\n    }\n  }\n\n  if (scale && scaleEnabled[scale.axis]) {\n    return [scale];\n  }\n\n  const enabledScales = [];\n  each(chart.scales, function(scaleItem) {\n    if (enabled[scaleItem.axis]) {\n      enabledScales.push(scaleItem);\n    }\n  });\n  return enabledScales;\n}\n\nconst chartStates = new WeakMap();\n\nfunction getState(chart) {\n  let state = chartStates.get(chart);\n  if (!state) {\n    state = {\n      originalScaleLimits: {},\n      updatedScaleLimits: {},\n      handlers: {},\n      panDelta: {}\n    };\n    chartStates.set(chart, state);\n  }\n  return state;\n}\n\nfunction removeState(chart) {\n  chartStates.delete(chart);\n}\n\nfunction zoomDelta(scale, zoom, center) {\n  const range = scale.max - scale.min;\n  const newRange = range * (zoom - 1);\n\n  const centerPoint = scale.isHorizontal() ? center.x : center.y;\n  // `scale.getValueForPixel()` can return a value less than the `scale.min` or\n  // greater than `scale.max` when `centerPoint` is outside chartArea.\n  const minPercent = Math.max(0, Math.min(1,\n    (scale.getValueForPixel(centerPoint) - scale.min) / range || 0\n  ));\n\n  const maxPercent = 1 - minPercent;\n\n  return {\n    min: newRange * minPercent,\n    max: newRange * maxPercent\n  };\n}\n\nfunction getLimit(state, scale, scaleLimits, prop, fallback) {\n  let limit = scaleLimits[prop];\n  if (limit === 'original') {\n    const original = state.originalScaleLimits[scale.id][prop];\n    limit = valueOrDefault(original.options, original.scale);\n  }\n  return valueOrDefault(limit, fallback);\n}\n\nfunction getRange(scale, pixel0, pixel1) {\n  const v0 = scale.getValueForPixel(pixel0);\n  const v1 = scale.getValueForPixel(pixel1);\n  return {\n    min: Math.min(v0, v1),\n    max: Math.max(v0, v1)\n  };\n}\n\nfunction updateRange(scale, {min, max}, limits, zoom = false) {\n  const state = getState(scale.chart);\n  const {id, axis, options: scaleOpts} = scale;\n\n  const scaleLimits = limits && (limits[id] || limits[axis]) || {};\n  const {minRange = 0} = scaleLimits;\n  const minLimit = getLimit(state, scale, scaleLimits, 'min', -Infinity);\n  const maxLimit = getLimit(state, scale, scaleLimits, 'max', Infinity);\n\n  const range = zoom ? Math.max(max - min, minRange) : scale.max - scale.min;\n  const offset = (range - max + min) / 2;\n  min -= offset;\n  max += offset;\n\n  if (min < minLimit) {\n    min = minLimit;\n    max = Math.min(minLimit + range, maxLimit);\n  } else if (max > maxLimit) {\n    max = maxLimit;\n    min = Math.max(maxLimit - range, minLimit);\n  }\n  scaleOpts.min = min;\n  scaleOpts.max = max;\n\n  state.updatedScaleLimits[scale.id] = {min, max};\n\n  // return true if the scale range is changed\n  return scale.parse(min) !== scale.min || scale.parse(max) !== scale.max;\n}\n\nfunction zoomNumericalScale(scale, zoom, center, limits) {\n  const delta = zoomDelta(scale, zoom, center);\n  const newRange = {min: scale.min + delta.min, max: scale.max - delta.max};\n  return updateRange(scale, newRange, limits, true);\n}\n\nfunction zoomRectNumericalScale(scale, from, to, limits) {\n  updateRange(scale, getRange(scale, from, to), limits, true);\n}\n\nconst integerChange = (v) => v === 0 || isNaN(v) ? 0 : v < 0 ? Math.min(Math.round(v), -1) : Math.max(Math.round(v), 1);\n\nfunction existCategoryFromMaxZoom(scale) {\n  const labels = scale.getLabels();\n  const maxIndex = labels.length - 1;\n\n  if (scale.min > 0) {\n    scale.min -= 1;\n  }\n  if (scale.max < maxIndex) {\n    scale.max += 1;\n  }\n}\n\nfunction zoomCategoryScale(scale, zoom, center, limits) {\n  const delta = zoomDelta(scale, zoom, center);\n  if (scale.min === scale.max && zoom < 1) {\n    existCategoryFromMaxZoom(scale);\n  }\n  const newRange = {min: scale.min + integerChange(delta.min), max: scale.max - integerChange(delta.max)};\n  return updateRange(scale, newRange, limits, true);\n}\n\nfunction scaleLength(scale) {\n  return scale.isHorizontal() ? scale.width : scale.height;\n}\n\nfunction panCategoryScale(scale, delta, limits) {\n  const labels = scale.getLabels();\n  const lastLabelIndex = labels.length - 1;\n  let {min, max} = scale;\n  // The visible range. Ticks can be skipped, and thus not reliable.\n  const range = Math.max(max - min, 1);\n  // How many pixels of delta is required before making a step. stepSize, but limited to max 1/10 of the scale length.\n  const stepDelta = Math.round(scaleLength(scale) / Math.max(range, 10));\n  const stepSize = Math.round(Math.abs(delta / stepDelta));\n  let applied;\n  if (delta < -stepDelta) {\n    max = Math.min(max + stepSize, lastLabelIndex);\n    min = range === 1 ? max : max - range;\n    applied = max === lastLabelIndex;\n  } else if (delta > stepDelta) {\n    min = Math.max(0, min - stepSize);\n    max = range === 1 ? min : min + range;\n    applied = min === 0;\n  }\n\n  return updateRange(scale, {min, max}, limits) || applied;\n}\n\nconst OFFSETS = {\n  second: 500, // 500 ms\n  minute: 30 * 1000, // 30 s\n  hour: 30 * 60 * 1000, // 30 m\n  day: 12 * 60 * 60 * 1000, // 12 h\n  week: 3.5 * 24 * 60 * 60 * 1000, // 3.5 d\n  month: 15 * 24 * 60 * 60 * 1000, // 15 d\n  quarter: 60 * 24 * 60 * 60 * 1000, // 60 d\n  year: 182 * 24 * 60 * 60 * 1000 // 182 d\n};\n\nfunction panNumericalScale(scale, delta, limits, canZoom = false) {\n  const {min: prevStart, max: prevEnd, options} = scale;\n  const round = options.time && options.time.round;\n  const offset = OFFSETS[round] || 0;\n  const newMin = scale.getValueForPixel(scale.getPixelForValue(prevStart + offset) - delta);\n  const newMax = scale.getValueForPixel(scale.getPixelForValue(prevEnd + offset) - delta);\n  const {min: minLimit = -Infinity, max: maxLimit = Infinity} = canZoom && limits && limits[scale.axis] || {};\n  if (isNaN(newMin) || isNaN(newMax) || newMin < minLimit || newMax > maxLimit) {\n    // At limit: No change but return true to indicate no need to store the delta.\n    // NaN can happen for 0-dimension scales (either because they were configured\n    // with min === max or because the chart has 0 plottable area).\n    return true;\n  }\n  return updateRange(scale, {min: newMin, max: newMax}, limits, canZoom);\n}\n\nfunction panNonLinearScale(scale, delta, limits) {\n  return panNumericalScale(scale, delta, limits, true);\n}\n\nconst zoomFunctions = {\n  category: zoomCategoryScale,\n  default: zoomNumericalScale,\n};\n\nconst zoomRectFunctions = {\n  default: zoomRectNumericalScale,\n};\n\nconst panFunctions = {\n  category: panCategoryScale,\n  default: panNumericalScale,\n  logarithmic: panNonLinearScale,\n  timeseries: panNonLinearScale,\n};\n\nfunction shouldUpdateScaleLimits(scale, originalScaleLimits, updatedScaleLimits) {\n  const {id, options: {min, max}} = scale;\n  if (!originalScaleLimits[id] || !updatedScaleLimits[id]) {\n    return true;\n  }\n  const previous = updatedScaleLimits[id];\n  return previous.min !== min || previous.max !== max;\n}\n\nfunction removeMissingScales(limits, scales) {\n  each(limits, (opt, key) => {\n    if (!scales[key]) {\n      delete limits[key];\n    }\n  });\n}\n\nfunction storeOriginalScaleLimits(chart, state) {\n  const {scales} = chart;\n  const {originalScaleLimits, updatedScaleLimits} = state;\n\n  each(scales, function(scale) {\n    if (shouldUpdateScaleLimits(scale, originalScaleLimits, updatedScaleLimits)) {\n      originalScaleLimits[scale.id] = {\n        min: {scale: scale.min, options: scale.options.min},\n        max: {scale: scale.max, options: scale.options.max},\n      };\n    }\n  });\n\n  removeMissingScales(originalScaleLimits, scales);\n  removeMissingScales(updatedScaleLimits, scales);\n  return originalScaleLimits;\n}\n\nfunction doZoom(scale, amount, center, limits) {\n  const fn = zoomFunctions[scale.type] || zoomFunctions.default;\n  callback(fn, [scale, amount, center, limits]);\n}\n\nfunction doZoomRect(scale, amount, from, to, limits) {\n  const fn = zoomRectFunctions[scale.type] || zoomRectFunctions.default;\n  callback(fn, [scale, amount, from, to, limits]);\n}\n\nfunction getCenter(chart) {\n  const ca = chart.chartArea;\n  return {\n    x: (ca.left + ca.right) / 2,\n    y: (ca.top + ca.bottom) / 2,\n  };\n}\n\n/**\n * @param chart The chart instance\n * @param {number | {x?: number, y?: number, focalPoint?: {x: number, y: number}}} amount The zoom percentage or percentages and focal point\n * @param {string} [transition] Which transition mode to use. Defaults to 'none'\n */\nfunction zoom(chart, amount, transition = 'none') {\n  const {x = 1, y = 1, focalPoint = getCenter(chart)} = typeof amount === 'number' ? {x: amount, y: amount} : amount;\n  const state = getState(chart);\n  const {options: {limits, zoom: zoomOptions}} = state;\n\n  storeOriginalScaleLimits(chart, state);\n\n  const xEnabled = x !== 1;\n  const yEnabled = y !== 1;\n  const enabledScales = getEnabledScalesByPoint(zoomOptions, focalPoint, chart);\n\n  each(enabledScales || chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      doZoom(scale, x, focalPoint, limits);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      doZoom(scale, y, focalPoint, limits);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(zoomOptions.onZoom, [{chart}]);\n}\n\nfunction zoomRect(chart, p0, p1, transition = 'none') {\n  const state = getState(chart);\n  const {options: {limits, zoom: zoomOptions}} = state;\n  const {mode = 'xy'} = zoomOptions;\n\n  storeOriginalScaleLimits(chart, state);\n  const xEnabled = directionEnabled(mode, 'x', chart);\n  const yEnabled = directionEnabled(mode, 'y', chart);\n\n  each(chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      doZoomRect(scale, p0.x, p1.x, limits);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      doZoomRect(scale, p0.y, p1.y, limits);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(zoomOptions.onZoom, [{chart}]);\n}\n\nfunction zoomScale(chart, scaleId, range, transition = 'none') {\n  storeOriginalScaleLimits(chart, getState(chart));\n  const scale = chart.scales[scaleId];\n  updateRange(scale, range, undefined, true);\n  chart.update(transition);\n}\n\nfunction resetZoom(chart, transition = 'default') {\n  const state = getState(chart);\n  const originalScaleLimits = storeOriginalScaleLimits(chart, state);\n\n  each(chart.scales, function(scale) {\n    const scaleOptions = scale.options;\n    if (originalScaleLimits[scale.id]) {\n      scaleOptions.min = originalScaleLimits[scale.id].min.options;\n      scaleOptions.max = originalScaleLimits[scale.id].max.options;\n    } else {\n      delete scaleOptions.min;\n      delete scaleOptions.max;\n    }\n  });\n  chart.update(transition);\n  callback(state.options.zoom.onZoomComplete, [{chart}]);\n}\n\nfunction getOriginalRange(state, scaleId) {\n  const original = state.originalScaleLimits[scaleId];\n  if (!original) {\n    return;\n  }\n  const {min, max} = original;\n  return valueOrDefault(max.options, max.scale) - valueOrDefault(min.options, min.scale);\n}\n\nfunction getZoomLevel(chart) {\n  const state = getState(chart);\n  let min = 1;\n  let max = 1;\n  each(chart.scales, function(scale) {\n    const origRange = getOriginalRange(state, scale.id);\n    if (origRange) {\n      const level = Math.round(origRange / (scale.max - scale.min) * 100) / 100;\n      min = Math.min(min, level);\n      max = Math.max(max, level);\n    }\n  });\n  return min < 1 ? min : max;\n}\n\nfunction panScale(scale, delta, limits, state) {\n  const {panDelta} = state;\n  // Add possible cumulative delta from previous pan attempts where scale did not change\n  const storedDelta = panDelta[scale.id] || 0;\n  if (sign(storedDelta) === sign(delta)) {\n    delta += storedDelta;\n  }\n  const fn = panFunctions[scale.type] || panFunctions.default;\n  if (callback(fn, [scale, delta, limits])) {\n    // The scale changed, reset cumulative delta\n    panDelta[scale.id] = 0;\n  } else {\n    // The scale did not change, store cumulative delta\n    panDelta[scale.id] = delta;\n  }\n}\n\nfunction pan(chart, delta, enabledScales, transition = 'none') {\n  const {x = 0, y = 0} = typeof delta === 'number' ? {x: delta, y: delta} : delta;\n  const state = getState(chart);\n  const {options: {pan: panOptions, limits}} = state;\n  const {onPan} = panOptions || {};\n\n  storeOriginalScaleLimits(chart, state);\n\n  const xEnabled = x !== 0;\n  const yEnabled = y !== 0;\n\n  each(enabledScales || chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      panScale(scale, x, limits, state);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      panScale(scale, y, limits, state);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(onPan, [{chart}]);\n}\n\nfunction getInitialScaleBounds(chart) {\n  const state = getState(chart);\n  storeOriginalScaleLimits(chart, state);\n  const scaleBounds = {};\n  for (const scaleId of Object.keys(chart.scales)) {\n    const {min, max} = state.originalScaleLimits[scaleId] || {min: {}, max: {}};\n    scaleBounds[scaleId] = {min: min.scale, max: max.scale};\n  }\n\n  return scaleBounds;\n}\n\nfunction isZoomedOrPanned(chart) {\n  const scaleBounds = getInitialScaleBounds(chart);\n  for (const scaleId of Object.keys(chart.scales)) {\n    const {min: originalMin, max: originalMax} = scaleBounds[scaleId];\n\n    if (originalMin !== undefined && chart.scales[scaleId].min !== originalMin) {\n      return true;\n    }\n\n    if (originalMax !== undefined && chart.scales[scaleId].max !== originalMax) {\n      return true;\n    }\n  }\n\n  return false;\n}\n\nfunction removeHandler(chart, type) {\n  const {handlers} = getState(chart);\n  const handler = handlers[type];\n  if (handler && handler.target) {\n    handler.target.removeEventListener(type, handler);\n    delete handlers[type];\n  }\n}\n\nfunction addHandler(chart, target, type, handler) {\n  const {handlers, options} = getState(chart);\n  const oldHandler = handlers[type];\n  if (oldHandler && oldHandler.target === target) {\n    // already attached\n    return;\n  }\n  removeHandler(chart, type);\n  handlers[type] = (event) => handler(chart, event, options);\n  handlers[type].target = target;\n  target.addEventListener(type, handlers[type]);\n}\n\nfunction mouseMove(chart, event) {\n  const state = getState(chart);\n  if (state.dragStart) {\n    state.dragging = true;\n    state.dragEnd = event;\n    chart.update('none');\n  }\n}\n\nfunction keyDown(chart, event) {\n  const state = getState(chart);\n  if (!state.dragStart || event.key !== 'Escape') {\n    return;\n  }\n\n  removeHandler(chart, 'keydown');\n  state.dragging = false;\n  state.dragStart = state.dragEnd = null;\n  chart.update('none');\n}\n\nfunction zoomStart(chart, event, zoomOptions) {\n  const {onZoomStart, onZoomRejected} = zoomOptions;\n  if (onZoomStart) {\n    const point = getRelativePosition(event, chart);\n    if (callback(onZoomStart, [{chart, event, point}]) === false) {\n      callback(onZoomRejected, [{chart, event}]);\n      return false;\n    }\n  }\n}\n\nfunction mouseDown(chart, event) {\n  const state = getState(chart);\n  const {pan: panOptions, zoom: zoomOptions = {}} = state.options;\n  if (\n    event.button !== 0 ||\n    keyPressed(getModifierKey(panOptions), event) ||\n    keyNotPressed(getModifierKey(zoomOptions.drag), event)\n  ) {\n    return callback(zoomOptions.onZoomRejected, [{chart, event}]);\n  }\n\n  if (zoomStart(chart, event, zoomOptions) === false) {\n    return;\n  }\n  state.dragStart = event;\n\n  addHandler(chart, chart.canvas, 'mousemove', mouseMove);\n  addHandler(chart, window.document, 'keydown', keyDown);\n}\n\nfunction computeDragRect(chart, mode, beginPointEvent, endPointEvent) {\n  const xEnabled = directionEnabled(mode, 'x', chart);\n  const yEnabled = directionEnabled(mode, 'y', chart);\n  let {top, left, right, bottom, width: chartWidth, height: chartHeight} = chart.chartArea;\n\n  const beginPoint = getRelativePosition(beginPointEvent, chart);\n  const endPoint = getRelativePosition(endPointEvent, chart);\n\n  if (xEnabled) {\n    left = Math.min(beginPoint.x, endPoint.x);\n    right = Math.max(beginPoint.x, endPoint.x);\n  }\n\n  if (yEnabled) {\n    top = Math.min(beginPoint.y, endPoint.y);\n    bottom = Math.max(beginPoint.y, endPoint.y);\n  }\n  const width = right - left;\n  const height = bottom - top;\n\n  return {\n    left,\n    top,\n    right,\n    bottom,\n    width,\n    height,\n    zoomX: xEnabled && width ? 1 + ((chartWidth - width) / chartWidth) : 1,\n    zoomY: yEnabled && height ? 1 + ((chartHeight - height) / chartHeight) : 1\n  };\n}\n\nfunction mouseUp(chart, event) {\n  const state = getState(chart);\n  if (!state.dragStart) {\n    return;\n  }\n\n  removeHandler(chart, 'mousemove');\n  const {mode, onZoomComplete, drag: {threshold = 0}} = state.options.zoom;\n  const rect = computeDragRect(chart, mode, state.dragStart, event);\n  const distanceX = directionEnabled(mode, 'x', chart) ? rect.width : 0;\n  const distanceY = directionEnabled(mode, 'y', chart) ? rect.height : 0;\n  const distance = Math.sqrt(distanceX * distanceX + distanceY * distanceY);\n\n  // Remove drag start and end before chart update to stop drawing selected area\n  state.dragStart = state.dragEnd = null;\n\n  if (distance <= threshold) {\n    state.dragging = false;\n    chart.update('none');\n    return;\n  }\n\n  zoomRect(chart, {x: rect.left, y: rect.top}, {x: rect.right, y: rect.bottom}, 'zoom');\n\n  setTimeout(() => (state.dragging = false), 500);\n  callback(onZoomComplete, [{chart}]);\n}\n\nfunction wheelPreconditions(chart, event, zoomOptions) {\n  // Before preventDefault, check if the modifier key required and pressed\n  if (keyNotPressed(getModifierKey(zoomOptions.wheel), event)) {\n    callback(zoomOptions.onZoomRejected, [{chart, event}]);\n    return;\n  }\n\n  if (zoomStart(chart, event, zoomOptions) === false) {\n    return;\n  }\n\n  // Prevent the event from triggering the default behavior (e.g. content scrolling).\n  if (event.cancelable) {\n    event.preventDefault();\n  }\n\n  // Firefox always fires the wheel event twice:\n  // First without the delta and right after that once with the delta properties.\n  if (event.deltaY === undefined) {\n    return;\n  }\n  return true;\n}\n\nfunction wheel(chart, event) {\n  const {handlers: {onZoomComplete}, options: {zoom: zoomOptions}} = getState(chart);\n\n  if (!wheelPreconditions(chart, event, zoomOptions)) {\n    return;\n  }\n\n  const rect = event.target.getBoundingClientRect();\n  const speed = 1 + (event.deltaY >= 0 ? -zoomOptions.wheel.speed : zoomOptions.wheel.speed);\n  const amount = {\n    x: speed,\n    y: speed,\n    focalPoint: {\n      x: event.clientX - rect.left,\n      y: event.clientY - rect.top\n    }\n  };\n\n  zoom(chart, amount);\n\n  if (onZoomComplete) {\n    onZoomComplete();\n  }\n}\n\nfunction addDebouncedHandler(chart, name, handler, delay) {\n  if (handler) {\n    getState(chart).handlers[name] = debounce(() => callback(handler, [{chart}]), delay);\n  }\n}\n\nfunction addListeners(chart, options) {\n  const canvas = chart.canvas;\n  const {wheel: wheelOptions, drag: dragOptions, onZoomComplete} = options.zoom;\n\n  // Install listeners. Do this dynamically based on options so that we can turn zoom on and off\n  // We also want to make sure listeners aren't always on. E.g. if you're scrolling down a page\n  // and the mouse goes over a chart you don't want it intercepted unless the plugin is enabled\n  if (wheelOptions.enabled) {\n    addHandler(chart, canvas, 'wheel', wheel);\n    addDebouncedHandler(chart, 'onZoomComplete', onZoomComplete, 250);\n  } else {\n    removeHandler(chart, 'wheel');\n  }\n  if (dragOptions.enabled) {\n    addHandler(chart, canvas, 'mousedown', mouseDown);\n    addHandler(chart, canvas.ownerDocument, 'mouseup', mouseUp);\n  } else {\n    removeHandler(chart, 'mousedown');\n    removeHandler(chart, 'mousemove');\n    removeHandler(chart, 'mouseup');\n    removeHandler(chart, 'keydown');\n  }\n}\n\nfunction removeListeners(chart) {\n  removeHandler(chart, 'mousedown');\n  removeHandler(chart, 'mousemove');\n  removeHandler(chart, 'mouseup');\n  removeHandler(chart, 'wheel');\n  removeHandler(chart, 'click');\n  removeHandler(chart, 'keydown');\n}\n\nfunction createEnabler(chart, state) {\n  return function(recognizer, event) {\n    const {pan: panOptions, zoom: zoomOptions = {}} = state.options;\n    if (!panOptions || !panOptions.enabled) {\n      return false;\n    }\n    const srcEvent = event && event.srcEvent;\n    if (!srcEvent) { // Sometimes Hammer queries this with a null event.\n      return true;\n    }\n    if (!state.panning && event.pointerType === 'mouse' && (\n      keyNotPressed(getModifierKey(panOptions), srcEvent) || keyPressed(getModifierKey(zoomOptions.drag), srcEvent))\n    ) {\n      callback(panOptions.onPanRejected, [{chart, event}]);\n      return false;\n    }\n    return true;\n  };\n}\n\nfunction pinchAxes(p0, p1) {\n  // fingers position difference\n  const pinchX = Math.abs(p0.clientX - p1.clientX);\n  const pinchY = Math.abs(p0.clientY - p1.clientY);\n\n  // diagonal fingers will change both (xy) axes\n  const p = pinchX / pinchY;\n  let x, y;\n  if (p > 0.3 && p < 1.7) {\n    x = y = true;\n  } else if (pinchX > pinchY) {\n    x = true;\n  } else {\n    y = true;\n  }\n  return {x, y};\n}\n\nfunction handlePinch(chart, state, e) {\n  if (state.scale) {\n    const {center, pointers} = e;\n    // Hammer reports the total scaling. We need the incremental amount\n    const zoomPercent = 1 / state.scale * e.scale;\n    const rect = e.target.getBoundingClientRect();\n    const pinch = pinchAxes(pointers[0], pointers[1]);\n    const mode = state.options.zoom.mode;\n    const amount = {\n      x: pinch.x && directionEnabled(mode, 'x', chart) ? zoomPercent : 1,\n      y: pinch.y && directionEnabled(mode, 'y', chart) ? zoomPercent : 1,\n      focalPoint: {\n        x: center.x - rect.left,\n        y: center.y - rect.top\n      }\n    };\n\n    zoom(chart, amount);\n\n    // Keep track of overall scale\n    state.scale = e.scale;\n  }\n}\n\nfunction startPinch(chart, state) {\n  if (state.options.zoom.pinch.enabled) {\n    state.scale = 1;\n  }\n}\n\nfunction endPinch(chart, state, e) {\n  if (state.scale) {\n    handlePinch(chart, state, e);\n    state.scale = null; // reset\n    callback(state.options.zoom.onZoomComplete, [{chart}]);\n  }\n}\n\nfunction handlePan(chart, state, e) {\n  const delta = state.delta;\n  if (delta) {\n    state.panning = true;\n    pan(chart, {x: e.deltaX - delta.x, y: e.deltaY - delta.y}, state.panScales);\n    state.delta = {x: e.deltaX, y: e.deltaY};\n  }\n}\n\nfunction startPan(chart, state, event) {\n  const {enabled, onPanStart, onPanRejected} = state.options.pan;\n  if (!enabled) {\n    return;\n  }\n  const rect = event.target.getBoundingClientRect();\n  const point = {\n    x: event.center.x - rect.left,\n    y: event.center.y - rect.top\n  };\n\n  if (callback(onPanStart, [{chart, event, point}]) === false) {\n    return callback(onPanRejected, [{chart, event}]);\n  }\n\n  state.panScales = getEnabledScalesByPoint(state.options.pan, point, chart);\n  state.delta = {x: 0, y: 0};\n  clearTimeout(state.panEndTimeout);\n  handlePan(chart, state, event);\n}\n\nfunction endPan(chart, state) {\n  state.delta = null;\n  if (state.panning) {\n    state.panEndTimeout = setTimeout(() => (state.panning = false), 500);\n    callback(state.options.pan.onPanComplete, [{chart}]);\n  }\n}\n\nconst hammers = new WeakMap();\nfunction startHammer(chart, options) {\n  const state = getState(chart);\n  const canvas = chart.canvas;\n  const {pan: panOptions, zoom: zoomOptions} = options;\n\n  const mc = new Hammer.Manager(canvas);\n  if (zoomOptions && zoomOptions.pinch.enabled) {\n    mc.add(new Hammer.Pinch());\n    mc.on('pinchstart', () => startPinch(chart, state));\n    mc.on('pinch', (e) => handlePinch(chart, state, e));\n    mc.on('pinchend', (e) => endPinch(chart, state, e));\n  }\n\n  if (panOptions && panOptions.enabled) {\n    mc.add(new Hammer.Pan({\n      threshold: panOptions.threshold,\n      enable: createEnabler(chart, state)\n    }));\n    mc.on('panstart', (e) => startPan(chart, state, e));\n    mc.on('panmove', (e) => handlePan(chart, state, e));\n    mc.on('panend', () => endPan(chart, state));\n  }\n\n  hammers.set(chart, mc);\n}\n\nfunction stopHammer(chart) {\n  const mc = hammers.get(chart);\n  if (mc) {\n    mc.remove('pinchstart');\n    mc.remove('pinch');\n    mc.remove('pinchend');\n    mc.remove('panstart');\n    mc.remove('pan');\n    mc.remove('panend');\n    mc.destroy();\n    hammers.delete(chart);\n  }\n}\n\nvar version = \"2.0.1\";\n\nfunction draw(chart, caller, options) {\n  const dragOptions = options.zoom.drag;\n  const {dragStart, dragEnd} = getState(chart);\n\n  if (dragOptions.drawTime !== caller || !dragEnd) {\n    return;\n  }\n  const {left, top, width, height} = computeDragRect(chart, options.zoom.mode, dragStart, dragEnd);\n  const ctx = chart.ctx;\n\n  ctx.save();\n  ctx.beginPath();\n  ctx.fillStyle = dragOptions.backgroundColor || 'rgba(225,225,225,0.3)';\n  ctx.fillRect(left, top, width, height);\n\n  if (dragOptions.borderWidth > 0) {\n    ctx.lineWidth = dragOptions.borderWidth;\n    ctx.strokeStyle = dragOptions.borderColor || 'rgba(225,225,225)';\n    ctx.strokeRect(left, top, width, height);\n  }\n  ctx.restore();\n}\n\nvar plugin = {\n  id: 'zoom',\n\n  version,\n\n  defaults: {\n    pan: {\n      enabled: false,\n      mode: 'xy',\n      threshold: 10,\n      modifierKey: null,\n    },\n    zoom: {\n      wheel: {\n        enabled: false,\n        speed: 0.1,\n        modifierKey: null\n      },\n      drag: {\n        enabled: false,\n        drawTime: 'beforeDatasetsDraw',\n        modifierKey: null\n      },\n      pinch: {\n        enabled: false\n      },\n      mode: 'xy',\n    }\n  },\n\n  start: function(chart, _args, options) {\n    const state = getState(chart);\n    state.options = options;\n\n    if (Object.prototype.hasOwnProperty.call(options.zoom, 'enabled')) {\n      console.warn('The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`.');\n    }\n    if (Object.prototype.hasOwnProperty.call(options.zoom, 'overScaleMode')\n      || Object.prototype.hasOwnProperty.call(options.pan, 'overScaleMode')) {\n      console.warn('The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired).');\n    }\n\n    if (Hammer) {\n      startHammer(chart, options);\n    }\n\n    chart.pan = (delta, panScales, transition) => pan(chart, delta, panScales, transition);\n    chart.zoom = (args, transition) => zoom(chart, args, transition);\n    chart.zoomRect = (p0, p1, transition) => zoomRect(chart, p0, p1, transition);\n    chart.zoomScale = (id, range, transition) => zoomScale(chart, id, range, transition);\n    chart.resetZoom = (transition) => resetZoom(chart, transition);\n    chart.getZoomLevel = () => getZoomLevel(chart);\n    chart.getInitialScaleBounds = () => getInitialScaleBounds(chart);\n    chart.isZoomedOrPanned = () => isZoomedOrPanned(chart);\n  },\n\n  beforeEvent(chart) {\n    const state = getState(chart);\n    if (state.panning || state.dragging) {\n      // cancel any event handling while panning or dragging\n      return false;\n    }\n  },\n\n  beforeUpdate: function(chart, args, options) {\n    const state = getState(chart);\n    state.options = options;\n    addListeners(chart, options);\n  },\n\n  beforeDatasetsDraw(chart, _args, options) {\n    draw(chart, 'beforeDatasetsDraw', options);\n  },\n\n  afterDatasetsDraw(chart, _args, options) {\n    draw(chart, 'afterDatasetsDraw', options);\n  },\n\n  beforeDraw(chart, _args, options) {\n    draw(chart, 'beforeDraw', options);\n  },\n\n  afterDraw(chart, _args, options) {\n    draw(chart, 'afterDraw', options);\n  },\n\n  stop: function(chart) {\n    removeListeners(chart);\n\n    if (Hammer) {\n      stopHammer(chart);\n    }\n    removeState(chart);\n  },\n\n  panFunctions,\n  zoomFunctions,\n  zoomRectFunctions,\n};\n\nexport { plugin as default, pan, resetZoom, zoom, zoomRect, zoomScale };\n",
         "import type { MouseEvent } from 'react';\nimport type {\n  ChartType,\n  ChartData,\n  DefaultDataPoint,\n  ChartDataset,\n  ChartOptions,\n  Chart,\n} from 'chart.js';\n\nimport type { ForwardedRef } from './types.js';\n\nconst defaultDatasetIdKey = 'label';\n\nexport function reforwardRef<T>(ref: ForwardedRef<T>, value: T) {\n  if (typeof ref === 'function') {\n    ref(value);\n  } else if (ref) {\n    ref.current = value;\n  }\n}\n\nexport function setOptions<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(chart: Chart<TType, TData, TLabel>, nextOptions: ChartOptions<TType>) {\n  const options = chart.options;\n\n  if (options && nextOptions) {\n    Object.assign(options, nextOptions);\n  }\n}\n\nexport function setLabels<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(\n  currentData: ChartData<TType, TData, TLabel>,\n  nextLabels: TLabel[] | undefined\n) {\n  currentData.labels = nextLabels;\n}\n\nexport function setDatasets<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(\n  currentData: ChartData<TType, TData, TLabel>,\n  nextDatasets: ChartDataset<TType, TData>[],\n  datasetIdKey = defaultDatasetIdKey\n) {\n  const addedDatasets: ChartDataset<TType, TData>[] = [];\n\n  currentData.datasets = nextDatasets.map(\n    (nextDataset: Record<string, unknown>) => {\n      // given the new set, find it's current match\n      const currentDataset = currentData.datasets.find(\n        (dataset: Record<string, unknown>) =>\n          dataset[datasetIdKey] === nextDataset[datasetIdKey]\n      );\n\n      // There is no original to update, so simply add new one\n      if (\n        !currentDataset ||\n        !nextDataset.data ||\n        addedDatasets.includes(currentDataset)\n      ) {\n        return { ...nextDataset } as ChartDataset<TType, TData>;\n      }\n\n      addedDatasets.push(currentDataset);\n\n      Object.assign(currentDataset, nextDataset);\n\n      return currentDataset;\n    }\n  );\n}\n\nexport function cloneData<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(data: ChartData<TType, TData, TLabel>, datasetIdKey = defaultDatasetIdKey) {\n  const nextData: ChartData<TType, TData, TLabel> = {\n    labels: [],\n    datasets: [],\n  };\n\n  setLabels(nextData, data.labels);\n  setDatasets(nextData, data.datasets, datasetIdKey);\n\n  return nextData;\n}\n\n/**\n * Get dataset from mouse click event\n * @param chart - Chart.js instance\n * @param event - Mouse click event\n * @returns Dataset\n */\nexport function getDatasetAtEvent(\n  chart: Chart,\n  event: MouseEvent<HTMLCanvasElement>\n) {\n  return chart.getElementsAtEventForMode(\n    event.nativeEvent,\n    'dataset',\n    { intersect: true },\n    false\n  );\n}\n\n/**\n * Get single dataset element from mouse click event\n * @param chart - Chart.js instance\n * @param event - Mouse click event\n * @returns Dataset\n */\nexport function getElementAtEvent(\n  chart: Chart,\n  event: MouseEvent<HTMLCanvasElement>\n) {\n  return chart.getElementsAtEventForMode(\n    event.nativeEvent,\n    'nearest',\n    { intersect: true },\n    false\n  );\n}\n\n/**\n * Get all dataset elements from mouse click event\n * @param chart - Chart.js instance\n * @param event - Mouse click event\n * @returns Dataset\n */\nexport function getElementsAtEvent(\n  chart: Chart,\n  event: MouseEvent<HTMLCanvasElement>\n) {\n  return chart.getElementsAtEventForMode(\n    event.nativeEvent,\n    'index',\n    { intersect: true },\n    false\n  );\n}\n",
         "import React, { useEffect, useRef, forwardRef } from 'react';\nimport { Chart as ChartJS } from 'chart.js';\nimport type { ChartType, DefaultDataPoint } from 'chart.js';\n\nimport type { ForwardedRef, ChartProps, BaseChartComponent } from './types.js';\nimport {\n  reforwardRef,\n  cloneData,\n  setOptions,\n  setLabels,\n  setDatasets,\n} from './utils.js';\n\nfunction ChartComponent<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(\n  props: ChartProps<TType, TData, TLabel>,\n  ref: ForwardedRef<ChartJS<TType, TData, TLabel>>\n) {\n  const {\n    height = 150,\n    width = 300,\n    redraw = false,\n    datasetIdKey,\n    type,\n    data,\n    options,\n    plugins = [],\n    fallbackContent,\n    updateMode,\n    ...canvasProps\n  } = props as ChartProps;\n  const canvasRef = useRef<HTMLCanvasElement>(null);\n  const chartRef = useRef<ChartJS | null>();\n\n  const renderChart = () => {\n    if (!canvasRef.current) return;\n\n    chartRef.current = new ChartJS(canvasRef.current, {\n      type,\n      data: cloneData(data, datasetIdKey),\n      options: options && { ...options },\n      plugins,\n    });\n\n    reforwardRef(ref, chartRef.current);\n  };\n\n  const destroyChart = () => {\n    reforwardRef(ref, null);\n\n    if (chartRef.current) {\n      chartRef.current.destroy();\n      chartRef.current = null;\n    }\n  };\n\n  useEffect(() => {\n    if (!redraw && chartRef.current && options) {\n      setOptions(chartRef.current, options);\n    }\n  }, [redraw, options]);\n\n  useEffect(() => {\n    if (!redraw && chartRef.current) {\n      setLabels(chartRef.current.config.data, data.labels);\n    }\n  }, [redraw, data.labels]);\n\n  useEffect(() => {\n    if (!redraw && chartRef.current && data.datasets) {\n      setDatasets(chartRef.current.config.data, data.datasets, datasetIdKey);\n    }\n  }, [redraw, data.datasets]);\n\n  useEffect(() => {\n    if (!chartRef.current) return;\n\n    if (redraw) {\n      destroyChart();\n      setTimeout(renderChart);\n    } else {\n      chartRef.current.update(updateMode);\n    }\n  }, [redraw, options, data.labels, data.datasets, updateMode]);\n\n  useEffect(() => {\n    if (!chartRef.current) return;\n\n    destroyChart();\n    setTimeout(renderChart);\n  }, [type]);\n\n  useEffect(() => {\n    renderChart();\n\n    return () => destroyChart();\n  }, []);\n\n  return (\n    <canvas\n      ref={canvasRef}\n      role='img'\n      height={height}\n      width={width}\n      {...canvasProps}\n    >\n      {fallbackContent}\n    </canvas>\n  );\n}\n\nexport const Chart = forwardRef(ChartComponent) as BaseChartComponent;\n",
         "import React, { forwardRef } from 'react';\nimport {\n  Chart as ChartJS,\n  LineController,\n  BarController,\n  RadarController,\n  DoughnutController,\n  PolarAreaController,\n  BubbleController,\n  PieController,\n  ScatterController,\n} from 'chart.js';\nimport type { ChartType, ChartComponentLike } from 'chart.js';\n\nimport type {\n  ChartProps,\n  ChartJSOrUndefined,\n  TypedChartComponent,\n} from './types.js';\nimport { Chart } from './chart.js';\n\nfunction createTypedChart<T extends ChartType>(\n  type: T,\n  registerables: ChartComponentLike\n) {\n  ChartJS.register(registerables);\n\n  return forwardRef<ChartJSOrUndefined<T>, Omit<ChartProps<T>, 'type'>>(\n    (props, ref) => <Chart {...props} ref={ref} type={type} />\n  ) as TypedChartComponent<T>;\n}\n\nexport const Line = /* #__PURE__ */ createTypedChart('line', LineController);\n\nexport const Bar = /* #__PURE__ */ createTypedChart('bar', BarController);\n\nexport const Radar = /* #__PURE__ */ createTypedChart('radar', RadarController);\n\nexport const Doughnut = /* #__PURE__ */ createTypedChart(\n  'doughnut',\n  DoughnutController\n);\n\nexport const PolarArea = /* #__PURE__ */ createTypedChart(\n  'polarArea',\n  PolarAreaController\n);\n\nexport const Bubble = /* #__PURE__ */ createTypedChart(\n  'bubble',\n  BubbleController\n);\n\nexport const Pie = /* #__PURE__ */ createTypedChart('pie', PieController);\n\nexport const Scatter = /* #__PURE__ */ createTypedChart(\n  'scatter',\n  ScatterController\n);\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\n////\n//\n// A few enums copied from `fb/Schema.ts` and `fb/Message.ts` because Webpack\n// v4 doesn't seem to be able to tree-shake the rest of those exports.\n//\n// We will have to keep these enums in sync when we re-generate the flatbuffers\n// code from the shchemas. See js/DEVELOP.md for info on how to run flatbuffers\n// code generation.\n//\n////\n\n/**\n * Logical types, vector layouts, and schemas\n *\n * @enum {number}\n */\nexport enum MetadataVersion {\n    /**\n     * 0.1.0 (October 2016).\n     */\n    V1 = 0,\n\n    /**\n     * 0.2.0 (February 2017). Non-backwards compatible with V1.\n     */\n    V2 = 1,\n\n    /**\n     * 0.3.0 -> 0.7.1 (May - December 2017). Non-backwards compatible with V2.\n     */\n    V3 = 2,\n\n    /**\n     * >= 0.8.0 (December 2017). Non-backwards compatible with V3.\n     */\n    V4 = 3,\n\n    /**\n     * >= 1.0.0 (July 2020. Backwards compatible with V4 (V5 readers can read V4\n     * metadata and IPC messages). Implementations are recommended to provide a\n     * V4 compatibility mode with V5 format changes disabled.\n     *\n     * Incompatible changes between V4 and V5:\n     * - Union buffer layout has changed. In V5, Unions don't have a validity\n     *   bitmap buffer.\n     */\n    V5 = 4\n}\n\n/**\n * @enum {number}\n */\nexport enum UnionMode {\n    Sparse = 0,\n    Dense = 1\n}\n\n/**\n * @enum {number}\n */\nexport enum Precision {\n    HALF = 0,\n    SINGLE = 1,\n    DOUBLE = 2\n}\n\n/**\n * @enum {number}\n */\nexport enum DateUnit {\n    DAY = 0,\n    MILLISECOND = 1\n}\n\n/**\n * @enum {number}\n */\nexport enum TimeUnit {\n    SECOND = 0,\n    MILLISECOND = 1,\n    MICROSECOND = 2,\n    NANOSECOND = 3\n}\n\n/**\n * @enum {number}\n */\nexport enum IntervalUnit {\n    YEAR_MONTH = 0,\n    DAY_TIME = 1,\n    MONTH_DAY_NANO = 2\n}\n\n/**\n * ----------------------------------------------------------------------\n * The root Message type\n * This union enables us to easily send different message types without\n * redundant storage, and in the future we can easily add new message types.\n *\n * Arrow implementations do not need to implement all of the message types,\n * which may include experimental metadata types. For maximum compatibility,\n * it is best to send data using RecordBatch\n *\n * @enum {number}\n */\nexport enum MessageHeader {\n    NONE = 0,\n    Schema = 1,\n    DictionaryBatch = 2,\n    RecordBatch = 3,\n    Tensor = 4,\n    SparseTensor = 5\n}\n\n/**\n * Main data type enumeration.\n *\n * Data types in this library are all *logical*. They can be expressed as\n * either a primitive physical type (bytes or bits of some fixed size), a\n * nested type consisting of other data types, or another data type (e.g. a\n * timestamp encoded as an int64).\n *\n * **Note**: Only enum values 0-17 (NONE through Map) are written to an Arrow\n * IPC payload.\n *\n * The rest of the values are specified here so TypeScript can narrow the type\n * signatures further beyond the base Arrow Types. The Arrow DataTypes include\n * metadata like `bitWidth` that impact the type signatures of the values we\n * accept and return.\n *\n * For example, the `Int8Vector` reads 1-byte numbers from an `Int8Array`, an\n * `Int32Vector` reads a 4-byte number from an `Int32Array`, and an `Int64Vector`\n * reads a pair of 4-byte lo, hi 32-bit integers as a zero-copy slice from the\n * underlying `Int32Array`.\n *\n * Library consumers benefit by knowing the narrowest type, since we can ensure\n * the types across all public methods are propagated, and never bail to `any`.\n * These values are _never_ used at runtime, and they will _never_ be written\n * to the flatbuffers metadata of serialized Arrow IPC payloads.\n */\nexport enum Type {\n    NONE = 0, /** The default placeholder type */\n    Null = 1, /** A NULL type having no physical storage */\n    Int = 2, /** Signed or unsigned 8, 16, 32, or 64-bit little-endian integer */\n    Float = 3, /** 2, 4, or 8-byte floating point value */\n    Binary = 4, /** Variable-length bytes (no guarantee of UTF8-ness) */\n    Utf8 = 5, /** UTF8 variable-length string as List<Char> */\n    Bool = 6, /** Boolean as 1 bit, LSB bit-packed ordering */\n    Decimal = 7, /** Precision-and-scale-based decimal type. Storage type depends on the parameters. */\n    Date = 8, /** int32_t days or int64_t milliseconds since the UNIX epoch */\n    Time = 9, /** Time as signed 32 or 64-bit integer, representing either seconds, milliseconds, microseconds, or nanoseconds since midnight since midnight */\n    Timestamp = 10, /** Exact timestamp encoded with int64 since UNIX epoch (Default unit millisecond) */\n    Interval = 11, /** YEAR_MONTH or DAY_TIME interval in SQL style */\n    List = 12, /** A list of some logical data type */\n    Struct = 13, /** Struct of logical types */\n    Union = 14, /** Union of logical types */\n    FixedSizeBinary = 15, /** Fixed-size binary. Each value occupies the same number of bytes */\n    FixedSizeList = 16, /** Fixed-size list. Each value occupies the same number of bytes */\n    Map = 17, /** Map of named logical types */\n\n    Dictionary = -1, /** Dictionary aka Category type */\n    Int8 = -2,\n    Int16 = -3,\n    Int32 = -4,\n    Int64 = -5,\n    Uint8 = -6,\n    Uint16 = -7,\n    Uint32 = -8,\n    Uint64 = -9,\n    Float16 = -10,\n    Float32 = -11,\n    Float64 = -12,\n    DateDay = -13,\n    DateMillisecond = -14,\n    TimestampSecond = -15,\n    TimestampMillisecond = -16,\n    TimestampMicrosecond = -17,\n    TimestampNanosecond = -18,\n    TimeSecond = -19,\n    TimeMillisecond = -20,\n    TimeMicrosecond = -21,\n    TimeNanosecond = -22,\n    DenseUnion = -23,\n    SparseUnion = -24,\n    IntervalDayTime = -25,\n    IntervalYearMonth = -26,\n}\n\nexport enum BufferType {\n    /**\n     * used in List type, Dense Union and variable length primitive types (String, Binary)\n     */\n    OFFSET = 0,\n\n    /**\n     * actual data, either wixed width primitive types in slots or variable width delimited by an OFFSET vector\n     */\n    DATA = 1,\n\n    /**\n     * Bit vector indicating if each value is null\n     */\n    VALIDITY = 2,\n\n    /**\n     * Type vector used in Union type\n     */\n    TYPE = 3\n}\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { ReadableInterop, ArrowJSONLike } from '../io/interfaces.js';\n\n/* eslint-disable unicorn/throw-new-error */\n\n/** @ignore */\ntype FSReadStream = import('fs').ReadStream;\n/** @ignore */\ntype FileHandle = import('fs').promises.FileHandle;\n\n/** @ignore */\nexport interface Subscription {\n    unsubscribe: () => void;\n}\n\n/** @ignore */\nexport interface Observer<T> {\n    closed?: boolean;\n    next: (value: T) => void;\n    error: (err: any) => void;\n    complete: () => void;\n}\n\n/** @ignore */\nexport interface Observable<T> {\n    subscribe: (observer: Observer<T>) => Subscription;\n}\n\n/** @ignore */\nconst [BigIntCtor, BigIntAvailable] = (() => {\n    const BigIntUnavailableError = () => { throw new Error('BigInt is not available in this environment'); };\n    function BigIntUnavailable() { throw BigIntUnavailableError(); }\n    BigIntUnavailable.asIntN = () => { throw BigIntUnavailableError(); };\n    BigIntUnavailable.asUintN = () => { throw BigIntUnavailableError(); };\n    return typeof BigInt !== 'undefined' ? [BigInt, true] : [<any>BigIntUnavailable, false];\n})() as [BigIntConstructor, boolean];\n\n/** @ignore */\nconst [BigInt64ArrayCtor, BigInt64ArrayAvailable] = (() => {\n    const BigInt64ArrayUnavailableError = () => { throw new Error('BigInt64Array is not available in this environment'); };\n    class BigInt64ArrayUnavailable {\n        static get BYTES_PER_ELEMENT() { return 8; }\n        static of() { throw BigInt64ArrayUnavailableError(); }\n        static from() { throw BigInt64ArrayUnavailableError(); }\n        constructor() { throw BigInt64ArrayUnavailableError(); }\n    }\n    return typeof BigInt64Array !== 'undefined' ? [BigInt64Array, true] : [<any>BigInt64ArrayUnavailable, false];\n})() as [BigInt64ArrayConstructor, boolean];\n\n/** @ignore */\nconst [BigUint64ArrayCtor, BigUint64ArrayAvailable] = (() => {\n    const BigUint64ArrayUnavailableError = () => { throw new Error('BigUint64Array is not available in this environment'); };\n    class BigUint64ArrayUnavailable {\n        static get BYTES_PER_ELEMENT() { return 8; }\n        static of() { throw BigUint64ArrayUnavailableError(); }\n        static from() { throw BigUint64ArrayUnavailableError(); }\n        constructor() { throw BigUint64ArrayUnavailableError(); }\n    }\n    return typeof BigUint64Array !== 'undefined' ? [BigUint64Array, true] : [<any>BigUint64ArrayUnavailable, false];\n})() as [BigUint64ArrayConstructor, boolean];\n\nexport { BigIntCtor as BigInt, BigIntAvailable };\nexport { BigInt64ArrayCtor as BigInt64Array, BigInt64ArrayAvailable };\nexport { BigUint64ArrayCtor as BigUint64Array, BigUint64ArrayAvailable };\n\n/** @ignore */ const isNumber = (x: any) => typeof x === 'number';\n/** @ignore */ const isBoolean = (x: any) => typeof x === 'boolean';\n/** @ignore */ const isFunction = (x: any) => typeof x === 'function';\n/** @ignore */\n// eslint-disable-next-line @typescript-eslint/ban-types\nexport const isObject = (x: any): x is Object => x != null && Object(x) === x;\n\n/** @ignore */\nexport const isPromise = <T = any>(x: any): x is PromiseLike<T> => {\n    return isObject(x) && isFunction(x.then);\n};\n\n/** @ignore */\nexport const isObservable = <T = any>(x: any): x is Observable<T> => {\n    return isObject(x) && isFunction(x.subscribe);\n};\n\n/** @ignore */\nexport const isIterable = <T = any>(x: any): x is Iterable<T> => {\n    return isObject(x) && isFunction(x[Symbol.iterator]);\n};\n\n/** @ignore */\nexport const isAsyncIterable = <T = any>(x: any): x is AsyncIterable<T> => {\n    return isObject(x) && isFunction(x[Symbol.asyncIterator]);\n};\n\n/** @ignore */\nexport const isArrowJSON = (x: any): x is ArrowJSONLike => {\n    return isObject(x) && isObject(x['schema']);\n};\n\n/** @ignore */\nexport const isArrayLike = <T = any>(x: any): x is ArrayLike<T> => {\n    return isObject(x) && isNumber(x['length']);\n};\n\n/** @ignore */\nexport const isIteratorResult = <T = any>(x: any): x is IteratorResult<T> => {\n    return isObject(x) && ('done' in x) && ('value' in x);\n};\n\n/** @ignore */\nexport const isUnderlyingSink = <T = any>(x: any): x is UnderlyingSink<T> => {\n    return isObject(x) &&\n        isFunction(x['abort']) &&\n        isFunction(x['close']) &&\n        isFunction(x['start']) &&\n        isFunction(x['write']);\n};\n\n/** @ignore */\nexport const isFileHandle = (x: any): x is FileHandle => {\n    return isObject(x) && isFunction(x['stat']) && isNumber(x['fd']);\n};\n\n/** @ignore */\nexport const isFSReadStream = (x: any): x is FSReadStream => {\n    return isReadableNodeStream(x) && isNumber((<any>x)['bytesRead']);\n};\n\n/** @ignore */\nexport const isFetchResponse = (x: any): x is Response => {\n    return isObject(x) && isReadableDOMStream(x['body']);\n};\n\nconst isReadableInterop = <T = any>(x: any): x is ReadableInterop<T> => ('_getDOMStream' in x && '_getNodeStream' in x);\n\n/** @ignore */\nexport const isWritableDOMStream = <T = any>(x: any): x is WritableStream<T> => {\n    return isObject(x) &&\n        isFunction(x['abort']) &&\n        isFunction(x['getWriter']) &&\n        !isReadableInterop(x);\n};\n\n/** @ignore */\nexport const isReadableDOMStream = <T = any>(x: any): x is ReadableStream<T> => {\n    return isObject(x) &&\n        isFunction(x['cancel']) &&\n        isFunction(x['getReader']) &&\n        !isReadableInterop(x);\n};\n\n/** @ignore */\nexport const isWritableNodeStream = (x: any): x is NodeJS.WritableStream => {\n    return isObject(x) &&\n        isFunction(x['end']) &&\n        isFunction(x['write']) &&\n        isBoolean(x['writable']) &&\n        !isReadableInterop(x);\n};\n\n/** @ignore */\nexport const isReadableNodeStream = (x: any): x is NodeJS.ReadableStream => {\n    return isObject(x) &&\n        isFunction(x['read']) &&\n        isFunction(x['pipe']) &&\n        isBoolean(x['readable']) &&\n        !isReadableInterop(x);\n};\n\n/** @ignore */\nexport const isFlatbuffersByteBuffer = (x: any): x is import('flatbuffers').ByteBuffer => {\n    return isObject(x) &&\n        isFunction(x['clear']) &&\n        isFunction(x['bytes']) &&\n        isFunction(x['position']) &&\n        isFunction(x['setPosition']) &&\n        isFunction(x['capacity']) &&\n        isFunction(x['getBufferIdentifier']) &&\n        isFunction(x['createLong']);\n};\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { BigInt64Array, BigUint64Array } from './compat.js';\n\n/** @ignore */ const undf = void (0);\n\n/** @ignore */\nexport function valueToString(x: any): string {\n    if (x === null) { return 'null'; }\n    if (x === undf) { return 'undefined'; }\n    switch (typeof x) {\n        case 'number': return `${x}`;\n        case 'bigint': return `${x}`;\n        case 'string': return `\"${x}\"`;\n    }\n    // If [Symbol.toPrimitive] is implemented (like in BN)\n    // use it instead of JSON.stringify(). This ensures we\n    // print BigInts, Decimals, and Binary in their native\n    // representation\n    if (typeof x[Symbol.toPrimitive] === 'function') {\n        return x[Symbol.toPrimitive]('string');\n    }\n    if (ArrayBuffer.isView(x)) {\n        if (x instanceof BigInt64Array || x instanceof BigUint64Array) {\n            return `[${[...x].map(x => valueToString(x))}]`;\n        }\n        return `[${x}]`;\n    }\n    return ArrayBuffer.isView(x) ? `[${x}]` : JSON.stringify(x, (_, y) => typeof y === 'bigint' ? `${y}` : y);\n}\n",
         "/******************************************************************************\nCopyright (c) Microsoft Corporation.\n\nPermission to use, copy, modify, and/or distribute this software for any\npurpose with or without fee is hereby granted.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY\nAND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM\nLOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR\nOTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR\nPERFORMANCE OF THIS SOFTWARE.\n***************************************************************************** */\n/* global Reflect, Promise, SuppressedError, Symbol */\n\nvar extendStatics = function(d, b) {\n  extendStatics = Object.setPrototypeOf ||\n      ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\n      function (d, b) { for (var p in b) if (Object.prototype.hasOwnProperty.call(b, p)) d[p] = b[p]; };\n  return extendStatics(d, b);\n};\n\nexport function __extends(d, b) {\n  if (typeof b !== \"function\" && b !== null)\n      throw new TypeError(\"Class extends value \" + String(b) + \" is not a constructor or null\");\n  extendStatics(d, b);\n  function __() { this.constructor = d; }\n  d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\n}\n\nexport var __assign = function() {\n  __assign = Object.assign || function __assign(t) {\n      for (var s, i = 1, n = arguments.length; i < n; i++) {\n          s = arguments[i];\n          for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p)) t[p] = s[p];\n      }\n      return t;\n  }\n  return __assign.apply(this, arguments);\n}\n\nexport function __rest(s, e) {\n  var t = {};\n  for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p) && e.indexOf(p) < 0)\n      t[p] = s[p];\n  if (s != null && typeof Object.getOwnPropertySymbols === \"function\")\n      for (var i = 0, p = Object.getOwnPropertySymbols(s); i < p.length; i++) {\n          if (e.indexOf(p[i]) < 0 && Object.prototype.propertyIsEnumerable.call(s, p[i]))\n              t[p[i]] = s[p[i]];\n      }\n  return t;\n}\n\nexport function __decorate(decorators, target, key, desc) {\n  var c = arguments.length, r = c < 3 ? target : desc === null ? desc = Object.getOwnPropertyDescriptor(target, key) : desc, d;\n  if (typeof Reflect === \"object\" && typeof Reflect.decorate === \"function\") r = Reflect.decorate(decorators, target, key, desc);\n  else for (var i = decorators.length - 1; i >= 0; i--) if (d = decorators[i]) r = (c < 3 ? d(r) : c > 3 ? d(target, key, r) : d(target, key)) || r;\n  return c > 3 && r && Object.defineProperty(target, key, r), r;\n}\n\nexport function __param(paramIndex, decorator) {\n  return function (target, key) { decorator(target, key, paramIndex); }\n}\n\nexport function __esDecorate(ctor, descriptorIn, decorators, contextIn, initializers, extraInitializers) {\n  function accept(f) { if (f !== void 0 && typeof f !== \"function\") throw new TypeError(\"Function expected\"); return f; }\n  var kind = contextIn.kind, key = kind === \"getter\" ? \"get\" : kind === \"setter\" ? \"set\" : \"value\";\n  var target = !descriptorIn && ctor ? contextIn[\"static\"] ? ctor : ctor.prototype : null;\n  var descriptor = descriptorIn || (target ? Object.getOwnPropertyDescriptor(target, contextIn.name) : {});\n  var _, done = false;\n  for (var i = decorators.length - 1; i >= 0; i--) {\n      var context = {};\n      for (var p in contextIn) context[p] = p === \"access\" ? {} : contextIn[p];\n      for (var p in contextIn.access) context.access[p] = contextIn.access[p];\n      context.addInitializer = function (f) { if (done) throw new TypeError(\"Cannot add initializers after decoration has completed\"); extraInitializers.push(accept(f || null)); };\n      var result = (0, decorators[i])(kind === \"accessor\" ? { get: descriptor.get, set: descriptor.set } : descriptor[key], context);\n      if (kind === \"accessor\") {\n          if (result === void 0) continue;\n          if (result === null || typeof result !== \"object\") throw new TypeError(\"Object expected\");\n          if (_ = accept(result.get)) descriptor.get = _;\n          if (_ = accept(result.set)) descriptor.set = _;\n          if (_ = accept(result.init)) initializers.unshift(_);\n      }\n      else if (_ = accept(result)) {\n          if (kind === \"field\") initializers.unshift(_);\n          else descriptor[key] = _;\n      }\n  }\n  if (target) Object.defineProperty(target, contextIn.name, descriptor);\n  done = true;\n};\n\nexport function __runInitializers(thisArg, initializers, value) {\n  var useValue = arguments.length > 2;\n  for (var i = 0; i < initializers.length; i++) {\n      value = useValue ? initializers[i].call(thisArg, value) : initializers[i].call(thisArg);\n  }\n  return useValue ? value : void 0;\n};\n\nexport function __propKey(x) {\n  return typeof x === \"symbol\" ? x : \"\".concat(x);\n};\n\nexport function __setFunctionName(f, name, prefix) {\n  if (typeof name === \"symbol\") name = name.description ? \"[\".concat(name.description, \"]\") : \"\";\n  return Object.defineProperty(f, \"name\", { configurable: true, value: prefix ? \"\".concat(prefix, \" \", name) : name });\n};\n\nexport function __metadata(metadataKey, metadataValue) {\n  if (typeof Reflect === \"object\" && typeof Reflect.metadata === \"function\") return Reflect.metadata(metadataKey, metadataValue);\n}\n\nexport function __awaiter(thisArg, _arguments, P, generator) {\n  function adopt(value) { return value instanceof P ? value : new P(function (resolve) { resolve(value); }); }\n  return new (P || (P = Promise))(function (resolve, reject) {\n      function fulfilled(value) { try { step(generator.next(value)); } catch (e) { reject(e); } }\n      function rejected(value) { try { step(generator[\"throw\"](value)); } catch (e) { reject(e); } }\n      function step(result) { result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected); }\n      step((generator = generator.apply(thisArg, _arguments || [])).next());\n  });\n}\n\nexport function __generator(thisArg, body) {\n  var _ = { label: 0, sent: function() { if (t[0] & 1) throw t[1]; return t[1]; }, trys: [], ops: [] }, f, y, t, g;\n  return g = { next: verb(0), \"throw\": verb(1), \"return\": verb(2) }, typeof Symbol === \"function\" && (g[Symbol.iterator] = function() { return this; }), g;\n  function verb(n) { return function (v) { return step([n, v]); }; }\n  function step(op) {\n      if (f) throw new TypeError(\"Generator is already executing.\");\n      while (g && (g = 0, op[0] && (_ = 0)), _) try {\n          if (f = 1, y && (t = op[0] & 2 ? y[\"return\"] : op[0] ? y[\"throw\"] || ((t = y[\"return\"]) && t.call(y), 0) : y.next) && !(t = t.call(y, op[1])).done) return t;\n          if (y = 0, t) op = [op[0] & 2, t.value];\n          switch (op[0]) {\n              case 0: case 1: t = op; break;\n              case 4: _.label++; return { value: op[1], done: false };\n              case 5: _.label++; y = op[1]; op = [0]; continue;\n              case 7: op = _.ops.pop(); _.trys.pop(); continue;\n              default:\n                  if (!(t = _.trys, t = t.length > 0 && t[t.length - 1]) && (op[0] === 6 || op[0] === 2)) { _ = 0; continue; }\n                  if (op[0] === 3 && (!t || (op[1] > t[0] && op[1] < t[3]))) { _.label = op[1]; break; }\n                  if (op[0] === 6 && _.label < t[1]) { _.label = t[1]; t = op; break; }\n                  if (t && _.label < t[2]) { _.label = t[2]; _.ops.push(op); break; }\n                  if (t[2]) _.ops.pop();\n                  _.trys.pop(); continue;\n          }\n          op = body.call(thisArg, _);\n      } catch (e) { op = [6, e]; y = 0; } finally { f = t = 0; }\n      if (op[0] & 5) throw op[1]; return { value: op[0] ? op[1] : void 0, done: true };\n  }\n}\n\nexport var __createBinding = Object.create ? (function(o, m, k, k2) {\n  if (k2 === undefined) k2 = k;\n  var desc = Object.getOwnPropertyDescriptor(m, k);\n  if (!desc || (\"get\" in desc ? !m.__esModule : desc.writable || desc.configurable)) {\n      desc = { enumerable: true, get: function() { return m[k]; } };\n  }\n  Object.defineProperty(o, k2, desc);\n}) : (function(o, m, k, k2) {\n  if (k2 === undefined) k2 = k;\n  o[k2] = m[k];\n});\n\nexport function __exportStar(m, o) {\n  for (var p in m) if (p !== \"default\" && !Object.prototype.hasOwnProperty.call(o, p)) __createBinding(o, m, p);\n}\n\nexport function __values(o) {\n  var s = typeof Symbol === \"function\" && Symbol.iterator, m = s && o[s], i = 0;\n  if (m) return m.call(o);\n  if (o && typeof o.length === \"number\") return {\n      next: function () {\n          if (o && i >= o.length) o = void 0;\n          return { value: o && o[i++], done: !o };\n      }\n  };\n  throw new TypeError(s ? \"Object is not iterable.\" : \"Symbol.iterator is not defined.\");\n}\n\nexport function __read(o, n) {\n  var m = typeof Symbol === \"function\" && o[Symbol.iterator];\n  if (!m) return o;\n  var i = m.call(o), r, ar = [], e;\n  try {\n      while ((n === void 0 || n-- > 0) && !(r = i.next()).done) ar.push(r.value);\n  }\n  catch (error) { e = { error: error }; }\n  finally {\n      try {\n          if (r && !r.done && (m = i[\"return\"])) m.call(i);\n      }\n      finally { if (e) throw e.error; }\n  }\n  return ar;\n}\n\n/** @deprecated */\nexport function __spread() {\n  for (var ar = [], i = 0; i < arguments.length; i++)\n      ar = ar.concat(__read(arguments[i]));\n  return ar;\n}\n\n/** @deprecated */\nexport function __spreadArrays() {\n  for (var s = 0, i = 0, il = arguments.length; i < il; i++) s += arguments[i].length;\n  for (var r = Array(s), k = 0, i = 0; i < il; i++)\n      for (var a = arguments[i], j = 0, jl = a.length; j < jl; j++, k++)\n          r[k] = a[j];\n  return r;\n}\n\nexport function __spreadArray(to, from, pack) {\n  if (pack || arguments.length === 2) for (var i = 0, l = from.length, ar; i < l; i++) {\n      if (ar || !(i in from)) {\n          if (!ar) ar = Array.prototype.slice.call(from, 0, i);\n          ar[i] = from[i];\n      }\n  }\n  return to.concat(ar || Array.prototype.slice.call(from));\n}\n\nexport function __await(v) {\n  return this instanceof __await ? (this.v = v, this) : new __await(v);\n}\n\nexport function __asyncGenerator(thisArg, _arguments, generator) {\n  if (!Symbol.asyncIterator) throw new TypeError(\"Symbol.asyncIterator is not defined.\");\n  var g = generator.apply(thisArg, _arguments || []), i, q = [];\n  return i = {}, verb(\"next\"), verb(\"throw\"), verb(\"return\"), i[Symbol.asyncIterator] = function () { return this; }, i;\n  function verb(n) { if (g[n]) i[n] = function (v) { return new Promise(function (a, b) { q.push([n, v, a, b]) > 1 || resume(n, v); }); }; }\n  function resume(n, v) { try { step(g[n](v)); } catch (e) { settle(q[0][3], e); } }\n  function step(r) { r.value instanceof __await ? Promise.resolve(r.value.v).then(fulfill, reject) : settle(q[0][2], r); }\n  function fulfill(value) { resume(\"next\", value); }\n  function reject(value) { resume(\"throw\", value); }\n  function settle(f, v) { if (f(v), q.shift(), q.length) resume(q[0][0], q[0][1]); }\n}\n\nexport function __asyncDelegator(o) {\n  var i, p;\n  return i = {}, verb(\"next\"), verb(\"throw\", function (e) { throw e; }), verb(\"return\"), i[Symbol.iterator] = function () { return this; }, i;\n  function verb(n, f) { i[n] = o[n] ? function (v) { return (p = !p) ? { value: __await(o[n](v)), done: false } : f ? f(v) : v; } : f; }\n}\n\nexport function __asyncValues(o) {\n  if (!Symbol.asyncIterator) throw new TypeError(\"Symbol.asyncIterator is not defined.\");\n  var m = o[Symbol.asyncIterator], i;\n  return m ? m.call(o) : (o = typeof __values === \"function\" ? __values(o) : o[Symbol.iterator](), i = {}, verb(\"next\"), verb(\"throw\"), verb(\"return\"), i[Symbol.asyncIterator] = function () { return this; }, i);\n  function verb(n) { i[n] = o[n] && function (v) { return new Promise(function (resolve, reject) { v = o[n](v), settle(resolve, reject, v.done, v.value); }); }; }\n  function settle(resolve, reject, d, v) { Promise.resolve(v).then(function(v) { resolve({ value: v, done: d }); }, reject); }\n}\n\nexport function __makeTemplateObject(cooked, raw) {\n  if (Object.defineProperty) { Object.defineProperty(cooked, \"raw\", { value: raw }); } else { cooked.raw = raw; }\n  return cooked;\n};\n\nvar __setModuleDefault = Object.create ? (function(o, v) {\n  Object.defineProperty(o, \"default\", { enumerable: true, value: v });\n}) : function(o, v) {\n  o[\"default\"] = v;\n};\n\nexport function __importStar(mod) {\n  if (mod && mod.__esModule) return mod;\n  var result = {};\n  if (mod != null) for (var k in mod) if (k !== \"default\" && Object.prototype.hasOwnProperty.call(mod, k)) __createBinding(result, mod, k);\n  __setModuleDefault(result, mod);\n  return result;\n}\n\nexport function __importDefault(mod) {\n  return (mod && mod.__esModule) ? mod : { default: mod };\n}\n\nexport function __classPrivateFieldGet(receiver, state, kind, f) {\n  if (kind === \"a\" && !f) throw new TypeError(\"Private accessor was defined without a getter\");\n  if (typeof state === \"function\" ? receiver !== state || !f : !state.has(receiver)) throw new TypeError(\"Cannot read private member from an object whose class did not declare it\");\n  return kind === \"m\" ? f : kind === \"a\" ? f.call(receiver) : f ? f.value : state.get(receiver);\n}\n\nexport function __classPrivateFieldSet(receiver, state, value, kind, f) {\n  if (kind === \"m\") throw new TypeError(\"Private method is not writable\");\n  if (kind === \"a\" && !f) throw new TypeError(\"Private accessor was defined without a setter\");\n  if (typeof state === \"function\" ? receiver !== state || !f : !state.has(receiver)) throw new TypeError(\"Cannot write private member to an object whose class did not declare it\");\n  return (kind === \"a\" ? f.call(receiver, value) : f ? f.value = value : state.set(receiver, value)), value;\n}\n\nexport function __classPrivateFieldIn(state, receiver) {\n  if (receiver === null || (typeof receiver !== \"object\" && typeof receiver !== \"function\")) throw new TypeError(\"Cannot use 'in' operator on non-object\");\n  return typeof state === \"function\" ? receiver === state : state.has(receiver);\n}\n\nexport function __addDisposableResource(env, value, async) {\n  if (value !== null && value !== void 0) {\n    if (typeof value !== \"object\" && typeof value !== \"function\") throw new TypeError(\"Object expected.\");\n    var dispose;\n    if (async) {\n        if (!Symbol.asyncDispose) throw new TypeError(\"Symbol.asyncDispose is not defined.\");\n        dispose = value[Symbol.asyncDispose];\n    }\n    if (dispose === void 0) {\n        if (!Symbol.dispose) throw new TypeError(\"Symbol.dispose is not defined.\");\n        dispose = value[Symbol.dispose];\n    }\n    if (typeof dispose !== \"function\") throw new TypeError(\"Object not disposable.\");\n    env.stack.push({ value: value, dispose: dispose, async: async });\n  }\n  else if (async) {\n    env.stack.push({ async: true });\n  }\n  return value;\n}\n\nvar _SuppressedError = typeof SuppressedError === \"function\" ? SuppressedError : function (error, suppressed, message) {\n  var e = new Error(message);\n  return e.name = \"SuppressedError\", e.error = error, e.suppressed = suppressed, e;\n};\n\nexport function __disposeResources(env) {\n  function fail(e) {\n    env.error = env.hasError ? new _SuppressedError(e, env.error, \"An error was suppressed during disposal.\") : e;\n    env.hasError = true;\n  }\n  function next() {\n    while (env.stack.length) {\n      var rec = env.stack.pop();\n      try {\n        var result = rec.dispose && rec.dispose.call(rec.value);\n        if (rec.async) return Promise.resolve(result).then(next, function(e) { fail(e); return next(); });\n      }\n      catch (e) {\n          fail(e);\n      }\n    }\n    if (env.hasError) throw env.error;\n  }\n  return next();\n}\n\nexport default {\n  __extends,\n  __assign,\n  __rest,\n  __decorate,\n  __param,\n  __metadata,\n  __awaiter,\n  __generator,\n  __createBinding,\n  __exportStar,\n  __values,\n  __read,\n  __spread,\n  __spreadArrays,\n  __spreadArray,\n  __await,\n  __asyncGenerator,\n  __asyncDelegator,\n  __asyncValues,\n  __makeTemplateObject,\n  __importStar,\n  __importDefault,\n  __classPrivateFieldGet,\n  __classPrivateFieldSet,\n  __classPrivateFieldIn,\n  __addDisposableResource,\n  __disposeResources,\n};\n",
@@ -6079,13 +6087,14 @@
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { makeData } from '../data.js';\nimport { Vector } from '../vector.js';\nimport { DataType, Struct, TypeMap } from '../type.js';\nimport { MessageHeader } from '../enum.js';\nimport { Footer } from './metadata/file.js';\nimport { Schema, Field } from '../schema.js';\nimport streamAdapters from '../io/adapters.js';\nimport { Message } from './metadata/message.js';\nimport * as metadata from './metadata/message.js';\nimport { ArrayBufferViewInput } from '../util/buffer.js';\nimport { ByteStream, AsyncByteStream } from '../io/stream.js';\nimport { RandomAccessFile, AsyncRandomAccessFile } from '../io/file.js';\nimport { VectorLoader, JSONVectorLoader } from '../visitor/vectorloader.js';\nimport { RecordBatch, _InternalEmptyPlaceholderRecordBatch } from '../recordbatch.js';\nimport {\n    FileHandle,\n    ArrowJSONLike,\n    ITERATOR_DONE,\n    ReadableInterop,\n} from '../io/interfaces.js';\nimport {\n    MessageReader, AsyncMessageReader, JSONMessageReader,\n    checkForMagicArrowString, magicLength, magicAndPadding, magicX2AndPadding\n} from './message.js';\nimport {\n    isPromise,\n    isIterable, isAsyncIterable,\n    isIteratorResult, isArrowJSON,\n    isFileHandle, isFetchResponse,\n    isReadableDOMStream, isReadableNodeStream\n} from '../util/compat.js';\n\n/** @ignore */ export type FromArg0 = ArrowJSONLike;\n/** @ignore */ export type FromArg1 = PromiseLike<ArrowJSONLike>;\n/** @ignore */ export type FromArg2 = Iterable<ArrayBufferViewInput> | ArrayBufferViewInput;\n/** @ignore */ export type FromArg3 = PromiseLike<Iterable<ArrayBufferViewInput> | ArrayBufferViewInput>;\n/** @ignore */ export type FromArg4 = Response | NodeJS.ReadableStream | ReadableStream<ArrayBufferViewInput> | AsyncIterable<ArrayBufferViewInput>;\n/** @ignore */ export type FromArg5 = FileHandle | PromiseLike<FileHandle> | PromiseLike<FromArg4>;\n/** @ignore */ export type FromArgs = FromArg0 | FromArg1 | FromArg2 | FromArg3 | FromArg4 | FromArg5;\n\n/** @ignore */ type OpenOptions = { autoDestroy?: boolean };\n/** @ignore */ type RecordBatchReaders<T extends TypeMap = any> = RecordBatchFileReader<T> | RecordBatchStreamReader<T>;\n/** @ignore */ type AsyncRecordBatchReaders<T extends TypeMap = any> = AsyncRecordBatchFileReader<T> | AsyncRecordBatchStreamReader<T>;\n/** @ignore */ type RecordBatchFileReaders<T extends TypeMap = any> = RecordBatchFileReader<T> | AsyncRecordBatchFileReader<T>;\n/** @ignore */ type RecordBatchStreamReaders<T extends TypeMap = any> = RecordBatchStreamReader<T> | AsyncRecordBatchStreamReader<T>;\n\nexport class RecordBatchReader<T extends TypeMap = any> extends ReadableInterop<RecordBatch<T>> {\n\n    protected _impl: RecordBatchReaderImpls<T>;\n    protected constructor(impl: RecordBatchReaderImpls<T>) {\n        super();\n        this._impl = impl;\n    }\n\n    public get closed() { return this._impl.closed; }\n    public get schema() { return this._impl.schema; }\n    public get autoDestroy() { return this._impl.autoDestroy; }\n    public get dictionaries() { return this._impl.dictionaries; }\n    public get numDictionaries() { return this._impl.numDictionaries; }\n    public get numRecordBatches() { return this._impl.numRecordBatches; }\n    public get footer(): Footer | null { return this._impl.isFile() ? this._impl.footer : null; }\n\n    public isSync(): this is RecordBatchReaders<T> { return this._impl.isSync(); }\n    public isAsync(): this is AsyncRecordBatchReaders<T> { return this._impl.isAsync(); }\n    public isFile(): this is RecordBatchFileReaders<T> { return this._impl.isFile(); }\n    public isStream(): this is RecordBatchStreamReaders<T> { return this._impl.isStream(); }\n\n    public next() {\n        return this._impl.next();\n    }\n    public throw(value?: any) {\n        return this._impl.throw(value);\n    }\n    public return(value?: any) {\n        return this._impl.return(value);\n    }\n    public cancel() {\n        return this._impl.cancel();\n    }\n    public reset(schema?: Schema<T> | null): this {\n        this._impl.reset(schema);\n        this._DOMStream = undefined;\n        this._nodeStream = undefined;\n        return this;\n    }\n    public open(options?: OpenOptions) {\n        const opening = this._impl.open(options);\n        return isPromise(opening) ? opening.then(() => this) : this;\n    }\n    public readRecordBatch(index: number): RecordBatch<T> | null | Promise<RecordBatch<T> | null> {\n        return this._impl.isFile() ? this._impl.readRecordBatch(index) : null;\n    }\n    public [Symbol.iterator](): IterableIterator<RecordBatch<T>> {\n        return (<IterableIterator<RecordBatch<T>>>this._impl)[Symbol.iterator]();\n    }\n    public [Symbol.asyncIterator](): AsyncIterableIterator<RecordBatch<T>> {\n        return (<AsyncIterableIterator<RecordBatch<T>>>this._impl)[Symbol.asyncIterator]();\n    }\n    public toDOMStream() {\n        return streamAdapters.toDOMStream<RecordBatch<T>>(\n            (this.isSync()\n                ? { [Symbol.iterator]: () => this } as Iterable<RecordBatch<T>>\n                : { [Symbol.asyncIterator]: () => this } as AsyncIterable<RecordBatch<T>>));\n    }\n    public toNodeStream() {\n        return streamAdapters.toNodeStream<RecordBatch<T>>(\n            (this.isSync()\n                ? { [Symbol.iterator]: () => this } as Iterable<RecordBatch<T>>\n                : { [Symbol.asyncIterator]: () => this } as AsyncIterable<RecordBatch<T>>),\n            { objectMode: true });\n    }\n\n    /** @nocollapse */\n    // @ts-ignore\n    public static throughNode(options?: import('stream').DuplexOptions & { autoDestroy: boolean }): import('stream').Duplex {\n        throw new Error(`\"throughNode\" not available in this environment`);\n    }\n    /** @nocollapse */\n    public static throughDOM<T extends TypeMap>(\n        // @ts-ignore\n        writableStrategy?: ByteLengthQueuingStrategy,\n        // @ts-ignore\n        readableStrategy?: { autoDestroy: boolean }\n    ): { writable: WritableStream<Uint8Array>; readable: ReadableStream<RecordBatch<T>> } {\n        throw new Error(`\"throughDOM\" not available in this environment`);\n    }\n\n    public static from<T extends RecordBatchReader>(source: T): T;\n    public static from<T extends TypeMap = any>(source: FromArg0): RecordBatchStreamReader<T>;\n    public static from<T extends TypeMap = any>(source: FromArg1): Promise<RecordBatchStreamReader<T>>;\n    public static from<T extends TypeMap = any>(source: FromArg2): RecordBatchFileReader<T> | RecordBatchStreamReader<T>;\n    public static from<T extends TypeMap = any>(source: FromArg3): Promise<RecordBatchFileReader<T> | RecordBatchStreamReader<T>>;\n    public static from<T extends TypeMap = any>(source: FromArg4): Promise<AsyncRecordBatchFileReader<T> | AsyncRecordBatchStreamReader<T>>;\n    public static from<T extends TypeMap = any>(source: FromArg5): Promise<AsyncRecordBatchFileReader<T> | AsyncRecordBatchStreamReader<T>>;\n    /** @nocollapse */\n    public static from<T extends TypeMap = any>(source: any) {\n        if (source instanceof RecordBatchReader) {\n            return source;\n        } else if (isArrowJSON(source)) {\n            return fromArrowJSON<T>(source);\n        } else if (isFileHandle(source)) {\n            return fromFileHandle<T>(source);\n        } else if (isPromise<any>(source)) {\n            return (async () => await RecordBatchReader.from<any>(await source))();\n        } else if (isFetchResponse(source) || isReadableDOMStream(source) || isReadableNodeStream(source) || isAsyncIterable(source)) {\n            return fromAsyncByteStream<T>(new AsyncByteStream(source));\n        }\n        return fromByteStream<T>(new ByteStream(source));\n    }\n\n    public static readAll<T extends RecordBatchReader>(source: T): T extends RecordBatchReaders ? IterableIterator<T> : AsyncIterableIterator<T>;\n    public static readAll<T extends TypeMap = any>(source: FromArg0): IterableIterator<RecordBatchStreamReader<T>>;\n    public static readAll<T extends TypeMap = any>(source: FromArg1): AsyncIterableIterator<RecordBatchStreamReader<T>>;\n    public static readAll<T extends TypeMap = any>(source: FromArg2): IterableIterator<RecordBatchFileReader<T> | RecordBatchStreamReader<T>>;\n    public static readAll<T extends TypeMap = any>(source: FromArg3): AsyncIterableIterator<RecordBatchFileReader<T> | RecordBatchStreamReader<T>>;\n    public static readAll<T extends TypeMap = any>(source: FromArg4): AsyncIterableIterator<AsyncRecordBatchReaders<T>>;\n    public static readAll<T extends TypeMap = any>(source: FromArg5): AsyncIterableIterator<AsyncRecordBatchReaders<T>>;\n    /** @nocollapse */\n    public static readAll<T extends TypeMap = any>(source: any) {\n        if (source instanceof RecordBatchReader) {\n            return source.isSync() ? readAllSync(source) : readAllAsync(source as AsyncRecordBatchReaders<T>);\n        } else if (isArrowJSON(source) || ArrayBuffer.isView(source) || isIterable<ArrayBufferViewInput>(source) || isIteratorResult(source)) {\n            return readAllSync<T>(source) as IterableIterator<RecordBatchReaders<T>>;\n        }\n        return readAllAsync<T>(source) as AsyncIterableIterator<RecordBatchReaders<T> | AsyncRecordBatchReaders<T>>;\n    }\n}\n\n//\n// Since TS is a structural type system, we define the following subclass stubs\n// so that concrete types exist to associate with with the interfaces below.\n//\n// The implementation for each RecordBatchReader is hidden away in the set of\n// `RecordBatchReaderImpl` classes in the second half of this file. This allows\n// us to export a single RecordBatchReader class, and swap out the impl based\n// on the io primitives or underlying arrow (JSON, file, or stream) at runtime.\n//\n// Async/await makes our job a bit harder, since it forces everything to be\n// either fully sync or fully async. This is why the logic for the reader impls\n// has been duplicated into both sync and async variants. Since the RBR\n// delegates to its impl, an RBR with an AsyncRecordBatchFileReaderImpl for\n// example will return async/await-friendly Promises, but one with a (sync)\n// RecordBatchStreamReaderImpl will always return values. Nothing should be\n// different about their logic, aside from the async handling. This is also why\n// this code looks highly structured, as it should be nearly identical and easy\n// to follow.\n//\n\n/** @ignore */\nexport class RecordBatchStreamReader<T extends TypeMap = any> extends RecordBatchReader<T> {\n    constructor(protected _impl: RecordBatchStreamReaderImpl<T>) { super(_impl); }\n    public readAll() { return [...this]; }\n    public [Symbol.iterator]() { return (this._impl as IterableIterator<RecordBatch<T>>)[Symbol.iterator](); }\n    public async *[Symbol.asyncIterator](): AsyncIterableIterator<RecordBatch<T>> { yield* this[Symbol.iterator](); }\n}\n/** @ignore */\nexport class AsyncRecordBatchStreamReader<T extends TypeMap = any> extends RecordBatchReader<T> {\n    constructor(protected _impl: AsyncRecordBatchStreamReaderImpl<T>) { super(_impl); }\n    public async readAll() {\n        const batches = new Array<RecordBatch<T>>();\n        for await (const batch of this) { batches.push(batch); }\n        return batches;\n    }\n    public [Symbol.iterator](): IterableIterator<RecordBatch<T>> { throw new Error(`AsyncRecordBatchStreamReader is not Iterable`); }\n    public [Symbol.asyncIterator]() { return (this._impl as AsyncIterableIterator<RecordBatch<T>>)[Symbol.asyncIterator](); }\n}\n/** @ignore */\nexport class RecordBatchFileReader<T extends TypeMap = any> extends RecordBatchStreamReader<T> {\n    constructor(protected _impl: RecordBatchFileReaderImpl<T>) { super(_impl); }\n}\n/** @ignore */\nexport class AsyncRecordBatchFileReader<T extends TypeMap = any> extends AsyncRecordBatchStreamReader<T> {\n    constructor(protected _impl: AsyncRecordBatchFileReaderImpl<T>) { super(_impl); }\n}\n\n//\n// Now override the return types for each sync/async RecordBatchReader variant\n//\n\n/** @ignore */\nexport interface RecordBatchStreamReader<T extends TypeMap = any> extends RecordBatchReader<T> {\n    open(options?: OpenOptions | undefined): this;\n    cancel(): void;\n    throw(value?: any): IteratorResult<any>;\n    return(value?: any): IteratorResult<any>;\n    next(value?: any): IteratorResult<RecordBatch<T>>;\n}\n\n/** @ignore */\nexport interface AsyncRecordBatchStreamReader<T extends TypeMap = any> extends RecordBatchReader<T> {\n    open(options?: OpenOptions | undefined): Promise<this>;\n    cancel(): Promise<void>;\n    throw(value?: any): Promise<IteratorResult<any>>;\n    return(value?: any): Promise<IteratorResult<any>>;\n    next(value?: any): Promise<IteratorResult<RecordBatch<T>>>;\n}\n\n/** @ignore */\nexport interface RecordBatchFileReader<T extends TypeMap = any> extends RecordBatchStreamReader<T> {\n    readRecordBatch(index: number): RecordBatch<T> | null;\n}\n\n/** @ignore */\nexport interface AsyncRecordBatchFileReader<T extends TypeMap = any> extends AsyncRecordBatchStreamReader<T> {\n    readRecordBatch(index: number): Promise<RecordBatch<T> | null>;\n}\n\n/** @ignore */\ntype RecordBatchReaderImpls<T extends TypeMap = any> =\n    RecordBatchJSONReaderImpl<T> |\n    RecordBatchFileReaderImpl<T> |\n    RecordBatchStreamReaderImpl<T> |\n    AsyncRecordBatchFileReaderImpl<T> |\n    AsyncRecordBatchStreamReaderImpl<T>;\n\n/** @ignore */\ninterface RecordBatchReaderImpl<T extends TypeMap = any> {\n\n    closed: boolean;\n    schema: Schema<T>;\n    autoDestroy: boolean;\n    dictionaries: Map<number, Vector>;\n\n    isFile(): this is RecordBatchFileReaders<T>;\n    isStream(): this is RecordBatchStreamReaders<T>;\n    isSync(): this is RecordBatchReaders<T>;\n    isAsync(): this is AsyncRecordBatchReaders<T>;\n\n    reset(schema?: Schema<T> | null): this;\n}\n\n/** @ignore */\ninterface RecordBatchStreamReaderImpl<T extends TypeMap = any> extends RecordBatchReaderImpl<T> {\n\n    open(options?: OpenOptions): this;\n    cancel(): void;\n\n    throw(value?: any): IteratorResult<any>;\n    return(value?: any): IteratorResult<any>;\n    next(value?: any): IteratorResult<RecordBatch<T>>;\n\n    [Symbol.iterator](): IterableIterator<RecordBatch<T>>;\n}\n\n/** @ignore */\ninterface AsyncRecordBatchStreamReaderImpl<T extends TypeMap = any> extends RecordBatchReaderImpl<T> {\n\n    open(options?: OpenOptions): Promise<this>;\n    cancel(): Promise<void>;\n\n    throw(value?: any): Promise<IteratorResult<any>>;\n    return(value?: any): Promise<IteratorResult<any>>;\n    next(value?: any): Promise<IteratorResult<RecordBatch<T>>>;\n\n    [Symbol.asyncIterator](): AsyncIterableIterator<RecordBatch<T>>;\n}\n\n/** @ignore */\ninterface RecordBatchFileReaderImpl<T extends TypeMap = any> extends RecordBatchStreamReaderImpl<T> {\n    readRecordBatch(index: number): RecordBatch<T> | null;\n}\n\n/** @ignore */\ninterface AsyncRecordBatchFileReaderImpl<T extends TypeMap = any> extends AsyncRecordBatchStreamReaderImpl<T> {\n    readRecordBatch(index: number): Promise<RecordBatch<T> | null>;\n}\n\n/** @ignore */\nabstract class RecordBatchReaderImpl<T extends TypeMap = any> implements RecordBatchReaderImpl<T> {\n\n    declare public schema: Schema<T>;\n    public closed = false;\n    public autoDestroy = true;\n    public dictionaries: Map<number, Vector>;\n\n    protected _dictionaryIndex = 0;\n    protected _recordBatchIndex = 0;\n    public get numDictionaries() { return this._dictionaryIndex; }\n    public get numRecordBatches() { return this._recordBatchIndex; }\n\n    constructor(dictionaries = new Map<number, Vector>()) {\n        this.dictionaries = dictionaries;\n    }\n\n    public isSync(): this is RecordBatchReaders<T> { return false; }\n    public isAsync(): this is AsyncRecordBatchReaders<T> { return false; }\n    public isFile(): this is RecordBatchFileReaders<T> { return false; }\n    public isStream(): this is RecordBatchStreamReaders<T> { return false; }\n\n    public reset(schema?: Schema<T> | null) {\n        this._dictionaryIndex = 0;\n        this._recordBatchIndex = 0;\n        this.schema = <any>schema;\n        this.dictionaries = new Map();\n        return this;\n    }\n\n    protected _loadRecordBatch(header: metadata.RecordBatch, body: any) {\n        const children = this._loadVectors(header, body, this.schema.fields);\n        const data = makeData({ type: new Struct(this.schema.fields), length: header.length, children });\n        return new RecordBatch(this.schema, data);\n    }\n    protected _loadDictionaryBatch(header: metadata.DictionaryBatch, body: any) {\n        const { id, isDelta } = header;\n        const { dictionaries, schema } = this;\n        const dictionary = dictionaries.get(id);\n        if (isDelta || !dictionary) {\n            const type = schema.dictionaries.get(id)!;\n            const data = this._loadVectors(header.data, body, [type]);\n            return (dictionary && isDelta ? dictionary.concat(\n                new Vector(data)) :\n                new Vector(data)).memoize() as Vector;\n        }\n        return dictionary.memoize();\n    }\n    protected _loadVectors(header: metadata.RecordBatch, body: any, types: (Field | DataType)[]) {\n        return new VectorLoader(body, header.nodes, header.buffers, this.dictionaries).visitMany(types);\n    }\n}\n\n/** @ignore */\nclass RecordBatchStreamReaderImpl<T extends TypeMap = any> extends RecordBatchReaderImpl<T> implements IterableIterator<RecordBatch<T>> {\n\n    protected _reader: MessageReader;\n    protected _handle: ByteStream | ArrowJSONLike;\n\n    constructor(source: ByteStream | ArrowJSONLike, dictionaries?: Map<number, Vector>) {\n        super(dictionaries);\n        this._reader = !isArrowJSON(source)\n            ? new MessageReader(this._handle = source)\n            : new JSONMessageReader(this._handle = source);\n    }\n\n    public isSync(): this is RecordBatchReaders<T> { return true; }\n    public isStream(): this is RecordBatchStreamReaders<T> { return true; }\n    public [Symbol.iterator](): IterableIterator<RecordBatch<T>> {\n        return this as IterableIterator<RecordBatch<T>>;\n    }\n    public cancel() {\n        if (!this.closed && (this.closed = true)) {\n            this.reset()._reader.return();\n            this._reader = <any>null;\n            this.dictionaries = <any>null;\n        }\n    }\n    public open(options?: OpenOptions) {\n        if (!this.closed) {\n            this.autoDestroy = shouldAutoDestroy(this, options);\n            if (!(this.schema || (this.schema = this._reader.readSchema()!))) {\n                this.cancel();\n            }\n        }\n        return this;\n    }\n    public throw(value?: any): IteratorResult<any> {\n        if (!this.closed && this.autoDestroy && (this.closed = true)) {\n            return this.reset()._reader.throw(value);\n        }\n        return ITERATOR_DONE;\n    }\n    public return(value?: any): IteratorResult<any> {\n        if (!this.closed && this.autoDestroy && (this.closed = true)) {\n            return this.reset()._reader.return(value);\n        }\n        return ITERATOR_DONE;\n    }\n    public next(): IteratorResult<RecordBatch<T>> {\n        if (this.closed) { return ITERATOR_DONE; }\n        let message: Message | null;\n        const { _reader: reader } = this;\n        while (message = this._readNextMessageAndValidate()) {\n            if (message.isSchema()) {\n                this.reset(message.header());\n            } else if (message.isRecordBatch()) {\n                this._recordBatchIndex++;\n                const header = message.header();\n                const buffer = reader.readMessageBody(message.bodyLength);\n                const recordBatch = this._loadRecordBatch(header, buffer);\n                return { done: false, value: recordBatch };\n            } else if (message.isDictionaryBatch()) {\n                this._dictionaryIndex++;\n                const header = message.header();\n                const buffer = reader.readMessageBody(message.bodyLength);\n                const vector = this._loadDictionaryBatch(header, buffer);\n                this.dictionaries.set(header.id, vector);\n            }\n        }\n        if (this.schema && this._recordBatchIndex === 0) {\n            this._recordBatchIndex++;\n            return { done: false, value: new _InternalEmptyPlaceholderRecordBatch<T>(this.schema) };\n        }\n        return this.return();\n    }\n    protected _readNextMessageAndValidate<T extends MessageHeader>(type?: T | null) {\n        return this._reader.readMessage<T>(type);\n    }\n}\n\n/** @ignore */\nclass AsyncRecordBatchStreamReaderImpl<T extends TypeMap = any> extends RecordBatchReaderImpl<T> implements AsyncIterableIterator<RecordBatch<T>> {\n\n    protected _handle: AsyncByteStream;\n    protected _reader: AsyncMessageReader;\n\n    constructor(source: AsyncByteStream, dictionaries?: Map<number, Vector>) {\n        super(dictionaries);\n        this._reader = new AsyncMessageReader(this._handle = source);\n    }\n    public isAsync(): this is AsyncRecordBatchReaders<T> { return true; }\n    public isStream(): this is RecordBatchStreamReaders<T> { return true; }\n    public [Symbol.asyncIterator](): AsyncIterableIterator<RecordBatch<T>> {\n        return this as AsyncIterableIterator<RecordBatch<T>>;\n    }\n    public async cancel() {\n        if (!this.closed && (this.closed = true)) {\n            await this.reset()._reader.return();\n            this._reader = <any>null;\n            this.dictionaries = <any>null;\n        }\n    }\n    public async open(options?: OpenOptions) {\n        if (!this.closed) {\n            this.autoDestroy = shouldAutoDestroy(this, options);\n            if (!(this.schema || (this.schema = (await this._reader.readSchema())!))) {\n                await this.cancel();\n            }\n        }\n        return this;\n    }\n    public async throw(value?: any): Promise<IteratorResult<any>> {\n        if (!this.closed && this.autoDestroy && (this.closed = true)) {\n            return await this.reset()._reader.throw(value);\n        }\n        return ITERATOR_DONE;\n    }\n    public async return(value?: any): Promise<IteratorResult<any>> {\n        if (!this.closed && this.autoDestroy && (this.closed = true)) {\n            return await this.reset()._reader.return(value);\n        }\n        return ITERATOR_DONE;\n    }\n    public async next() {\n        if (this.closed) { return ITERATOR_DONE; }\n        let message: Message | null;\n        const { _reader: reader } = this;\n        while (message = await this._readNextMessageAndValidate()) {\n            if (message.isSchema()) {\n                await this.reset(message.header());\n            } else if (message.isRecordBatch()) {\n                this._recordBatchIndex++;\n                const header = message.header();\n                const buffer = await reader.readMessageBody(message.bodyLength);\n                const recordBatch = this._loadRecordBatch(header, buffer);\n                return { done: false, value: recordBatch };\n            } else if (message.isDictionaryBatch()) {\n                this._dictionaryIndex++;\n                const header = message.header();\n                const buffer = await reader.readMessageBody(message.bodyLength);\n                const vector = this._loadDictionaryBatch(header, buffer);\n                this.dictionaries.set(header.id, vector);\n            }\n        }\n        if (this.schema && this._recordBatchIndex === 0) {\n            this._recordBatchIndex++;\n            return { done: false, value: new _InternalEmptyPlaceholderRecordBatch<T>(this.schema) };\n        }\n        return await this.return();\n    }\n    protected async _readNextMessageAndValidate<T extends MessageHeader>(type?: T | null) {\n        return await this._reader.readMessage<T>(type);\n    }\n}\n\n/** @ignore */\nclass RecordBatchFileReaderImpl<T extends TypeMap = any> extends RecordBatchStreamReaderImpl<T> {\n\n    protected _footer?: Footer;\n    declare protected _handle: RandomAccessFile;\n    public get footer() { return this._footer!; }\n    public get numDictionaries() { return this._footer ? this._footer.numDictionaries : 0; }\n    public get numRecordBatches() { return this._footer ? this._footer.numRecordBatches : 0; }\n\n    constructor(source: RandomAccessFile | ArrayBufferViewInput, dictionaries?: Map<number, Vector>) {\n        super(source instanceof RandomAccessFile ? source : new RandomAccessFile(source), dictionaries);\n    }\n    public isSync(): this is RecordBatchReaders<T> { return true; }\n    public isFile(): this is RecordBatchFileReaders<T> { return true; }\n    public open(options?: OpenOptions) {\n        if (!this.closed && !this._footer) {\n            this.schema = (this._footer = this._readFooter()).schema;\n            for (const block of this._footer.dictionaryBatches()) {\n                block && this._readDictionaryBatch(this._dictionaryIndex++);\n            }\n        }\n        return super.open(options);\n    }\n    public readRecordBatch(index: number) {\n        if (this.closed) { return null; }\n        if (!this._footer) { this.open(); }\n        const block = this._footer?.getRecordBatch(index);\n        if (block && this._handle.seek(block.offset)) {\n            const message = this._reader.readMessage(MessageHeader.RecordBatch);\n            if (message?.isRecordBatch()) {\n                const header = message.header();\n                const buffer = this._reader.readMessageBody(message.bodyLength);\n                const recordBatch = this._loadRecordBatch(header, buffer);\n                return recordBatch;\n            }\n        }\n        return null;\n    }\n    protected _readDictionaryBatch(index: number) {\n        const block = this._footer?.getDictionaryBatch(index);\n        if (block && this._handle.seek(block.offset)) {\n            const message = this._reader.readMessage(MessageHeader.DictionaryBatch);\n            if (message?.isDictionaryBatch()) {\n                const header = message.header();\n                const buffer = this._reader.readMessageBody(message.bodyLength);\n                const vector = this._loadDictionaryBatch(header, buffer);\n                this.dictionaries.set(header.id, vector);\n            }\n        }\n    }\n    protected _readFooter() {\n        const { _handle } = this;\n        const offset = _handle.size - magicAndPadding;\n        const length = _handle.readInt32(offset);\n        const buffer = _handle.readAt(offset - length, length);\n        return Footer.decode(buffer);\n    }\n    protected _readNextMessageAndValidate<T extends MessageHeader>(type?: T | null): Message<T> | null {\n        if (!this._footer) { this.open(); }\n        if (this._footer && this._recordBatchIndex < this.numRecordBatches) {\n            const block = this._footer?.getRecordBatch(this._recordBatchIndex);\n            if (block && this._handle.seek(block.offset)) {\n                return this._reader.readMessage(type);\n            }\n        }\n        return null;\n    }\n}\n\n/** @ignore */\nclass AsyncRecordBatchFileReaderImpl<T extends TypeMap = any> extends AsyncRecordBatchStreamReaderImpl<T>\n    implements AsyncRecordBatchFileReaderImpl<T> {\n\n    protected _footer?: Footer;\n    declare protected _handle: AsyncRandomAccessFile;\n    public get footer() { return this._footer!; }\n    public get numDictionaries() { return this._footer ? this._footer.numDictionaries : 0; }\n    public get numRecordBatches() { return this._footer ? this._footer.numRecordBatches : 0; }\n\n    constructor(source: FileHandle, byteLength?: number, dictionaries?: Map<number, Vector>);\n    constructor(source: FileHandle | AsyncRandomAccessFile, dictionaries?: Map<number, Vector>);\n    constructor(source: FileHandle | AsyncRandomAccessFile, ...rest: any[]) {\n        const byteLength = typeof rest[0] !== 'number' ? <number>rest.shift() : undefined;\n        const dictionaries = rest[0] instanceof Map ? <Map<number, Vector>>rest.shift() : undefined;\n        super(source instanceof AsyncRandomAccessFile ? source : new AsyncRandomAccessFile(source, byteLength), dictionaries);\n    }\n    public isFile(): this is RecordBatchFileReaders<T> { return true; }\n    public isAsync(): this is AsyncRecordBatchReaders<T> { return true; }\n    public async open(options?: OpenOptions) {\n        if (!this.closed && !this._footer) {\n            this.schema = (this._footer = await this._readFooter()).schema;\n            for (const block of this._footer.dictionaryBatches()) {\n                block && await this._readDictionaryBatch(this._dictionaryIndex++);\n            }\n        }\n        return await super.open(options);\n    }\n    public async readRecordBatch(index: number) {\n        if (this.closed) { return null; }\n        if (!this._footer) { await this.open(); }\n        const block = this._footer?.getRecordBatch(index);\n        if (block && (await this._handle.seek(block.offset))) {\n            const message = await this._reader.readMessage(MessageHeader.RecordBatch);\n            if (message?.isRecordBatch()) {\n                const header = message.header();\n                const buffer = await this._reader.readMessageBody(message.bodyLength);\n                const recordBatch = this._loadRecordBatch(header, buffer);\n                return recordBatch;\n            }\n        }\n        return null;\n    }\n    protected async _readDictionaryBatch(index: number) {\n        const block = this._footer?.getDictionaryBatch(index);\n        if (block && (await this._handle.seek(block.offset))) {\n            const message = await this._reader.readMessage(MessageHeader.DictionaryBatch);\n            if (message?.isDictionaryBatch()) {\n                const header = message.header();\n                const buffer = await this._reader.readMessageBody(message.bodyLength);\n                const vector = this._loadDictionaryBatch(header, buffer);\n                this.dictionaries.set(header.id, vector);\n            }\n        }\n    }\n    protected async _readFooter() {\n        const { _handle } = this;\n        _handle._pending && await _handle._pending;\n        const offset = _handle.size - magicAndPadding;\n        const length = await _handle.readInt32(offset);\n        const buffer = await _handle.readAt(offset - length, length);\n        return Footer.decode(buffer);\n    }\n    protected async _readNextMessageAndValidate<T extends MessageHeader>(type?: T | null): Promise<Message<T> | null> {\n        if (!this._footer) { await this.open(); }\n        if (this._footer && this._recordBatchIndex < this.numRecordBatches) {\n            const block = this._footer.getRecordBatch(this._recordBatchIndex);\n            if (block && await this._handle.seek(block.offset)) {\n                return await this._reader.readMessage(type);\n            }\n        }\n        return null;\n    }\n}\n\n/** @ignore */\nclass RecordBatchJSONReaderImpl<T extends TypeMap = any> extends RecordBatchStreamReaderImpl<T> {\n    constructor(source: ArrowJSONLike, dictionaries?: Map<number, Vector>) {\n        super(source, dictionaries);\n    }\n    protected _loadVectors(header: metadata.RecordBatch, body: any, types: (Field | DataType)[]) {\n        return new JSONVectorLoader(body, header.nodes, header.buffers, this.dictionaries).visitMany(types);\n    }\n}\n\n//\n// Define some helper functions and static implementations down here. There's\n// a bit of branching in the static methods that can lead to the same routines\n// being executed, so we've broken those out here for readability.\n//\n\n/** @ignore */\nfunction shouldAutoDestroy(self: { autoDestroy: boolean }, options?: OpenOptions) {\n    return options && (typeof options['autoDestroy'] === 'boolean') ? options['autoDestroy'] : self['autoDestroy'];\n}\n\n/** @ignore */\nfunction* readAllSync<T extends TypeMap = any>(source: RecordBatchReaders<T> | FromArg0 | FromArg2) {\n    const reader = RecordBatchReader.from<T>(<any>source) as RecordBatchReaders<T>;\n    try {\n        if (!reader.open({ autoDestroy: false }).closed) {\n            do { yield reader; } while (!(reader.reset().open()).closed);\n        }\n    } finally { reader.cancel(); }\n}\n\n/** @ignore */\nasync function* readAllAsync<T extends TypeMap = any>(source: AsyncRecordBatchReaders<T> | FromArg1 | FromArg3 | FromArg4 | FromArg5) {\n    const reader = await RecordBatchReader.from<T>(<any>source) as RecordBatchReader<T>;\n    try {\n        if (!(await reader.open({ autoDestroy: false })).closed) {\n            do { yield reader; } while (!(await reader.reset().open()).closed);\n        }\n    } finally { await reader.cancel(); }\n}\n\n/** @ignore */\nfunction fromArrowJSON<T extends TypeMap>(source: ArrowJSONLike) {\n    return new RecordBatchStreamReader(new RecordBatchJSONReaderImpl<T>(source));\n}\n\n/** @ignore */\nfunction fromByteStream<T extends TypeMap>(source: ByteStream) {\n    const bytes = source.peek((magicLength + 7) & ~7);\n    return bytes && bytes.byteLength >= 4 ? !checkForMagicArrowString(bytes)\n        ? new RecordBatchStreamReader(new RecordBatchStreamReaderImpl<T>(source))\n        : new RecordBatchFileReader(new RecordBatchFileReaderImpl<T>(source.read()))\n        : new RecordBatchStreamReader(new RecordBatchStreamReaderImpl<T>(function* (): any { }()));\n}\n\n/** @ignore */\nasync function fromAsyncByteStream<T extends TypeMap>(source: AsyncByteStream) {\n    const bytes = await source.peek((magicLength + 7) & ~7);\n    return bytes && bytes.byteLength >= 4 ? !checkForMagicArrowString(bytes)\n        ? new AsyncRecordBatchStreamReader(new AsyncRecordBatchStreamReaderImpl<T>(source))\n        : new RecordBatchFileReader(new RecordBatchFileReaderImpl<T>(await source.read()))\n        : new AsyncRecordBatchStreamReader(new AsyncRecordBatchStreamReaderImpl<T>(async function* (): any { }()));\n}\n\n/** @ignore */\nasync function fromFileHandle<T extends TypeMap>(source: FileHandle) {\n    const { size } = await source.stat();\n    const file = new AsyncRandomAccessFile(source, size);\n    if (size >= magicX2AndPadding && checkForMagicArrowString(await file.readAt(0, (magicLength + 7) & ~7))) {\n        return new AsyncRecordBatchFileReader(new AsyncRecordBatchFileReaderImpl<T>(file));\n    }\n    return new AsyncRecordBatchStreamReader(new AsyncRecordBatchStreamReaderImpl<T>(file));\n}\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { Data } from '../data.js';\nimport { Vector } from '../vector.js';\nimport { Visitor } from '../visitor.js';\nimport { Type, UnionMode } from '../enum.js';\nimport { RecordBatch } from '../recordbatch.js';\nimport { TypeToDataType } from '../interfaces.js';\nimport { rebaseValueOffsets } from '../util/buffer.js';\nimport { packBools, truncateBitmap } from '../util/bit.js';\nimport { BufferRegion, FieldNode } from '../ipc/metadata/message.js';\nimport {\n    DataType, Dictionary,\n    Float, Int, Date_, Interval, Time, Timestamp, Union,\n    Bool, Null, Utf8, Binary, Decimal, FixedSizeBinary, List, FixedSizeList, Map_, Struct,\n} from '../type.js';\n\n/** @ignore */\nexport interface VectorAssembler extends Visitor {\n    visit<T extends DataType>(node: Vector<T> | Data<T>): this;\n    visitMany<T extends DataType>(nodes: readonly Data<T>[]): this[];\n    getVisitFn<T extends Type>(node: T): (data: Data<TypeToDataType<T>>) => this;\n    getVisitFn<T extends DataType>(node: Vector<T> | Data<T> | T): (data: Data<T>) => this;\n\n    visitBool<T extends Bool>(data: Data<T>): this;\n    visitInt<T extends Int>(data: Data<T>): this;\n    visitFloat<T extends Float>(data: Data<T>): this;\n    visitUtf8<T extends Utf8>(data: Data<T>): this;\n    visitBinary<T extends Binary>(data: Data<T>): this;\n    visitFixedSizeBinary<T extends FixedSizeBinary>(data: Data<T>): this;\n    visitDate<T extends Date_>(data: Data<T>): this;\n    visitTimestamp<T extends Timestamp>(data: Data<T>): this;\n    visitTime<T extends Time>(data: Data<T>): this;\n    visitDecimal<T extends Decimal>(data: Data<T>): this;\n    visitList<T extends List>(data: Data<T>): this;\n    visitStruct<T extends Struct>(data: Data<T>): this;\n    visitUnion<T extends Union>(data: Data<T>): this;\n    visitInterval<T extends Interval>(data: Data<T>): this;\n    visitFixedSizeList<T extends FixedSizeList>(data: Data<T>): this;\n    visitMap<T extends Map_>(data: Data<T>): this;\n}\n\n/** @ignore */\nexport class VectorAssembler extends Visitor {\n\n    /** @nocollapse */\n    public static assemble<T extends Vector | RecordBatch>(...args: (T | T[])[]) {\n        const unwrap = (nodes: (T | T[])[]): Data[] =>\n            nodes.flatMap((node: T | T[]) => Array.isArray(node) ? unwrap(node) :\n                (node instanceof RecordBatch) ? node.data.children : node.data);\n        const assembler = new VectorAssembler();\n        assembler.visitMany(unwrap(args));\n        return assembler;\n    }\n\n    private constructor() { super(); }\n\n    public visit<T extends DataType>(data: Vector<T> | Data<T>): this {\n        if (data instanceof Vector) {\n            this.visitMany(data.data);\n            return this;\n        }\n        const { type } = data;\n        if (!DataType.isDictionary(type)) {\n            const { length, nullCount } = data;\n            if (length > 2147483647) {\n                /* istanbul ignore next */\n                throw new RangeError('Cannot write arrays larger than 2^31 - 1 in length');\n            }\n            if (!DataType.isNull(type)) {\n                addBuffer.call(this, nullCount <= 0\n                    ? new Uint8Array(0) // placeholder validity buffer\n                    : truncateBitmap(data.offset, length, data.nullBitmap)\n                );\n            }\n            this.nodes.push(new FieldNode(length, nullCount));\n        }\n        return super.visit(data);\n    }\n\n    public visitNull<T extends Null>(_null: Data<T>) {\n        return this;\n    }\n\n    public visitDictionary<T extends Dictionary>(data: Data<T>) {\n        // Assemble the indices here, Dictionary assembled separately.\n        return this.visit(data.clone(data.type.indices));\n    }\n\n    public get nodes() { return this._nodes; }\n    public get buffers() { return this._buffers; }\n    public get byteLength() { return this._byteLength; }\n    public get bufferRegions() { return this._bufferRegions; }\n\n    protected _byteLength = 0;\n    protected _nodes: FieldNode[] = [];\n    protected _buffers: ArrayBufferView[] = [];\n    protected _bufferRegions: BufferRegion[] = [];\n}\n\n/** @ignore */\nfunction addBuffer(this: VectorAssembler, values: ArrayBufferView) {\n    const byteLength = (values.byteLength + 7) & ~7; // Round up to a multiple of 8\n    this.buffers.push(values);\n    this.bufferRegions.push(new BufferRegion(this._byteLength, byteLength));\n    this._byteLength += byteLength;\n    return this;\n}\n\n/** @ignore */\nfunction assembleUnion<T extends Union>(this: VectorAssembler, data: Data<T>) {\n    const { type, length, typeIds, valueOffsets } = data;\n    // All Union Vectors have a typeIds buffer\n    addBuffer.call(this, typeIds);\n    // If this is a Sparse Union, treat it like all other Nested types\n    if (type.mode === UnionMode.Sparse) {\n        return assembleNestedVector.call(this, data);\n    } else if (type.mode === UnionMode.Dense) {\n        // If this is a Dense Union, add the valueOffsets buffer and potentially slice the children\n        if (data.offset <= 0) {\n            // If the Vector hasn't been sliced, write the existing valueOffsets\n            addBuffer.call(this, valueOffsets);\n            // We can treat this like all other Nested types\n            return assembleNestedVector.call(this, data);\n        } else {\n            // A sliced Dense Union is an unpleasant case. Because the offsets are different for\n            // each child vector, we need to \"rebase\" the valueOffsets for each child\n            // Union typeIds are not necessary 0-indexed\n            const maxChildTypeId = typeIds.reduce((x, y) => Math.max(x, y), typeIds[0]);\n            const childLengths = new Int32Array(maxChildTypeId + 1);\n            // Set all to -1 to indicate that we haven't observed a first occurrence of a particular child yet\n            const childOffsets = new Int32Array(maxChildTypeId + 1).fill(-1);\n            const shiftedOffsets = new Int32Array(length);\n            // If we have a non-zero offset, then the value offsets do not start at\n            // zero. We must a) create a new offsets array with shifted offsets and\n            // b) slice the values array accordingly\n            const unshiftedOffsets = rebaseValueOffsets(-valueOffsets[0], length, valueOffsets);\n            for (let typeId, shift, index = -1; ++index < length;) {\n                if ((shift = childOffsets[typeId = typeIds[index]]) === -1) {\n                    shift = childOffsets[typeId] = unshiftedOffsets[typeId];\n                }\n                shiftedOffsets[index] = unshiftedOffsets[index] - shift;\n                ++childLengths[typeId];\n            }\n            addBuffer.call(this, shiftedOffsets);\n            // Slice and visit children accordingly\n            for (let child: Data | null, childIndex = -1, numChildren = type.children.length; ++childIndex < numChildren;) {\n                if (child = data.children[childIndex]) {\n                    const typeId = type.typeIds[childIndex];\n                    const childLength = Math.min(length, childLengths[typeId]);\n                    this.visit(child.slice(childOffsets[typeId], childLength));\n                }\n            }\n        }\n    }\n    return this;\n}\n\n/** @ignore */\nfunction assembleBoolVector<T extends Bool>(this: VectorAssembler, data: Data<T>) {\n    // Bool vector is a special case of FlatVector, as its data buffer needs to stay packed\n    let values: Uint8Array;\n    if (data.nullCount >= data.length) {\n        // If all values are null, just insert a placeholder empty data buffer (fastest path)\n        return addBuffer.call(this, new Uint8Array(0));\n    } else if ((values = data.values) instanceof Uint8Array) {\n        // If values is already a Uint8Array, slice the bitmap (fast path)\n        return addBuffer.call(this, truncateBitmap(data.offset, data.length, values));\n    }\n    // Otherwise if the underlying data *isn't* a Uint8Array, enumerate the\n    // values as bools and re-pack them into a Uint8Array. This code isn't\n    // reachable unless you're trying to manipulate the Data internals,\n    // we're only doing this for safety.\n    /* istanbul ignore next */\n    return addBuffer.call(this, packBools(data.values));\n}\n\n/** @ignore */\nfunction assembleFlatVector<T extends Int | Float | FixedSizeBinary | Date_ | Timestamp | Time | Decimal | Interval>(this: VectorAssembler, data: Data<T>) {\n    return addBuffer.call(this, data.values.subarray(0, data.length * data.stride));\n}\n\n/** @ignore */\nfunction assembleFlatListVector<T extends Utf8 | Binary>(this: VectorAssembler, data: Data<T>) {\n    const { length, values, valueOffsets } = data;\n    const firstOffset = valueOffsets[0];\n    const lastOffset = valueOffsets[length];\n    const byteLength = Math.min(lastOffset - firstOffset, values.byteLength - firstOffset);\n    // Push in the order FlatList types read their buffers\n    addBuffer.call(this, rebaseValueOffsets(-valueOffsets[0], length, valueOffsets)); // valueOffsets buffer first\n    addBuffer.call(this, values.subarray(firstOffset, firstOffset + byteLength)); // sliced values buffer second\n    return this;\n}\n\n/** @ignore */\nfunction assembleListVector<T extends Map_ | List | FixedSizeList>(this: VectorAssembler, data: Data<T>) {\n    const { length, valueOffsets } = data;\n    // If we have valueOffsets (MapVector, ListVector), push that buffer first\n    if (valueOffsets) {\n        addBuffer.call(this, rebaseValueOffsets(valueOffsets[0], length, valueOffsets));\n    }\n    // Then insert the List's values child\n    return this.visit(data.children[0]);\n}\n\n/** @ignore */\nfunction assembleNestedVector<T extends Struct | Union>(this: VectorAssembler, data: Data<T>) {\n    return this.visitMany(data.type.children.map((_, i) => data.children[i]).filter(Boolean))[0];\n}\n\nVectorAssembler.prototype.visitBool = assembleBoolVector;\nVectorAssembler.prototype.visitInt = assembleFlatVector;\nVectorAssembler.prototype.visitFloat = assembleFlatVector;\nVectorAssembler.prototype.visitUtf8 = assembleFlatListVector;\nVectorAssembler.prototype.visitBinary = assembleFlatListVector;\nVectorAssembler.prototype.visitFixedSizeBinary = assembleFlatVector;\nVectorAssembler.prototype.visitDate = assembleFlatVector;\nVectorAssembler.prototype.visitTimestamp = assembleFlatVector;\nVectorAssembler.prototype.visitTime = assembleFlatVector;\nVectorAssembler.prototype.visitDecimal = assembleFlatVector;\nVectorAssembler.prototype.visitList = assembleListVector;\nVectorAssembler.prototype.visitStruct = assembleNestedVector;\nVectorAssembler.prototype.visitUnion = assembleUnion;\nVectorAssembler.prototype.visitInterval = assembleFlatVector;\nVectorAssembler.prototype.visitFixedSizeList = assembleListVector;\nVectorAssembler.prototype.visitMap = assembleListVector;\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { Data } from '../data.js';\nimport { Table } from '../table.js';\nimport { MAGIC } from './message.js';\nimport { Vector } from '../vector.js';\nimport { DataType, TypeMap } from '../type.js';\nimport { Schema, Field } from '../schema.js';\nimport { Message } from './metadata/message.js';\nimport * as metadata from './metadata/message.js';\nimport { FileBlock, Footer } from './metadata/file.js';\nimport { MessageHeader, MetadataVersion } from '../enum.js';\nimport { compareSchemas } from '../visitor/typecomparator.js';\nimport { WritableSink, AsyncByteQueue } from '../io/stream.js';\nimport { VectorAssembler } from '../visitor/vectorassembler.js';\nimport { JSONTypeAssembler } from '../visitor/jsontypeassembler.js';\nimport { JSONVectorAssembler } from '../visitor/jsonvectorassembler.js';\nimport { ArrayBufferViewInput, toUint8Array } from '../util/buffer.js';\nimport { RecordBatch, _InternalEmptyPlaceholderRecordBatch } from '../recordbatch.js';\nimport { Writable, ReadableInterop, ReadableDOMStreamOptions } from '../io/interfaces.js';\nimport { isPromise, isAsyncIterable, isWritableDOMStream, isWritableNodeStream, isIterable, isObject } from '../util/compat.js';\n\nexport interface RecordBatchStreamWriterOptions {\n    /**\n     *\n     */\n    autoDestroy?: boolean;\n    /**\n     * A flag indicating whether the RecordBatchWriter should construct pre-0.15.0\n     * encapsulated IPC Messages, which reserves  4 bytes for the Message metadata\n     * length instead of 8.\n     * @see https://issues.apache.org/jira/browse/ARROW-6313\n     */\n    writeLegacyIpcFormat?: boolean;\n}\n\nexport class RecordBatchWriter<T extends TypeMap = any> extends ReadableInterop<Uint8Array> implements Writable<RecordBatch<T>> {\n\n    /** @nocollapse */\n    // @ts-ignore\n    public static throughNode(options?: import('stream').DuplexOptions & { autoDestroy: boolean }): import('stream').Duplex {\n        throw new Error(`\"throughNode\" not available in this environment`);\n    }\n    /** @nocollapse */\n    public static throughDOM<T extends TypeMap>(\n        // @ts-ignore\n        writableStrategy?: QueuingStrategy<RecordBatch<T>> & { autoDestroy: boolean },\n        // @ts-ignore\n        readableStrategy?: { highWaterMark?: number; size?: any }\n    ): { writable: WritableStream<Table<T> | RecordBatch<T>>; readable: ReadableStream<Uint8Array> } {\n        throw new Error(`\"throughDOM\" not available in this environment`);\n    }\n\n    constructor(options?: RecordBatchStreamWriterOptions) {\n        super();\n        isObject(options) || (options = { autoDestroy: true, writeLegacyIpcFormat: false });\n        this._autoDestroy = (typeof options.autoDestroy === 'boolean') ? options.autoDestroy : true;\n        this._writeLegacyIpcFormat = (typeof options.writeLegacyIpcFormat === 'boolean') ? options.writeLegacyIpcFormat : false;\n    }\n\n    protected _position = 0;\n    protected _started = false;\n    protected _autoDestroy: boolean;\n    protected _writeLegacyIpcFormat: boolean;\n    // @ts-ignore\n    protected _sink = new AsyncByteQueue();\n    protected _schema: Schema | null = null;\n    protected _dictionaryBlocks: FileBlock[] = [];\n    protected _recordBatchBlocks: FileBlock[] = [];\n    protected _dictionaryDeltaOffsets = new Map<number, number>();\n\n    public toString(sync: true): string;\n    public toString(sync?: false): Promise<string>;\n    public toString(sync: any = false) {\n        return this._sink.toString(sync) as Promise<string> | string;\n    }\n    public toUint8Array(sync: true): Uint8Array;\n    public toUint8Array(sync?: false): Promise<Uint8Array>;\n    public toUint8Array(sync: any = false) {\n        return this._sink.toUint8Array(sync) as Promise<Uint8Array> | Uint8Array;\n    }\n\n    public writeAll(input: Table<T> | Iterable<RecordBatch<T>>): this;\n    public writeAll(input: AsyncIterable<RecordBatch<T>>): Promise<this>;\n    public writeAll(input: PromiseLike<AsyncIterable<RecordBatch<T>>>): Promise<this>;\n    public writeAll(input: PromiseLike<Table<T> | Iterable<RecordBatch<T>>>): Promise<this>;\n    public writeAll(input: PromiseLike<any> | Table<T> | Iterable<RecordBatch<T>> | AsyncIterable<RecordBatch<T>>) {\n        if (isPromise<any>(input)) {\n            return input.then((x) => this.writeAll(x));\n        } else if (isAsyncIterable<RecordBatch<T>>(input)) {\n            return writeAllAsync(this, input);\n        }\n        return writeAll(this, <any>input);\n    }\n\n    public get closed() { return this._sink.closed; }\n    public [Symbol.asyncIterator]() { return this._sink[Symbol.asyncIterator](); }\n    public toDOMStream(options?: ReadableDOMStreamOptions) { return this._sink.toDOMStream(options); }\n    public toNodeStream(options?: import('stream').ReadableOptions) { return this._sink.toNodeStream(options); }\n\n    public close() {\n        return this.reset()._sink.close();\n    }\n    public abort(reason?: any) {\n        return this.reset()._sink.abort(reason);\n    }\n    public finish() {\n        this._autoDestroy ? this.close() : this.reset(this._sink, this._schema);\n        return this;\n    }\n    public reset(sink: WritableSink<ArrayBufferViewInput> = this._sink, schema: Schema<T> | null = null) {\n        if ((sink === this._sink) || (sink instanceof AsyncByteQueue)) {\n            this._sink = sink as AsyncByteQueue;\n        } else {\n            this._sink = new AsyncByteQueue();\n            if (sink && isWritableDOMStream(sink)) {\n                this.toDOMStream({ type: 'bytes' }).pipeTo(sink);\n            } else if (sink && isWritableNodeStream(sink)) {\n                this.toNodeStream({ objectMode: false }).pipe(sink);\n            }\n        }\n\n        if (this._started && this._schema) {\n            this._writeFooter(this._schema);\n        }\n\n        this._started = false;\n        this._dictionaryBlocks = [];\n        this._recordBatchBlocks = [];\n        this._dictionaryDeltaOffsets = new Map();\n\n        if (!schema || !(compareSchemas(schema, this._schema))) {\n            if (schema == null) {\n                this._position = 0;\n                this._schema = null;\n            } else {\n                this._started = true;\n                this._schema = schema;\n                this._writeSchema(schema);\n            }\n        }\n\n        return this;\n    }\n\n    public write(payload?: Table<T> | RecordBatch<T> | Iterable<RecordBatch<T>> | null) {\n        let schema: Schema<T> | null = null;\n\n        if (!this._sink) {\n            throw new Error(`RecordBatchWriter is closed`);\n        } else if (payload == null) {\n            return this.finish() && undefined;\n        } else if (payload instanceof Table && !(schema = payload.schema)) {\n            return this.finish() && undefined;\n        } else if (payload instanceof RecordBatch && !(schema = payload.schema)) {\n            return this.finish() && undefined;\n        }\n\n        if (schema && !compareSchemas(schema, this._schema)) {\n            if (this._started && this._autoDestroy) {\n                return this.close();\n            }\n            this.reset(this._sink, schema);\n        }\n\n        if (payload instanceof RecordBatch) {\n            if (!(payload instanceof _InternalEmptyPlaceholderRecordBatch)) {\n                this._writeRecordBatch(payload);\n            }\n        } else if (payload instanceof Table) {\n            this.writeAll(payload.batches);\n        } else if (isIterable(payload)) {\n            this.writeAll(payload);\n        }\n    }\n\n    protected _writeMessage<T extends MessageHeader>(message: Message<T>, alignment = 8) {\n        const a = alignment - 1;\n        const buffer = Message.encode(message);\n        const flatbufferSize = buffer.byteLength;\n        const prefixSize = !this._writeLegacyIpcFormat ? 8 : 4;\n        const alignedSize = (flatbufferSize + prefixSize + a) & ~a;\n        const nPaddingBytes = alignedSize - flatbufferSize - prefixSize;\n\n        if (message.headerType === MessageHeader.RecordBatch) {\n            this._recordBatchBlocks.push(new FileBlock(alignedSize, message.bodyLength, this._position));\n        } else if (message.headerType === MessageHeader.DictionaryBatch) {\n            this._dictionaryBlocks.push(new FileBlock(alignedSize, message.bodyLength, this._position));\n        }\n\n        // If not in legacy pre-0.15.0 mode, write the stream continuation indicator\n        if (!this._writeLegacyIpcFormat) {\n            this._write(Int32Array.of(-1));\n        }\n        // Write the flatbuffer size prefix including padding\n        this._write(Int32Array.of(alignedSize - prefixSize));\n        // Write the flatbuffer\n        if (flatbufferSize > 0) { this._write(buffer); }\n        // Write any padding\n        return this._writePadding(nPaddingBytes);\n    }\n\n    protected _write(chunk: ArrayBufferViewInput) {\n        if (this._started) {\n            const buffer = toUint8Array(chunk);\n            if (buffer && buffer.byteLength > 0) {\n                this._sink.write(buffer);\n                this._position += buffer.byteLength;\n            }\n        }\n        return this;\n    }\n\n    protected _writeSchema(schema: Schema<T>) {\n        return this._writeMessage(Message.from(schema));\n    }\n\n    // @ts-ignore\n    protected _writeFooter(schema: Schema<T>) {\n        // eos bytes\n        return this._writeLegacyIpcFormat\n            ? this._write(Int32Array.of(0))\n            : this._write(Int32Array.of(-1, 0));\n    }\n\n    protected _writeMagic() {\n        return this._write(MAGIC);\n    }\n\n    protected _writePadding(nBytes: number) {\n        return nBytes > 0 ? this._write(new Uint8Array(nBytes)) : this;\n    }\n\n    protected _writeRecordBatch(batch: RecordBatch<T>) {\n        const { byteLength, nodes, bufferRegions, buffers } = VectorAssembler.assemble(batch);\n        const recordBatch = new metadata.RecordBatch(batch.numRows, nodes, bufferRegions);\n        const message = Message.from(recordBatch, byteLength);\n        return this\n            ._writeDictionaries(batch)\n            ._writeMessage(message)\n            ._writeBodyBuffers(buffers);\n    }\n\n    protected _writeDictionaryBatch(dictionary: Data, id: number, isDelta = false) {\n        this._dictionaryDeltaOffsets.set(id, dictionary.length + (this._dictionaryDeltaOffsets.get(id) || 0));\n        const { byteLength, nodes, bufferRegions, buffers } = VectorAssembler.assemble(new Vector([dictionary]));\n        const recordBatch = new metadata.RecordBatch(dictionary.length, nodes, bufferRegions);\n        const dictionaryBatch = new metadata.DictionaryBatch(recordBatch, id, isDelta);\n        const message = Message.from(dictionaryBatch, byteLength);\n        return this\n            ._writeMessage(message)\n            ._writeBodyBuffers(buffers);\n    }\n\n    protected _writeBodyBuffers(buffers: ArrayBufferView[]) {\n        let buffer: ArrayBufferView;\n        let size: number, padding: number;\n        for (let i = -1, n = buffers.length; ++i < n;) {\n            if ((buffer = buffers[i]) && (size = buffer.byteLength) > 0) {\n                this._write(buffer);\n                if ((padding = ((size + 7) & ~7) - size) > 0) {\n                    this._writePadding(padding);\n                }\n            }\n        }\n        return this;\n    }\n\n    protected _writeDictionaries(batch: RecordBatch<T>) {\n        for (let [id, dictionary] of batch.dictionaries) {\n            let offset = this._dictionaryDeltaOffsets.get(id) || 0;\n            if (offset === 0 || (dictionary = dictionary?.slice(offset)).length > 0) {\n                for (const data of dictionary.data) {\n                    this._writeDictionaryBatch(data, id, offset > 0);\n                    offset += data.length;\n                }\n            }\n        }\n        return this;\n    }\n}\n\n/** @ignore */\nexport class RecordBatchStreamWriter<T extends TypeMap = any> extends RecordBatchWriter<T> {\n    public static writeAll<T extends TypeMap = any>(input: Table<T> | Iterable<RecordBatch<T>>, options?: RecordBatchStreamWriterOptions): RecordBatchStreamWriter<T>;\n    public static writeAll<T extends TypeMap = any>(input: AsyncIterable<RecordBatch<T>>, options?: RecordBatchStreamWriterOptions): Promise<RecordBatchStreamWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(input: PromiseLike<AsyncIterable<RecordBatch<T>>>, options?: RecordBatchStreamWriterOptions): Promise<RecordBatchStreamWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(input: PromiseLike<Table<T> | Iterable<RecordBatch<T>>>, options?: RecordBatchStreamWriterOptions): Promise<RecordBatchStreamWriter<T>>;\n    /** @nocollapse */\n    public static writeAll<T extends TypeMap = any>(input: any, options?: RecordBatchStreamWriterOptions) {\n        const writer = new RecordBatchStreamWriter<T>(options);\n        if (isPromise<any>(input)) {\n            return input.then((x) => writer.writeAll(x));\n        } else if (isAsyncIterable<RecordBatch<T>>(input)) {\n            return writeAllAsync(writer, input);\n        }\n        return writeAll(writer, input);\n    }\n}\n\n/** @ignore */\nexport class RecordBatchFileWriter<T extends TypeMap = any> extends RecordBatchWriter<T> {\n    public static writeAll<T extends TypeMap = any>(input: Table<T> | Iterable<RecordBatch<T>>): RecordBatchFileWriter<T>;\n    public static writeAll<T extends TypeMap = any>(input: AsyncIterable<RecordBatch<T>>): Promise<RecordBatchFileWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(input: PromiseLike<AsyncIterable<RecordBatch<T>>>): Promise<RecordBatchFileWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(input: PromiseLike<Table<T> | Iterable<RecordBatch<T>>>): Promise<RecordBatchFileWriter<T>>;\n    /** @nocollapse */\n    public static writeAll<T extends TypeMap = any>(input: any) {\n        const writer = new RecordBatchFileWriter<T>();\n        if (isPromise<any>(input)) {\n            return input.then((x) => writer.writeAll(x));\n        } else if (isAsyncIterable<RecordBatch<T>>(input)) {\n            return writeAllAsync(writer, input);\n        }\n        return writeAll(writer, input);\n    }\n\n    constructor() {\n        super();\n        this._autoDestroy = true;\n    }\n\n    // @ts-ignore\n    protected _writeSchema(schema: Schema<T>) {\n        return this._writeMagic()._writePadding(2);\n    }\n\n    protected _writeFooter(schema: Schema<T>) {\n        const buffer = Footer.encode(new Footer(\n            schema, MetadataVersion.V4,\n            this._recordBatchBlocks, this._dictionaryBlocks\n        ));\n        return super\n            ._writeFooter(schema) // EOS bytes for sequential readers\n            ._write(buffer) // Write the flatbuffer\n            ._write(Int32Array.of(buffer.byteLength)) // then the footer size suffix\n            ._writeMagic(); // then the magic suffix\n    }\n}\n\n/** @ignore */\nexport class RecordBatchJSONWriter<T extends TypeMap = any> extends RecordBatchWriter<T> {\n\n    public static writeAll<T extends TypeMap = any>(this: typeof RecordBatchWriter, input: Table<T> | Iterable<RecordBatch<T>>): RecordBatchJSONWriter<T>;\n    // @ts-ignore\n    public static writeAll<T extends TypeMap = any>(this: typeof RecordBatchWriter, input: AsyncIterable<RecordBatch<T>>): Promise<RecordBatchJSONWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(this: typeof RecordBatchWriter, input: PromiseLike<AsyncIterable<RecordBatch<T>>>): Promise<RecordBatchJSONWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(this: typeof RecordBatchWriter, input: PromiseLike<Table<T> | Iterable<RecordBatch<T>>>): Promise<RecordBatchJSONWriter<T>>;\n    /** @nocollapse */\n    public static writeAll<T extends TypeMap = any>(this: typeof RecordBatchWriter, input: any) {\n        return new RecordBatchJSONWriter<T>().writeAll(input as any);\n    }\n\n    private _recordBatches: RecordBatch[];\n    private _dictionaries: RecordBatch[];\n\n    constructor() {\n        super();\n        this._autoDestroy = true;\n        this._recordBatches = [];\n        this._dictionaries = [];\n    }\n\n    protected _writeMessage() { return this; }\n    // @ts-ignore\n    protected _writeFooter(schema: Schema<T>) { return this; }\n    protected _writeSchema(schema: Schema<T>) {\n        return this._write(`{\\n  \"schema\": ${JSON.stringify({ fields: schema.fields.map(field => fieldToJSON(field)) }, null, 2)}`);\n    }\n    protected _writeDictionaries(batch: RecordBatch<T>) {\n        if (batch.dictionaries.size > 0) {\n            this._dictionaries.push(batch);\n        }\n        return this;\n    }\n    protected _writeDictionaryBatch(dictionary: Data, id: number, isDelta = false) {\n        this._dictionaryDeltaOffsets.set(id, dictionary.length + (this._dictionaryDeltaOffsets.get(id) || 0));\n        this._write(this._dictionaryBlocks.length === 0 ? `    ` : `,\\n    `);\n        this._write(`${dictionaryBatchToJSON(dictionary, id, isDelta)}`);\n        this._dictionaryBlocks.push(new FileBlock(0, 0, 0));\n        return this;\n    }\n    protected _writeRecordBatch(batch: RecordBatch<T>) {\n        this._writeDictionaries(batch);\n        this._recordBatches.push(batch);\n        return this;\n    }\n    public close() {\n\n        if (this._dictionaries.length > 0) {\n            this._write(`,\\n  \"dictionaries\": [\\n`);\n            for (const batch of this._dictionaries) {\n                super._writeDictionaries(batch);\n            }\n            this._write(`\\n  ]`);\n        }\n\n        if (this._recordBatches.length > 0) {\n            for (let i = -1, n = this._recordBatches.length; ++i < n;) {\n                this._write(i === 0 ? `,\\n  \"batches\": [\\n    ` : `,\\n    `);\n                this._write(`${recordBatchToJSON(this._recordBatches[i])}`);\n                this._recordBatchBlocks.push(new FileBlock(0, 0, 0));\n            }\n            this._write(`\\n  ]`);\n        }\n\n        if (this._schema) {\n            this._write(`\\n}`);\n        }\n\n        this._dictionaries = [];\n        this._recordBatches = [];\n\n        return super.close();\n    }\n}\n\n/** @ignore */\nfunction writeAll<T extends TypeMap = any>(writer: RecordBatchWriter<T>, input: Table<T> | Iterable<RecordBatch<T>>) {\n    let chunks = input as Iterable<RecordBatch<T>>;\n    if (input instanceof Table) {\n        chunks = input.batches;\n        writer.reset(undefined, input.schema);\n    }\n    for (const batch of chunks) {\n        writer.write(batch);\n    }\n    return writer.finish();\n}\n\n/** @ignore */\nasync function writeAllAsync<T extends TypeMap = any>(writer: RecordBatchWriter<T>, batches: AsyncIterable<RecordBatch<T>>) {\n    for await (const batch of batches) {\n        writer.write(batch);\n    }\n    return writer.finish();\n}\n\n/** @ignore */\nfunction fieldToJSON({ name, type, nullable }: Field): Record<string, unknown> {\n    const assembler = new JSONTypeAssembler();\n    return {\n        'name': name, 'nullable': nullable,\n        'type': assembler.visit(type),\n        'children': (type.children || []).map((field: any) => fieldToJSON(field)),\n        'dictionary': !DataType.isDictionary(type) ? undefined : {\n            'id': type.id,\n            'isOrdered': type.isOrdered,\n            'indexType': assembler.visit(type.indices)\n        }\n    };\n}\n\n/** @ignore */\nfunction dictionaryBatchToJSON(dictionary: Data, id: number, isDelta = false) {\n    const [columns] = JSONVectorAssembler.assemble(new RecordBatch({ [id]: dictionary }));\n    return JSON.stringify({\n        'id': id,\n        'isDelta': isDelta,\n        'data': {\n            'count': dictionary.length,\n            'columns': columns\n        }\n    }, null, 2);\n}\n\n/** @ignore */\nfunction recordBatchToJSON(records: RecordBatch) {\n    const [columns] = JSONVectorAssembler.assemble(records);\n    return JSON.stringify({\n        'count': records.numRows,\n        'columns': columns\n    }, null, 2);\n}\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { Table } from '../table.js';\nimport { TypeMap } from '../type.js';\nimport { isPromise } from '../util/compat.js';\nimport {\n    FromArg0, FromArg1, FromArg2, FromArg3, FromArg4, FromArg5,\n    RecordBatchReader,\n    RecordBatchFileReader, RecordBatchStreamReader,\n    AsyncRecordBatchFileReader, AsyncRecordBatchStreamReader\n} from './reader.js';\nimport { RecordBatchFileWriter, RecordBatchStreamWriter } from './writer.js';\n\ntype RecordBatchReaders<T extends TypeMap = any> = RecordBatchFileReader<T> | RecordBatchStreamReader<T>;\ntype AsyncRecordBatchReaders<T extends TypeMap = any> = AsyncRecordBatchFileReader<T> | AsyncRecordBatchStreamReader<T>;\n\n/**\n * Deserialize the IPC format into a {@link Table}. This function is a\n * convenience wrapper for {@link RecordBatchReader}. Opposite of {@link tableToIPC}.\n */\nexport function tableFromIPC<T extends TypeMap = any>(source: FromArg0 | FromArg2): Table<T>;\nexport function tableFromIPC<T extends TypeMap = any>(source: FromArg1): Promise<Table<T>>;\nexport function tableFromIPC<T extends TypeMap = any>(source: FromArg3 | FromArg4 | FromArg5): Promise<Table<T>>;\nexport function tableFromIPC<T extends TypeMap = any>(source: RecordBatchReaders<T>): Table<T>;\nexport function tableFromIPC<T extends TypeMap = any>(source: AsyncRecordBatchReaders<T>): Promise<Table<T>>;\nexport function tableFromIPC<T extends TypeMap = any>(source: RecordBatchReader<T>): Table<T> | Promise<Table<T>>;\nexport function tableFromIPC<T extends TypeMap = any>(input: any): Table<T> | Promise<Table<T>> {\n    const reader = RecordBatchReader.from<T>(input) as RecordBatchReader<T> | Promise<RecordBatchReader<T>>;\n    if (isPromise<RecordBatchReader<T>>(reader)) {\n        return reader.then((reader) => tableFromIPC(reader)) as Promise<Table<T>>;\n    }\n    if (reader.isAsync()) {\n        return (reader as AsyncRecordBatchReaders<T>).readAll().then((xs) => new Table(xs));\n    }\n    return new Table((reader as RecordBatchReaders<T>).readAll());\n}\n\n/**\n * Serialize a {@link Table} to the IPC format. This function is a convenience\n * wrapper for {@link RecordBatchStreamWriter} and {@link RecordBatchFileWriter}.\n * Opposite of {@link tableFromIPC}.\n *\n * @param table The Table to serialize.\n * @param type Whether to serialize the Table as a file or a stream.\n */\nexport function tableToIPC<T extends TypeMap = any>(table: Table, type: 'file' | 'stream' = 'stream'): Uint8Array {\n    return (type === 'stream' ? RecordBatchStreamWriter : RecordBatchFileWriter)\n        .writeAll<T>(table)\n        .toUint8Array(true);\n}\n",
         "/**\n * Copyright (c) Streamlit Inc. (2018-2022) Snowflake Inc. (2022)\n *\n * Licensed under the Apache License, Version 2.0 (the \"License\");\n * you may not use this file except in compliance with the License.\n * You may obtain a copy of the License at\n *\n *     http://www.apache.org/licenses/LICENSE-2.0\n *\n * Unless required by applicable law or agreed to in writing, software\n * distributed under the License is distributed on an \"AS IS\" BASIS,\n * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n * See the License for the specific language governing permissions and\n * limitations under the License.\n */\nimport { tableToIPC, tableFromIPC, Type } from \"apache-arrow\";\nvar ArrowTable = /** @class */ (function () {\n    function ArrowTable(dataBuffer, indexBuffer, columnsBuffer, styler) {\n        var _this = this;\n        this.getCell = function (rowIndex, columnIndex) {\n            var isBlankCell = rowIndex < _this.headerRows && columnIndex < _this.headerColumns;\n            var isIndexCell = rowIndex >= _this.headerRows && columnIndex < _this.headerColumns;\n            var isColumnsCell = rowIndex < _this.headerRows && columnIndex >= _this.headerColumns;\n            if (isBlankCell) {\n                var classNames = [\"blank\"];\n                if (columnIndex > 0) {\n                    classNames.push(\"level\" + rowIndex);\n                }\n                return {\n                    type: \"blank\",\n                    classNames: classNames.join(\" \"),\n                    content: \"\"\n                };\n            }\n            else if (isColumnsCell) {\n                var dataColumnIndex = columnIndex - _this.headerColumns;\n                var classNames = [\n                    \"col_heading\",\n                    \"level\" + rowIndex,\n                    \"col\" + dataColumnIndex\n                ];\n                return {\n                    type: \"columns\",\n                    classNames: classNames.join(\" \"),\n                    content: _this.getContent(_this.columnsTable, dataColumnIndex, rowIndex)\n                };\n            }\n            else if (isIndexCell) {\n                var dataRowIndex = rowIndex - _this.headerRows;\n                var classNames = [\n                    \"row_heading\",\n                    \"level\" + columnIndex,\n                    \"row\" + dataRowIndex\n                ];\n                return {\n                    type: \"index\",\n                    id: \"T_\".concat(_this.uuid, \"level\").concat(columnIndex, \"_row\").concat(dataRowIndex),\n                    classNames: classNames.join(\" \"),\n                    content: _this.getContent(_this.indexTable, dataRowIndex, columnIndex)\n                };\n            }\n            else {\n                var dataRowIndex = rowIndex - _this.headerRows;\n                var dataColumnIndex = columnIndex - _this.headerColumns;\n                var classNames = [\n                    \"data\",\n                    \"row\" + dataRowIndex,\n                    \"col\" + dataColumnIndex\n                ];\n                var content = _this.styler\n                    ? _this.getContent(_this.styler.displayValuesTable, dataRowIndex, dataColumnIndex)\n                    : _this.getContent(_this.dataTable, dataRowIndex, dataColumnIndex);\n                return {\n                    type: \"data\",\n                    id: \"T_\".concat(_this.uuid, \"row\").concat(dataRowIndex, \"_col\").concat(dataColumnIndex),\n                    classNames: classNames.join(\" \"),\n                    content: content\n                };\n            }\n        };\n        this.getContent = function (table, rowIndex, columnIndex) {\n            var column = table.getChildAt(columnIndex);\n            if (column === null) {\n                return \"\";\n            }\n            var columnTypeId = _this.getColumnTypeId(table, columnIndex);\n            switch (columnTypeId) {\n                case Type.Timestamp: {\n                    return _this.nanosToDate(column.get(rowIndex));\n                }\n                default: {\n                    return column.get(rowIndex);\n                }\n            }\n        };\n        this.dataTable = tableFromIPC(dataBuffer);\n        this.indexTable = tableFromIPC(indexBuffer);\n        this.columnsTable = tableFromIPC(columnsBuffer);\n        this.styler = styler\n            ? {\n                caption: styler.caption,\n                displayValuesTable: tableFromIPC(styler.displayValues),\n                styles: styler.styles,\n                uuid: styler.uuid\n            }\n            : undefined;\n    }\n    Object.defineProperty(ArrowTable.prototype, \"rows\", {\n        get: function () {\n            return this.indexTable.numRows + this.columnsTable.numCols;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"columns\", {\n        get: function () {\n            return this.indexTable.numCols + this.columnsTable.numRows;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"headerRows\", {\n        get: function () {\n            return this.rows - this.dataRows;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"headerColumns\", {\n        get: function () {\n            return this.columns - this.dataColumns;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"dataRows\", {\n        get: function () {\n            return this.dataTable.numRows;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"dataColumns\", {\n        get: function () {\n            return this.dataTable.numCols;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"uuid\", {\n        get: function () {\n            return this.styler && this.styler.uuid;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"caption\", {\n        get: function () {\n            return this.styler && this.styler.caption;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"styles\", {\n        get: function () {\n            return this.styler && this.styler.styles;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"table\", {\n        get: function () {\n            return this.dataTable;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"index\", {\n        get: function () {\n            return this.indexTable;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"columnTable\", {\n        get: function () {\n            return this.columnsTable;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    /**\n     * Serialize arrow table.\n     */\n    ArrowTable.prototype.serialize = function () {\n        return {\n            data: tableToIPC(this.dataTable),\n            index: tableToIPC(this.indexTable),\n            columns: tableToIPC(this.columnsTable)\n        };\n    };\n    /**\n     * Returns apache-arrow specific typeId of column.\n     */\n    ArrowTable.prototype.getColumnTypeId = function (table, columnIndex) {\n        return table.schema.fields[columnIndex].type.typeId;\n    };\n    ArrowTable.prototype.nanosToDate = function (nanos) {\n        return new Date(nanos / 1e6);\n    };\n    return ArrowTable;\n}());\nexport { ArrowTable };\n",
         "/**\n * Copyright (c) Streamlit Inc. (2018-2022) Snowflake Inc. (2022)\n *\n * Licensed under the Apache License, Version 2.0 (the \"License\");\n * you may not use this file except in compliance with the License.\n * You may obtain a copy of the License at\n *\n *     http://www.apache.org/licenses/LICENSE-2.0\n *\n * Unless required by applicable law or agreed to in writing, software\n * distributed under the License is distributed on an \"AS IS\" BASIS,\n * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n * See the License for the specific language governing permissions and\n * limitations under the License.\n */\nvar __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\n// Safari doesn't support the EventTarget class, so we use a shim.\nimport { ArrowTable } from \"./ArrowTable\";\n/** Messages from Component -> Streamlit */\nvar ComponentMessageType;\n(function (ComponentMessageType) {\n    // A component sends this message when it's ready to receive messages\n    // from Streamlit. Streamlit won't send any messages until it gets this.\n    // Data: { apiVersion: number }\n    ComponentMessageType[\"COMPONENT_READY\"] = \"streamlit:componentReady\";\n    // The component has a new widget value. Send it back to Streamlit, which\n    // will then re-run the app.\n    // Data: { value: any }\n    ComponentMessageType[\"SET_COMPONENT_VALUE\"] = \"streamlit:setComponentValue\";\n    // The component has a new height for its iframe.\n    // Data: { height: number }\n    ComponentMessageType[\"SET_FRAME_HEIGHT\"] = \"streamlit:setFrameHeight\";\n})(ComponentMessageType || (ComponentMessageType = {}));\n/**\n * Streamlit communication API.\n *\n * Components can send data to Streamlit via the functions defined here,\n * and receive data from Streamlit via the `events` property.\n */\nexport var Streamlit = /** @class */ (function () {\n    function Streamlit() {\n    }\n    /**\n     * The Streamlit component API version we're targeting.\n     * There's currently only 1!\n     */\n    Streamlit.API_VERSION = 1;\n    Streamlit.RENDER_EVENT = \"streamlit:render\";\n    /** Dispatches events received from Streamlit. */\n    Streamlit.events = new EventTarget();\n    Streamlit.registeredMessageListener = false;\n    /**\n     * Tell Streamlit that the component is ready to start receiving data.\n     * Streamlit will defer emitting RENDER events until it receives the\n     * COMPONENT_READY message.\n     */\n    Streamlit.setComponentReady = function () {\n        if (!Streamlit.registeredMessageListener) {\n            // Register for message events if we haven't already\n            window.addEventListener(\"message\", Streamlit.onMessageEvent);\n            Streamlit.registeredMessageListener = true;\n        }\n        Streamlit.sendBackMsg(ComponentMessageType.COMPONENT_READY, {\n            apiVersion: Streamlit.API_VERSION\n        });\n    };\n    /**\n     * Report the component's height to Streamlit.\n     * This should be called every time the component changes its DOM - that is,\n     * when it's first loaded, and any time it updates.\n     */\n    Streamlit.setFrameHeight = function (height) {\n        if (height === undefined) {\n            // `height` is optional. If undefined, it defaults to scrollHeight,\n            // which is the entire height of the element minus its border,\n            // scrollbar, and margin.\n            height = document.body.scrollHeight;\n        }\n        if (height === Streamlit.lastFrameHeight) {\n            // Don't bother updating if our height hasn't changed.\n            return;\n        }\n        Streamlit.lastFrameHeight = height;\n        Streamlit.sendBackMsg(ComponentMessageType.SET_FRAME_HEIGHT, { height: height });\n    };\n    /**\n     * Set the component's value. This value will be returned to the Python\n     * script, and the script will be re-run.\n     *\n     * For example:\n     *\n     * JavaScript:\n     * Streamlit.setComponentValue(\"ahoy!\")\n     *\n     * Python:\n     * value = st.my_component(...)\n     * st.write(value) # -> \"ahoy!\"\n     *\n     * The value must be an ArrowTable, a typed array, an ArrayBuffer, or be\n     * serializable to JSON.\n     */\n    Streamlit.setComponentValue = function (value) {\n        var dataType;\n        if (value instanceof ArrowTable) {\n            dataType = \"dataframe\";\n            value = value.serialize();\n        }\n        else if (isTypedArray(value)) {\n            // All typed arrays get sent as Uint8Array, because that's what our\n            // protobuf library uses for the \"bytes\" field type.\n            dataType = \"bytes\";\n            value = new Uint8Array(value.buffer);\n        }\n        else if (value instanceof ArrayBuffer) {\n            dataType = \"bytes\";\n            value = new Uint8Array(value);\n        }\n        else {\n            dataType = \"json\";\n        }\n        Streamlit.sendBackMsg(ComponentMessageType.SET_COMPONENT_VALUE, {\n            value: value,\n            dataType: dataType\n        });\n    };\n    /** Receive a ForwardMsg from the Streamlit app */\n    Streamlit.onMessageEvent = function (event) {\n        var type = event.data[\"type\"];\n        switch (type) {\n            case Streamlit.RENDER_EVENT:\n                Streamlit.onRenderMessage(event.data);\n                break;\n        }\n    };\n    /**\n     * Handle an untyped Streamlit render event and redispatch it as a\n     * StreamlitRenderEvent.\n     */\n    Streamlit.onRenderMessage = function (data) {\n        var args = data[\"args\"];\n        if (args == null) {\n            console.error(\"Got null args in onRenderMessage. This should never happen\");\n            args = {};\n        }\n        // Parse our dataframe arguments with arrow, and merge them into our args dict\n        var dataframeArgs = data[\"dfs\"] && data[\"dfs\"].length > 0\n            ? Streamlit.argsDataframeToObject(data[\"dfs\"])\n            : {};\n        args = __assign(__assign({}, args), dataframeArgs);\n        var disabled = Boolean(data[\"disabled\"]);\n        var theme = data[\"theme\"];\n        if (theme) {\n            _injectTheme(theme);\n        }\n        // Dispatch a render event!\n        var eventData = { disabled: disabled, args: args, theme: theme };\n        var event = new CustomEvent(Streamlit.RENDER_EVENT, {\n            detail: eventData\n        });\n        Streamlit.events.dispatchEvent(event);\n    };\n    Streamlit.argsDataframeToObject = function (argsDataframe) {\n        var argsDataframeArrow = argsDataframe.map(function (_a) {\n            var key = _a.key, value = _a.value;\n            return [key, Streamlit.toArrowTable(value)];\n        });\n        return Object.fromEntries(argsDataframeArrow);\n    };\n    Streamlit.toArrowTable = function (df) {\n        var _a;\n        var data = (_a = df.data, _a.data), index = _a.index, columns = _a.columns, styler = _a.styler;\n        return new ArrowTable(data, index, columns, styler);\n    };\n    /** Post a message to the Streamlit app. */\n    Streamlit.sendBackMsg = function (type, data) {\n        window.parent.postMessage(__assign({ isStreamlitMessage: true, type: type }, data), \"*\");\n    };\n    return Streamlit;\n}());\nvar _injectTheme = function (theme) {\n    var style = document.createElement(\"style\");\n    document.head.appendChild(style);\n    style.innerHTML = \"\\n    :root {\\n      --primary-color: \".concat(theme.primaryColor, \";\\n      --background-color: \").concat(theme.backgroundColor, \";\\n      --secondary-background-color: \").concat(theme.secondaryBackgroundColor, \";\\n      --text-color: \").concat(theme.textColor, \";\\n      --font: \").concat(theme.font, \";\\n    }\\n\\n    body {\\n      background-color: var(--background-color);\\n      color: var(--text-color);\\n    }\\n  \");\n};\n/** True if the value is a TypedArray. */\nfunction isTypedArray(value) {\n    var isBigIntArray = false;\n    try {\n        isBigIntArray =\n            value instanceof BigInt64Array || value instanceof BigUint64Array;\n    }\n    catch (e) {\n        // Ignore cause Safari does not support this\n        // https://caniuse.com/mdn-javascript_builtins_bigint64array\n    }\n    return (value instanceof Int8Array ||\n        value instanceof Uint8Array ||\n        value instanceof Uint8ClampedArray ||\n        value instanceof Int16Array ||\n        value instanceof Uint16Array ||\n        value instanceof Int32Array ||\n        value instanceof Uint32Array ||\n        value instanceof Float32Array ||\n        value instanceof Float64Array ||\n        isBigIntArray);\n}\n",
         "/**\n * Copyright (c) Streamlit Inc. (2018-2022) Snowflake Inc. (2022)\n *\n * Licensed under the Apache License, Version 2.0 (the \"License\");\n * you may not use this file except in compliance with the License.\n * You may obtain a copy of the License at\n *\n *     http://www.apache.org/licenses/LICENSE-2.0\n *\n * Unless required by applicable law or agreed to in writing, software\n * distributed under the License is distributed on an \"AS IS\" BASIS,\n * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n * See the License for the specific language governing permissions and\n * limitations under the License.\n */\nvar __extends = (this && this.__extends) || (function () {\n    var extendStatics = function (d, b) {\n        extendStatics = Object.setPrototypeOf ||\n            ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\n            function (d, b) { for (var p in b) if (Object.prototype.hasOwnProperty.call(b, p)) d[p] = b[p]; };\n        return extendStatics(d, b);\n    };\n    return function (d, b) {\n        if (typeof b !== \"function\" && b !== null)\n            throw new TypeError(\"Class extends value \" + String(b) + \" is not a constructor or null\");\n        extendStatics(d, b);\n        function __() { this.constructor = d; }\n        d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\n    };\n})();\nimport hoistNonReactStatics from \"hoist-non-react-statics\";\nimport React from \"react\";\nimport { Streamlit } from \"./streamlit\";\n/**\n * Optional Streamlit React-based component base class.\n *\n * You are not required to extend this base class to create a Streamlit\n * component. If you decide not to extend it, you should implement the\n * `componentDidMount` and `componentDidUpdate` functions in your own class,\n * so that your plugin properly resizes.\n */\nvar StreamlitComponentBase = /** @class */ (function (_super) {\n    __extends(StreamlitComponentBase, _super);\n    function StreamlitComponentBase() {\n        return _super !== null && _super.apply(this, arguments) || this;\n    }\n    StreamlitComponentBase.prototype.componentDidMount = function () {\n        // After we're rendered for the first time, tell Streamlit that our height\n        // has changed.\n        Streamlit.setFrameHeight();\n    };\n    StreamlitComponentBase.prototype.componentDidUpdate = function () {\n        // After we're updated, tell Streamlit that our height may have changed.\n        Streamlit.setFrameHeight();\n    };\n    return StreamlitComponentBase;\n}(React.PureComponent));\nexport { StreamlitComponentBase };\n/**\n * Wrapper for React-based Streamlit components.\n *\n * Bootstraps the communication interface between Streamlit and the component.\n */\nexport function withStreamlitConnection(WrappedComponent) {\n    var ComponentWrapper = /** @class */ (function (_super) {\n        __extends(ComponentWrapper, _super);\n        function ComponentWrapper(props) {\n            var _this = _super.call(this, props) || this;\n            _this.componentDidMount = function () {\n                // Set up event listeners, and signal to Streamlit that we're ready.\n                // We won't render the component until we receive the first RENDER_EVENT.\n                Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, _this.onRenderEvent);\n                Streamlit.setComponentReady();\n            };\n            _this.componentDidUpdate = function () {\n                // If our child threw an error, we display it in render(). In this\n                // case, the child won't be mounted and therefore won't call\n                // `setFrameHeight` on its own. We do it here so that the rendered\n                // error will be visible.\n                if (_this.state.componentError != null) {\n                    Streamlit.setFrameHeight();\n                }\n            };\n            _this.componentWillUnmount = function () {\n                Streamlit.events.removeEventListener(Streamlit.RENDER_EVENT, _this.onRenderEvent);\n            };\n            /**\n             * Streamlit is telling this component to redraw.\n             * We save the render data in State, so that it can be passed to the\n             * component in our own render() function.\n             */\n            _this.onRenderEvent = function (event) {\n                // Update our state with the newest render data\n                _this.setState({ renderData: event.detail });\n            };\n            _this.state = {\n                renderData: undefined,\n                componentError: undefined\n            };\n            return _this;\n        }\n        ComponentWrapper.prototype.render = function () {\n            // If our wrapped component threw an error, display it.\n            if (this.state.componentError != null) {\n                return (React.createElement(\"div\", null,\n                    React.createElement(\"h1\", null, \"Component Error\"),\n                    React.createElement(\"span\", null, this.state.componentError.message)));\n            }\n            // Don't render until we've gotten our first RENDER_EVENT from Streamlit.\n            if (this.state.renderData == null) {\n                return null;\n            }\n            return (React.createElement(WrappedComponent, { width: window.innerWidth, disabled: this.state.renderData.disabled, args: this.state.renderData.args, theme: this.state.renderData.theme }));\n        };\n        /**\n         * Error boundary function. This will be called if our wrapped\n         * component throws an error. We store the caught error in our state,\n         * and display it in the next render().\n         */\n        ComponentWrapper.getDerivedStateFromError = function (error) {\n            return { componentError: error };\n        };\n        return ComponentWrapper;\n    }(React.PureComponent));\n    return hoistNonReactStatics(ComponentWrapper, WrappedComponent);\n}\n",
-        "/*!\n* chartjs-plugin-zoom v2.0.1\n* undefined\n * (c) 2016-2023 chartjs-plugin-zoom Contributors\n * Released under the MIT License\n */\nimport Hammer from 'hammerjs';\nimport { each, valueOrDefault, callback, sign, getRelativePosition } from 'chart.js/helpers';\n\nconst getModifierKey = opts => opts && opts.enabled && opts.modifierKey;\nconst keyPressed = (key, event) => key && event[key + 'Key'];\nconst keyNotPressed = (key, event) => key && !event[key + 'Key'];\n\n/**\n * @param {string|function} mode can be 'x', 'y' or 'xy'\n * @param {string} dir can be 'x' or 'y'\n * @param {import('chart.js').Chart} chart instance of the chart in question\n * @returns {boolean}\n */\nfunction directionEnabled(mode, dir, chart) {\n  if (mode === undefined) {\n    return true;\n  } else if (typeof mode === 'string') {\n    return mode.indexOf(dir) !== -1;\n  } else if (typeof mode === 'function') {\n    return mode({chart}).indexOf(dir) !== -1;\n  }\n\n  return false;\n}\n\nfunction directionsEnabled(mode, chart) {\n  if (typeof mode === 'function') {\n    mode = mode({chart});\n  }\n  if (typeof mode === 'string') {\n    return {x: mode.indexOf('x') !== -1, y: mode.indexOf('y') !== -1};\n  }\n\n  return {x: false, y: false};\n}\n\n/**\n * Debounces calling `fn` for `delay` ms\n * @param {function} fn - Function to call. No arguments are passed.\n * @param {number} delay - Delay in ms. 0 = immediate invocation.\n * @returns {function}\n */\nfunction debounce(fn, delay) {\n  let timeout;\n  return function() {\n    clearTimeout(timeout);\n    timeout = setTimeout(fn, delay);\n    return delay;\n  };\n}\n\n/**\n * Checks which axis is under the mouse cursor.\n * @param {{x: number, y: number}} point - the mouse location\n * @param {import('chart.js').Chart} [chart] instance of the chart in question\n * @return {import('chart.js').Scale}\n */\nfunction getScaleUnderPoint({x, y}, chart) {\n  const scales = chart.scales;\n  const scaleIds = Object.keys(scales);\n  for (let i = 0; i < scaleIds.length; i++) {\n    const scale = scales[scaleIds[i]];\n    if (y >= scale.top && y <= scale.bottom && x >= scale.left && x <= scale.right) {\n      return scale;\n    }\n  }\n  return null;\n}\n\n/**\n * Evaluate the chart's mode, scaleMode, and overScaleMode properties to\n * determine which axes are eligible for scaling.\n * options.overScaleMode can be a function if user want zoom only one scale of many for example.\n * @param options - Zoom or pan options\n * @param {{x: number, y: number}} point - the mouse location\n * @param {import('chart.js').Chart} [chart] instance of the chart in question\n * @return {import('chart.js').Scale[]}\n */\nfunction getEnabledScalesByPoint(options, point, chart) {\n  const {mode = 'xy', scaleMode, overScaleMode} = options || {};\n  const scale = getScaleUnderPoint(point, chart);\n\n  const enabled = directionsEnabled(mode, chart);\n  const scaleEnabled = directionsEnabled(scaleMode, chart);\n\n  // Convert deprecated overScaleEnabled to new scaleEnabled.\n  if (overScaleMode) {\n    const overScaleEnabled = directionsEnabled(overScaleMode, chart);\n    for (const axis of ['x', 'y']) {\n      if (overScaleEnabled[axis]) {\n        scaleEnabled[axis] = enabled[axis];\n        enabled[axis] = false;\n      }\n    }\n  }\n\n  if (scale && scaleEnabled[scale.axis]) {\n    return [scale];\n  }\n\n  const enabledScales = [];\n  each(chart.scales, function(scaleItem) {\n    if (enabled[scaleItem.axis]) {\n      enabledScales.push(scaleItem);\n    }\n  });\n  return enabledScales;\n}\n\nconst chartStates = new WeakMap();\n\nfunction getState(chart) {\n  let state = chartStates.get(chart);\n  if (!state) {\n    state = {\n      originalScaleLimits: {},\n      updatedScaleLimits: {},\n      handlers: {},\n      panDelta: {}\n    };\n    chartStates.set(chart, state);\n  }\n  return state;\n}\n\nfunction removeState(chart) {\n  chartStates.delete(chart);\n}\n\nfunction zoomDelta(scale, zoom, center) {\n  const range = scale.max - scale.min;\n  const newRange = range * (zoom - 1);\n\n  const centerPoint = scale.isHorizontal() ? center.x : center.y;\n  // `scale.getValueForPixel()` can return a value less than the `scale.min` or\n  // greater than `scale.max` when `centerPoint` is outside chartArea.\n  const minPercent = Math.max(0, Math.min(1,\n    (scale.getValueForPixel(centerPoint) - scale.min) / range || 0\n  ));\n\n  const maxPercent = 1 - minPercent;\n\n  return {\n    min: newRange * minPercent,\n    max: newRange * maxPercent\n  };\n}\n\nfunction getLimit(state, scale, scaleLimits, prop, fallback) {\n  let limit = scaleLimits[prop];\n  if (limit === 'original') {\n    const original = state.originalScaleLimits[scale.id][prop];\n    limit = valueOrDefault(original.options, original.scale);\n  }\n  return valueOrDefault(limit, fallback);\n}\n\nfunction getRange(scale, pixel0, pixel1) {\n  const v0 = scale.getValueForPixel(pixel0);\n  const v1 = scale.getValueForPixel(pixel1);\n  return {\n    min: Math.min(v0, v1),\n    max: Math.max(v0, v1)\n  };\n}\n\nfunction updateRange(scale, {min, max}, limits, zoom = false) {\n  const state = getState(scale.chart);\n  const {id, axis, options: scaleOpts} = scale;\n\n  const scaleLimits = limits && (limits[id] || limits[axis]) || {};\n  const {minRange = 0} = scaleLimits;\n  const minLimit = getLimit(state, scale, scaleLimits, 'min', -Infinity);\n  const maxLimit = getLimit(state, scale, scaleLimits, 'max', Infinity);\n\n  const range = zoom ? Math.max(max - min, minRange) : scale.max - scale.min;\n  const offset = (range - max + min) / 2;\n  min -= offset;\n  max += offset;\n\n  if (min < minLimit) {\n    min = minLimit;\n    max = Math.min(minLimit + range, maxLimit);\n  } else if (max > maxLimit) {\n    max = maxLimit;\n    min = Math.max(maxLimit - range, minLimit);\n  }\n  scaleOpts.min = min;\n  scaleOpts.max = max;\n\n  state.updatedScaleLimits[scale.id] = {min, max};\n\n  // return true if the scale range is changed\n  return scale.parse(min) !== scale.min || scale.parse(max) !== scale.max;\n}\n\nfunction zoomNumericalScale(scale, zoom, center, limits) {\n  const delta = zoomDelta(scale, zoom, center);\n  const newRange = {min: scale.min + delta.min, max: scale.max - delta.max};\n  return updateRange(scale, newRange, limits, true);\n}\n\nfunction zoomRectNumericalScale(scale, from, to, limits) {\n  updateRange(scale, getRange(scale, from, to), limits, true);\n}\n\nconst integerChange = (v) => v === 0 || isNaN(v) ? 0 : v < 0 ? Math.min(Math.round(v), -1) : Math.max(Math.round(v), 1);\n\nfunction existCategoryFromMaxZoom(scale) {\n  const labels = scale.getLabels();\n  const maxIndex = labels.length - 1;\n\n  if (scale.min > 0) {\n    scale.min -= 1;\n  }\n  if (scale.max < maxIndex) {\n    scale.max += 1;\n  }\n}\n\nfunction zoomCategoryScale(scale, zoom, center, limits) {\n  const delta = zoomDelta(scale, zoom, center);\n  if (scale.min === scale.max && zoom < 1) {\n    existCategoryFromMaxZoom(scale);\n  }\n  const newRange = {min: scale.min + integerChange(delta.min), max: scale.max - integerChange(delta.max)};\n  return updateRange(scale, newRange, limits, true);\n}\n\nfunction scaleLength(scale) {\n  return scale.isHorizontal() ? scale.width : scale.height;\n}\n\nfunction panCategoryScale(scale, delta, limits) {\n  const labels = scale.getLabels();\n  const lastLabelIndex = labels.length - 1;\n  let {min, max} = scale;\n  // The visible range. Ticks can be skipped, and thus not reliable.\n  const range = Math.max(max - min, 1);\n  // How many pixels of delta is required before making a step. stepSize, but limited to max 1/10 of the scale length.\n  const stepDelta = Math.round(scaleLength(scale) / Math.max(range, 10));\n  const stepSize = Math.round(Math.abs(delta / stepDelta));\n  let applied;\n  if (delta < -stepDelta) {\n    max = Math.min(max + stepSize, lastLabelIndex);\n    min = range === 1 ? max : max - range;\n    applied = max === lastLabelIndex;\n  } else if (delta > stepDelta) {\n    min = Math.max(0, min - stepSize);\n    max = range === 1 ? min : min + range;\n    applied = min === 0;\n  }\n\n  return updateRange(scale, {min, max}, limits) || applied;\n}\n\nconst OFFSETS = {\n  second: 500, // 500 ms\n  minute: 30 * 1000, // 30 s\n  hour: 30 * 60 * 1000, // 30 m\n  day: 12 * 60 * 60 * 1000, // 12 h\n  week: 3.5 * 24 * 60 * 60 * 1000, // 3.5 d\n  month: 15 * 24 * 60 * 60 * 1000, // 15 d\n  quarter: 60 * 24 * 60 * 60 * 1000, // 60 d\n  year: 182 * 24 * 60 * 60 * 1000 // 182 d\n};\n\nfunction panNumericalScale(scale, delta, limits, canZoom = false) {\n  const {min: prevStart, max: prevEnd, options} = scale;\n  const round = options.time && options.time.round;\n  const offset = OFFSETS[round] || 0;\n  const newMin = scale.getValueForPixel(scale.getPixelForValue(prevStart + offset) - delta);\n  const newMax = scale.getValueForPixel(scale.getPixelForValue(prevEnd + offset) - delta);\n  const {min: minLimit = -Infinity, max: maxLimit = Infinity} = canZoom && limits && limits[scale.axis] || {};\n  if (isNaN(newMin) || isNaN(newMax) || newMin < minLimit || newMax > maxLimit) {\n    // At limit: No change but return true to indicate no need to store the delta.\n    // NaN can happen for 0-dimension scales (either because they were configured\n    // with min === max or because the chart has 0 plottable area).\n    return true;\n  }\n  return updateRange(scale, {min: newMin, max: newMax}, limits, canZoom);\n}\n\nfunction panNonLinearScale(scale, delta, limits) {\n  return panNumericalScale(scale, delta, limits, true);\n}\n\nconst zoomFunctions = {\n  category: zoomCategoryScale,\n  default: zoomNumericalScale,\n};\n\nconst zoomRectFunctions = {\n  default: zoomRectNumericalScale,\n};\n\nconst panFunctions = {\n  category: panCategoryScale,\n  default: panNumericalScale,\n  logarithmic: panNonLinearScale,\n  timeseries: panNonLinearScale,\n};\n\nfunction shouldUpdateScaleLimits(scale, originalScaleLimits, updatedScaleLimits) {\n  const {id, options: {min, max}} = scale;\n  if (!originalScaleLimits[id] || !updatedScaleLimits[id]) {\n    return true;\n  }\n  const previous = updatedScaleLimits[id];\n  return previous.min !== min || previous.max !== max;\n}\n\nfunction removeMissingScales(limits, scales) {\n  each(limits, (opt, key) => {\n    if (!scales[key]) {\n      delete limits[key];\n    }\n  });\n}\n\nfunction storeOriginalScaleLimits(chart, state) {\n  const {scales} = chart;\n  const {originalScaleLimits, updatedScaleLimits} = state;\n\n  each(scales, function(scale) {\n    if (shouldUpdateScaleLimits(scale, originalScaleLimits, updatedScaleLimits)) {\n      originalScaleLimits[scale.id] = {\n        min: {scale: scale.min, options: scale.options.min},\n        max: {scale: scale.max, options: scale.options.max},\n      };\n    }\n  });\n\n  removeMissingScales(originalScaleLimits, scales);\n  removeMissingScales(updatedScaleLimits, scales);\n  return originalScaleLimits;\n}\n\nfunction doZoom(scale, amount, center, limits) {\n  const fn = zoomFunctions[scale.type] || zoomFunctions.default;\n  callback(fn, [scale, amount, center, limits]);\n}\n\nfunction doZoomRect(scale, amount, from, to, limits) {\n  const fn = zoomRectFunctions[scale.type] || zoomRectFunctions.default;\n  callback(fn, [scale, amount, from, to, limits]);\n}\n\nfunction getCenter(chart) {\n  const ca = chart.chartArea;\n  return {\n    x: (ca.left + ca.right) / 2,\n    y: (ca.top + ca.bottom) / 2,\n  };\n}\n\n/**\n * @param chart The chart instance\n * @param {number | {x?: number, y?: number, focalPoint?: {x: number, y: number}}} amount The zoom percentage or percentages and focal point\n * @param {string} [transition] Which transition mode to use. Defaults to 'none'\n */\nfunction zoom(chart, amount, transition = 'none') {\n  const {x = 1, y = 1, focalPoint = getCenter(chart)} = typeof amount === 'number' ? {x: amount, y: amount} : amount;\n  const state = getState(chart);\n  const {options: {limits, zoom: zoomOptions}} = state;\n\n  storeOriginalScaleLimits(chart, state);\n\n  const xEnabled = x !== 1;\n  const yEnabled = y !== 1;\n  const enabledScales = getEnabledScalesByPoint(zoomOptions, focalPoint, chart);\n\n  each(enabledScales || chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      doZoom(scale, x, focalPoint, limits);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      doZoom(scale, y, focalPoint, limits);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(zoomOptions.onZoom, [{chart}]);\n}\n\nfunction zoomRect(chart, p0, p1, transition = 'none') {\n  const state = getState(chart);\n  const {options: {limits, zoom: zoomOptions}} = state;\n  const {mode = 'xy'} = zoomOptions;\n\n  storeOriginalScaleLimits(chart, state);\n  const xEnabled = directionEnabled(mode, 'x', chart);\n  const yEnabled = directionEnabled(mode, 'y', chart);\n\n  each(chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      doZoomRect(scale, p0.x, p1.x, limits);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      doZoomRect(scale, p0.y, p1.y, limits);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(zoomOptions.onZoom, [{chart}]);\n}\n\nfunction zoomScale(chart, scaleId, range, transition = 'none') {\n  storeOriginalScaleLimits(chart, getState(chart));\n  const scale = chart.scales[scaleId];\n  updateRange(scale, range, undefined, true);\n  chart.update(transition);\n}\n\nfunction resetZoom(chart, transition = 'default') {\n  const state = getState(chart);\n  const originalScaleLimits = storeOriginalScaleLimits(chart, state);\n\n  each(chart.scales, function(scale) {\n    const scaleOptions = scale.options;\n    if (originalScaleLimits[scale.id]) {\n      scaleOptions.min = originalScaleLimits[scale.id].min.options;\n      scaleOptions.max = originalScaleLimits[scale.id].max.options;\n    } else {\n      delete scaleOptions.min;\n      delete scaleOptions.max;\n    }\n  });\n  chart.update(transition);\n  callback(state.options.zoom.onZoomComplete, [{chart}]);\n}\n\nfunction getOriginalRange(state, scaleId) {\n  const original = state.originalScaleLimits[scaleId];\n  if (!original) {\n    return;\n  }\n  const {min, max} = original;\n  return valueOrDefault(max.options, max.scale) - valueOrDefault(min.options, min.scale);\n}\n\nfunction getZoomLevel(chart) {\n  const state = getState(chart);\n  let min = 1;\n  let max = 1;\n  each(chart.scales, function(scale) {\n    const origRange = getOriginalRange(state, scale.id);\n    if (origRange) {\n      const level = Math.round(origRange / (scale.max - scale.min) * 100) / 100;\n      min = Math.min(min, level);\n      max = Math.max(max, level);\n    }\n  });\n  return min < 1 ? min : max;\n}\n\nfunction panScale(scale, delta, limits, state) {\n  const {panDelta} = state;\n  // Add possible cumulative delta from previous pan attempts where scale did not change\n  const storedDelta = panDelta[scale.id] || 0;\n  if (sign(storedDelta) === sign(delta)) {\n    delta += storedDelta;\n  }\n  const fn = panFunctions[scale.type] || panFunctions.default;\n  if (callback(fn, [scale, delta, limits])) {\n    // The scale changed, reset cumulative delta\n    panDelta[scale.id] = 0;\n  } else {\n    // The scale did not change, store cumulative delta\n    panDelta[scale.id] = delta;\n  }\n}\n\nfunction pan(chart, delta, enabledScales, transition = 'none') {\n  const {x = 0, y = 0} = typeof delta === 'number' ? {x: delta, y: delta} : delta;\n  const state = getState(chart);\n  const {options: {pan: panOptions, limits}} = state;\n  const {onPan} = panOptions || {};\n\n  storeOriginalScaleLimits(chart, state);\n\n  const xEnabled = x !== 0;\n  const yEnabled = y !== 0;\n\n  each(enabledScales || chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      panScale(scale, x, limits, state);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      panScale(scale, y, limits, state);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(onPan, [{chart}]);\n}\n\nfunction getInitialScaleBounds(chart) {\n  const state = getState(chart);\n  storeOriginalScaleLimits(chart, state);\n  const scaleBounds = {};\n  for (const scaleId of Object.keys(chart.scales)) {\n    const {min, max} = state.originalScaleLimits[scaleId] || {min: {}, max: {}};\n    scaleBounds[scaleId] = {min: min.scale, max: max.scale};\n  }\n\n  return scaleBounds;\n}\n\nfunction isZoomedOrPanned(chart) {\n  const scaleBounds = getInitialScaleBounds(chart);\n  for (const scaleId of Object.keys(chart.scales)) {\n    const {min: originalMin, max: originalMax} = scaleBounds[scaleId];\n\n    if (originalMin !== undefined && chart.scales[scaleId].min !== originalMin) {\n      return true;\n    }\n\n    if (originalMax !== undefined && chart.scales[scaleId].max !== originalMax) {\n      return true;\n    }\n  }\n\n  return false;\n}\n\nfunction removeHandler(chart, type) {\n  const {handlers} = getState(chart);\n  const handler = handlers[type];\n  if (handler && handler.target) {\n    handler.target.removeEventListener(type, handler);\n    delete handlers[type];\n  }\n}\n\nfunction addHandler(chart, target, type, handler) {\n  const {handlers, options} = getState(chart);\n  const oldHandler = handlers[type];\n  if (oldHandler && oldHandler.target === target) {\n    // already attached\n    return;\n  }\n  removeHandler(chart, type);\n  handlers[type] = (event) => handler(chart, event, options);\n  handlers[type].target = target;\n  target.addEventListener(type, handlers[type]);\n}\n\nfunction mouseMove(chart, event) {\n  const state = getState(chart);\n  if (state.dragStart) {\n    state.dragging = true;\n    state.dragEnd = event;\n    chart.update('none');\n  }\n}\n\nfunction keyDown(chart, event) {\n  const state = getState(chart);\n  if (!state.dragStart || event.key !== 'Escape') {\n    return;\n  }\n\n  removeHandler(chart, 'keydown');\n  state.dragging = false;\n  state.dragStart = state.dragEnd = null;\n  chart.update('none');\n}\n\nfunction zoomStart(chart, event, zoomOptions) {\n  const {onZoomStart, onZoomRejected} = zoomOptions;\n  if (onZoomStart) {\n    const point = getRelativePosition(event, chart);\n    if (callback(onZoomStart, [{chart, event, point}]) === false) {\n      callback(onZoomRejected, [{chart, event}]);\n      return false;\n    }\n  }\n}\n\nfunction mouseDown(chart, event) {\n  const state = getState(chart);\n  const {pan: panOptions, zoom: zoomOptions = {}} = state.options;\n  if (\n    event.button !== 0 ||\n    keyPressed(getModifierKey(panOptions), event) ||\n    keyNotPressed(getModifierKey(zoomOptions.drag), event)\n  ) {\n    return callback(zoomOptions.onZoomRejected, [{chart, event}]);\n  }\n\n  if (zoomStart(chart, event, zoomOptions) === false) {\n    return;\n  }\n  state.dragStart = event;\n\n  addHandler(chart, chart.canvas, 'mousemove', mouseMove);\n  addHandler(chart, window.document, 'keydown', keyDown);\n}\n\nfunction computeDragRect(chart, mode, beginPointEvent, endPointEvent) {\n  const xEnabled = directionEnabled(mode, 'x', chart);\n  const yEnabled = directionEnabled(mode, 'y', chart);\n  let {top, left, right, bottom, width: chartWidth, height: chartHeight} = chart.chartArea;\n\n  const beginPoint = getRelativePosition(beginPointEvent, chart);\n  const endPoint = getRelativePosition(endPointEvent, chart);\n\n  if (xEnabled) {\n    left = Math.min(beginPoint.x, endPoint.x);\n    right = Math.max(beginPoint.x, endPoint.x);\n  }\n\n  if (yEnabled) {\n    top = Math.min(beginPoint.y, endPoint.y);\n    bottom = Math.max(beginPoint.y, endPoint.y);\n  }\n  const width = right - left;\n  const height = bottom - top;\n\n  return {\n    left,\n    top,\n    right,\n    bottom,\n    width,\n    height,\n    zoomX: xEnabled && width ? 1 + ((chartWidth - width) / chartWidth) : 1,\n    zoomY: yEnabled && height ? 1 + ((chartHeight - height) / chartHeight) : 1\n  };\n}\n\nfunction mouseUp(chart, event) {\n  const state = getState(chart);\n  if (!state.dragStart) {\n    return;\n  }\n\n  removeHandler(chart, 'mousemove');\n  const {mode, onZoomComplete, drag: {threshold = 0}} = state.options.zoom;\n  const rect = computeDragRect(chart, mode, state.dragStart, event);\n  const distanceX = directionEnabled(mode, 'x', chart) ? rect.width : 0;\n  const distanceY = directionEnabled(mode, 'y', chart) ? rect.height : 0;\n  const distance = Math.sqrt(distanceX * distanceX + distanceY * distanceY);\n\n  // Remove drag start and end before chart update to stop drawing selected area\n  state.dragStart = state.dragEnd = null;\n\n  if (distance <= threshold) {\n    state.dragging = false;\n    chart.update('none');\n    return;\n  }\n\n  zoomRect(chart, {x: rect.left, y: rect.top}, {x: rect.right, y: rect.bottom}, 'zoom');\n\n  setTimeout(() => (state.dragging = false), 500);\n  callback(onZoomComplete, [{chart}]);\n}\n\nfunction wheelPreconditions(chart, event, zoomOptions) {\n  // Before preventDefault, check if the modifier key required and pressed\n  if (keyNotPressed(getModifierKey(zoomOptions.wheel), event)) {\n    callback(zoomOptions.onZoomRejected, [{chart, event}]);\n    return;\n  }\n\n  if (zoomStart(chart, event, zoomOptions) === false) {\n    return;\n  }\n\n  // Prevent the event from triggering the default behavior (e.g. content scrolling).\n  if (event.cancelable) {\n    event.preventDefault();\n  }\n\n  // Firefox always fires the wheel event twice:\n  // First without the delta and right after that once with the delta properties.\n  if (event.deltaY === undefined) {\n    return;\n  }\n  return true;\n}\n\nfunction wheel(chart, event) {\n  const {handlers: {onZoomComplete}, options: {zoom: zoomOptions}} = getState(chart);\n\n  if (!wheelPreconditions(chart, event, zoomOptions)) {\n    return;\n  }\n\n  const rect = event.target.getBoundingClientRect();\n  const speed = 1 + (event.deltaY >= 0 ? -zoomOptions.wheel.speed : zoomOptions.wheel.speed);\n  const amount = {\n    x: speed,\n    y: speed,\n    focalPoint: {\n      x: event.clientX - rect.left,\n      y: event.clientY - rect.top\n    }\n  };\n\n  zoom(chart, amount);\n\n  if (onZoomComplete) {\n    onZoomComplete();\n  }\n}\n\nfunction addDebouncedHandler(chart, name, handler, delay) {\n  if (handler) {\n    getState(chart).handlers[name] = debounce(() => callback(handler, [{chart}]), delay);\n  }\n}\n\nfunction addListeners(chart, options) {\n  const canvas = chart.canvas;\n  const {wheel: wheelOptions, drag: dragOptions, onZoomComplete} = options.zoom;\n\n  // Install listeners. Do this dynamically based on options so that we can turn zoom on and off\n  // We also want to make sure listeners aren't always on. E.g. if you're scrolling down a page\n  // and the mouse goes over a chart you don't want it intercepted unless the plugin is enabled\n  if (wheelOptions.enabled) {\n    addHandler(chart, canvas, 'wheel', wheel);\n    addDebouncedHandler(chart, 'onZoomComplete', onZoomComplete, 250);\n  } else {\n    removeHandler(chart, 'wheel');\n  }\n  if (dragOptions.enabled) {\n    addHandler(chart, canvas, 'mousedown', mouseDown);\n    addHandler(chart, canvas.ownerDocument, 'mouseup', mouseUp);\n  } else {\n    removeHandler(chart, 'mousedown');\n    removeHandler(chart, 'mousemove');\n    removeHandler(chart, 'mouseup');\n    removeHandler(chart, 'keydown');\n  }\n}\n\nfunction removeListeners(chart) {\n  removeHandler(chart, 'mousedown');\n  removeHandler(chart, 'mousemove');\n  removeHandler(chart, 'mouseup');\n  removeHandler(chart, 'wheel');\n  removeHandler(chart, 'click');\n  removeHandler(chart, 'keydown');\n}\n\nfunction createEnabler(chart, state) {\n  return function(recognizer, event) {\n    const {pan: panOptions, zoom: zoomOptions = {}} = state.options;\n    if (!panOptions || !panOptions.enabled) {\n      return false;\n    }\n    const srcEvent = event && event.srcEvent;\n    if (!srcEvent) { // Sometimes Hammer queries this with a null event.\n      return true;\n    }\n    if (!state.panning && event.pointerType === 'mouse' && (\n      keyNotPressed(getModifierKey(panOptions), srcEvent) || keyPressed(getModifierKey(zoomOptions.drag), srcEvent))\n    ) {\n      callback(panOptions.onPanRejected, [{chart, event}]);\n      return false;\n    }\n    return true;\n  };\n}\n\nfunction pinchAxes(p0, p1) {\n  // fingers position difference\n  const pinchX = Math.abs(p0.clientX - p1.clientX);\n  const pinchY = Math.abs(p0.clientY - p1.clientY);\n\n  // diagonal fingers will change both (xy) axes\n  const p = pinchX / pinchY;\n  let x, y;\n  if (p > 0.3 && p < 1.7) {\n    x = y = true;\n  } else if (pinchX > pinchY) {\n    x = true;\n  } else {\n    y = true;\n  }\n  return {x, y};\n}\n\nfunction handlePinch(chart, state, e) {\n  if (state.scale) {\n    const {center, pointers} = e;\n    // Hammer reports the total scaling. We need the incremental amount\n    const zoomPercent = 1 / state.scale * e.scale;\n    const rect = e.target.getBoundingClientRect();\n    const pinch = pinchAxes(pointers[0], pointers[1]);\n    const mode = state.options.zoom.mode;\n    const amount = {\n      x: pinch.x && directionEnabled(mode, 'x', chart) ? zoomPercent : 1,\n      y: pinch.y && directionEnabled(mode, 'y', chart) ? zoomPercent : 1,\n      focalPoint: {\n        x: center.x - rect.left,\n        y: center.y - rect.top\n      }\n    };\n\n    zoom(chart, amount);\n\n    // Keep track of overall scale\n    state.scale = e.scale;\n  }\n}\n\nfunction startPinch(chart, state) {\n  if (state.options.zoom.pinch.enabled) {\n    state.scale = 1;\n  }\n}\n\nfunction endPinch(chart, state, e) {\n  if (state.scale) {\n    handlePinch(chart, state, e);\n    state.scale = null; // reset\n    callback(state.options.zoom.onZoomComplete, [{chart}]);\n  }\n}\n\nfunction handlePan(chart, state, e) {\n  const delta = state.delta;\n  if (delta) {\n    state.panning = true;\n    pan(chart, {x: e.deltaX - delta.x, y: e.deltaY - delta.y}, state.panScales);\n    state.delta = {x: e.deltaX, y: e.deltaY};\n  }\n}\n\nfunction startPan(chart, state, event) {\n  const {enabled, onPanStart, onPanRejected} = state.options.pan;\n  if (!enabled) {\n    return;\n  }\n  const rect = event.target.getBoundingClientRect();\n  const point = {\n    x: event.center.x - rect.left,\n    y: event.center.y - rect.top\n  };\n\n  if (callback(onPanStart, [{chart, event, point}]) === false) {\n    return callback(onPanRejected, [{chart, event}]);\n  }\n\n  state.panScales = getEnabledScalesByPoint(state.options.pan, point, chart);\n  state.delta = {x: 0, y: 0};\n  clearTimeout(state.panEndTimeout);\n  handlePan(chart, state, event);\n}\n\nfunction endPan(chart, state) {\n  state.delta = null;\n  if (state.panning) {\n    state.panEndTimeout = setTimeout(() => (state.panning = false), 500);\n    callback(state.options.pan.onPanComplete, [{chart}]);\n  }\n}\n\nconst hammers = new WeakMap();\nfunction startHammer(chart, options) {\n  const state = getState(chart);\n  const canvas = chart.canvas;\n  const {pan: panOptions, zoom: zoomOptions} = options;\n\n  const mc = new Hammer.Manager(canvas);\n  if (zoomOptions && zoomOptions.pinch.enabled) {\n    mc.add(new Hammer.Pinch());\n    mc.on('pinchstart', () => startPinch(chart, state));\n    mc.on('pinch', (e) => handlePinch(chart, state, e));\n    mc.on('pinchend', (e) => endPinch(chart, state, e));\n  }\n\n  if (panOptions && panOptions.enabled) {\n    mc.add(new Hammer.Pan({\n      threshold: panOptions.threshold,\n      enable: createEnabler(chart, state)\n    }));\n    mc.on('panstart', (e) => startPan(chart, state, e));\n    mc.on('panmove', (e) => handlePan(chart, state, e));\n    mc.on('panend', () => endPan(chart, state));\n  }\n\n  hammers.set(chart, mc);\n}\n\nfunction stopHammer(chart) {\n  const mc = hammers.get(chart);\n  if (mc) {\n    mc.remove('pinchstart');\n    mc.remove('pinch');\n    mc.remove('pinchend');\n    mc.remove('panstart');\n    mc.remove('pan');\n    mc.remove('panend');\n    mc.destroy();\n    hammers.delete(chart);\n  }\n}\n\nvar version = \"2.0.1\";\n\nfunction draw(chart, caller, options) {\n  const dragOptions = options.zoom.drag;\n  const {dragStart, dragEnd} = getState(chart);\n\n  if (dragOptions.drawTime !== caller || !dragEnd) {\n    return;\n  }\n  const {left, top, width, height} = computeDragRect(chart, options.zoom.mode, dragStart, dragEnd);\n  const ctx = chart.ctx;\n\n  ctx.save();\n  ctx.beginPath();\n  ctx.fillStyle = dragOptions.backgroundColor || 'rgba(225,225,225,0.3)';\n  ctx.fillRect(left, top, width, height);\n\n  if (dragOptions.borderWidth > 0) {\n    ctx.lineWidth = dragOptions.borderWidth;\n    ctx.strokeStyle = dragOptions.borderColor || 'rgba(225,225,225)';\n    ctx.strokeRect(left, top, width, height);\n  }\n  ctx.restore();\n}\n\nvar plugin = {\n  id: 'zoom',\n\n  version,\n\n  defaults: {\n    pan: {\n      enabled: false,\n      mode: 'xy',\n      threshold: 10,\n      modifierKey: null,\n    },\n    zoom: {\n      wheel: {\n        enabled: false,\n        speed: 0.1,\n        modifierKey: null\n      },\n      drag: {\n        enabled: false,\n        drawTime: 'beforeDatasetsDraw',\n        modifierKey: null\n      },\n      pinch: {\n        enabled: false\n      },\n      mode: 'xy',\n    }\n  },\n\n  start: function(chart, _args, options) {\n    const state = getState(chart);\n    state.options = options;\n\n    if (Object.prototype.hasOwnProperty.call(options.zoom, 'enabled')) {\n      console.warn('The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`.');\n    }\n    if (Object.prototype.hasOwnProperty.call(options.zoom, 'overScaleMode')\n      || Object.prototype.hasOwnProperty.call(options.pan, 'overScaleMode')) {\n      console.warn('The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired).');\n    }\n\n    if (Hammer) {\n      startHammer(chart, options);\n    }\n\n    chart.pan = (delta, panScales, transition) => pan(chart, delta, panScales, transition);\n    chart.zoom = (args, transition) => zoom(chart, args, transition);\n    chart.zoomRect = (p0, p1, transition) => zoomRect(chart, p0, p1, transition);\n    chart.zoomScale = (id, range, transition) => zoomScale(chart, id, range, transition);\n    chart.resetZoom = (transition) => resetZoom(chart, transition);\n    chart.getZoomLevel = () => getZoomLevel(chart);\n    chart.getInitialScaleBounds = () => getInitialScaleBounds(chart);\n    chart.isZoomedOrPanned = () => isZoomedOrPanned(chart);\n  },\n\n  beforeEvent(chart) {\n    const state = getState(chart);\n    if (state.panning || state.dragging) {\n      // cancel any event handling while panning or dragging\n      return false;\n    }\n  },\n\n  beforeUpdate: function(chart, args, options) {\n    const state = getState(chart);\n    state.options = options;\n    addListeners(chart, options);\n  },\n\n  beforeDatasetsDraw(chart, _args, options) {\n    draw(chart, 'beforeDatasetsDraw', options);\n  },\n\n  afterDatasetsDraw(chart, _args, options) {\n    draw(chart, 'afterDatasetsDraw', options);\n  },\n\n  beforeDraw(chart, _args, options) {\n    draw(chart, 'beforeDraw', options);\n  },\n\n  afterDraw(chart, _args, options) {\n    draw(chart, 'afterDraw', options);\n  },\n\n  stop: function(chart) {\n    removeListeners(chart);\n\n    if (Hammer) {\n      stopHammer(chart);\n    }\n    removeState(chart);\n  },\n\n  panFunctions,\n  zoomFunctions,\n  zoomRectFunctions,\n};\n\nexport { plugin as default, pan, resetZoom, zoom, zoomRect, zoomScale };\n",
-        "import React from \"react\"\r\nimport { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport { Line, getElementAtEvent } from \"react-chartjs-2\"\r\nimport {\r\n  Streamlit,\r\n  StreamlitComponentBase,\r\n  withStreamlitConnection,\r\n} from \"streamlit-component-lib\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass DraggableLineChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.state = {\r\n      activePoint: null,\r\n      chartData: this.createChartData(\r\n        props.args.data,\r\n        props.args.options.colors\r\n      ),\r\n      options: this.createOptions(props.args.options),\r\n    }\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        chartData: this.createChartData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: this.createOptions(this.props.args.options),\r\n      })\r\n    }\r\n  }\r\n\r\n  createChartData(data, options) {\r\n    const datasets = Object.entries(data).map(([colName, colData], index) => {\r\n      const data = Object.values(colData)\r\n      return {\r\n        data,\r\n        label: colName,\r\n        fill: false,\r\n        lineTension: 0.3,\r\n        cubicInterpolationMode: \"monotone\",\r\n      }\r\n    })\r\n\r\n    if (options.colors) {\r\n      datasets.forEach((dataset, index) => {\r\n        dataset.backgroundColor = options.colors[index]\r\n        dataset.borderColor = options.colors[index]\r\n      })\r\n    }\r\n\r\n    return {\r\n      labels: Object.keys(data.Col1),\r\n      datasets: datasets,\r\n    }\r\n  }\r\n\r\n  createOptions(options) {\r\n    return {\r\n      responsive: true,\r\n      animation: {\r\n        duration: 0,\r\n      },\r\n      tooltips: {\r\n        mode: \"nearest\",\r\n      },\r\n      onHover: (event, chartElement) => {\r\n        if (chartElement.length > 0) {\r\n          event.native.target.style.cursor = \"crosshair\"\r\n        } else {\r\n          event.native.target.style.cursor = \"default\"\r\n        }\r\n      },\r\n      plugins: {\r\n        zoom: {\r\n          zoom: {\r\n            wheel: {\r\n              enabled: true,\r\n            },\r\n            mode: \"x\",\r\n          },\r\n          pan: {\r\n            enabled: false,\r\n          },\r\n        },\r\n        title: {\r\n          display: true,\r\n          text: options.title,\r\n        },\r\n        legend: {\r\n          onHover: (event, legendItem, legend) => {\r\n            if (legendItem) {\r\n              event.native.target.style.cursor = \"pointer\"\r\n            } else {\r\n              event.native.target.style.cursor = \"default\"\r\n            }\r\n          },\r\n        },\r\n      },\r\n      scales: {\r\n        x: {\r\n          display: true,\r\n          title: {\r\n            display: true,\r\n            text: options.x_label,\r\n          },\r\n        },\r\n        y: {\r\n          display: true,\r\n          title: {\r\n            display: true,\r\n            text: options.y_label,\r\n          },\r\n        },\r\n      },\r\n    }\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      this.setState({ activePoint: points[0] })\r\n    }\r\n  }\r\n\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const data = this.chartRef.current.data.datasets.reduce(\r\n        (acc, dataset) => {\r\n          const colData = dataset.data.reduce((colAcc, value, index) => {\r\n            colAcc[this.state.chartData.labels[index]] = value\r\n            return colAcc\r\n          }, {})\r\n          acc[dataset.label] = colData\r\n          return acc\r\n        },\r\n        {}\r\n      )\r\n\r\n      Streamlit.setComponentValue(data)\r\n    }\r\n    this.setState({ activePoint: null })\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const position = getRelativePosition(event, this.chartRef.current)\r\n      const chartArea = chart.chartArea\r\n      const yAxis = chart.scales.y\r\n      const yValue = this.map(\r\n        position.y,\r\n        chartArea.bottom,\r\n        chartArea.top,\r\n        yAxis.min,\r\n        yAxis.max\r\n      )\r\n      chart.data.datasets[this.state.activePoint.datasetIndex].data[\r\n        this.state.activePoint.index\r\n      ] = yValue\r\n      chart.update()\r\n    }\r\n  }\r\n\r\n  map = (value, start1, stop1, start2, stop2) => {\r\n    return start2 + (stop2 - start2) * ((value - start1) / (stop1 - start1))\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Line\r\n        ref={this.chartRef}\r\n        data={this.state.chartData}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default withStreamlitConnection(DraggableLineChart)\r\n",
+        "export function createChartData(data, options) {\r\n  const datasets = Object.entries(data).map(([colName, colData], index) => {\r\n    const data = Object.values(colData)\r\n    return {\r\n      data,\r\n      label: colName,\r\n      fill: false,\r\n      lineTension: 0.3,\r\n      cubicInterpolationMode: \"monotone\",\r\n    }\r\n  })\r\n\r\n  if (options && options.colors) {\r\n    datasets.forEach((dataset, index) => {\r\n      dataset.backgroundColor = options.colors[index]\r\n      dataset.borderColor = options.colors[index]\r\n    })\r\n  }\r\n\r\n  return {\r\n    labels: Object.keys(data.Col1),\r\n    datasets: datasets,\r\n  }\r\n}\r\n",
+        "export function createOptions(options, theme) {\r\n  return {\r\n    responsive: true,\r\n    animation: {\r\n      duration: 0,\r\n    },\r\n    tooltips: {\r\n      mode: \"nearest\",\r\n    },\r\n    onHover: createHoverOptions(),\r\n    plugins: {\r\n      zoom: createZoomOptions(),\r\n      title: createTitleOptions(options),\r\n      legend: createLegendOptions(),\r\n    },\r\n    scales: createScalesOptions(options, theme),\r\n  }\r\n}\r\n\r\nfunction createHoverOptions() {\r\n  return (event, chartElement) => {\r\n    if (chartElement.length > 0) {\r\n      event.native.target.style.cursor = \"crosshair\"\r\n    } else {\r\n      event.native.target.style.cursor = \"default\"\r\n    }\r\n  }\r\n}\r\n\r\nfunction createZoomOptions() {\r\n  return {\r\n    zoom: {\r\n      wheel: {\r\n        enabled: true,\r\n      },\r\n      mode: \"x\",\r\n    },\r\n    pan: {\r\n      enabled: false,\r\n    },\r\n  }\r\n}\r\n\r\nfunction createTitleOptions(options) {\r\n  return {\r\n    display: true,\r\n    text: options.title,\r\n  }\r\n}\r\n\r\nfunction createLegendOptions() {\r\n  return {\r\n    onHover: (event, legendItem, legend) => {\r\n      if (legendItem) {\r\n        event.native.target.style.cursor = \"pointer\"\r\n      } else {\r\n        event.native.target.style.cursor = \"default\"\r\n      }\r\n    },\r\n  }\r\n}\r\n\r\nfunction createScalesOptions(options, theme) {\r\n  return {\r\n    x: {\r\n      display: true,\r\n      title: {\r\n        display: true,\r\n        text: options.x_label,\r\n      },\r\n      grid: {\r\n        display: options.x_grid,\r\n        color: theme.fadedText05\r\n      },\r\n    },\r\n    y: {\r\n      display: true,\r\n      title: {\r\n        display: true,\r\n        text: options.y_label,\r\n      },\r\n      grid: {\r\n        display: options.y_grid,\r\n        color: theme.fadedText05\r\n      },\r\n    },\r\n  }\r\n}\r\n",
+        "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\nimport { Line, getElementAtEvent } from \"react-chartjs-2\"\r\nimport {\r\n  Streamlit,\r\n  StreamlitComponentBase,\r\n  withStreamlitConnection,\r\n} from \"streamlit-component-lib\"\r\nimport { createChartData } from \"./chartData\"\r\nimport { createOptions } from \"./chartOptions\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass DraggableLineChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.state = {\r\n      activePoint: null,\r\n      chartData: createChartData(props.args.data, props.args.options.colors),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        chartData: createChartData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      this.setState({ activePoint: points[0] })\r\n    }\r\n  }\r\n\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const data = this.chartRef.current.data.datasets.reduce(\r\n        (acc, dataset) => {\r\n          const colData = dataset.data.reduce((colAcc, value, index) => {\r\n            colAcc[this.state.chartData.labels[index]] = value\r\n            return colAcc\r\n          }, {})\r\n          acc[dataset.label] = colData\r\n          return acc\r\n        },\r\n        {}\r\n      )\r\n\r\n      Streamlit.setComponentValue(data)\r\n    }\r\n    this.setState({ activePoint: null })\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const position = getRelativePosition(event, this.chartRef.current)\r\n      const chartArea = chart.chartArea\r\n      const yAxis = chart.scales.y\r\n      const yValue = this.map(\r\n        position.y,\r\n        chartArea.bottom,\r\n        chartArea.top,\r\n        yAxis.min,\r\n        yAxis.max\r\n      )\r\n      chart.data.datasets[this.state.activePoint.datasetIndex].data[\r\n        this.state.activePoint.index\r\n      ] = yValue\r\n      chart.update()\r\n    }\r\n  }\r\n\r\n  map = (value, start1, stop1, start2, stop2) => {\r\n    return start2 + (stop2 - start2) * ((value - start1) / (stop1 - start1))\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Line\r\n        ref={this.chartRef}\r\n        data={this.state.chartData}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default withStreamlitConnection(DraggableLineChart)\r\n",
         "import React from \"react\"\r\nimport ReactDOM from \"react-dom\"\r\nimport DraggableLinechart from \"./DraggableLineChart\"\r\n\r\nReactDOM.render(\r\n  <React.StrictMode>\r\n    <DraggableLinechart />\r\n  </React.StrictMode>,\r\n  document.getElementById(\"root\")\r\n)\r\n"
     ],
     "version": 3
 }
```

### Comparing `draggable-line-chart-0.1.0/draggable_line_chart.egg-info/PKG-INFO` & `draggable-line-chart-0.2.0/draggable_line_chart.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-line-chart
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Streamlit component that displays a line chart with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.
 Home-page: 
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
@@ -38,11 +38,13 @@
 
 
 plot_options = {
     "title": "My Plot",
     "colors": ['#1f77b4', '#ff7f0e', '#2ca02c'],
     "x_label": "X Axis",
     "y_label": "Y Axis",
+    "x_grid": True,
+    "y_grid": True,
 }
 new_data = draggable_line_chart(data=initial_data.to_dict(), options=plot_options)
 new_data
 ```
```

### Comparing `draggable-line-chart-0.1.0/draggable_line_chart.egg-info/SOURCES.txt` & `draggable-line-chart-0.2.0/draggable_line_chart.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 draggable_line_chart.egg-info/SOURCES.txt
 draggable_line_chart.egg-info/dependency_links.txt
 draggable_line_chart.egg-info/requires.txt
 draggable_line_chart.egg-info/top_level.txt
 draggable_line_chart/frontend/build/asset-manifest.json
 draggable_line_chart/frontend/build/bootstrap.min.css
 draggable_line_chart/frontend/build/index.html
-draggable_line_chart/frontend/build/static/js/main.a519b502.js
-draggable_line_chart/frontend/build/static/js/main.a519b502.js.LICENSE.txt
-draggable_line_chart/frontend/build/static/js/main.a519b502.js.map
+draggable_line_chart/frontend/build/static/js/main.8e0bbc33.js
+draggable_line_chart/frontend/build/static/js/main.8e0bbc33.js.LICENSE.txt
+draggable_line_chart/frontend/build/static/js/main.8e0bbc33.js.map
```

### Comparing `draggable-line-chart-0.1.0/setup.py` & `draggable-line-chart-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="draggable-line-chart",
-    version="0.1.0",
+    version="0.2.0",
     author="Brayan Munoz",
     author_email="balexander.munoz@udea.edu.co",
     description="A Streamlit component that displays a line chart with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```
