# Comparing `tmp/py_astrolab-0.6.8.tar.gz` & `tmp/py_astrolab-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.6.8.tar", max compression
+gzip compressed data, was "py_astrolab-0.6.9.tar", max compression
```

## Comparing `py_astrolab-0.6.8.tar` & `py_astrolab-0.6.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.8/README.md
--rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.8/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.8/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.8/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    80189 2023-08-04 16:28:34.232678 py_astrolab-0.6.8/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.8/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.8/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.8/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.8/py_astrolab/charts/wonderful_mistake.py
--rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.8/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.8/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.8/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.8/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.8/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.8/py_astrolab/report.py
--rwxr-xr-x   0        0        0    18590 2023-08-02 18:39:26.606720 py_astrolab-0.6.8/py_astrolab/transits.py
--rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.8/py_astrolab/types.py
--rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.8/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      664 2023-08-05 08:58:13.186740 py_astrolab-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.8/PKG-INFO
+-rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.9/README.md
+-rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.9/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    15760 2023-08-05 16:48:33.637644 py_astrolab-0.6.9/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.9/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    81152 2023-08-05 17:25:42.772461 py_astrolab-0.6.9/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.9/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.9/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.9/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.9/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.9/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12401 2023-08-05 08:59:16.353294 py_astrolab-0.6.9/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.9/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.9/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.9/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.9/py_astrolab/report.py
+-rwxr-xr-x   0        0        0    18772 2023-08-05 16:24:05.463756 py_astrolab-0.6.9/py_astrolab/transits.py
+-rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.9/py_astrolab/types.py
+-rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.9/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      664 2023-08-05 17:26:28.665862 py_astrolab-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.9/PKG-INFO
```

### Comparing `py_astrolab-0.6.8/py_astrolab/__init__.py` & `py_astrolab-0.6.9/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/aspects.py` & `py_astrolab-0.6.9/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.6.9/py_astrolab/charts/charts_svg.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,16 +265,16 @@
         # get color configuration
 
         # Immediately generate template.
         self.template = self.makeTemplate()
 
     # draw transit ring
     def __transitRing(self, r):
-        out = '<circle cx="%s" cy="%s" r="%s" style="fill: none; stroke: %s; stroke-width: 36px; stroke-opacity: 1;"/>' % (
-            r, r, r-18, self.colors_settings['paper_1'])
+        out = '<circle class="transitRing" cx="%s" cy="%s" r="%s" style="fill: none; stroke: %s; stroke-width: 36px; stroke-opacity: 1;"/>' % (
+            r, r, r-18, self.colors_settings['paper_2'])
         out += '<circle cx="%s" cy="%s" r="%s" style="fill: none; stroke: %s; stroke-width: 1px; stroke-opacity: .6;"/>' % (
             r, r, r, self.colors_settings['zodiac_transit_ring_3'])
         return out
 
     # draw degree ring
     def __degreeRing(self, r):
         out = ''
@@ -380,14 +380,15 @@
         orb = aspect_dict['orbit'] if not isAxis else None
         offset = (int(self.houses_degree_ut[6]) / -1) + int(degA)
         x1 = self.__sliceToX(0, ar, offset) + (r - ar)
         y1 = self.__sliceToY(0, ar, offset) + (r - ar)
         offset = (int(self.houses_degree_ut[6]) / -1) + int(degB)
         x2 = self.__sliceToX(0, ar, offset) + (r - ar)
         y2 = self.__sliceToY(0, ar, offset) + (r - ar)
+        stroke_opacity = '0' if self.chart_type == 'Transit' else '1'
         if isAxis:
             width = x2 - x1
             height = y2 - y1
             start = {'x': x1, 'y': y1}
             end = {'x': x2, 'y': y2}
             cut_by = 8.4
             ratio = width / cut_by
@@ -395,15 +396,15 @@
             lastCut = {'x': start['x'] + (cut_by - 1) * ratio, 'y': start['y'] + (height / width) * (cut_by - 1) * ratio }
             label = 'Asc' if 'Ascendant' in aspect_id else 'Mc'
             add_arrow = f'marker-start: url(#arrowhead{label});'
         else:
             add_arrow = ''
         if isAxis:
             axis_stroke_width = '2.5'
-            axis_stroke_opacity = '1'
+            axis_stroke_opacity = '.8'
             line = f'''
                 <g class="axis" id="{aspect_id}" style="stroke-width: {axis_stroke_width}; stroke-opacity: {axis_stroke_opacity}; transform: translate(0, 0);" stroke-linecap="round" >
                     <line x1="{start["x"]}" y1="{start["y"]}" x2="{firstCut["x"]}" y2="{firstCut["y"]}" style="stroke: {color}; {add_arrow}" />
                     <line x1="{firstCut["x"]}" y1="{firstCut["y"]}" x2="{lastCut["x"]}" y2="{lastCut["y"]}" style="stroke: none; stroke-opacity: 0;" />
                     <line x1="{lastCut["x"]}" y1="{lastCut["y"]}" x2="{end["x"]}" y2="{end["y"]}" style="stroke: {color};"/>
                 </g>
             '''
