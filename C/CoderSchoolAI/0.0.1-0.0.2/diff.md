# Comparing `tmp/CoderSchoolAI-0.0.1.tar.gz` & `tmp/CoderSchoolAI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoderSchoolAI-0.0.1.tar", last modified: Sun Jun  4 12:54:56 2023, max compression
+gzip compressed data, was "CoderSchoolAI-0.0.2.tar", last modified: Sun Jun  4 13:48:35 2023, max compression
```

## Comparing `CoderSchoolAI-0.0.1.tar` & `CoderSchoolAI-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 12:54:56.941165 CoderSchoolAI-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-04 12:54:56.770168 CoderSchoolAI-0.0.1/CoderSchoolAI/
-drwxrwxrwx   0        0        0        0 2023-06-04 12:54:56.750670 CoderSchoolAI-0.0.1/CoderSchoolAI/Assets/
-drwxrwxrwx   0        0        0        0 2023-06-04 12:54:56.810163 CoderSchoolAI-0.0.1/CoderSchoolAI/Assets/CoderSchoolAI/
--rw-rw-rw-   0        0        0   143548 2023-05-26 14:42:41.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Assets/CoderSchoolAI/CoderSchoolAI-Logo.png
-drwxrwxrwx   0        0        0        0 2023-06-04 12:54:56.847167 CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/
--rw-rw-rw-   0        0        0     4420 2023-05-24 16:35:17.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/Agent.py
--rw-rw-rw-   0        0        0     3057 2023-05-18 18:22:36.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/Attributes.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:54:56.862165 CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/CoderSchoolEnvironments/
--rw-rw-rw-   0        0        0    18664 2023-06-04 03:36:59.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/CoderSchoolEnvironments/SnakeEnvironment.py
--rw-rw-rw-   0        0        0        0 2023-05-12 04:23:34.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/CoderSchoolEnvironments/__init__.py
--rw-rw-rw-   0        0        0     6696 2023-05-27 19:21:43.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/Shell.py
--rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:54:56.889168 CoderSchoolAI-0.0.1/CoderSchoolAI/Neural/
--rw-rw-rw-   0        0        0     1661 2023-05-23 05:50:30.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Neural/Block.py
--rw-rw-rw-   0        0        0        0 2023-05-18 17:47:49.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Neural/Net.py
--rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Neural/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:54:56.908165 CoderSchoolAI-0.0.1/CoderSchoolAI/Training/
--rw-rw-rw-   0        0        0     6527 2023-05-26 16:55:20.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Training/Algorithms.py
--rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Training/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:54:56.938166 CoderSchoolAI-0.0.1/CoderSchoolAI/Util/
--rw-rw-rw-   0        0        0        0 2023-05-12 04:04:54.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Util/__init__.py
--rw-rw-rw-   0        0        0     1010 2023-05-12 05:33:20.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Util/data_utils.py
--rw-rw-rw-   0        0        0      524 2023-05-12 03:04:18.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/Util/misc_utils.py
--rw-rw-rw-   0        0        0     1779 2023-05-15 01:01:24.000000 CoderSchoolAI-0.0.1/CoderSchoolAI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:54:56.792167 CoderSchoolAI-0.0.1/CoderSchoolAI.egg-info/
--rw-rw-rw-   0        0        0      397 2023-06-04 12:54:56.000000 CoderSchoolAI-0.0.1/CoderSchoolAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      838 2023-06-04 12:54:56.000000 CoderSchoolAI-0.0.1/CoderSchoolAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 12:54:56.000000 CoderSchoolAI-0.0.1/CoderSchoolAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 12:54:56.000000 CoderSchoolAI-0.0.1/CoderSchoolAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 12:54:56.000000 CoderSchoolAI-0.0.1/CoderSchoolAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      183 2023-05-26 14:30:52.000000 CoderSchoolAI-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      397 2023-06-04 12:54:56.940165 CoderSchoolAI-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-10 01:13:09.000000 CoderSchoolAI-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-04 12:54:56.942166 CoderSchoolAI-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      597 2023-05-26 06:28:14.000000 CoderSchoolAI-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.817320 CoderSchoolAI-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.742370 CoderSchoolAI-0.0.2/CoderSchoolAI/
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.726319 CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.767320 CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/CoderSchoolAI/
+-rw-rw-rw-   0        0        0   143548 2023-05-26 14:42:41.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/CoderSchoolAI/CoderSchoolAI-Logo.png
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.771319 CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/Snake/
+-rw-rw-rw-   0        0        0    42206 2023-06-04 13:26:34.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/Snake/Apple.png
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.779319 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/
+-rw-rw-rw-   0        0        0     4420 2023-05-24 16:35:17.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Agent.py
+-rw-rw-rw-   0        0        0     3057 2023-05-18 18:22:36.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Attributes.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.788346 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/CoderSchoolEnvironments/
+-rw-rw-rw-   0        0        0    19236 2023-06-04 13:45:33.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/CoderSchoolEnvironments/SnakeEnvironment.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 04:23:34.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/CoderSchoolEnvironments/__init__.py
+-rw-rw-rw-   0        0        0     6696 2023-05-27 19:21:43.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Shell.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.797318 CoderSchoolAI-0.0.2/CoderSchoolAI/Neural/
+-rw-rw-rw-   0        0        0     1661 2023-05-23 05:50:30.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Neural/Block.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 17:47:49.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Neural/Net.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Neural/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.803321 CoderSchoolAI-0.0.2/CoderSchoolAI/Training/
+-rw-rw-rw-   0        0        0     6527 2023-05-26 16:55:20.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Training/Algorithms.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Training/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.809320 CoderSchoolAI-0.0.2/CoderSchoolAI/Util/
+-rw-rw-rw-   0        0        0        0 2023-05-12 04:04:54.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Util/__init__.py
+-rw-rw-rw-   0        0        0     1010 2023-05-12 05:33:20.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Util/data_utils.py
+-rw-rw-rw-   0        0        0      524 2023-05-12 03:04:18.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Util/misc_utils.py
+-rw-rw-rw-   0        0        0     1781 2023-06-04 13:02:10.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.813325 CoderSchoolAI-0.0.2/CoderSchoolAI/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-04 13:42:40.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/cli/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-06-04 13:24:08.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/cli/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.765320 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      970 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      183 2023-05-26 14:30:52.000000 CoderSchoolAI-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      397 2023-06-04 13:48:35.815317 CoderSchoolAI-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-10 01:13:09.000000 CoderSchoolAI-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 13:48:35.817320 CoderSchoolAI-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      724 2023-06-04 13:47:50.000000 CoderSchoolAI-0.0.2/setup.py
```

### Comparing `CoderSchoolAI-0.0.1/CoderSchoolAI/Assets/CoderSchoolAI/CoderSchoolAI-Logo.png` & `CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/CoderSchoolAI/CoderSchoolAI-Logo.png`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/Agent.py` & `CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Agent.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/Attributes.py` & `CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Attributes.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/CoderSchoolEnvironments/SnakeEnvironment.py` & `CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/CoderSchoolEnvironments/SnakeEnvironment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pkg_resources
 import sys
 import numpy as np
 from typing import List, Tuple, Dict, Any, Optional, Union, Callable
 '''
 For more information regarding Spaces, see https://gym.openai.com/docs/spaces/
 '''
 import pygame
@@ -200,15 +201,18 @@
         
         # Initialize game_state attributes, internal variables, and callbacks
         self.game_state = np.zeros((height, width, 1), dtype=np.float32)
         self.__last_moving_direction = SnakeAgent.SnakeAction.RIGHT
         self.apple_position = self.spawn_new_apple()
         self._apples_consumed = 0
         self._soft_reset = False
-        
+        apple_res = pkg_resources.resource_filename('CoderSchoolAI', 'Assets/Snake/Apple.png')
+        self.apple_asset = pygame.image.load(apple_res).convert()
+        self.apple_asset = pygame.transform.scale(self.apple_asset, (self.cell_size, self.cell_size))
+
         """Register the Attributes"""
         # Game State Attribute
         self.register_attribute(ObsAttribute(name="game_state", 
         # Number of parameters in the environment to be trained on x height of image x width of image. In this case we are only training on object types.
                                              space= BoxType(shape=(1, height, width), low=0, high=1, dtype=np.float32), 
                                              update_func=self.__update_game_state_callback))
         if self.verbose:
@@ -335,32 +339,37 @@
     def render_env(self):
         """
         Renders the Snake Game to the screen Via PyGame.
         """
         if not self.console_only:
             #Fills the world with the Blank Color
             self.screen.fill(self.WORLD_COLOR)
-            for i in range(self.width):  # Assuming grid_size is the number of cells
-                pygame.draw.line(self.screen, (255, 255, 255), (i * self.cell_size, 0), (i * self.cell_size, self.width * self.cell_size))  # Vertical lines
-            for i in range(self.width):  # Assuming grid_size is the number of cells
-                pygame.draw.line(self.screen, (255, 255, 255), (0, i * self.cell_size), (self.height * self.cell_size, i * self.cell_size))  # Horizontal lines
             # Draw the game state
             for pos in self.snake_agent.body:
                     rect = pygame.Rect(pos[0] * self.cell_size, pos[1] * self.cell_size, self.cell_size, self.cell_size)
                     pygame.draw.rect(self.screen, self.BODY_COLOR, rect)
 
             # Draw the head of the snake
             head_position = self.snake_agent.body[-1]
             rect = pygame.Rect(head_position[0] * self.cell_size, head_position[1] * self.cell_size, self.cell_size, self.cell_size)
             pygame.draw.rect(self.screen, self.HEAD_COLOR, rect)
 
             # Draw the apple
-            rect = pygame.Rect(self.apple_position[0] * self.cell_size, self.apple_position[1] * self.cell_size, self.cell_size, self.cell_size)
-            pygame.draw.rect(self.screen, self.APPLE_COLOR, rect)
-
+            # rect = pygame.Rect(self.apple_position[0] * self.cell_size, self.apple_position[1] * self.cell_size, self.cell_size, self.cell_size)
+            # pygame.draw.rect(self.screen, self.APPLE_COLOR, rect)
+            apple_rect = self.apple_asset.get_rect()
+            apple_rect.topleft = (self.apple_position[0]*self.cell_size, self.apple_position[1]*self.cell_size)
+            self.screen.blit(self.apple_asset, apple_rect)
+            
+            # Draw the grid Lines
+            for i in range(self.width):  # Assuming grid_size is the number of cells
+                pygame.draw.line(self.screen, (255, 255, 255), (i * self.cell_size, 0), (i * self.cell_size, self.width * self.cell_size))  # Vertical lines
+            for i in range(self.width):  # Assuming grid_size is the number of cells
+                pygame.draw.line(self.screen, (255, 255, 255), (0, i * self.cell_size), (self.height * self.cell_size, i * self.cell_size))  # Horizontal lines
+            
             #Draw the score
             score_text = self.font.render(f'Score: {self._apples_consumed}', True, (225, 220, 128))
             self.screen.blit(score_text, (self.width * self.cell_size - score_text.get_width() - 5, 5))  # Draw the score on the top right corner
 
             pygame.display.flip()
             pygame.display.update()
```

