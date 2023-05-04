# Comparing `tmp/violet-simulator-0.2.2.tar.gz` & `tmp/violet_simulator-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "violet-simulator-0.2.2.tar", max compression
+gzip compressed data, was "violet_simulator-0.2.3.tar", last modified: Thu May  4 14:45:33 2023, max compression
```

## Comparing `violet-simulator-0.2.2.tar` & `violet_simulator-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1073 2022-06-03 12:50:50.829791 violet-simulator-0.2.2/LICENSE
--rw-r--r--   0        0        0     1259 2022-06-05 13:12:31.964851 violet-simulator-0.2.2/README.md
--rw-r--r--   0        0        0      769 2022-06-13 17:32:42.314894 violet-simulator-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6216 2022-06-05 13:12:31.965460 violet-simulator-0.2.2/vi/__init__.py
--rw-r--r--   0        0        0      649 2022-06-11 13:44:21.082397 violet-simulator-0.2.2/vi/_static.py
--rw-r--r--   0        0        0    20201 2022-06-13 17:34:46.112976 violet-simulator-0.2.2/vi/agent.py
--rw-r--r--   0        0        0    16127 2022-06-13 17:34:46.113407 violet-simulator-0.2.2/vi/config.py
--rw-r--r--   0        0        0     1151 2022-06-11 11:55:32.622674 violet-simulator-0.2.2/vi/metrics.py
--rw-r--r--   0        0        0    10566 2022-06-13 17:34:46.113767 violet-simulator-0.2.2/vi/proximity.py
--rw-r--r--   0        0        0     2535 2022-05-28 20:41:14.428020 violet-simulator-0.2.2/vi/replay.py
--rw-r--r--   0        0        0    15468 2022-06-13 17:34:46.114132 violet-simulator-0.2.2/vi/simulation.py
--rw-r--r--   0        0        0     1355 2022-06-09 21:33:37.333645 violet-simulator-0.2.2/vi/util.py
--rw-r--r--   0        0        0     2067 2022-06-13 17:34:55.124052 violet-simulator-0.2.2/setup.py
--rw-r--r--   0        0        0     2060 2022-06-13 17:34:55.124258 violet-simulator-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-04 10:04:14.538843 violet_simulator-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1250 2023-05-04 11:07:23.861471 violet_simulator-0.2.3/README.md
+-rw-r--r--   0        0        0     1100 2023-05-04 14:45:33.685229 violet_simulator-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6215 2023-05-04 11:55:19.107727 violet_simulator-0.2.3/vi/__init__.py
+-rw-r--r--   0        0        0      754 2023-05-04 11:56:20.032548 violet_simulator-0.2.3/vi/_static.py
+-rw-r--r--   0        0        0    20219 2023-05-04 11:47:40.841524 violet_simulator-0.2.3/vi/agent.py
+-rw-r--r--   0        0        0    16075 2023-05-04 11:53:52.918788 violet_simulator-0.2.3/vi/config.py
+-rw-r--r--   0        0        0     9734 2023-05-04 10:58:54.083770 violet_simulator-0.2.3/vi/metrics.py
+-rw-r--r--   0        0        0    10571 2023-05-04 11:45:47.034248 violet_simulator-0.2.3/vi/proximity.py
+-rw-r--r--   0        0        0     2536 2023-05-04 11:33:22.900862 violet_simulator-0.2.3/vi/replay.py
+-rw-r--r--   0        0        0    15462 2023-05-04 11:47:49.827135 violet_simulator-0.2.3/vi/simulation.py
+-rw-r--r--   0        0        0     1430 2023-05-04 11:56:40.310462 violet_simulator-0.2.3/vi/util.py
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 violet_simulator-0.2.3/PKG-INFO
```

### Comparing `violet-simulator-0.2.2/LICENSE` & `violet_simulator-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `violet-simulator-0.2.2/README.md` & `violet_simulator-0.2.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 Install the latest version of Violet with:
 
 ```bash
 pip3 install -U violet-simulator
 ```
 
-Or with [Poetry](https://python-poetry.org):
+Or with [PDM](https://pdm.fming.dev):
 
 ```bash
