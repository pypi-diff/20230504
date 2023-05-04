# Comparing `tmp/mabby-0.1.1.tar.gz` & `tmp/mabby-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mabby-0.1.1.tar", max compression
+gzip compressed data, was "mabby-0.1.2.tar", max compression
```

## Comparing `mabby-0.1.1.tar` & `mabby-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-03-07 22:18:31.213711 mabby-0.1.1/LICENSE
--rw-r--r--   0        0        0     2153 2023-03-20 02:10:38.999007 mabby-0.1.1/README.md
--rw-r--r--   0        0        0      406 2023-03-20 00:10:12.363583 mabby-0.1.1/mabby/__init__.py
--rw-r--r--   0        0        0      286 2023-03-20 00:10:12.363951 mabby-0.1.1/mabby/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-20 00:10:12.364202 mabby-0.1.1/mabby/simulation/__init__.py
--rw-r--r--   0        0        0     1678 2023-03-20 00:10:12.364550 mabby-0.1.1/mabby/simulation/agent.py
--rw-r--r--   0        0        0     1490 2023-03-20 00:10:12.364985 mabby-0.1.1/mabby/simulation/arms.py
--rw-r--r--   0        0        0     1232 2023-03-20 00:10:12.365264 mabby-0.1.1/mabby/simulation/bandit.py
--rw-r--r--   0        0        0      317 2023-03-20 00:10:12.365591 mabby-0.1.1/mabby/simulation/exceptions.py
--rw-r--r--   0        0        0     2687 2023-03-20 00:10:12.366104 mabby-0.1.1/mabby/simulation/simulation.py
--rw-r--r--   0        0        0     4311 2023-03-20 00:10:12.366361 mabby-0.1.1/mabby/simulation/stats.py
--rw-r--r--   0        0        0      409 2023-03-20 00:10:12.366894 mabby-0.1.1/mabby/strategies/__init__.py
--rw-r--r--   0        0        0      107 2023-03-20 00:10:12.367148 mabby-0.1.1/mabby/strategies/exceptions.py
--rw-r--r--   0        0        0     1927 2023-03-20 00:10:12.367461 mabby-0.1.1/mabby/strategies/semi_uniform.py
--rw-r--r--   0        0        0     1037 2023-03-20 00:10:12.367731 mabby-0.1.1/mabby/strategies/strategy.py
--rw-r--r--   0        0        0     1798 2023-03-20 00:10:12.367973 mabby-0.1.1/mabby/strategies/ts.py
--rw-r--r--   0        0        0     1408 2023-03-20 00:10:12.368188 mabby-0.1.1/mabby/strategies/ucb.py
--rw-r--r--   0        0        0      282 2023-03-20 00:10:12.284944 mabby-0.1.1/mabby/utils.py
--rw-r--r--   0        0        0      880 2023-03-20 02:41:05.694777 mabby-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2884 1970-01-01 00:00:00.000000 mabby-0.1.1/setup.py
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 mabby-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-04 15:12:10.403316 mabby-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2374 2023-05-04 16:12:37.708752 mabby-0.1.2/README.md
+-rw-r--r--   0        0        0      901 2023-05-04 15:12:10.413613 mabby-0.1.2/mabby/__init__.py
+-rw-r--r--   0        0        0     4102 2023-05-04 15:12:10.413798 mabby-0.1.2/mabby/agent.py
+-rw-r--r--   0        0        0     3820 2023-05-04 15:12:10.414092 mabby-0.1.2/mabby/arms.py
+-rw-r--r--   0        0        0     3317 2023-05-04 15:12:10.414355 mabby-0.1.2/mabby/bandit.py
+-rw-r--r--   0        0        0      475 2023-05-04 15:12:10.414521 mabby-0.1.2/mabby/exceptions.py
+-rw-r--r--   0        0        0     4323 2023-05-04 15:12:10.414745 mabby-0.1.2/mabby/simulation.py
+-rw-r--r--   0        0        0     8566 2023-05-04 15:12:10.414981 mabby-0.1.2/mabby/stats.py
+-rw-r--r--   0        0        0      743 2023-05-04 18:01:36.800971 mabby-0.1.2/mabby/strategies/__init__.py
+-rw-r--r--   0        0        0     4717 2023-05-04 18:01:36.801292 mabby-0.1.2/mabby/strategies/semi_uniform.py
+-rw-r--r--   0        0        0     2255 2023-05-04 15:12:10.415642 mabby-0.1.2/mabby/strategies/strategy.py
+-rw-r--r--   0        0        0     2298 2023-05-04 15:12:10.415870 mabby-0.1.2/mabby/strategies/thompson.py
+-rw-r--r--   0        0        0     1737 2023-05-04 15:12:10.416097 mabby-0.1.2/mabby/strategies/ucb.py
+-rw-r--r--   0        0        0      599 2023-05-04 15:12:10.416382 mabby-0.1.2/mabby/utils.py
+-rw-r--r--   0        0        0     1603 2023-05-04 18:10:29.488093 mabby-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3130 1970-01-01 00:00:00.000000 mabby-0.1.2/setup.py
+-rw-r--r--   0        0        0     3006 1970-01-01 00:00:00.000000 mabby-0.1.2/PKG-INFO
```

### Comparing `mabby-0.1.1/LICENSE` & `mabby-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mabby-0.1.1/README.md` & `mabby-0.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,57 @@
 <h1 align="center">
 <img src="https://raw.githubusercontent.com/ew2664/mabby/main/assets/mabby-logo-title.png" width="500">
 </h1>
 
