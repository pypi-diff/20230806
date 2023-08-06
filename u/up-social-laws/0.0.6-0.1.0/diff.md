# Comparing `tmp/up_social_laws-0.0.6.tar.gz` & `tmp/up_social_laws-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_social_laws-0.0.6.tar", last modified: Fri Jul 21 05:00:12 2023, max compression
+gzip compressed data, was "up_social_laws-0.1.0.tar", last modified: Sun Aug  6 08:40:15 2023, max compression
```

## Comparing `up_social_laws-0.0.6.tar` & `up_social_laws-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:00:12.116948 up_social_laws-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-21 05:00:12.112947 up_social_laws-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:00:12.116948 up_social_laws-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:00:12.112947 up_social_laws-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)    21874 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/test/test_social_law.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:00:12.112947 up_social_laws-0.0.6/up_social_laws/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/up_social_laws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/up_social_laws/ma_centralizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/up_social_laws/ma_problem_waitfor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/up_social_laws/robustness_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    52291 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/up_social_laws/robustness_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/up_social_laws/sa_to_ma_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/up_social_laws/single_agent_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    17703 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/up_social_laws/social_law.py
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/up_social_laws/synthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-21 05:00:01.000000 up_social_laws-0.0.6/up_social_laws/waitfor_specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:00:12.112947 up_social_laws-0.0.6/up_social_laws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-21 05:00:12.000000 up_social_laws-0.0.6/up_social_laws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 05:00:12.000000 up_social_laws-0.0.6/up_social_laws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:00:12.000000 up_social_laws-0.0.6/up_social_laws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 05:00:12.000000 up_social_laws-0.0.6/up_social_laws.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:40:15.200603 up_social_laws-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-06 08:40:15.200603 up_social_laws-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 08:40:15.200603 up_social_laws-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:40:15.196603 up_social_laws-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    21997 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/test/test_social_law.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:40:15.196603 up_social_laws-0.1.0/up_social_laws/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/up_social_laws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/up_social_laws/ma_centralizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/up_social_laws/ma_problem_waitfor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/up_social_laws/robustness_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52426 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/up_social_laws/robustness_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/up_social_laws/sa_to_ma_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/up_social_laws/single_agent_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/up_social_laws/social_law.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/up_social_laws/synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-06 08:40:02.000000 up_social_laws-0.1.0/up_social_laws/waitfor_specification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:40:15.200603 up_social_laws-0.1.0/up_social_laws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-06 08:40:15.000000 up_social_laws-0.1.0/up_social_laws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-06 08:40:15.000000 up_social_laws-0.1.0/up_social_laws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 08:40:15.000000 up_social_laws-0.1.0/up_social_laws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 08:40:15.000000 up_social_laws-0.1.0/up_social_laws.egg-info/top_level.txt
```

### Comparing `up_social_laws-0.0.6/LICENSE` & `up_social_laws-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `up_social_laws-0.0.6/PKG-INFO` & `up_social_laws-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up_social_laws
-Version: 0.0.6
+Version: 0.1.0
 Summary: Unified Planning Integration of Social Laws
 Home-page: https://github.com/aiplan4eu/up-social-laws
 Author: Technion Cognitive Robotics Lab
 Author-email: karpase@technion.ac.il
 License: APACHE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `up_social_laws-0.0.6/README.md` & `up_social_laws-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `up_social_laws-0.0.6/setup.py` & `up_social_laws-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `up_social_laws-0.0.6/test/test_social_law.py` & `up_social_laws-0.1.0/test/test_social_law.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,15 +244,16 @@
             glname = l[-1]
             globj = unified_planning.model.Object(glname, loc)
             
             dobj = unified_planning.model.Object(d, direction)
 
             problem.set_initial_value(Dot(car, car.fluent("start")(slobj)), True)
             problem.set_initial_value(Dot(car, car.fluent("traveldirection")(dobj)), True)        
-            problem.add_goal(Dot(car, car.fluent("at")(globj)))
+            car.add_public_goal(car.fluent("at")(globj))
+            #problem.add_goal(Dot(car, car.fluent("at")(globj)))
 
             if len(yields_list) > 0:
                 yields = set()
                 for l1_name, ly_name in yields_list:
                     problem.set_initial_value(yieldsto(problem.object(l1_name), problem.object(ly_name)), True)     
                     yields.add(problem.object(l1_name))
                 for l1 in problem.objects(loc):
