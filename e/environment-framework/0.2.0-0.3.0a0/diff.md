# Comparing `tmp/environment_framework-0.2.0.tar.gz` & `tmp/environment_framework-0.3.0a0.tar.gz`

## Comparing `environment_framework-0.2.0.tar` & `environment_framework-0.3.0a0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 environment_framework-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 environment_framework-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 environment_framework-0.2.0/makefile
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 environment_framework-0.2.0/mypy.ini
--rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 environment_framework-0.2.0/pylintrc
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 environment_framework-0.2.0/pytest.ini
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 environment_framework-0.2.0/version.py
--rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 environment_framework-0.2.0/example/grid_world.ipynb
--rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 environment_framework-0.2.0/example/grid_world.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 environment_framework-0.2.0/requirements/dev.txt
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 environment_framework-0.2.0/requirements/main.txt
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/__init__.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/estimator.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/game.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/gym.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/ilevel.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/level.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/observer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/py.typed
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/simulator.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/visualizer.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 environment_framework-0.2.0/tests/test_gym.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 environment_framework-0.2.0/tests/test_level.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 environment_framework-0.2.0/tests/test_simulator.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 environment_framework-0.2.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 environment_framework-0.2.0/LICENSE
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 environment_framework-0.2.0/README.md
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 environment_framework-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 environment_framework-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/makefile
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/mypy.ini
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/pylintrc
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/pytest.ini
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/version.py
+-rw-r--r--   0        0        0    12089 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/example/grid_world.ipynb
+-rw-r--r--   0        0        0     5896 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/example/grid_world.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/requirements/dev.txt
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/requirements/main.txt
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/__init__.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/estimator.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/game.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/gym.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/ilevel.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/level.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/observer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/py.typed
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/pygame_wrapper.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/simulator.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/visualizer.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/tests/test_gym.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/tests/test_level.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/tests/test_simulator.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/LICENSE
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/README.md
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/PKG-INFO
```

### Comparing `environment_framework-0.2.0/CODE_OF_CONDUCT.md` & `environment_framework-0.3.0a0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `environment_framework-0.2.0/CONTRIBUTING.md` & `environment_framework-0.3.0a0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `environment_framework-0.2.0/makefile` & `environment_framework-0.3.0a0/makefile`

 * *Files identical despite different names*

### Comparing `environment_framework-0.2.0/pylintrc` & `environment_framework-0.3.0a0/pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # run arbitrary code.
 extension-pkg-allow-list=
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code. (This is an alternative name to extension-pkg-allow-list
 # for backward compatibility.)
-extension-pkg-whitelist=
+extension-pkg-whitelist=pygame
 
 # Return non-zero exit code if any of these messages/categories are detected,
 # even if score is above --fail-under value. Syntax same as enable. Messages
 # specified are enabled, while categories only check already-enabled messages.
 fail-on=
 
 # Specify a score threshold to be exceeded before program exits with error.
```

### Comparing `environment_framework-0.2.0/example/grid_world.ipynb` & `environment_framework-0.3.0a0/example/grid_world.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9816191259279902%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict([('lines_to_next_cell', 2)])}, 'source': "*

 * *            "{insert: [(2, 'In this notebook we implement the GridWorld game with the\\n'), (3, "*

 * *            "'`environment-framework` and use stable-baseliens3 to train a `DQN`-agent on it.')], "*

 * *            "delete: [2]}}, 1: {'execution_count': 1, 'metadata': {delete: "*

 * *            "['lines_to_next_cell']}, 'source': {insert: [(0, '# pylint: "*

 * *            "disable=redefined-outer-name\\n'), (1, 'import math\\n […]*