@@ -412,15 +413,15 @@
                 width_max = 5
                 width_min = 1
                 max_orb = 5
                 aspect_stroke_width = max(width_min, min(width_max, width_max - (abs(orb) / max_orb) * (width_max - width_min)))
             else:
                 aspect_stroke_width = '1.5'
             line = f'<line class="aspect" id="{aspect_id}" x1="' + str(x1) + '" y1="' + str(y1) + '" x2="' + str(x2) + '" y2="' + str(
-                y2) + '" style="stroke: ' + color + f'; stroke-width: {aspect_stroke_width}; stroke-opacity: 1;" stroke-linecap="round" />'
+                y2) + '" style="stroke: ' + color + f'; stroke-width: {aspect_stroke_width}; stroke-opacity: {stroke_opacity};" stroke-linecap="round" />'
         if not isAxis:
             mid_x = (x1 + x2) / 2
             mid_y = (y1 + y2) / 2
             dx = x2 - x1
             dy = y2 - y1
             angle = math.atan2(dy, dx) * 180 / math.pi
             if angle < 0:
@@ -936,15 +937,15 @@
                 planet_y = self.__sliceToY(0, (r+rplanet), t_offset)
                 output = output + f'<g><g id="{self.planets_settings[i]["name"].title()}GTransit" transform="scale(0.9) translate(15, 15)"><use x="' + str(planet_x) + '" y="' + str(planet_y) + '" xlink:href="#' + self.planets_settings[i]['name'] + '" /></g></g>'
                 # transit planet line
                 x1 = self.__sliceToX(0, r+3, t_offset) - 3
                 y1 = self.__sliceToY(0, r+3, t_offset) - 3
                 x2 = self.__sliceToX(0, r-3, t_offset) + 3
                 y2 = self.__sliceToY(0, r-3, t_offset) + 3