@@ -347,16 +348,18 @@
         problem.waitfor.annotate_as_waitfor(agent2.name, move.name, free(l2))
 
         problem.set_initial_value(Dot(agent1, at(nw)), True)
         problem.set_initial_value(Dot(agent2, at(se)), True)
         problem.set_initial_value(free(nw), False)
         problem.set_initial_value(free(se), False)
 
-        problem.add_goal(Dot(agent1, at(sw)))
-        problem.add_goal(Dot(agent2, at(ne)))
+        agent1.add_public_goal(at(sw))
+        agent2.add_public_goal(at(ne))
+        # problem.add_goal(Dot(agent1, at(sw)))
+        # problem.add_goal(Dot(agent2, at(ne)))
 
 
         slrc = SocialLawRobustnessChecker(
             planner_name="fast-downward",
             robustness_verifier_name="SimpleInstantaneousActionRobustnessVerifier",
             save_pddl_prefix="synth"
             )
@@ -477,15 +480,15 @@
     def test_all_cases_durative(self):
         for t in self.test_cases:
             problem = get_intersection_problem(t.cars, t.yields_list, t.wait_drive, durative=True).problem
             with open("waitfor.json", "w") as f:
                 f.write(str(problem.waitfor))
 
             slrc = SocialLawRobustnessChecker(                                
-                save_pddl_prefix=t.name,                
+                save_pddl_prefix=t.name
                 )
             self.assertEqual(slrc.is_robust(problem).status, t.expected_outcome, t.name)
 
     def test_sa_ma_converter(self):
         reader = PDDLReader()
         random.seed(2023)
```

### Comparing `up_social_laws-0.0.6/up_social_laws/__init__.py` & `up_social_laws-0.1.0/up_social_laws/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # This is a hack, since getting the (agent, original action) from the solution of the robustness verification compilation is difficult
 name_separator = "__"
 
-__version__="0.0.6"
+__version__="0.1.0"
```

### Comparing `up_social_laws-0.0.6/up_social_laws/ma_centralizer.py` & `up_social_laws-0.1.0/up_social_laws/ma_centralizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,14 +135,20 @@
 
         for goal in problem.goals:
             if goal.is_dot():                
                 new_problem.add_goal(fmap.get_agent_version(goal.agent(), goal.args[0]))
             else:
                 new_problem.add_goal(fmap.get_environment_version(goal))
 
+        for agent in problem.agents:
+            for goal in agent.public_goals:
+                new_problem.add_goal(fmap.get_agent_version(agent, goal))
+            for goal in agent.private_goals:
+                new_problem.add_goal(fmap.get_agent_version(agent, goal))
+
         return CompilerResult(
             new_problem, partial(replace_action, map=new_to_old), self.name
         )
 
 
 
 env = get_environment()
```

### Comparing `up_social_laws-0.0.6/up_social_laws/ma_problem_waitfor.py` & `up_social_laws-0.1.0/up_social_laws/ma_problem_waitfor.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,19 +54,25 @@
         return MultiAgentProblem.__hash__(self) + hash(self.waitfor)     
 
     def clone(self):
         new_p = MultiAgentProblemWithWaitfor(self._name, self._env)
         for f in self.ma_environment.fluents:
             new_p.ma_environment.add_fluent(f)
         for ag in self.agents:
-            new_ag = Agent(ag.name, self)
-            for f in ag.fluents:
-                new_ag.add_fluent(f)
-            for a in ag.actions:
-                new_ag.add_action(a.clone())
+            new_ag = ag.clone(self)
+            # Agent(ag.name, self)
+            # for f in ag.fluents:
+            #     new_ag.add_fluent(f)
+            # for a in ag.actions:
+            #     new_ag.add_action(a.clone())
+            # for g in ag.private_goals:
+            #     new_ag.add_private_goal(g)
+            # for g in ag.public_goals:
+            #     new_ag.add_public_goal(g)
+            new_p.add_agent(new_ag)
         new_p._user_types = self._user_types[:]
         new_p._user_types_hierarchy = self._user_types_hierarchy.copy()
         new_p._objects = self._objects[:]
         new_p._initial_value = self._initial_value.copy()
         new_p._goals = self._goals[:]
         new_p._initial_defaults = self._initial_defaults.copy()
         new_p._waitfor = self.waitfor.clone()