```diff
@@ -1,72 +1,68 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "d60e0b29-66d5-421d-b914-fb3029e59e15",
-            "metadata": {},
+            "metadata": {
+                "lines_to_next_cell": 2
+            },
             "source": [
                 "# Grid World example\n",
                 "\n",
-                "In this notebook we implement the GridWorld game with the `environment-framework` and use stable-baseliens3 to train a `DQN`-agent on it."
+                "In this notebook we implement the GridWorld game with the\n",
+                "`environment-framework` and use stable-baseliens3 to train a `DQN`-agent on it."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "id": "34ec77d0-740e-4fda-b709-1a237ff49e43",
             "metadata": {
-                "lines_to_next_cell": 2,
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "from enum import Enum\n",
+                "# pylint: disable=redefined-outer-name\n",
+                "import math\n",
                 "from random import randint\n",
-                "from typing import Any, List, Tuple\n",
+                "from typing import Any, Callable, Optional\n",
                 "\n",
+                "import numpy as np\n",
+                "from gymnasium.spaces import Box, Discrete, Space\n",
+                "from numpy.typing import NDArray\n",
                 "from stable_baselines3.common.evaluation import evaluate_policy\n",
+                "from stable_baselines3.common.utils import set_random_seed\n",
+                "from stable_baselines3.common.vec_env import SubprocVecEnv\n",
                 "from stable_baselines3.dqn import DQN\n",
                 "\n",
-                "from numpy.typing import NDArray\n",
-                "from gymnasium.spaces import Space, Discrete\n",
-                "\n",
-                "import cv2\n",
-                "import numpy as np\n",
-                "\n",
-                "from gymnasium.spaces import Space, Box\n",
-                "import math\n",
-                "import numpy as np\n",
-                "\n",
-                "from environment_framework import Level\n",
-                "from environment_framework import EnvironmentFrameworkGym\n",
-                "from environment_framework import Simulator"
+                "from environment_framework import EnvironmentFrameworkGym, Level, PygameHumanVisualizer, Simulator"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "206b9f02-7f3c-4861-bf6d-81dd4652381e",
             "metadata": {
                 "lines_to_next_cell": 2
             },
             "source": [
                 "## Implement the `Game`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 2,
             "id": "42cf31a4-d776-41e9-adbb-44fe9056d083",
             "metadata": {
                 "lines_to_next_cell": 2,
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "class Action(Enum):\n",
+                "class Action:\n",
                 "    UP = 0\n",
                 "    DOWN = 1\n",
                 "    RIGHT = 2\n",
                 "    LEFT = 3\n",
                 "\n",
                 "\n",
                 "class GridWorldGame:\n",
@@ -75,21 +71,20 @@
                 "        self.player_position = (0, 0)\n",
                 "        self.target_position = (0, 0)\n",
                 "        self.reset()\n",
                 "\n",
                 "    @property\n",
                 "    def done(self) -> bool:\n",
                 "        return self.player_position == self.target_position\n",
-                "    \n",
+                "\n",
                 "    @property\n",
                 "    def space(self) -> Space:\n",
                 "        return Discrete(4)\n",
-                "        \n",
                 "\n",
-                "    def act(self, action: Action, **_: Any) -> None:\n",
+                "    def act(self, action: int, **_: Any) -> None:\n",
                 "        if action == Action.UP:\n",
                 "            self.player_position = (self.player_position[0], self.player_position[1] - 1)\n",
                 "        if action == Action.DOWN:\n",
                 "            self.player_position = (self.player_position[0], self.player_position[1] + 1)\n",
                 "        if action == Action.RIGHT:\n",
                 "            self.player_position = (self.player_position[0] + 1, self.player_position[1])\n",
                 "        if action == Action.LEFT:\n",
@@ -116,15 +111,15 @@
             },
             "source": [
                 "## Implement the `Observer` and the `Estimator`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 3,
             "id": "e4109d2c-3202-4499-8e2e-0c58e4456f30",
             "metadata": {
                 "lines_to_next_cell": 2,
                 "tags": []
             },
             "outputs": [],
             "source": [
@@ -132,23 +127,26 @@
                 "    def __init__(self, game: GridWorldGame) -> None:\n",
                 "        self.game = game\n",
                 "\n",
                 "    @property\n",
                 "    def space(self) -> Space:\n",
                 "        return Box(shape=(4,), low=-math.inf, high=math.inf)\n",
                 "\n",
-                "    def observe(self, _: Any) -> NDArray:\n",
-                "        return np.array([*self.game.player_position, *self.game.target_position])\n",
+                "    def observe(self) -> NDArray:\n",
+                "        return np.array(\n",
+                "            [*self.game.player_position, *self.game.target_position],\n",
+                "            dtype=np.float32,\n",
+                "        )\n",
                 "\n",
                 "\n",
                 "class GridWorldEstimator:\n",
                 "    def __init__(self, game: GridWorldGame) -> None:\n",
                 "        self.game = game\n",
                 "\n",
-                "    def estimate(self, _: Any) -> float:\n",
+                "    def estimate(self) -> float:\n",
                 "        return -1 + float(self.game.done)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7bee370d-7f88-44a4-a1dd-d9d5a84f24a1",
             "metadata": {
@@ -157,196 +155,256 @@
             },
             "source": [
                 "## Add a nice little `Visualizer`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 4,
             "id": "b8855c93-3335-4475-80aa-3e3a64ae5300",
             "metadata": {
                 "lines_to_next_cell": 2,
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "class GridWorldVisualizer:\n",
-                "    # We use BGR\n",
-                "    BLUE = [255, 0, 0]\n",
+                "class GridWorldVisualizer(PygameHumanVisualizer):\n",
+                "    BLUE = [0, 0, 255]\n",
                 "    GREEN = [0, 255, 0]\n",
                 "\n",
                 "    def __init__(self, game: GridWorldGame) -> None:\n",
+                "        super().__init__(50)\n",
                 "        self.game = game\n",
                 "\n",
-                "    def render(self, _: Any) -> Any:\n",
+                "    def render_rgb(self) -> NDArray[np.uint8]:\n",
                 "        frame = [[[0 for k in range(3)] for j in range(self.game.size)] for i in range(self.game.size)]\n",
                 "        frame[self.game.player_position[1]][self.game.player_position[0]] = self.BLUE\n",
                 "        frame[self.game.target_position[1]][self.game.target_position[0]] = self.GREEN\n",
-                "        return frame"
+                "        return np.array(frame, dtype=np.uint8)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "30c63509-6c5b-49c5-9717-97ce0cd74e48",
             "metadata": {
                 "lines_to_next_cell": 2
             },
             "source": [
                 "## Connect all together with a `Level`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 5,
             "id": "18451c66-de76-411a-adff-51a2b23c5c30",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "class GridWorldLevel(Level):\n",
                 "    _game: GridWorldGame\n",
                 "    _observer: GridWorldObserver\n",
                 "    _estimator: GridWorldEstimator\n",
                 "    _visualizer: GridWorldVisualizer\n",
                 "\n",
-                "    def __init__(\n",
-                "        self,\n",
-                "        game: GridWorldGame,\n",
-                "        observer: GridWorldObserver,\n",
-                "        estimator: GridWorldEstimator,\n",
-                "        visualizer: GridWorldVisualizer,\n",
-                "    ) -> None:\n",
-                "        super().__init__(game, observer, estimator, visualizer)\n",
-                "\n",
                 "    def reset(self) -> None:\n",
                 "        self._game.reset()\n",
                 "\n",
-                "    def step(self, action: Action) -> Any:\n",
-                "        if isinstance(action, np.int64):  # handle integer inputs\n",
-                "            action = Action(action)\n",
+                "    def step(self, action: int) -> Any:\n",
                 "        self._game.act(action)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "370e3268-a7b6-4e51-9f03-ece9dec0acc3",
             "metadata": {},
             "source": [
                 "## Look at a random selecting agent"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "id": "89f7c5dc-de16-4dd1-bb63-8b30a349ca02",
+            "execution_count": 6,
+            "id": "b14743ec-c00e-411f-96a1-6883b72a8c40",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "game = GridWorldGame(7)\n",
-                "scale_factor = 50\n",
-                "level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))\n",
-                "simulator = Simulator(level)\n",
-                "while not simulator.done:\n",
-                "    action = Action(randint(0, 3))\n",
+                "level = GridWorldLevel(\n",
+                "    game,\n",
+                "    GridWorldObserver(game),\n",
+                "    GridWorldEstimator(game),\n",
+                "    GridWorldVisualizer(game),\n",
+                ")\n",
+                "simulator = Simulator(level, 50)\n",
+                "\n",
+                "FPS = 4\n",
+                "DONE = False\n",
+                "while not DONE:\n",
+                "    action = simulator.action_space.sample()\n",
                 "    simulator.step(action)\n",
-                "    frame = np.array(simulator.render(), dtype=np.uint8)\n",
-                "    frame = cv2.resize(frame, (scale_factor * game.size, scale_factor * game.size), interpolation=cv2.INTER_AREA)\n",
-                "    cv2.imshow(\"GridWorld\", frame)\n",
-                "    cv2.waitKey(33)\n",
-                "cv2.waitKey(500)\n",
-                "cv2.destroyAllWindows()"
+                "    obs = simulator.observe()\n",
+                "    reward = simulator.estimate()\n",
+                "    simulator.render_human(FPS)\n",
+                "    DONE = simulator.truncated or simulator.done\n",
+                "simulator.close()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3f3ca062-0efb-42c9-9abc-52b344960c2e",
-            "metadata": {},
+            "metadata": {
+                "lines_to_next_cell": 2
+            },
             "source": [
                 "## Use stable-baselines3 to train an DQN-agent in the environment"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "id": "3392de7b-d58b-47ae-94e6-5bad09bdfc39",
+            "execution_count": 7,
+            "id": "ac1b88e9-a25f-4e5d-a80a-fd8de93368ca",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "game = GridWorldGame(7)\n",
-                "level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))\n",
-                "env = EnvironmentFrameworkGym(level, render_mode=\"rgb_array\")\n",
+                "def make_env(render_mode: Optional[str], rank: int, seed: int = 0, **_: Any) -> Callable:\n",
+                "    def _init() -> EnvironmentFrameworkGym:\n",
+                "        game = GridWorldGame(7)\n",
+                "        level = GridWorldLevel(\n",
+                "            game,\n",
+                "            GridWorldObserver(game),\n",
+                "            GridWorldEstimator(game),\n",
+                "            GridWorldVisualizer(game),\n",
+                "        )\n",
+                "        env = EnvironmentFrameworkGym(level, 10, render_mode=render_mode)\n",
+                "        env.reset(seed=seed + rank)\n",
+                "        return env\n",
                 "\n",
-                "model = DQN(\"MlpPolicy\", env)\n",
+                "    set_random_seed(seed)\n",
+                "    return _init"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "3392de7b-d58b-47ae-94e6-5bad09bdfc39",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "21c6aae45a4e49fdbbf4e9795d9b03d3",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Output()"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\"></pre>\n"
+                        ],
+                        "text/plain": []
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\">\n",
+                            "</pre>\n"
+                        ],
+                        "text/plain": [
+                            "\n"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "<stable_baselines3.dqn.dqn.DQN at 0x7fa48829e290>"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "N_CPU = 1\n",
+                "vec_env = SubprocVecEnv([make_env(None, i) for i in range(N_CPU)])\n",
+                "model = DQN(\"MlpPolicy\", vec_env)\n",
                 "model.learn(\n",
                 "    total_timesteps=int(5e5),\n",
                 "    progress_bar=True,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "id": "bd172f4e-7492-4860-9a42-ada5056eb064",
+            "execution_count": 9,
+            "id": "34db8e65-7046-49f0-b6c4-cdf3b18d2289",
             "metadata": {},
             "outputs": [],
             "source": [
-                "evaluate_policy(model, env, n_eval_episodes=10)"
+                "model.save(\"gridworld-dqn.zip\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "id": "34db8e65-7046-49f0-b6c4-cdf3b18d2289",
-            "metadata": {},
+            "execution_count": 10,
+            "id": "8876ed8d-6d89-41ef-ada9-ab3ceabf86b8",
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
-                "model.save(\"gridworld-dqn.zip\")"
+                "del model"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 11,
             "id": "ca143958-07db-4562-a43a-72f442a5d2b2",
             "metadata": {
                 "tags": []
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/home/rb/git/environment-framework/venv/lib/python3.10/site-packages/stable_baselines3/common/evaluation.py:67: UserWarning: Evaluation environment is not wrapped with a ``Monitor`` wrapper. This may result in reporting modified episode lengths and rewards, if other wrappers happen to modify these. Consider wrapping environment first with ``Monitor`` wrapper.\n",
+                        "  warnings.warn(\n"
+                    ]
+                }
+            ],
             "source": [
                 "game = GridWorldGame(7)\n",
-                "scale_factor = 50\n",
                 "level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))\n",
-                "env = EnvironmentFrameworkGym(level, render_mode=\"rgb_array\")\n",
-                "\n",
+                "env = EnvironmentFrameworkGym(level, 10, render_mode=\"human\")\n",
                 "model = DQN.load(\"gridworld-dqn.zip\", env=env)\n",
-                "vec_env = model.get_env()\n",
-                "obs = vec_env.reset()\n",
-                "for _ in range(50):\n",
-                "    obs = np.array(obs)\n",
-                "    action, _states = model.predict(obs)  # type: ignore\n",
-                "    obs, _, _, _ = vec_env.step(action)\n",
-                "    frame = np.array(vec_env.render(), dtype=np.uint8)\n",
-                "    frame = cv2.resize(frame, (scale_factor * game.size, scale_factor * game.size), interpolation=cv2.INTER_AREA)\n",
-                "    cv2.imshow(\"GridWorld\", frame)\n",
-                "    cv2.waitKey(250)\n",
-                "cv2.waitKey(500)\n",
-                "cv2.destroyAllWindows()"
+                "evaluate_policy(model, env, n_eval_episodes=10)\n",
+                "env.close()"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "07e4cc1f-cc51-4eb2-9872-aa116814209d",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "jupytext": {
             "formats": "ipynb,py:hydrogen"
         },
         "kernelspec": {
```