-                output = output + '<line x1="'+str(x1)+'" y1="'+str(y1)+'" x2="'+str(x2)+'" y2="'+str(
+                output = output + f'<line id="{self.planets_settings[i]["name"].title()}GTransitLine" x1="'+str(x1)+'" y1="'+str(y1)+'" x2="'+str(x2)+'" y2="'+str(
                     y2)+'" style="stroke: black'+'; stroke-width: 1px; stroke-opacity:.8;"/>'
 
                 # transit planet degree text
                 rotate = self.houses_degree_ut[0] - self.t_planets_degree_ut[i]
                 textanchor = "end"
                 t_offset += group_offset[i]
                 rtext = -3.0
@@ -958,16 +959,15 @@
 
                 if textanchor == "end":
                     xo = 1
                 else:
                     xo = -1
                 deg_x = self.__sliceToX(0, (r-rtext), t_offset + xo) + rtext
                 deg_y = self.__sliceToY(0, (r-rtext), t_offset + xo) + rtext
-                degree = int(t_offset)
-                output += '<g transform="translate(%s,%s)">' % (deg_x, deg_y)
+                output += f'<g id="{self.planets_settings[i]["name"].title()}GTransitLineText" transform="translate({deg_x}, {deg_y})">'
                 output += '<text transform="rotate(%s)" text-anchor="%s' % (
                     rotate, textanchor)
                 output += '" style="fill: black' + \
                     '; font-size: 10px;">' + \
                     self.__dec2deg(self.t_planets_degree[i], type="1")
                 output += '</text></g>'
 
@@ -1286,20 +1286,21 @@
         out += '<text y="36" style="fill:#630e73; font-size: 10px;">' + \
             self.language_settings['water']+' '+str(pw)+'%</text>'
         out += '</g>'
         return out
 
     def __makeAxis(self, r, ar):
         out = ''
+        axis_stroke_opacity = '.8'
         for axis in self.user.axis_list:
             if axis.name in {'Ascendant', 'Midheaven'}:
                 axis_data = next((ax for ax in self.axes_settings if ax['name'] == axis.name), None)
                 arrow_top = f'''
                     <marker id="arrowhead{axis_data['label_short']}" markerWidth="12" markerHeight="12" refX="6" refY="6" orient="auto-start-reverse">
-                        <polyline points="0,2 6,6 0,10" style="fill: none; stroke: {axis_data['color']};" />
+                        <polyline points="0,2 6,6 0,10" style="fill: none; stroke: {axis_data['color']}; stroke-opacity: {axis_stroke_opacity}" />
                     </marker>
                 '''
                 if axis_data:
                     axis_id = f"{axis_data['label_short'].replace('Asc', 'Ascendant').replace('Mc', 'Midheaven')}G"
                     aspect_dict = {
                         'p1_abs_pos': axis.abs_pos,
                         'p2_abs_pos': (axis.abs_pos + 180) % 360,
@@ -1310,14 +1311,26 @@
                     if self.chart_type == 'Transit' or self.chart_type == 'Composite':
                         c1 = self.c3 - 49
                         c2 = self.c3 + 40
                     else:
                         c1 = self.c2
                         c2 = self.c3
                     out += self.drawTick(c1, c2, r, axis.name, offset)
+        if self.chart_type == 'Transit':
+            for axis in self.t_user.axis_list:
+                if axis.name in {'Ascendant', 'Midheaven'}:
+                    axis_data = next((ax for ax in self.axes_settings if ax['name'] == axis.name), None)
+                    if axis_data:
+                        axis_id = f"{axis_data['label_short'].replace('Asc', 'Ascendant').replace('Mc', 'Midheaven')}GTransit"
+                        aspect_dict = {
+                            'p1_abs_pos': axis.abs_pos,
+                            'p2_abs_pos': (axis.abs_pos + 180) % 360,
+                            'color': axis_data['color'],
+                        }
+                        out += arrow_top + self.__drawAspect(r, r-self.c1+29, aspect_dict, axis_id, True)
         return out
 
     def drawTick(self, c1, c2, r, id, offset) -> str:
         out = ''
         for c in [c1, c2]:
             # Calculate the start and end points of the tick mark
             tick_start_x = self.__sliceToX(0, r-c, offset) + c
@@ -1562,19 +1575,17 @@
             td['c2'] = 'class="circle" id="c2" cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-72) + '"'
             td['c2style'] = 'fill: %s; fill-opacity: 1; stroke: %s; stroke-opacity:.4; stroke-width: 1px' % (
                 self.colors_settings['paper_1'], self.colors_settings['zodiac_transit_ring_1'])
             td['c3'] = 'class="circle" id="c3" cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-160) + '"'
             td['c3style'] = 'fill: %s; fill-opacity: 1; stroke: %s; stroke-width: 1px' % (
-                self.colors_settings['paper_2'], self.colors_settings['zodiac_transit_ring_0'])
-            td['makeAspects'] = ''
-            td['makeAspectGrid'] = ''
-            # td['makeAspects'] = self.__makeAspectsTransit(r, (r-160))
-            # td['makeAspectGrid'] = self.__makeAspectTransitGrid(r)
+                self.colors_settings['paper_1'], self.colors_settings['zodiac_transit_ring_0'])
+            td['makeAspects'] = self.__makeAspectsTransit(r, (r-160))
+            td['makeAspectGrid'] = self.__makeAspectTransitGrid(r)
             td['makePatterns'] = ''
             td['makeAxis'] = self.__makeAxis(r, (r-self.c1-18))
             td['chart_width'] = self.full_width
         else:
             td['transitRing'] = ""
             if self.chart_type == 'minimal':
                 td['degreeRing'] = ''
```

### Comparing `py_astrolab-0.6.8/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.6.9/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.6.9/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.6.9/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.6.9/py_astrolab/charts/wonderful_mistake.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/fetch_geonames.py` & `py_astrolab-0.6.9/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/main.py` & `py_astrolab-0.6.9/py_astrolab/main.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/print_all_data.py` & `py_astrolab-0.6.9/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/relationship_score.py` & `py_astrolab-0.6.9/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/report.py` & `py_astrolab-0.6.9/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/transits.py` & `py_astrolab-0.6.9/py_astrolab/transits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime, timedelta
-from itertools import combinations, product
+from itertools import product
 from typing import Union
 
 import swisseph as swe
 
 from py_astrolab import KrInstance
 
 
@@ -337,10 +337,14 @@
             'house': self.point_in_house(moon_longitude)
         }
         return output
 
     def point_in_house(self, point_long):
         for house in self.user.houses_list:
             lower_bound = house['abs_pos']
-            upper_bound = house['abs_pos'] + 30
-            if lower_bound <= point_long < upper_bound:
-                return house['name']
+            upper_bound = (house['abs_pos'] + 30) % 360
+            if lower_bound <= upper_bound:
+                if lower_bound <= point_long < upper_bound:
+                    return house['name']
+            else:
+                if point_long >= lower_bound or point_long < upper_bound:
+                    return house['name']
```

### Comparing `py_astrolab-0.6.8/py_astrolab/types.py` & `py_astrolab-0.6.9/py_astrolab/types.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/py_astrolab/utilities.py` & `py_astrolab-0.6.9/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.8/pyproject.toml` & `py_astrolab-0.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.6.8"
+version = "0.6.9"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.6.8/PKG-INFO` & `py_astrolab-0.6.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.6.8
+Version: 0.6.9
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