### Comparing `CoderSchoolAI-0.0.1/CoderSchoolAI/Environment/Shell.py` & `CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Shell.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.1/CoderSchoolAI/Neural/Block.py` & `CoderSchoolAI-0.0.2/CoderSchoolAI/Neural/Block.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.1/CoderSchoolAI/Training/Algorithms.py` & `CoderSchoolAI-0.0.2/CoderSchoolAI/Training/Algorithms.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.1/CoderSchoolAI/Util/data_utils.py` & `CoderSchoolAI-0.0.2/CoderSchoolAI/Util/data_utils.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.1/CoderSchoolAI/Util/misc_utils.py` & `CoderSchoolAI-0.0.2/CoderSchoolAI/Util/misc_utils.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.1/CoderSchoolAI/__init__.py` & `CoderSchoolAI-0.0.2/CoderSchoolAI/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
 Development Environment: 
 
 Contribution Guidelines:
 
 """
 
-__version__ = '0.0.1'
+__version__ = '0.0.1'
```

### Comparing `CoderSchoolAI-0.0.1/CoderSchoolAI.egg-info/SOURCES.txt` & `CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 MANIFEST.in
 README.md
 setup.py
 CoderSchoolAI/__init__.py
 CoderSchoolAI.egg-info/PKG-INFO
 CoderSchoolAI.egg-info/SOURCES.txt
 CoderSchoolAI.egg-info/dependency_links.txt
+CoderSchoolAI.egg-info/entry_points.txt
 CoderSchoolAI.egg-info/requires.txt
 CoderSchoolAI.egg-info/top_level.txt
 CoderSchoolAI/Assets/CoderSchoolAI/CoderSchoolAI-Logo.png
+CoderSchoolAI/Assets/Snake/Apple.png
 CoderSchoolAI/Environment/Agent.py
 CoderSchoolAI/Environment/Attributes.py
 CoderSchoolAI/Environment/Shell.py
 CoderSchoolAI/Environment/__init__.py
 CoderSchoolAI/Environment/CoderSchoolEnvironments/SnakeEnvironment.py
 CoderSchoolAI/Environment/CoderSchoolEnvironments/__init__.py
 CoderSchoolAI/Neural/Block.py
 CoderSchoolAI/Neural/Net.py
 CoderSchoolAI/Neural/__init__.py
 CoderSchoolAI/Training/Algorithms.py
 CoderSchoolAI/Training/__init__.py
 CoderSchoolAI/Util/__init__.py
 CoderSchoolAI/Util/data_utils.py
-CoderSchoolAI/Util/misc_utils.py
+CoderSchoolAI/Util/misc_utils.py
+CoderSchoolAI/cli/__init__.py
+CoderSchoolAI/cli/cli.py
```

### Comparing `CoderSchoolAI-0.0.1/setup.py` & `CoderSchoolAI-0.0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CoderSchoolAI',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     include_package_data=True,
     description='A Comprehensive Python Library for Creating and Developing Agent AIs.',
+    entry_points={
+        'console_scripts': [
+            'coderschoolai = CoderSchoolAI.cli.cli:main'
+        ]
+    },
     author='Jonathan Koch, ',
     author_email='johnnykoch002@example.com, ',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
     ],
```