### Comparing `environment_framework-0.2.0/example/grid_world.py` & `environment_framework-0.3.0a0/example/grid_world.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,45 +12,40 @@
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
 # # Grid World example
 #
-# In this notebook we implement the GridWorld game with the `environment-framework` and use stable-baseliens3 to train a `DQN`-agent on it.
+# In this notebook we implement the GridWorld game with the
+# `environment-framework` and use stable-baseliens3 to train a `DQN`-agent on it.
+
 
 # %%
-from enum import Enum
+# pylint: disable=redefined-outer-name
+import math
 from random import randint
-from typing import Any, List, Tuple
+from typing import Any, Callable, Optional
 
+import numpy as np
+from gymnasium.spaces import Box, Discrete, Space
+from numpy.typing import NDArray
 from stable_baselines3.common.evaluation import evaluate_policy
+from stable_baselines3.common.utils import set_random_seed
+from stable_baselines3.common.vec_env import SubprocVecEnv
 from stable_baselines3.dqn import DQN
 
-from numpy.typing import NDArray
-from gymnasium.spaces import Space, Discrete
-
-import cv2
-import numpy as np
-
-from gymnasium.spaces import Space, Box
-import math
-import numpy as np
-
-from environment_framework import Level
-from environment_framework import EnvironmentFrameworkGym
-from environment_framework import Simulator
-
+from environment_framework import EnvironmentFrameworkGym, Level, PygameHumanVisualizer, Simulator
 
 # %% [markdown]
 # ## Implement the `Game`
 
 
 # %%