+[![PyPI](https://img.shields.io/pypi/v/mabby)](https://pypi.org/project/mabby/)
 [![license](https://img.shields.io/github/license/ew2664/mabby)](https://github.com/ew2664/mabby/blob/main/LICENSE)
 [![issues](https://img.shields.io/github/issues/ew2664/mabby)](https://github.com/ew2664/mabby/issues)
-[![build](https://img.shields.io/github/actions/workflow/status/ew2664/mabby/ci.yml)](https://github.com/ew2664/mabby/actions/workflows/ci.yml)
+[![build](https://img.shields.io/github/actions/workflow/status/ew2664/mabby/build.yml)](https://github.com/ew2664/mabby/actions/workflows/build.yml)
+[![docs](https://img.shields.io/github/actions/workflow/status/ew2664/mabby/docs.yml?label=docs)](https://ew2664.github.io/mabby/)
 [![coverage](https://coveralls.io/repos/github/ew2664/mabby/badge.svg)](https://coveralls.io/github/ew2664/mabby)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![poetry](https://img.shields.io/badge/packaging-poetry-008adf)](https://python-poetry.org/)
-[![black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
-[![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
 **mabby** is a library for simulating [multi-armed bandits (MABs)](https://en.wikipedia.org/wiki/Multi-armed_bandit), a resource-allocation problem and framework in reinforcement learning. It allows users to quickly yet flexibly define and run bandit simulations, with the ability to:
 
 - choose from a wide range of classic bandit algorithms to use
 - configure environments with custom arm spaces and rewards distributions
 - collect and visualize simulation metrics like regret and optimality
 
 ## Installation
 
+Prerequisites: [Python 3.9+](https://www.python.org/downloads/) and `pip`
+
 Install **mabby** with `pip`:
 
 ```bash
 pip install mabby
 ```
 
-## Examples
+## Basic Usage
+
+The code example below demonstrates the basic steps of running a simulation with **mabby**. For more in-depth examples, please see the [Usage Examples](https://ew2664.github.io/mabby/examples/) section of the **mabby** documentation.
+
+```python
+import mabby as mb
+
+# configure bandit arms
+bandit = mb.BernoulliArm.bandit(p=[0.3, 0.6])
 
-- [**Bernoulli Bandits**](./examples/bernoulli_bandit.py): a four-armed Bernoulli bandit simulation comparing epsilon-greedy, UCB1, and Thompson sampling strategies
+# configure bandit strategy
+strategy = mb.strategies.EpsilonGreedyStrategy(eps=0.2)
+
+# setup simulation
+simulation = mb.Simulation(bandit=bandit, strategies=[strategy])
+
+# run simulation
+stats = simulation.run(trials=100, steps=300)
+
+# plot regret statistics
+stats.plot_regret()
+```
 
 ## Contributing
 
-Please see [CONTRIBUTING](CONTRIBUTING.md) for more information.
+Please see [CONTRIBUTING](https://ew2664.github.io/mabby/contributing/) for more information.
 
 ## License
 
-This software is licensed under the Apache 2.0 license. Please see [LICENSE](LICENSE) for more information.
+This software is licensed under the Apache 2.0 license. Please see [LICENSE](https://ew2664.github.io/mabby/license/) for more information.
```

### Comparing `mabby-0.1.1/mabby/simulation/agent.py` & `mabby-0.1.2/mabby/strategies/ucb.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,63 @@
+"""Provides implementations of upper confidence bound (UCB) strategies."""
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
-
 import numpy as np
 from numpy.random import Generator
 from numpy.typing import NDArray
+from overrides import override
+
+from mabby.strategies.strategy import Strategy
+from mabby.utils import random_argmax
 
-from mabby.simulation.exceptions import AgentUsageError
 
-if TYPE_CHECKING:
-    from mabby.strategies import Strategy
+class UCB1Strategy(Strategy):
+    """Strategy using the UCB1 bandit algorithm."""
 
+    _t: int
+    _Qs: NDArray[np.float64]
+    _Ns: NDArray[np.uint32]
 
-class Agent:
-    _rng: Generator
+    def __init__(self, alpha: float) -> None:
+        """Initializes a UCB1 strategy.
 
-    def __init__(self, strategy: Strategy, name: str | None = None):
-        self.strategy = strategy
-        self._name = name
-        self._primed = False
-        self._choice: int | None = None
+        Args:
+            alpha: The exploration parameter.
+        """
+        if alpha < 0:
+            raise ValueError("alpha must be greater than 0")
+        self.alpha = alpha
 
+    @override
     def __repr__(self) -> str:
-        if self._name is None:
-            return str(self.strategy)
-        return self._name
-
-    def prime(self, k: int, steps: int, rng: Generator) -> None:
-        self._primed = True
-        self._choice = None
-        self._rng = rng
-        self.strategy.prime(k, steps)
-
-    def choose(self) -> int:
-        if not self._primed:
-            raise AgentUsageError("choose() can only be called on a primed agent")
-        self._choice = self.strategy.choose(self._rng)
-        return self._choice
-
-    def update(self, reward: float) -> None:
-        if self._choice is None:
-            raise AgentUsageError("update() can only be called after choose()")
-        self.strategy.update(self._choice, reward, self._rng)
-        self._choice = None
+        return f"ucb1 (alpha={self.alpha})"
+
+    @override
+    def prime(self, k: int, steps: int) -> None:
+        self._t = 0
+        self._Qs = np.zeros(k, dtype=np.float64)
+        self._Ns = np.zeros(k, dtype=np.uint32)
+
+    @override
+    def choose(self, rng: Generator) -> int:
+        if self._t < len(self._Ns):
+            return self._t
+        return random_argmax(self._compute_UCBs(), rng=rng)
+
+    def _compute_UCBs(self) -> NDArray[np.float64]:
+        return self._Qs + self.alpha * np.sqrt(np.log(self._t) / self._Ns)
+
+    @override
+    def update(self, choice: int, reward: float, rng: Generator | None = None) -> None:
+        self._t += 1
+        self._Ns[choice] += 1
+        self._Qs[choice] += (reward - self._Qs[choice]) / self._Ns[choice]
 
     @property
+    @override
     def Qs(self) -> NDArray[np.float64]:
-        if not self._primed:
-            raise AgentUsageError("agent has no Q values before it is run")
-        return self.strategy.Qs
+        return self._Qs
 
     @property
+    @override
     def Ns(self) -> NDArray[np.uint32]:
-        if not self._primed:
-            raise AgentUsageError("agent has no Q values before it is run")
-        return self.strategy.Ns
+        return self._Ns
```

### Comparing `mabby-0.1.1/mabby/simulation/stats.py` & `mabby-0.1.2/mabby/simulation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,119 @@
+"""Provides [`Simulation`][mabby.simulation.Simulation] class for bandit simulations."""
+
 from __future__ import annotations
 
 from collections.abc import Iterable
-from dataclasses import dataclass
-from enum import Enum
-from typing import TYPE_CHECKING, Callable
+from itertools import zip_longest
+from typing import TYPE_CHECKING
 
 import numpy as np
-from matplotlib import pyplot as plt
-from numpy.typing import NDArray
+from numpy.random import Generator
 
-from mabby.exceptions import StatsUsageError
+from mabby.agent import Agent
+from mabby.exceptions import SimulationUsageError
+from mabby.stats import AgentStats, Metric, SimulationStats
 
 if TYPE_CHECKING:
-    from mabby import Agent, Bandit, Simulation
-
-
-@dataclass
-class MetricMapping:
-    base: Metric
-    transform: Callable[[NDArray[np.float64]], NDArray[np.float64]]
+    from mabby.bandit import Bandit
+    from mabby.strategies import Strategy
 
 
-class Metric(Enum):
-    REGRET = "Regret"
-    REWARDS = "Rewards"
-    OPTIMALITY = "Optimality"
-    CUM_REGRET = "Cumulative Regret", "REGRET", np.cumsum
-    CUM_REWARDS = "Cumulative Rewards", "REWARDS", np.cumsum
+class Simulation:
+    """Simulation of a multi-armed bandit problem.
 
-    __MAPPING__: dict[str, Metric] = {}
+    A simulation consists of multiple trials of one or more bandit strategies run on a
+    configured multi-armed bandit.
+    """
 
     def __init__(
         self,
-        label: str,
-        base: str | None = None,
-        transform: Callable[[NDArray[np.float64]], NDArray[np.float64]] | None = None,
+        bandit: Bandit,
+        agents: Iterable[Agent] | None = None,
+        strategies: Iterable[Strategy] | None = None,
+        names: Iterable[str] | None = None,
+        rng: Generator | None = None,
+        seed: int | None = None,
     ):
-        self.__class__.__MAPPING__[self._name_] = self
-        self._label = label
-        self._mapping: MetricMapping | None = (
-            MetricMapping(base=self.__class__.__MAPPING__[base], transform=transform)
-            if base and transform
-            else None
-        )
-
-    def __repr__(self) -> str:
-        return self._label
-
-    def is_base(self) -> bool:
-        return self._mapping is None
-
-    @property
-    def base(self) -> Metric:
-        if self._mapping is not None:
-            return self._mapping.base
-        return self
-
-    @classmethod
-    def map_to_base(cls, metrics: Iterable[Metric]) -> Iterable[Metric]:
-        return set(m.base for m in metrics)
-
-    def transform(self, values: NDArray[np.float64]) -> NDArray[np.float64]:
-        if self._mapping is not None:
-            return self._mapping.transform(values)
-        return values
-
-
-class SimulationStats:
-    def __init__(self, simulation: Simulation):
-        self._simulation: Simulation = simulation
-        self._stats_dict: dict[Agent, AgentStats] = {}
+        """Initializes a simulation.
 
-    def add(self, agent_stats: AgentStats) -> None:
-        self._stats_dict[agent_stats.agent] = agent_stats
+        One of ``agents`` or ``strategies`` must be supplied. If ``agents`` is supplied,
+        ``strategies`` and ``names`` are ignored. Otherwise, an ``agent`` is created for
+        each ``strategy`` and given a name from ``names`` if available.
+
+        Args:
+            bandit: A configured multi-armed bandit to simulate on.
+            agents: A list of agents to simulate.
+            strategies: A list of strategies to simulate.
+            names: A list of names for agents.
+            rng: A random number generator.
+            seed: A seed for random number generation if ``rng`` is not provided.
+
+        Raises:
+            SimulationUsageError: If neither ``agents`` nor ``strategies`` are supplied.
+        """
+        self.agents = self._create_agents(agents, strategies, names)
+        if len(list(self.agents)) == 0:
+            raise ValueError("no strategies or agents were supplied")
+        self.bandit = bandit
+        if len(self.bandit) == 0:
+            raise ValueError("bandit cannot be empty")
+        self._rng = rng if rng else np.random.default_rng(seed)
+
+    @staticmethod
+    def _create_agents(
+        agents: Iterable[Agent] | None = None,
+        strategies: Iterable[Strategy] | None = None,
+        names: Iterable[str] | None = None,
+    ) -> Iterable[Agent]:
+        if agents is not None:
+            return agents
+        if strategies is not None and names is not None:
+            return [
+                strategy.agent(name=name)
+                for strategy, name in zip_longest(strategies, names)
+                if strategy
+            ]
+        if strategies is not None:
+            return [strategy.agent() for strategy in strategies]
+        raise SimulationUsageError("one of agents or strategies must be supplied")
+
+    def run(
+        self, trials: int, steps: int, metrics: Iterable[Metric] | None = None
+    ) -> SimulationStats:
+        """Runs a simulation.
+
+        In a simulation run, each agent or strategy is run for the specified number of
+        trials, and each trial is run for the given number of steps.
+
+        If ``metrics`` is not specified, all available metrics are tracked by default.
+
+        Args:
+            trials: The number of trials in the simulation.
+            steps: The number of steps in a trial.
+            metrics: A list of metrics to collect.
+
+        Returns:
+            A ``SimulationStats`` object with the results of the simulation.
+        """
+        sim_stats = SimulationStats(simulation=self)
+        for agent in self.agents:
+            agent_stats = self._run_trials_for_agent(agent, trials, steps, metrics)
+            sim_stats.add(agent_stats)
+        return sim_stats
 
-    def __getitem__(self, agent: Agent) -> AgentStats:
-        return self._stats_dict[agent]
-
-    def __setitem__(self, agent: Agent, agent_stats: AgentStats) -> None:
-        if agent != agent_stats.agent:
-            raise StatsUsageError("agents specified in key and value don't match")
-        self._stats_dict[agent] = agent_stats
-
-    def __contains__(self, agent: Agent) -> bool:
-        return agent in self._stats_dict
-
-    def plot(self, metric: Metric) -> None:
-        for agent, agent_stats in self._stats_dict.items():
-            plt.plot(agent_stats[metric], label=str(agent))
-        plt.legend()
-        plt.show()
-
-    def plot_regret(self, cumulative: bool = True) -> None:
-        self.plot(metric=Metric.CUM_REGRET if cumulative else Metric.REGRET)
-
-    def plot_optimality(self) -> None:
-        self.plot(metric=Metric.OPTIMALITY)
-
-    def plot_rewards(self, cumulative: bool = True) -> None:
-        self.plot(metric=Metric.CUM_REWARDS if cumulative else Metric.REWARDS)
-
-
-class AgentStats:
-    def __init__(
+    def _run_trials_for_agent(
         self,
         agent: Agent,
-        bandit: Bandit,
+        trials: int,
         steps: int,
         metrics: Iterable[Metric] | None = None,
-    ):
-        self.agent = agent
-        self._bandit = bandit
-        self._steps = steps
-        self._counts = np.zeros(steps)
-
-        base_metrics = Metric.map_to_base(list(Metric) if metrics is None else metrics)
-        self._stats = {stat: np.zeros(steps) for stat in base_metrics}
-
-    def __len__(self) -> int:
-        return self._steps
-
-    def __getitem__(self, metric: Metric) -> NDArray[np.float64]:
-        with np.errstate(divide="ignore", invalid="ignore"):
-            values = self._stats[metric.base] / self._counts
-        return metric.transform(values)
-
-    def update(self, step: int, choice: int, reward: float) -> None:
-        regret = self._bandit.regret(choice)
-        if Metric.REGRET in self._stats:
-            self._stats[Metric.REGRET][step] += regret
-        if Metric.OPTIMALITY in self._stats:
-            self._stats[Metric.OPTIMALITY][step] += int(self._bandit.is_opt(choice))
-        if Metric.REWARDS in self._stats:
-            self._stats[Metric.REWARDS][step] += reward
-        self._counts[step] += 1
+    ) -> AgentStats:
+        agent_stats = AgentStats(agent, self.bandit, steps, metrics)
+        for _ in range(trials):
+            agent.prime(len(self.bandit), steps, self._rng)
+            for step in range(steps):
+                choice = agent.choose()
+                reward = self.bandit.play(choice)
+                agent.update(reward)
+                agent_stats.update(step, choice, reward)
+        return agent_stats
```

### Comparing `mabby-0.1.1/mabby/strategies/ts.py` & `mabby-0.1.2/mabby/strategies/thompson.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,53 @@
+"""Provides implementations of Thompson sampling strategies."""
+
 from __future__ import annotations
 
 import numpy as np
 from numpy.random import Generator
 from numpy.typing import NDArray
+from overrides import override
 
-from mabby.strategies.exceptions import StrategyUsageError
+from mabby.exceptions import StrategyUsageError
 from mabby.strategies.strategy import Strategy
 from mabby.utils import random_argmax
 
 
 class BetaTSStrategy(Strategy):
+    """Thompson sampling strategy with Beta priors."""
+
     _a: NDArray[np.uint32]
     _b: NDArray[np.uint32]
 
     def __init__(self, general: bool = False):
-        super().__init__()
+        """Initializes a Beta Thompson sampling strategy.
+
+        If ``general`` is ``False``, rewards used for updates must be either 0 or 1.
+        Otherwise, rewards must be with support [0, 1].
+
+        Args:
+            general: Whether to use a generalized version of the strategy.
+        """
         self.general = general
 
+    @override
     def __repr__(self) -> str:
         return f"{'generalized ' if self.general else ''}beta ts"
 
+    @override
     def prime(self, k: int, steps: int) -> None:
         self._a = np.ones(k, dtype=np.uint32)
         self._b = np.ones(k, dtype=np.uint32)
 
+    @override
     def choose(self, rng: Generator) -> int:
         samples = rng.beta(a=self._a, b=self._b)
         return random_argmax(samples, rng=rng)
 
+    @override
     def update(self, choice: int, reward: float, rng: Generator | None = None) -> None:
         if rng is None:
             raise StrategyUsageError("TS strategies require rng")
         if self.general and (reward > 1 or reward < 0):
             raise StrategyUsageError(
                 "general Beta TS agents can only be used with rewards from 0 to 1"
             )
@@ -40,13 +56,15 @@
                 "Beta TS agents can only be used with Bernoulli rewards"
             )
         pseudo_reward = rng.binomial(n=1, p=reward) if self.general else reward
         self._a[choice] += pseudo_reward
         self._b[choice] += 1 - pseudo_reward
 
     @property
+    @override
     def Qs(self) -> NDArray[np.float64]:
         return self._a / (self._a + self._b)
 
     @property
+    @override
     def Ns(self) -> NDArray[np.uint32]:
         return ((self._a + self._b).astype(np.int64) - 2).astype(np.uint32)
```

### Comparing `mabby-0.1.1/setup.py` & `mabby-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['mabby', 'mabby.simulation', 'mabby.strategies']
+['mabby', 'mabby.strategies']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['matplotlib>=3.7.0,<4.0.0', 'numpy>=1.24.2,<2.0.0']
+['matplotlib>=3.7.0,<4.0.0', 'numpy>=1.24.2,<2.0.0', 'overrides>=7.3.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'mabby',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A multi-armed bandit (MAB) simulation library',
-    'long_description': '<h1 align="center">\n<img src="https://raw.githubusercontent.com/ew2664/mabby/main/assets/mabby-logo-title.png" width="500">\n</h1>\n\n[![license](https://img.shields.io/github/license/ew2664/mabby)](https://github.com/ew2664/mabby/blob/main/LICENSE)\n[![issues](https://img.shields.io/github/issues/ew2664/mabby)](https://github.com/ew2664/mabby/issues)\n[![build](https://img.shields.io/github/actions/workflow/status/ew2664/mabby/ci.yml)](https://github.com/ew2664/mabby/actions/workflows/ci.yml)\n[![coverage](https://coveralls.io/repos/github/ew2664/mabby/badge.svg)](https://coveralls.io/github/ew2664/mabby)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n[![poetry](https://img.shields.io/badge/packaging-poetry-008adf)](https://python-poetry.org/)\n[![black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)\n[![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n\n**mabby** is a library for simulating [multi-armed bandits (MABs)](https://en.wikipedia.org/wiki/Multi-armed_bandit), a resource-allocation problem and framework in reinforcement learning. It allows users to quickly yet flexibly define and run bandit simulations, with the ability to:\n\n- choose from a wide range of classic bandit algorithms to use\n- configure environments with custom arm spaces and rewards distributions\n- collect and visualize simulation metrics like regret and optimality\n\n## Installation\n\nInstall **mabby** with `pip`:\n\n```bash\npip install mabby\n```\n\n## Examples\n\n- [**Bernoulli Bandits**](./examples/bernoulli_bandit.py): a four-armed Bernoulli bandit simulation comparing epsilon-greedy, UCB1, and Thompson sampling strategies\n\n## Contributing\n\nPlease see [CONTRIBUTING](CONTRIBUTING.md) for more information.\n\n## License\n\nThis software is licensed under the Apache 2.0 license. Please see [LICENSE](LICENSE) for more information.\n',
+    'long_description': '<h1 align="center">\n<img src="https://raw.githubusercontent.com/ew2664/mabby/main/assets/mabby-logo-title.png" width="500">\n</h1>\n\n[![PyPI](https://img.shields.io/pypi/v/mabby)](https://pypi.org/project/mabby/)\n[![license](https://img.shields.io/github/license/ew2664/mabby)](https://github.com/ew2664/mabby/blob/main/LICENSE)\n[![issues](https://img.shields.io/github/issues/ew2664/mabby)](https://github.com/ew2664/mabby/issues)\n[![build](https://img.shields.io/github/actions/workflow/status/ew2664/mabby/build.yml)](https://github.com/ew2664/mabby/actions/workflows/build.yml)\n[![docs](https://img.shields.io/github/actions/workflow/status/ew2664/mabby/docs.yml?label=docs)](https://ew2664.github.io/mabby/)\n[![coverage](https://coveralls.io/repos/github/ew2664/mabby/badge.svg)](https://coveralls.io/github/ew2664/mabby)\n\n**mabby** is a library for simulating [multi-armed bandits (MABs)](https://en.wikipedia.org/wiki/Multi-armed_bandit), a resource-allocation problem and framework in reinforcement learning. It allows users to quickly yet flexibly define and run bandit simulations, with the ability to:\n\n- choose from a wide range of classic bandit algorithms to use\n- configure environments with custom arm spaces and rewards distributions\n- collect and visualize simulation metrics like regret and optimality\n\n## Installation\n\nPrerequisites: [Python 3.9+](https://www.python.org/downloads/) and `pip`\n\nInstall **mabby** with `pip`:\n\n```bash\npip install mabby\n```\n\n## Basic Usage\n\nThe code example below demonstrates the basic steps of running a simulation with **mabby**. For more in-depth examples, please see the [Usage Examples](https://ew2664.github.io/mabby/examples/) section of the **mabby** documentation.\n\n```python\nimport mabby as mb\n\n# configure bandit arms\nbandit = mb.BernoulliArm.bandit(p=[0.3, 0.6])\n\n# configure bandit strategy\nstrategy = mb.strategies.EpsilonGreedyStrategy(eps=0.2)\n\n# setup simulation\nsimulation = mb.Simulation(bandit=bandit, strategies=[strategy])\n\n# run simulation\nstats = simulation.run(trials=100, steps=300)\n\n# plot regret statistics\nstats.plot_regret()\n```\n\n## Contributing\n\nPlease see [CONTRIBUTING](https://ew2664.github.io/mabby/contributing/) for more information.\n\n## License\n\nThis software is licensed under the Apache 2.0 license. Please see [LICENSE](https://ew2664.github.io/mabby/license/) for more information.\n',
     'author': 'Ethan Wu',
     'author_email': 'ew2664@columbia.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mabby-0.1.1/PKG-INFO` & `mabby-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,76 @@
 Metadata-Version: 2.1
 Name: mabby
-Version: 0.1.1
+Version: 0.1.2
 Summary: A multi-armed bandit (MAB) simulation library
 License: Apache-2.0
 Author: Ethan Wu
 Author-email: ew2664@columbia.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: overrides (>=7.3.1,<8.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
 <img src="https://raw.githubusercontent.com/ew2664/mabby/main/assets/mabby-logo-title.png" width="500">
 </h1>
 
+[![PyPI](https://img.shields.io/pypi/v/mabby)](https://pypi.org/project/mabby/)
 [![license](https://img.shields.io/github/license/ew2664/mabby)](https://github.com/ew2664/mabby/blob/main/LICENSE)
 [![issues](https://img.shields.io/github/issues/ew2664/mabby)](https://github.com/ew2664/mabby/issues)
-[![build](https://img.shields.io/github/actions/workflow/status/ew2664/mabby/ci.yml)](https://github.com/ew2664/mabby/actions/workflows/ci.yml)
+[![build](https://img.shields.io/github/actions/workflow/status/ew2664/mabby/build.yml)](https://github.com/ew2664/mabby/actions/workflows/build.yml)
+[![docs](https://img.shields.io/github/actions/workflow/status/ew2664/mabby/docs.yml?label=docs)](https://ew2664.github.io/mabby/)
 [![coverage](https://coveralls.io/repos/github/ew2664/mabby/badge.svg)](https://coveralls.io/github/ew2664/mabby)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![poetry](https://img.shields.io/badge/packaging-poetry-008adf)](https://python-poetry.org/)
-[![black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
-[![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
 **mabby** is a library for simulating [multi-armed bandits (MABs)](https://en.wikipedia.org/wiki/Multi-armed_bandit), a resource-allocation problem and framework in reinforcement learning. It allows users to quickly yet flexibly define and run bandit simulations, with the ability to:
 
 - choose from a wide range of classic bandit algorithms to use
 - configure environments with custom arm spaces and rewards distributions
 - collect and visualize simulation metrics like regret and optimality
 
 ## Installation
 
+Prerequisites: [Python 3.9+](https://www.python.org/downloads/) and `pip`
+
 Install **mabby** with `pip`:
 
 ```bash
 pip install mabby
 ```
 
-## Examples
+## Basic Usage
+
+The code example below demonstrates the basic steps of running a simulation with **mabby**. For more in-depth examples, please see the [Usage Examples](https://ew2664.github.io/mabby/examples/) section of the **mabby** documentation.
+
+```python
+import mabby as mb
+
+# configure bandit arms
+bandit = mb.BernoulliArm.bandit(p=[0.3, 0.6])
 
-- [**Bernoulli Bandits**](./examples/bernoulli_bandit.py): a four-armed Bernoulli bandit simulation comparing epsilon-greedy, UCB1, and Thompson sampling strategies
+# configure bandit strategy
+strategy = mb.strategies.EpsilonGreedyStrategy(eps=0.2)
+
+# setup simulation
+simulation = mb.Simulation(bandit=bandit, strategies=[strategy])
+
+# run simulation
+stats = simulation.run(trials=100, steps=300)
+
+# plot regret statistics
+stats.plot_regret()
+```
 
 ## Contributing
 
-Please see [CONTRIBUTING](CONTRIBUTING.md) for more information.
+Please see [CONTRIBUTING](https://ew2664.github.io/mabby/contributing/) for more information.
 
 ## License
 
-This software is licensed under the Apache 2.0 license. Please see [LICENSE](LICENSE) for more information.
+This software is licensed under the Apache 2.0 license. Please see [LICENSE](https://ew2664.github.io/mabby/license/) for more information.
```