-poetry add violet-simulator
+pdm add violet-simulator
 ```
 
 ## Example
 
 ```python
 from vi import Agent, Simulation
 
@@ -38,8 +38,8 @@
     # Step 2: Add 100 agents to the simulation.
     .batch_spawn_agents(100, Agent, images=["examples/images/white.png"])
     # Step 3: Profit! 🎉
     .run()
 )
 ```
 
-For more information you can check the [documentation](https://api.violet.m-rots.com), [examples](https://github.com/m-rots/violet/tree/main/examples) and the [User Guide](https://violet.m-rots.com).
+For more information you can check the [documentation](https://api.violet.m-rots.com), [examples](https://github.com/m-rots/violet/tree/main/examples) and the [User Guide](https://violet.m-rots.com).
```

### Comparing `violet-simulator-0.2.2/vi/__init__.py` & `violet_simulator-0.2.3/vi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
 And there we have it!
 A disco of a simulation with agents swapping colours whenever they get close to someone.
 
 Now, there's way more to explore.
 But this should give you an impression on how to change the behaviour of your agents with Violet.
 Explore some of the modules on the left and experiment away!
 """
-
 from dataclasses import dataclass
 
 from pygame.math import Vector2
 from serde.de import deserialize
 from serde.se import serialize
 
 from .agent import Agent
```

### Comparing `violet-simulator-0.2.2/vi/_static.py` & `violet_simulator-0.2.3/vi/_static.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 import pygame as pg
-from pygame.mask import Mask
-from pygame.math import Vector2
-from pygame.rect import Rect
 from pygame.sprite import Group, Sprite
-from pygame.surface import Surface
 
 from .util import round_pos
 
 
+if TYPE_CHECKING:
+    from pygame.mask import Mask
+    from pygame.math import Vector2
+    from pygame.rect import Rect
+    from pygame.surface import Surface
+
 class _StaticSprite(Sprite):
     id: int
 
     image: Surface
     rect: Rect
     mask: Mask
```

### Comparing `violet-simulator-0.2.2/vi/agent.py` & `violet_simulator-0.2.3/vi/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 
 from __future__ import annotations
 
 from copy import copy
 from typing import TYPE_CHECKING, Any, Generator, Optional
 
 import pygame as pg
-from pygame.mask import Mask
 from pygame.math import Vector2
-from pygame.rect import Rect
 from pygame.sprite import Group, Sprite
-from pygame.surface import Surface
-from typing_extensions import Self
 
-from .config import Config
-from .proximity import ProximityIter
 from .util import random_angle, random_pos, round_pos
 
+
 if TYPE_CHECKING:
+    from pygame.mask import Mask
+    from pygame.rect import Rect
+    from pygame.surface import Surface
+    from typing_extensions import Self
+
     from ._static import _StaticSprite
+    from .config import Config
+    from .proximity import ProximityIter
     from .simulation import HeadlessSimulation, Shared
 
 
 class Agent(Sprite):
     """
     The `Agent` class is home to Violet's various additions and is
     built on top of [PyGame's Sprite](https://www.pygame.org/docs/ref/sprite.html) class.
@@ -41,15 +43,15 @@
     """
 
     id: int
     """The unique identifier of the agent."""
 
     config: Config
     """The config of the simulation that's shared with all agents.
-    
+
     The config can be overriden when inheriting the Agent class.
     However, the config must always:
 
     1. Inherit `Config`
     2. Be decorated by `@deserialize` and `@dataclass`
     """
 
@@ -74,15 +76,15 @@
     Instead, you should manually add the move delta to `pos`, like so:
 
     >>> self.pos += self.move
 
     The vector `Vector2(2, 1)` indicates that the agent will be moving 2 pixels along the x axis
     and 1 pixel along the y axis.
     You can use the `Vector2` class to calculate the agent's velocity by calling `length`.
-    
+
     This property is also used to automatically rotate the agent's image
     when `vi.config.Schema.image_rotation` is enabled.
     """
 
     pos: Vector2
     """The current (centre) position of the agent."""
```

### Comparing `violet-simulator-0.2.2/vi/config.py` & `violet_simulator-0.2.3/vi/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import Any, Generic, Optional, Type, TypeVar, Union
 
 from serde.de import deserialize
 from serde.se import serialize
 from serde.toml import from_toml
@@ -33,28 +35,25 @@
                     combinations.append({key: value})
 
             # Single value
             elif values is not None:
                 combinations.append({key: values})
 
         # If we have a list of dicts, we can simply add our key!
-        else:
-            # Multiple values
-            if isinstance(values, list):
-                original_length = len(combinations)
-                _embiggen(combinations, len(values))
-
-                for index, entry in enumerate(combinations):
-                    value_index = index // original_length
-                    entry[key] = values[value_index]
-
-            # Single value
-            elif values is not None:
-                for entry in combinations:
-                    entry[key] = values
+        elif isinstance(values, list): # Multiple values
+            original_length = len(combinations)
+            _embiggen(combinations, len(values))
+
+            for index, entry in enumerate(combinations):
+                value_index = index // original_length
+                entry[key] = values[value_index]
+
+        elif values is not None: # Single value
+            for entry in combinations:
+                entry[key] = values
 
     for index, entry in enumerate(combinations):
         entry["id"] = index + 1
 
     return combinations
 
 
@@ -187,29 +186,29 @@
     """
 
     id: int = 0
     """The identifier of the config."""
 
     duration: int = 0
     """The duration of the simulation in frames.
-    
+
     Defaults to `0`, indicating that the simulation runs indefinitely.
     """
 
     fps_limit: int = 60
     """Limit the number of frames-per-second.
-    
+
     Defaults to 60 fps, equal to most screens' refresh rates.
 
     Set to `0` to uncap the framerate.
     """
 
     image_rotation: bool = False
     """Opt-in image rotation support.
-    
+
     Please be aware that the rotation of images degrades performance by ~15%
     and currently causes a bug where agents clip into obstacles.
     """
 
     movement_speed: Union[float, MatrixFloat] = 0.5
     """The per-frame movement speed of the agents."""
 
@@ -217,15 +216,15 @@
     """Print the current number of frames-per-second in the terminal"""
 
     radius: Union[int, MatrixInt] = 25
     """The radius (in pixels) in which agents are considered to be in proximity."""
 
     seed: Optional[Union[int, MatrixInt]] = None
     """The PRNG seed to use for the simulation.
-    
+
     Defaults to `None`, indicating that no seed is used.
     """
 
     visualise_chunks: bool = False
     """Draw the borders of the proximity-chunks on screen."""
 
     window: Window = field(default_factory=Window)
```

### Comparing `violet-simulator-0.2.2/vi/proximity.py` & `violet_simulator-0.2.3/vi/proximity.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     Optional,
     Type,
     TypeVar,
     Union,
     overload,
 )
 
-from pygame.sprite import Group
 
 if TYPE_CHECKING:
+    from pygame.sprite import Group
+
     from .agent import Agent
 
 AgentClass = TypeVar("AgentClass", bound="Agent")
 T = TypeVar("T")
 U = TypeVar("U")
```

### Comparing `violet-simulator-0.2.2/vi/replay.py` & `violet_simulator-0.2.3/vi/replay.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import TYPE_CHECKING, Any, Optional
 
 import pygame as pg
 
 from .config import Window
 
+
 if TYPE_CHECKING:
     from polars import DataFrame, Series
 
 
 def load_images(image_paths: list[str]) -> list[pg.surface.Surface]:
     return [pg.image.load(path).convert_alpha() for path in image_paths]
```

### Comparing `violet-simulator-0.2.2/vi/simulation.py` & `violet_simulator-0.2.3/vi/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,34 +41,36 @@
 import random
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Optional, Type, TypeVar
 
 import pygame as pg
 from pygame.gfxdraw import hline, vline
 from pygame.math import Vector2
-from typing_extensions import Self
 
 from ._static import _StaticSprite
 from .config import Config
 from .metrics import Metrics
 from .proximity import ProximityEngine
 
+
 if TYPE_CHECKING:
+    from typing_extensions import Self
+
     from .agent import Agent
 
     AgentClass = TypeVar("AgentClass", bound=Agent)
 
 
 @dataclass
 class Shared:
     """A mutatable container for data that needs to be shared between `vi.agent.Agent` and `Simulation`."""
 
     prng_move: random.Random
     """A PRNG for agent movement exclusively.
-    
+
     To make sure that the agent's movement isn't influenced by other random function calls,
     all agents share a decoupled PRNG for movement exclusively.
     This ensures that the agents will always move the exact same way given a seed.
     """
 
     counter: int = 0
     """A counter that increases each tick of the simulation."""
@@ -142,25 +144,25 @@
 
     # Proximity
     _proximity: ProximityEngine
 
     # Config that's passed on to agents as well
     config: Config
     """The config of the simulation that's shared with all agents.
-    
+
     The config can be overriden when inheriting the Simulation class.
     However, the config must always:
 
     1. Inherit `Config`
     2. Be decorated by `@serde`
     """
 
     _metrics: Metrics
     """A collection of all the Snapshots that have been created in the simulation.
-    
+
     Each agent produces a Snapshot at every frame in the simulation.
     """
 
     def __init__(self, config: Optional[Config] = None):
         self.config = config if config else Config()
         self._metrics = Metrics()
```

### Comparing `violet-simulator-0.2.2/vi/util.py` & `violet_simulator-0.2.3/vi/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+from __future__ import annotations
+
 import random
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from pygame.math import Vector2
-from pygame.rect import Rect
+
+
+if TYPE_CHECKING:
+    from pygame.rect import Rect
 
 
 def probability(threshold: float, prng: Optional[random.Random] = None) -> bool:
     """Randomly retrieve True or False depending on the given probability.
 
     The probability should be between 0 and 1.
     If you give a probability equal or higher than 1, this function will always return True.
```

### Comparing `violet-simulator-0.2.2/PKG-INFO` & `violet_simulator-0.2.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: violet-simulator
-Version: 0.2.2
+Version: 0.2.3
 Summary: A smol simulator framework built on top of PyGame
 Home-page: https://violet.m-rots.com
+Author-Email: Storm Timmermans <stormtimmermans@icloud.com>
 License: MIT
-Author: Storm Timmermans
-Author-email: stormtimmermans@icloud.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: polars (>=0.13.38,<0.14.0)
-Requires-Dist: pygame (>=2.1.2,<3.0.0)
-Requires-Dist: pyserde[toml] (>=0.7.3,<0.8.0)
-Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
-Project-URL: Documentation, https://api.violet.m-rots.com/vi
+Project-URL: Homepage, https://violet.m-rots.com
 Project-URL: Repository, https://github.com/m-rots/violet
+Project-URL: Documentation, https://api.violet.m-rots.com/vi
+Requires-Python: >=3.9
+Requires-Dist: pygame>=2.4.0
+Requires-Dist: polars>=0.17.11
+Requires-Dist: pyserde[toml]>=0.10.4
+Requires-Dist: typing-extensions>=4.5.0
 Description-Content-Type: text/markdown
 
 # Violet
 
 A smol simulator framework built on top of [PyGame](https://www.pygame.org/docs/).
 
 - Automatic agent wandering behaviour
@@ -38,18 +34,18 @@
 
 Install the latest version of Violet with:
 
 ```bash
 pip3 install -U violet-simulator
 ```
 
-Or with [Poetry](https://python-poetry.org):
+Or with [PDM](https://pdm.fming.dev):
 
 ```bash
-poetry add violet-simulator
+pdm add violet-simulator
 ```
 
 ## Example
 
 ```python
 from vi import Agent, Simulation
```