-class Action(Enum):
+class Action:
     UP = 0
     DOWN = 1
     RIGHT = 2
     LEFT = 3
 
 
 class GridWorldGame:
@@ -59,21 +54,20 @@
         self.player_position = (0, 0)
         self.target_position = (0, 0)
         self.reset()
 
     @property
     def done(self) -> bool:
         return self.player_position == self.target_position
-    
+
     @property
     def space(self) -> Space:
         return Discrete(4)
-        
 
-    def act(self, action: Action, **_: Any) -> None:
+    def act(self, action: int, **_: Any) -> None:
         if action == Action.UP:
             self.player_position = (self.player_position[0], self.player_position[1] - 1)
         if action == Action.DOWN:
             self.player_position = (self.player_position[0], self.player_position[1] + 1)
         if action == Action.RIGHT:
             self.player_position = (self.player_position[0] + 1, self.player_position[1])
         if action == Action.LEFT:
@@ -101,127 +95,128 @@
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
     @property
     def space(self) -> Space:
         return Box(shape=(4,), low=-math.inf, high=math.inf)
 
-    def observe(self, _: Any) -> NDArray:
-        return np.array([*self.game.player_position, *self.game.target_position])
+    def observe(self) -> NDArray:
+        return np.array(
+            [*self.game.player_position, *self.game.target_position],
+            dtype=np.float32,
+        )
 
 
 class GridWorldEstimator:
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
-    def estimate(self, _: Any) -> float:
+    def estimate(self) -> float:
         return -1 + float(self.game.done)
 
 
 # %% [markdown]
 # ## Add a nice little `Visualizer`
 
 
 # %%
-class GridWorldVisualizer:
-    # We use BGR
-    BLUE = [255, 0, 0]
+class GridWorldVisualizer(PygameHumanVisualizer):
+    BLUE = [0, 0, 255]
     GREEN = [0, 255, 0]
 
     def __init__(self, game: GridWorldGame) -> None:
+        super().__init__(50)
         self.game = game
 
-    def render(self, _: Any) -> Any:
+    def render_rgb(self) -> NDArray[np.uint8]:
         frame = [[[0 for k in range(3)] for j in range(self.game.size)] for i in range(self.game.size)]
         frame[self.game.player_position[1]][self.game.player_position[0]] = self.BLUE
         frame[self.game.target_position[1]][self.game.target_position[0]] = self.GREEN
-        return frame
+        return np.array(frame, dtype=np.uint8)
 
 
 # %% [markdown]
 # ## Connect all together with a `Level`
 
 
 # %%
 class GridWorldLevel(Level):
     _game: GridWorldGame
     _observer: GridWorldObserver
     _estimator: GridWorldEstimator
     _visualizer: GridWorldVisualizer
 
-    def __init__(
-        self,
-        game: GridWorldGame,
-        observer: GridWorldObserver,
-        estimator: GridWorldEstimator,
-        visualizer: GridWorldVisualizer,
-    ) -> None:
-        super().__init__(game, observer, estimator, visualizer)
-
     def reset(self) -> None:
         self._game.reset()
 
-    def step(self, action: Action) -> Any:
-        if isinstance(action, np.int64):  # handle integer inputs
-            action = Action(action)
+    def step(self, action: int) -> Any:
         self._game.act(action)
 
 
 # %% [markdown]
 # ## Look at a random selecting agent
 
 # %%
 game = GridWorldGame(7)
-scale_factor = 50
-level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))
-simulator = Simulator(level)
-while not simulator.done:
-    action = Action(randint(0, 3))
+level = GridWorldLevel(
+    game,
+    GridWorldObserver(game),
+    GridWorldEstimator(game),
+    GridWorldVisualizer(game),
+)
+simulator = Simulator(level, 50)
+
+FPS = 4
+DONE = False
+while not DONE:
+    action = simulator.action_space.sample()
     simulator.step(action)
-    frame = np.array(simulator.render(), dtype=np.uint8)
-    frame = cv2.resize(frame, (scale_factor * game.size, scale_factor * game.size), interpolation=cv2.INTER_AREA)
-    cv2.imshow("GridWorld", frame)
-    cv2.waitKey(33)
-cv2.waitKey(500)
-cv2.destroyAllWindows()
+    obs = simulator.observe()
+    reward = simulator.estimate()
+    simulator.render_human(FPS)
+    DONE = simulator.truncated or simulator.done
+simulator.close()
 
 # %% [markdown]
 # ## Use stable-baselines3 to train an DQN-agent in the environment
 
+
 # %%
-game = GridWorldGame(7)
-level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))
-env = EnvironmentFrameworkGym(level, render_mode="rgb_array")
+def make_env(render_mode: Optional[str], rank: int, seed: int = 0, **_: Any) -> Callable:
+    def _init() -> EnvironmentFrameworkGym:
+        game = GridWorldGame(7)
+        level = GridWorldLevel(
+            game,
+            GridWorldObserver(game),
+            GridWorldEstimator(game),
+            GridWorldVisualizer(game),
+        )
+        env = EnvironmentFrameworkGym(level, 10, render_mode=render_mode)
+        env.reset(seed=seed + rank)
+        return env
+
+    set_random_seed(seed)
+    return _init
+
 