```

### Comparing `up_social_laws-0.0.6/up_social_laws/robustness_checker.py` & `up_social_laws-0.1.0/up_social_laws/robustness_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     def satisfies(optimality_guarantee: OptimalityGuarantee) -> bool:
         if optimality_guarantee == OptimalityGuarantee.SATISFICING:
             return True
         return False
 
     @staticmethod
     def supported_kind() -> "ProblemKind":
-        supported_kind = unified_planning.model.problem_kind.multi_agent_kind.union(unified_planning.model.problem_kind.actions_cost_kind).union(unified_planning.model.problem_kind.temporal_kind)        
+        supported_kind = unified_planning.model.problem_kind.multi_agent_kind.union(unified_planning.model.problem_kind.actions_cost_kind).union(unified_planning.model.problem_kind.temporal_kind)
         final_supported_kind = supported_kind.intersection(SingleAgentProjection.supported_kind())
         
         return final_supported_kind
 
     @staticmethod
     def supports(problem_kind):
         return problem_kind <= SocialLawRobustnessChecker.supported_kind()
```

### Comparing `up_social_laws-0.0.6/up_social_laws/robustness_verification.py` & `up_social_laws-0.1.0/up_social_laws/robustness_verification.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,18 @@
 
     def get_agent_goal(self, problem : MultiAgentProblem, agent : Agent):
         """ Returns the individual goal of the given agent"""        
         l = []
         for goal in problem.goals:
             if goal.is_dot() and goal.agent() == agent.name:
                 l.append(goal)
+        for goal in agent.private_goals:
+            l.append(goal)
+        for goal in agent.public_goals:
+            l.append(goal)
         return l
 
     def get_action_preconditions(self, problem : MultiAgentProblemWithWaitfor, agent : Agent, action : Action, fail : bool, wait: bool) -> List[FNode]:
         """ Get the preconditions for the given action of the given agent. fail/wait specify which preconditions we want (True to return, False to omit) """
         assert fail or wait
         if wait and not fail:
             return problem.waitfor.get_preconditions_wait(agent.name, action.name)
```

### Comparing `up_social_laws-0.0.6/up_social_laws/sa_to_ma_converter.py` & `up_social_laws-0.1.0/up_social_laws/sa_to_ma_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,18 +131,16 @@
     def assign_goal_to_agent(self, goal):        
         agent = None
         for arg in goal.args:
             if arg.object() in self.agent_map:
                 agent = self.agent_map[arg.object()]
                 break
         if agent is None:
-            agent = random.choice(list(self.agent_map.values()))
-        #TODO: add back
-        # Commented out because this function is not available
-        #agent.add_goal(goal)
+            agent = random.choice(list(self.agent_map.values()))        
+        agent.add_public_goal(goal)
         
 
     def _compile(self, problem: "up.model.AbstractProblem", compilation_kind: "up.engines.CompilationKind") -> CompilerResult:
         '''Creates a problem that is a multi-agent version of the original problem'''
         assert isinstance(problem, Problem)
 
         #Represents the map from the new action to the old action
```

### Comparing `up_social_laws-0.0.6/up_social_laws/single_agent_projection.py` & `up_social_laws-0.1.0/up_social_laws/single_agent_projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,20 @@
         for goal in problem.goals:            
             if goal.is_dot():
                 if goal.agent() == self.agent.name:  # Compare agent names to handle social laws which change agents
                     new_problem.add_goal(goal.args[0])            
             else:
                 new_problem.add_goal(goal)            
 
+        for goal in self.agent.public_goals:
+            new_problem.add_goal(goal)
+        for goal in self.agent.private_goals:
+            new_problem.add_goal(goal)
+
+
         return CompilerResult(
             new_problem, partial(replace_action, map=new_to_old), self.name
         )
 
     # def get_original_action(self, action: Action) -> Action:
     #     '''After the method get_rewritten_problem is called, this function maps
     #     the actions of the transformed problem into the actions of the original problem.'''
```

### Comparing `up_social_laws-0.0.6/up_social_laws/social_law.py` & `up_social_laws-0.1.0/up_social_laws/social_law.py`

 * *Files 11% similar despite different names*

```diff
@@ -115,39 +115,15 @@
 
     @property
     def name(self):
         return "sl"
 
     @staticmethod
     def supported_kind() -> ProblemKind:
-        supported_kind = ProblemKind()
-        supported_kind.set_problem_class("ACTION_BASED_MULTI_AGENT")
-        supported_kind.set_typing("FLAT_TYPING")
-        supported_kind.set_typing("HIERARCHICAL_TYPING")
-        supported_kind.set_numbers("CONTINUOUS_NUMBERS")
-        supported_kind.set_numbers("DISCRETE_NUMBERS")
-        supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
-        supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
-        supported_kind.set_fluents_type("NUMERIC_FLUENTS")
-        supported_kind.set_fluents_type("OBJECT_FLUENTS")
-        supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITIES")
-        supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
-        supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
-        supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
-        supported_kind.set_effects_kind("INCREASE_EFFECTS")
-        supported_kind.set_effects_kind("DECREASE_EFFECTS")
-        supported_kind.set_time("CONTINUOUS_TIME")
-        supported_kind.set_time("DISCRETE_TIME")
-        supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
-        supported_kind.set_time("TIMED_EFFECTS")
-        supported_kind.set_time("TIMED_GOALS")
-        supported_kind.set_time("DURATION_INEQUALITIES")
-        supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
+        supported_kind = unified_planning.model.problem_kind.multi_agent_kind.union(unified_planning.model.problem_kind.actions_cost_kind).union(unified_planning.model.problem_kind.temporal_kind)
         return supported_kind
 
     @staticmethod
     def supports(problem_kind):
         return problem_kind <= SocialLaw.supported_kind()
 
     @staticmethod
@@ -174,22 +150,27 @@
         new_problem = MultiAgentProblemWithWaitfor()
         new_problem.name = f'{self.name}_{problem.name}'
 
         for f in problem.ma_environment.fluents:
             default_val = problem.ma_environment.fluents_defaults[f]
             new_problem.ma_environment.add_fluent(f, default_initial_value=default_val)
         for ag in problem.agents:
-            new_ag = up.model.multi_agent.Agent(ag.name, new_problem)
-            for f in ag.fluents:
-                default_val = ag.fluents_defaults[f]
-                new_ag.add_fluent(f, default_initial_value=default_val)
-            for a in ag.actions:
-                new_action = a.clone()                
-                new_ag.add_action(new_action)
-                new_to_old[new_action] = (ag, a)
+            new_ag = ag.clone(new_problem)            
+            # up.model.multi_agent.Agent(ag.name, new_problem)
+            # for f in ag.fluents:
+            #     default_val = ag.fluents_defaults[f]
+            #     new_ag.add_fluent(f, default_initial_value=default_val)
+            # for a in ag.actions:
+            #     new_action = a.clone()                
+            #     new_ag.add_action(new_action)
+            #     new_to_old[new_action] = (ag, a)
+            # for g in ag.private_goals:
+            #     new_ag.add_private_goal(g)
+            # for g in ag.public_goals:
+            #     new_ag.add_public_goal(g)                
             new_problem.add_agent(new_ag)
         new_problem._user_types = problem._user_types[:]
         new_problem._user_types_hierarchy = problem._user_types_hierarchy.copy()
         new_problem._objects = problem._objects[:]
         new_problem._initial_value = problem._initial_value.copy()
         new_problem._goals = problem._goals[:]
         new_problem._initial_defaults = problem._initial_defaults.copy()
```

### Comparing `up_social_laws-0.0.6/up_social_laws/synthesis.py` & `up_social_laws-0.1.0/up_social_laws/synthesis.py`

 * *Files identical despite different names*

### Comparing `up_social_laws-0.0.6/up_social_laws/waitfor_specification.py` & `up_social_laws-0.1.0/up_social_laws/waitfor_specification.py`

 * *Files identical despite different names*

### Comparing `up_social_laws-0.0.6/up_social_laws.egg-info/PKG-INFO` & `up_social_laws-0.1.0/up_social_laws.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up-social-laws
-Version: 0.0.6
+Version: 0.1.0
 Summary: Unified Planning Integration of Social Laws
 Home-page: https://github.com/aiplan4eu/up-social-laws
 Author: Technion Cognitive Robotics Lab
 Author-email: karpase@technion.ac.il
 License: APACHE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `up_social_laws-0.0.6/up_social_laws.egg-info/SOURCES.txt` & `up_social_laws-0.1.0/up_social_laws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