-model = DQN("MlpPolicy", env)
+# %%
+N_CPU = 1
+vec_env = SubprocVecEnv([make_env(None, i) for i in range(N_CPU)])
+model = DQN("MlpPolicy", vec_env)
 model.learn(
     total_timesteps=int(5e5),
     progress_bar=True,
 )
 
 # %%
-evaluate_policy(model, env, n_eval_episodes=10)
+model.save("gridworld-dqn.zip")
 
 # %%
-model.save("gridworld-dqn.zip")
+del model
 
 # %%
 game = GridWorldGame(7)
-scale_factor = 50
 level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))
-env = EnvironmentFrameworkGym(level, render_mode="rgb_array")
-
+env = EnvironmentFrameworkGym(level, 10, render_mode="human")
 model = DQN.load("gridworld-dqn.zip", env=env)
-vec_env = model.get_env()
-obs = vec_env.reset()
-for _ in range(50):
-    obs = np.array(obs)
-    action, _states = model.predict(obs)  # type: ignore
-    obs, _, _, _ = vec_env.step(action)
-    frame = np.array(vec_env.render(), dtype=np.uint8)
-    frame = cv2.resize(frame, (scale_factor * game.size, scale_factor * game.size), interpolation=cv2.INTER_AREA)
-    cv2.imshow("GridWorld", frame)
-    cv2.waitKey(250)
-cv2.waitKey(500)
-cv2.destroyAllWindows()
-
-# %%
+evaluate_policy(model, env, n_eval_episodes=10)
+env.close()
```

### Comparing `environment_framework-0.2.0/requirements/dev.txt` & `environment_framework-0.3.0a0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `environment_framework-0.2.0/requirements/main.txt` & `environment_framework-0.3.0a0/requirements/main.txt`

 * *Files identical despite different names*

### Comparing `environment_framework-0.2.0/src/environment_framework/game.py` & `environment_framework-0.3.0a0/src/environment_framework/game.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.2.0/src/environment_framework/gym.py` & `environment_framework-0.3.0a0/src/environment_framework/gym.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 import gymnasium as gym
 
 from environment_framework.ilevel import ILevel
 from environment_framework.simulator import Simulator
 
 
 class EnvironmentFrameworkGym(gym.Env):
-    metadata = {"render_modes": ["rgb_array"], "render_fps": 4}
+    metadata = {"render_modes": ["rgb_array", "human"], "render_fps": 16}
 
     def __init__(
         self,
         level: ILevel,
+        max_episode_steps: int,
         render_mode: Any = Optional[None],
     ) -> None:
         super().__init__()
 
-        self.simulator = Simulator(level)
+        self.simulator = Simulator(level, max_episode_steps)
 
         self.observation_space = self.simulator.observation_space
         self.action_space = self.simulator.action_space
 
         supported_render_modes: List[str] = EnvironmentFrameworkGym.metadata["render_modes"]
         if render_mode and render_mode not in supported_render_modes:
             raise Exception("Specified unsupported render mode")
@@ -31,20 +32,25 @@
 
     def step(
         self,
         action: List,
     ) -> Tuple[Any, float, bool, bool, Dict]:
         action = self.simulator.step(action)
         reward = self.simulator.estimate()
-        # TODO: Implement gymnasium specific terminate / truncate strategy
-        return self.simulator.observe(), reward, self.simulator.done, False, {}
+        if self.render_mode == "human":
+            self.simulator.render_human(
+                EnvironmentFrameworkGym.metadata["render_fps"],
+            )
+        return self.simulator.observe(), reward, self.simulator.done, self.simulator.truncated, {}
 
     def reset(  # pylint: disable=unused-argument
         self, *, seed: Optional[int] = None, options: Optional[Dict] = None
     ) -> Tuple[Any, Dict[str, Any]]:
         super().reset(seed=seed)
         self.simulator.reset()
         return self.simulator.observe(), {}
 
     def render(self) -> Optional[Any]:
-        frame = self.simulator.render()
-        return frame
+        return self.simulator.render_rgb()
+
+    def close(self) -> None:
+        self.simulator.close()
```

### Comparing `environment_framework-0.2.0/src/environment_framework/ilevel.py` & `environment_framework-0.3.0a0/src/environment_framework/ilevel.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,26 +63,32 @@
 
         Returns
         -------
             observation: List[float]
                 Observation of the current level state.
         """
 
-    def estimate(self, estimated: Any) -> float:
+    def estimate(self) -> float:
         """
         Estimates the level state and returns a estimation value.
 
         Returns
         -------
             estimation: float
                 Estimated reward of the current level state.
         """
 
-    def render(self) -> Any:
+    def render_rgb(self) -> Any:
         """
         Renders the current level state into a visualisation.
 
         Returns
         -------
             visualisation: Any
                 Rendered visualisation of the current level state.
         """
+
+    def render_human(self, fps: int) -> Any:
+        pass
+
+    def close(self) -> Any:
+        pass
```

### Comparing `environment_framework-0.2.0/src/environment_framework/level.py` & `environment_framework-0.3.0a0/src/environment_framework/level.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from environment_framework.estimator import Estimator
 from environment_framework.game import Game
 from environment_framework.observer import Observer
 from environment_framework.visualizer import Visualizer
 
 
-class Level(ABC):  # pylint: disable=too-many-instance-attributes
+class Level(ABC):
     """
     Manages the lifecycle of a game and its observer and estimator.
     Is used within the Simulator to step through a Simulation.
     """
 
     def __init__(
         self,
@@ -102,30 +102,36 @@
         Observes the level and returns an observation.
 
         Returns
         -------
             observation: List[float]
                 Observation of the current level state.
         """
-        return self._observer.observe(None)
+        return self._observer.observe()
 
-    def estimate(self, estimated: Any) -> float:
+    def estimate(self) -> float:
         """
         Estimates the level state and returns a estimation value.
 
         Returns
         -------
             estimation: float
                 Estimated reward of the current level state.
         """
-        return self._estimator.estimate(estimated)
+        return self._estimator.estimate()
 
-    def render(self) -> Any:
+    def render_rgb(self) -> Any:
         """
         Renders the current level state into a visualisation.
 
         Returns
         -------
             visualisation: Any
                 Rendered visualisation of the current level state.
         """
-        return self._visualizer.render(None)
+        return self._visualizer.render_rgb()
+
+    def render_human(self, fps: int) -> Any:
+        return self._visualizer.render_human(fps)
+
+    def close(self) -> Any:
+        self._visualizer.close()
```

### Comparing `environment_framework-0.2.0/src/environment_framework/observer.py` & `environment_framework-0.3.0a0/src/environment_framework/observer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import Any, Protocol
+from typing import Protocol
 
+import numpy as np
 from gymnasium.spaces import Space
 from numpy.typing import NDArray
 
 
 class Observer(Protocol):
-    # TODO: Add low and high poperties for the observation space
     @property
     def space(self) -> Space:
         """
         The shape of the observation which is returned by observe().
 
         Returns
         -------
         shape: Tuple[int, ...]:
             The shape of the observation list.
         """
 
-    def observe(self, observed: Any) -> NDArray:
+    def observe(self) -> NDArray[np.float32]:
         """
         Returns an observation of the an observed object.
 
         Parameters
         ----------
         observed: Any
             The object which is observed.
```

### Comparing `environment_framework-0.2.0/src/environment_framework/simulator.py` & `environment_framework-0.3.0a0/src/environment_framework/simulator.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,21 +8,18 @@
 
 class Simulator:  # pylint: disable = too-many-instance-attributes
     """
     Runs simulations on a Level.
     """
 
     # TODO: Add a proper state which is passed to the observe,estimate and render method.
-    # TODO: Rename episodes to simulation.
-    def __init__(self, level: ILevel, max_episode_steps: int = 100000) -> None:
+    def __init__(self, level: ILevel, max_episode_steps: int) -> None:
         self.level = level
         self._max_episode_steps = max_episode_steps
         self.current_episodes_steps_done = 0
-        self.episodes_done = 0
-        self.steps_done = 0
 
     @property
     def action_space(self) -> Space:
         return self.level.action_space
 
     @property
     def observation_space(self) -> Space:
@@ -34,30 +31,31 @@
         If the current simulation is finished.
 
         Returns
         -------
             done: bool
                 Simulator is finished.
         """
-        return self.level.done or (self.current_episodes_steps_done >= self._max_episode_steps)
+        return self.level.done
+
+    @property
+    def truncated(self) -> bool:
+        return self.current_episodes_steps_done >= self._max_episode_steps
 
     def clear_counter(self) -> None:
         """
         Clear the counters of the Simulator.
         """
-        self.episodes_done = 0
-        self.steps_done = 0
         self.current_episodes_steps_done = 0
 
     def reset(self) -> None:
         """
         Reset the Level and prepare for a new simulation.
         """
         self.level.reset()
-        self.episodes_done += 1
         self.current_episodes_steps_done = 0
 
     def step(self, action: Any) -> Any:
         """
         Take a step in the Simulator through performing an action in the Level.
 
         Parameters
@@ -67,52 +65,47 @@
 
         Returns
         -------
             taken_action: Any
                 Returns the action taken in the Level.
         """
         self.current_episodes_steps_done += 1
-        self.steps_done += 1
         return self.level.step(action)
 
     def observe(self) -> NDArray:
         """
         Observes the level and returns an observation.
 
         Returns
         -------
             observation: List[float]
                 Observation of the current level state.
         """
-        # TODO: pass state
         return self.level.observe()
 
     def estimate(self) -> float:
         """
         Estimates the level state and returns a estimation value.
 
         Returns
         -------
             estimation: float
                 Estimated reward of the current level state.
         """
-        # TODO: pass state
-        return self.level.estimate(
-            {
-                "simulator": {
-                    "curr_episode_step": self.current_episodes_steps_done,
-                    "max_steps_per_episode": self._max_episode_steps,
-                }
-            }
-        )
+        return self.level.estimate()
 
-    def render(self) -> Any:
+    def render_rgb(self) -> Any:
         """
         Renders the current level state into a visualisation.
 
         Returns
         -------
             visualisation: Any
                 Rendered visualisation of the current level state.
         """
-        # TODO: pass state
-        return self.level.render()
+        return self.level.render_rgb()
+
+    def render_human(self, fps: int) -> None:
+        self.level.render_human(fps)
+
+    def close(self) -> None:
+        self.level.close()
```

### Comparing `environment_framework-0.2.0/tests/test_gym.py` & `environment_framework-0.3.0a0/tests/test_gym.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,45 +61,46 @@
     game_mock = MagicMock(spec_set=Game)
     observer_mock = MagicMock(spec_set=Observer)
     estimator_mock = MagicMock(spec_set=Estimator)
     visualizer_mock = MagicMock(spec_set=Visualizer)
 
     level: ILevel = TestLevel(game_mock, observer_mock, estimator_mock, visualizer_mock)
     simulator_mock = MagicMock(spec_set=Simulator)
-    gym = EnvironmentFrameworkGym(level, "rgb_array")
+    gym = EnvironmentFrameworkGym(level, 100, render_mode="rgb_array")
     gym.simulator = simulator_mock
     return gym, simulator_mock
 
 
-def test_step(setup: EnvironmentFrameworkGym) -> None:
+def test_step(setup: SetupT) -> None:
     gym, simulator_mock = setup
 
     simulator_mock.estimate.return_value = 42
     simulator_mock.observe.return_value = np.array([42])
     simulator_mock.done = True
+    simulator_mock.truncated = False
 
     observation, reward, done, truncated, extra = gym.step([10])
 
     assert observation == np.array([42])
     assert reward == 42
     assert truncated == False
     assert done
     assert extra == {}
 
 
-def test_reset(setup: EnvironmentFrameworkGym) -> None:
+def test_reset(setup: SetupT) -> None:
     gym, simulator_mock = setup
 
     simulator_mock.observe.return_value = [42]
     observation = gym.reset()
 
     simulator_mock.reset.assert_called_once()
     assert observation == ([42], {})
 
 
-def test_render(setup: EnvironmentFrameworkGym) -> None:
+def test_render(setup: SetupT) -> None:
     gym, simulator_mock = setup
-    simulator_mock.render.return_value = "frame"
+    simulator_mock.render_rgb.return_value = "frame"
     frame = gym.render()
 
-    simulator_mock.render.assert_called_once()
+    simulator_mock.render_rgb.assert_called_once()
     assert frame == "frame"
```

### Comparing `environment_framework-0.2.0/tests/test_level.py` & `environment_framework-0.3.0a0/tests/test_level.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,22 +43,22 @@
     assert not level.done
 
 
 def test_observe(setup: Level) -> None:
     level = setup
     level.observe()
 
-    level._observer.observe.assert_called_once_with(None)
+    level._observer.observe.assert_called_once()
 
 
 def test_estimate(setup: Level) -> None:
     level = setup
-    level.estimate("estimated")
+    level.estimate()
 
-    level._estimator.estimate.assert_called_once_with("estimated")
+    level._estimator.estimate.assert_called_once()
 
 
 def test_render(setup: Level) -> None:
     level = setup
-    level.render()
+    level.render_rgb()
 
-    level._visualizer.render.assert_called_once_with(None)
+    level._visualizer.render_rgb.assert_called_once()
```

### Comparing `environment_framework-0.2.0/tests/test_simulator.py` & `environment_framework-0.3.0a0/tests/test_simulator.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,49 +35,43 @@
     assert not simulator.done
 
     simulator.level.done = True
     assert simulator.done
 
     simulator.level.done = False
     simulator.current_episodes_steps_done = 9999
-    assert not simulator.done
+    assert not simulator.truncated
 
     simulator.current_episodes_steps_done = 10000
-    assert simulator.done
+    assert simulator.truncated
 
 
 def test_clear_counter(setup: Simulator) -> None:
     simulator = setup
-    simulator.episodes_done = 10
-    simulator.steps_done = 100
     simulator.current_episodes_steps_done = 1000
 
     simulator.clear_counter()
 
-    assert simulator.episodes_done == 0
-    assert simulator.steps_done == 0
     assert simulator.current_episodes_steps_done == 0
 
 
 def test_reset(setup: Simulator) -> None:
     simulator = setup
     simulator.current_episodes_steps_done = 100
     simulator.reset()
 
     simulator.level.reset.assert_called_once()
-    assert simulator.episodes_done == 1
     assert simulator.current_episodes_steps_done == 0
 
 
 def test_step(setup: Simulator) -> None:
     simulator = setup
     simulator.step(10)
 
     simulator.level.step.assert_called_once_with(10)
-    assert simulator.steps_done == 1
     assert simulator.current_episodes_steps_done == 1
 
 
 def test_observe(setup: Simulator) -> None:
     simulator = setup
     simulator.observe()
     simulator.level.observe.assert_called_once()
@@ -87,9 +81,9 @@
     simulator = setup
     simulator.estimate()
     simulator.level.estimate.assert_called_once()
 
 
 def test_render(setup: Simulator) -> None:
     simulator = setup
-    simulator.render()
-    simulator.level.render.assert_called_once()
+    simulator.render_rgb()
+    simulator.level.render_rgb.assert_called_once()
```

### Comparing `environment_framework-0.2.0/.gitignore` & `environment_framework-0.3.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `environment_framework-0.2.0/LICENSE` & `environment_framework-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `environment_framework-0.2.0/README.md` & `environment_framework-0.3.0a0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 ```bash
 pip3 install "environment-framework[extra]"
 jupyter lab
 ```
 
 ```python
-class Action(Enum):
+class Action:
     UP = 0
     DOWN = 1
     RIGHT = 2
     LEFT = 3
 
 class GridWorldGame:
     def __init__(self, size: int) -> None:
@@ -54,16 +54,15 @@
     def done(self) -> bool:
         return self.player_position == self.target_position
 
     @property
     def space(self) -> Space:
         return Discrete(4)
 
-
-    def act(self, action: Action, **_: Any) -> None:
+    def act(self, action: int, **_: Any) -> None:
         if action == Action.UP:
             self.player_position = (self.player_position[0], self.player_position[1] - 1)
         if action == Action.DOWN:
             self.player_position = (self.player_position[0], self.player_position[1] + 1)
         if action == Action.RIGHT:
             self.player_position = (self.player_position[0] + 1, self.player_position[1])
         if action == Action.LEFT:
@@ -84,67 +83,71 @@
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
     @property
     def space(self) -> Space:
         return Box(shape=(4,), low=-math.inf, high=math.inf)
 
-    def observe(self, _: Any) -> NDArray:
-        return np.array([*self.game.player_position, *self.game.target_position])
+    def observe(self) -> NDArray:
+        return np.array(
+            [*self.game.player_position, *self.game.target_position],
+            dtype=np.float32,
+        )
 
 class GridWorldEstimator:
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
-    def estimate(self, _: Any) -> float:
+    def estimate(self) -> float:
         return -1 + float(self.game.done)
 
-class GridWorldVisualizer:
-    # We use BGR
-    BLUE = [255, 0, 0]
+class GridWorldVisualizer(PygameHumanVisualizer):
+    BLUE = [0, 0, 255]
     GREEN = [0, 255, 0]
 
     def __init__(self, game: GridWorldGame) -> None:
+        super().__init__(50)
         self.game = game
 
-    def render(self, _: Any) -> Any:
+    def render_rgb(self) -> NDArray[np.uint8]:
         frame = [[[0 for k in range(3)] for j in range(self.game.size)] for i in range(self.game.size)]
         frame[self.game.player_position[1]][self.game.player_position[0]] = self.BLUE
         frame[self.game.target_position[1]][self.game.target_position[0]] = self.GREEN
-        return frame
+        return np.array(frame, dtype=np.uint8)
 
 class GridWorldLevel(Level):
     _game: GridWorldGame
     _observer: GridWorldObserver
     _estimator: GridWorldEstimator
     _visualizer: GridWorldVisualizer
 
-    def __init__(
-        self,
-        game: GridWorldGame,
-        observer: GridWorldObserver,
-        estimator: GridWorldEstimator,
-        visualizer: GridWorldVisualizer,
-    ) -> None:
-        super().__init__(game, observer, estimator, visualizer)
-
     def reset(self) -> None:
         self._game.reset()
 
-    def step(self, action: Action) -> Any:
-        if isinstance(action, np.int64):  # handle integer inputs
-            action = Action(action)
+    def step(self, action: int) -> Any:
         self._game.act(action)
 
 game = GridWorldGame(7)
-level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))
-simulator = Simulator(level)
-while not simulator.done:
-    action = Action(randint(0, 3))
+level = GridWorldLevel(
+    game,
+    GridWorldObserver(game),
+    GridWorldEstimator(game),
+    GridWorldVisualizer(game),
+)
+simulator = Simulator(level, 50)
+FPS = 4
+DONE = False
+while not DONE:
+    action = simulator.action_space.sample()
     simulator.step(action)
+    obs = simulator.observe()
+    reward = simulator.estimate()
+    simulator.render_human(FPS)
+    DONE = simulator.truncated or simulator.done
+simulator.close()
 ```
 
 ### 📃 Documentation
 
 Some doc-strings are already added. Documentation is a work-in-progress and will be updated on a time by time basis.
 
 ### 💃🕺 Contribution
```

### Comparing `environment_framework-0.2.0/pyproject.toml` & `environment_framework-0.3.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 description = "Loose building blocks to create agent-environment loops."
 requires-python = ">=3.8"
 authors = [
     { name = "Reto Barmettler"},
 ]
 dependencies = [
     "gymnasium>=0.26",
-    "numpy"
+    "numpy",
+    "pygame"
 ]
 classifiers =[
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -108,15 +109,15 @@
     "311"
 ]
 
 [tool.hatch.envs.type]
 features = [
     "type"
 ]
-scripts.typing = "mypy src/"
+scripts.typing = "mypy src/ && mypy example/*.py"
 
 [[tool.hatch.envs.type.matrix]]
 python = [
     "38", "39", "310", "311"
 ]
 
 [tool.hatch.envs.test]
```

### Comparing `environment_framework-0.2.0/PKG-INFO` & `environment_framework-0.3.0a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: environment-framework
-Version: 0.2.0
+Version: 0.3.0a0
 Summary: Loose building blocks to create agent-environment loops.
 Project-URL: Source, https://github.com/crzdg/environment-framework
 Author: Reto Barmettler
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: gymnasium>=0.26
 Requires-Dist: numpy
+Requires-Dist: pygame
 Provides-Extra: ci
 Requires-Dist: genbadge[all]; extra == 'ci'
 Requires-Dist: hatch; extra == 'ci'
 Requires-Dist: hatch-regex-commit; extra == 'ci'
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Provides-Extra: extra
@@ -78,15 +79,15 @@
 
 ```bash
 pip3 install "environment-framework[extra]"
 jupyter lab
 ```
 
 ```python
-class Action(Enum):
+class Action:
     UP = 0
     DOWN = 1
     RIGHT = 2
     LEFT = 3
 
 class GridWorldGame:
     def __init__(self, size: int) -> None:
@@ -99,16 +100,15 @@
     def done(self) -> bool:
         return self.player_position == self.target_position
 
     @property
     def space(self) -> Space:
         return Discrete(4)
 
-
-    def act(self, action: Action, **_: Any) -> None:
+    def act(self, action: int, **_: Any) -> None:
         if action == Action.UP:
             self.player_position = (self.player_position[0], self.player_position[1] - 1)
         if action == Action.DOWN:
             self.player_position = (self.player_position[0], self.player_position[1] + 1)
         if action == Action.RIGHT:
             self.player_position = (self.player_position[0] + 1, self.player_position[1])
         if action == Action.LEFT:
@@ -129,67 +129,71 @@
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
     @property
     def space(self) -> Space:
         return Box(shape=(4,), low=-math.inf, high=math.inf)
 
-    def observe(self, _: Any) -> NDArray:
-        return np.array([*self.game.player_position, *self.game.target_position])
+    def observe(self) -> NDArray:
+        return np.array(
+            [*self.game.player_position, *self.game.target_position],
+            dtype=np.float32,
+        )
 
 class GridWorldEstimator:
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
-    def estimate(self, _: Any) -> float:
+    def estimate(self) -> float:
         return -1 + float(self.game.done)
 
-class GridWorldVisualizer:
-    # We use BGR
-    BLUE = [255, 0, 0]
+class GridWorldVisualizer(PygameHumanVisualizer):
+    BLUE = [0, 0, 255]
     GREEN = [0, 255, 0]
 
     def __init__(self, game: GridWorldGame) -> None:
+        super().__init__(50)
         self.game = game
 
-    def render(self, _: Any) -> Any:
+    def render_rgb(self) -> NDArray[np.uint8]:
         frame = [[[0 for k in range(3)] for j in range(self.game.size)] for i in range(self.game.size)]
         frame[self.game.player_position[1]][self.game.player_position[0]] = self.BLUE
         frame[self.game.target_position[1]][self.game.target_position[0]] = self.GREEN
-        return frame
+        return np.array(frame, dtype=np.uint8)
 
 class GridWorldLevel(Level):
     _game: GridWorldGame
     _observer: GridWorldObserver
     _estimator: GridWorldEstimator
     _visualizer: GridWorldVisualizer
 
-    def __init__(
-        self,
-        game: GridWorldGame,
-        observer: GridWorldObserver,
-        estimator: GridWorldEstimator,
-        visualizer: GridWorldVisualizer,
-    ) -> None:
-        super().__init__(game, observer, estimator, visualizer)
-
     def reset(self) -> None:
         self._game.reset()
 
-    def step(self, action: Action) -> Any:
-        if isinstance(action, np.int64):  # handle integer inputs
-            action = Action(action)
+    def step(self, action: int) -> Any:
         self._game.act(action)
 
 game = GridWorldGame(7)
-level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))
-simulator = Simulator(level)
-while not simulator.done:
-    action = Action(randint(0, 3))
+level = GridWorldLevel(
+    game,
+    GridWorldObserver(game),
+    GridWorldEstimator(game),
+    GridWorldVisualizer(game),
+)
+simulator = Simulator(level, 50)
+FPS = 4
+DONE = False
+while not DONE:
+    action = simulator.action_space.sample()
     simulator.step(action)
+    obs = simulator.observe()
+    reward = simulator.estimate()
+    simulator.render_human(FPS)
+    DONE = simulator.truncated or simulator.done
+simulator.close()
 ```
 
 ### 📃 Documentation
 
 Some doc-strings are already added. Documentation is a work-in-progress and will be updated on a time by time basis.
 
 ### 💃🕺 Contribution
```

