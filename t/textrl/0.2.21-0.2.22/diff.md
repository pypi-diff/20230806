# Comparing `tmp/textrl-0.2.21.tar.gz` & `tmp/textrl-0.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textrl-0.2.21.tar", last modified: Thu Aug  3 22:40:59 2023, max compression
+gzip compressed data, was "textrl-0.2.22.tar", last modified: Sun Aug  6 04:38:05 2023, max compression
```

## Comparing `textrl-0.2.21.tar` & `textrl-0.2.22.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-03 22:40:59.962817 textrl-0.2.21/
--rw-r--r--   0 voidful    (501) staff       (20)     4206 2022-12-05 09:09:02.000000 textrl-0.2.21/.gitignore
--rw-r--r--   0 voidful    (501) staff       (20)     1064 2023-02-09 14:54:56.000000 textrl-0.2.21/LICENSE
--rw-r--r--   0 voidful    (501) staff       (20)    18232 2023-08-03 22:40:59.958844 textrl-0.2.21/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)    17515 2023-04-25 10:23:10.000000 textrl-0.2.21/README.md
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-03 22:40:59.921512 textrl-0.2.21/example/
--rw-r--r--   0 voidful    (501) staff       (20)     7679 2023-03-27 13:57:09.000000 textrl-0.2.21/example/2022-12-10-textrl-elon-musk.ipynb
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-03 22:40:59.923474 textrl-0.2.21/img/
--rw-r--r--   0 voidful    (501) staff       (20)   373908 2023-04-17 05:47:18.000000 textrl-0.2.21/img/Designer.png
--rw-r--r--   0 voidful    (501) staff       (20)       61 2022-12-05 09:17:42.000000 textrl-0.2.21/requirement.txt
--rw-r--r--   0 voidful    (501) staff       (20)       38 2023-08-03 22:40:59.962917 textrl-0.2.21/setup.cfg
--rw-r--r--   0 voidful    (501) staff       (20)     1095 2023-08-03 22:39:44.000000 textrl-0.2.21/setup.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-03 22:40:59.942741 textrl-0.2.21/textrl/
--rw-r--r--   0 voidful    (501) staff       (20)      184 2023-02-13 19:45:54.000000 textrl-0.2.21/textrl/__init__.py
--rw-r--r--   0 voidful    (501) staff       (20)    13501 2023-08-03 22:39:00.000000 textrl-0.2.21/textrl/actor.py
--rw-r--r--   0 voidful    (501) staff       (20)     1150 2023-06-20 16:43:55.000000 textrl-0.2.21/textrl/dump.py
--rw-r--r--   0 voidful    (501) staff       (20)     7405 2023-07-25 02:42:31.000000 textrl-0.2.21/textrl/environment.py
--rw-r--r--   0 voidful    (501) staff       (20)    23448 2023-02-13 19:43:59.000000 textrl-0.2.21/textrl/evaluator.py
--rw-r--r--   0 voidful    (501) staff       (20)     7511 2023-02-13 19:43:59.000000 textrl-0.2.21/textrl/trainer.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-03 22:40:59.958170 textrl-0.2.21/textrl.egg-info/
--rw-r--r--   0 voidful    (501) staff       (20)    18232 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)      433 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/SOURCES.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/dependency_links.txt
--rw-r--r--   0 voidful    (501) staff       (20)       50 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/entry_points.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2022-12-05 09:10:02.000000 textrl-0.2.21/textrl.egg-info/not-zip-safe
--rw-r--r--   0 voidful    (501) staff       (20)       17 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/requires.txt
--rw-r--r--   0 voidful    (501) staff       (20)        7 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/top_level.txt
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-06 04:38:05.720419 textrl-0.2.22/
+-rw-r--r--   0 voidful    (501) staff       (20)     4206 2022-12-05 09:09:02.000000 textrl-0.2.22/.gitignore
+-rw-r--r--   0 voidful    (501) staff       (20)     1064 2023-02-09 14:54:56.000000 textrl-0.2.22/LICENSE
+-rw-r--r--   0 voidful    (501) staff       (20)    18027 2023-08-06 04:38:05.719232 textrl-0.2.22/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)    17310 2023-08-06 04:37:11.000000 textrl-0.2.22/README.md
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-06 04:38:05.076302 textrl-0.2.22/example/
+-rw-r--r--   0 voidful    (501) staff       (20)     7679 2023-03-27 13:57:09.000000 textrl-0.2.22/example/2022-12-10-textrl-elon-musk.ipynb
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-06 04:38:05.078800 textrl-0.2.22/img/
+-rw-r--r--   0 voidful    (501) staff       (20)   373908 2023-04-17 05:47:18.000000 textrl-0.2.22/img/Designer.png
+-rw-r--r--   0 voidful    (501) staff       (20)       61 2022-12-05 09:17:42.000000 textrl-0.2.22/requirement.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       38 2023-08-06 04:38:05.720677 textrl-0.2.22/setup.cfg
+-rw-r--r--   0 voidful    (501) staff       (20)     1095 2023-08-06 04:37:11.000000 textrl-0.2.22/setup.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-06 04:38:05.401658 textrl-0.2.22/textrl/
+-rw-r--r--   0 voidful    (501) staff       (20)      184 2023-02-13 19:45:54.000000 textrl-0.2.22/textrl/__init__.py
+-rw-r--r--   0 voidful    (501) staff       (20)    12359 2023-08-06 04:37:11.000000 textrl-0.2.22/textrl/actor.py
+-rw-r--r--   0 voidful    (501) staff       (20)     1150 2023-06-20 16:43:55.000000 textrl-0.2.22/textrl/dump.py
+-rw-r--r--   0 voidful    (501) staff       (20)     7405 2023-07-25 02:42:31.000000 textrl-0.2.22/textrl/environment.py
+-rw-r--r--   0 voidful    (501) staff       (20)    23448 2023-02-13 19:43:59.000000 textrl-0.2.22/textrl/evaluator.py
+-rw-r--r--   0 voidful    (501) staff       (20)     7511 2023-02-13 19:43:59.000000 textrl-0.2.22/textrl/trainer.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-06 04:38:05.717897 textrl-0.2.22/textrl.egg-info/
+-rw-r--r--   0 voidful    (501) staff       (20)    18027 2023-08-06 04:38:04.000000 textrl-0.2.22/textrl.egg-info/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)      433 2023-08-06 04:38:04.000000 textrl-0.2.22/textrl.egg-info/SOURCES.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2023-08-06 04:38:04.000000 textrl-0.2.22/textrl.egg-info/dependency_links.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       50 2023-08-06 04:38:04.000000 textrl-0.2.22/textrl.egg-info/entry_points.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2022-12-05 09:10:02.000000 textrl-0.2.22/textrl.egg-info/not-zip-safe
+-rw-r--r--   0 voidful    (501) staff       (20)       17 2023-08-06 04:38:04.000000 textrl-0.2.22/textrl.egg-info/requires.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        7 2023-08-06 04:38:04.000000 textrl-0.2.22/textrl.egg-info/top_level.txt
```

### Comparing `textrl-0.2.21/.gitignore` & `textrl-0.2.22/.gitignore`

 * *Files identical despite different names*

### Comparing `textrl-0.2.21/LICENSE` & `textrl-0.2.22/LICENSE`

 * *Files identical despite different names*

### Comparing `textrl-0.2.21/PKG-INFO` & `textrl-0.2.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textrl
-Version: 0.2.21
+Version: 0.2.22
 Summary: TextRL - use reinforcement learning to adjust text generation results.
 Home-page: https://github.com/voidful/TextRL
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: transformer huggingface nlp generation reinforcement learning deep learning
 Platform: UNKNOWN
@@ -228,16 +228,15 @@
 
 observaton_list = [{"input":"explain how attention work in seq2seq model"}]
 env = TextRLEnv(model, tokenizer, observation_input=observaton_list, max_length=20, compare_sample=2)
 actor = TextRLActor(env, model, tokenizer,
                     act_deterministically=False,
                     temperature=1.0,
                     top_k=0,
-                    top_p=1.0,
-                    repetition_penalty=2)
+                    top_p=1.0)
 agent = actor.agent_ppo(update_interval=2, minibatch_size=2, epochs=10)
 print(actor.predict(observaton_list[0]))
 
 train_agent_with_evaluation(
     agent,
     env,
     steps=100,
@@ -293,16 +292,15 @@
 
 observaton_list = [{"input":"explain how attention work in seq2seq model"}]
 env = TextRLEnv(model, tokenizer, observation_input=observaton_list, max_length=20, compare_sample=2)
 actor = TextRLActor(env, model, tokenizer,
                     act_deterministically=False,
                     temperature=1.0,
                     top_k=0,
-                    top_p=1.0,
-                    repetition_penalty=2)
+                    top_p=1.0)
 agent = actor.agent_ppo(update_interval=2, minibatch_size=2, epochs=10)
 
 print(actor.predict(observaton_list[0]))
 
 train_agent_with_evaluation(
     agent,
     env,
@@ -485,16 +483,15 @@
 
 ```python
 actor = TextRLActor(env, model, tokenizer,
                     act_deterministically=False,  # select the max probability token for each step or not
                     temperature=1,                # temperature for sampling
                     compare_sample=2,             # num of sample to rank
                     top_k=0,                      # top k sampling
-                    top_p=1.0,                    # top p sampling
-                    repetition_penalty=2)         # repetition penalty from CTRL paper (https://arxiv.org/abs/1909.05858)
+                    top_p=1.0,)                    # top p sampling
 ```
 
 When training a reinforcement learning (RL) model, several key parameters need to be tuned to ensure optimal performance. Here is a list of important parameters and their descriptions:
 
 1. **Update Interval**: This determines how often the RL agent updates its policy based on collected experiences. A smaller update interval means the agent learns more frequently from recent experiences, while a larger interval allows more experiences to accumulate before learning. In the example above, the update interval is set to 10.
 
 ```python
```

### Comparing `textrl-0.2.21/README.md` & `textrl-0.2.22/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -209,16 +209,15 @@
 
 observaton_list = [{"input":"explain how attention work in seq2seq model"}]
 env = TextRLEnv(model, tokenizer, observation_input=observaton_list, max_length=20, compare_sample=2)
 actor = TextRLActor(env, model, tokenizer,
                     act_deterministically=False,
                     temperature=1.0,
                     top_k=0,
-                    top_p=1.0,
-                    repetition_penalty=2)
+                    top_p=1.0)
 agent = actor.agent_ppo(update_interval=2, minibatch_size=2, epochs=10)
 print(actor.predict(observaton_list[0]))
 
 train_agent_with_evaluation(
     agent,
     env,
     steps=100,
@@ -274,16 +273,15 @@
 
 observaton_list = [{"input":"explain how attention work in seq2seq model"}]
 env = TextRLEnv(model, tokenizer, observation_input=observaton_list, max_length=20, compare_sample=2)
 actor = TextRLActor(env, model, tokenizer,
                     act_deterministically=False,
                     temperature=1.0,
                     top_k=0,
-                    top_p=1.0,
-                    repetition_penalty=2)
+                    top_p=1.0)
 agent = actor.agent_ppo(update_interval=2, minibatch_size=2, epochs=10)
 
 print(actor.predict(observaton_list[0]))
 
 train_agent_with_evaluation(
     agent,
     env,
@@ -466,16 +464,15 @@
 
 ```python
 actor = TextRLActor(env, model, tokenizer,
                     act_deterministically=False,  # select the max probability token for each step or not
                     temperature=1,                # temperature for sampling
                     compare_sample=2,             # num of sample to rank
                     top_k=0,                      # top k sampling
-                    top_p=1.0,                    # top p sampling
-                    repetition_penalty=2)         # repetition penalty from CTRL paper (https://arxiv.org/abs/1909.05858)
+                    top_p=1.0,)                    # top p sampling
 ```
 
 When training a reinforcement learning (RL) model, several key parameters need to be tuned to ensure optimal performance. Here is a list of important parameters and their descriptions:
 
 1. **Update Interval**: This determines how often the RL agent updates its policy based on collected experiences. A smaller update interval means the agent learns more frequently from recent experiences, while a larger interval allows more experiences to accumulate before learning. In the example above, the update interval is set to 10.
 
 ```python
```

### Comparing `textrl-0.2.21/example/2022-12-10-textrl-elon-musk.ipynb` & `textrl-0.2.22/example/2022-12-10-textrl-elon-musk.ipynb`

 * *Files identical despite different names*

### Comparing `textrl-0.2.21/img/Designer.png` & `textrl-0.2.22/img/Designer.png`

 * *Files identical despite different names*

### Comparing `textrl-0.2.21/setup.py` & `textrl-0.2.22/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='textrl',
-    version='0.2.21',
+    version='0.2.22',
     description='TextRL - use reinforcement learning to adjust text generation results.',
     url='https://github.com/voidful/TextRL',
     author='Voidful',
     author_email='voidful.stack@gmail.com',
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     setup_requires=['setuptools-git'],
```

### Comparing `textrl-0.2.21/textrl/actor.py` & `textrl-0.2.22/textrl/actor.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 
 class TextRLActor:
     def __init__(self, env, model, tokenizer, optimizer='sgd', gpu_id=0,
                  unfreeze_layer_from_past=0,
                  act_deterministically=True,
                  temperature=1.0,
                  top_k=0,
-                 top_p=1.0,
-                 repetition_penalty=1.0):
+                 top_p=1.0):
         self.agent = None
         self.n_actions = max(model.config.vocab_size, tokenizer.vocab_size)
         self.env = env
         self.gpu_id = gpu_id
         self.device = torch.device("cuda:{}".format(gpu_id))
         self.model = model
         if hasattr(model.config, 'word_embed_proj_dim'):
@@ -48,15 +47,14 @@
             self.obs_size = model.config.hidden_size
         self.converter = self.model.lm_head
         self.act_deterministically = act_deterministically
         self.temperature = temperature
         self.top_k = top_k
         self.top_p = top_p
         self.optimizer = optimizer
-        self.repetition_penalty = repetition_penalty
         self.unfreeze_layer_from_past = unfreeze_layer_from_past
 
         parents = [parent[0] for parent in model.named_children()]
         if 'transformer' in parents:  # gpt2/bloom:
             transformers_model = model.transformer
         elif 'model' in parents:  # bart
             transformers_model = model.model
@@ -79,16 +77,15 @@
         policy = torch.nn.Sequential(
             self.middle_model,
             self.remaining_model,
             self.converter,
             SoftmaxCategoricalHead(self.env,
                                    temperature=self.temperature,
                                    top_k=self.top_k,
-                                   top_p=self.top_p,
-                                   repetition_penalty=self.repetition_penalty)
+                                   top_p=self.top_p)
         )
         vf = torch.nn.Sequential(
             torch.nn.Linear(self.obs_size, self.obs_size // 2),
             torch.nn.Linear(self.obs_size // 2, self.obs_size // 4),
             torch.nn.Linear(self.obs_size // 4, 1)
         )
         model = pfrl.nn.Branched(policy, vf)
@@ -179,35 +176,23 @@
         indices_to_remove = sorted_indices_to_remove.scatter(2, sorted_indices, sorted_indices_to_remove)
         logits = logits.masked_fill(indices_to_remove, filter_value)
 
     return logits
 
 
 class SoftmaxCategoricalHead(torch.nn.Module):
-    def __init__(self, env, temperature=1.0, top_k=0, top_p=1.0, repetition_penalty=1.0):
+    def __init__(self, env, temperature=1.0, top_k=0, top_p=1.0):
         super().__init__()
         self.env = env
         self.softmax = torch.nn.Softmax(dim=-1)
         self.temperature = temperature
         self.top_k = top_k
         self.top_p = top_p
-        self.repetition_penalty = repetition_penalty
 
     def forward(self, logits):
-        # repetition penalty from CTRL paper (https://arxiv.org/abs/1909.05858)
-        # repetition penalty from https://github.com/huggingface/transformers/pull/2303/files#diff-6b72b98c4c2dcfc6cc606843917733f5d858374fbc22a735ff483bbc0c1e63ea
-        if self.repetition_penalty != 1.0:
-            for seq_num, predicted in enumerate(self.env.predicted):
-                for previous_tokens in set(predicted):
-                    prev_token_id = self.env.tokenizer.convert_tokens_to_ids(previous_tokens)
-                    # if score < 0 then repetition penalty has to multiplied to reduce the previous token probability
-                    if torch.all(logits[:, seq_num, prev_token_id] < 0):
-                        logits[:, seq_num, prev_token_id] *= self.repetition_penalty
-                    else:
-                        logits[:, seq_num, prev_token_id] /= self.repetition_penalty
         logits = logits / self.temperature
         logits = top_k_top_p_filtering(logits, top_k=self.top_k, top_p=self.top_p)
         return torch.distributions.Categorical(logits=logits)
 
 
 class TextPPO(pfrl.agents.PPO):
     def _update_if_dataset_is_ready(self):
```

### Comparing `textrl-0.2.21/textrl/dump.py` & `textrl-0.2.22/textrl/dump.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.21/textrl/environment.py` & `textrl-0.2.22/textrl/environment.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.21/textrl/evaluator.py` & `textrl-0.2.22/textrl/evaluator.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.21/textrl/trainer.py` & `textrl-0.2.22/textrl/trainer.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.21/textrl.egg-info/PKG-INFO` & `textrl-0.2.22/textrl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textrl
-Version: 0.2.21
+Version: 0.2.22
 Summary: TextRL - use reinforcement learning to adjust text generation results.
 Home-page: https://github.com/voidful/TextRL
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: transformer huggingface nlp generation reinforcement learning deep learning
 Platform: UNKNOWN
@@ -228,16 +228,15 @@
 
 observaton_list = [{"input":"explain how attention work in seq2seq model"}]
 env = TextRLEnv(model, tokenizer, observation_input=observaton_list, max_length=20, compare_sample=2)
 actor = TextRLActor(env, model, tokenizer,
                     act_deterministically=False,
                     temperature=1.0,
                     top_k=0,
-                    top_p=1.0,
-                    repetition_penalty=2)
+                    top_p=1.0)
 agent = actor.agent_ppo(update_interval=2, minibatch_size=2, epochs=10)
 print(actor.predict(observaton_list[0]))
 
 train_agent_with_evaluation(
     agent,
     env,
     steps=100,
@@ -293,16 +292,15 @@
 
 observaton_list = [{"input":"explain how attention work in seq2seq model"}]
 env = TextRLEnv(model, tokenizer, observation_input=observaton_list, max_length=20, compare_sample=2)
 actor = TextRLActor(env, model, tokenizer,
                     act_deterministically=False,
                     temperature=1.0,
                     top_k=0,
-                    top_p=1.0,
-                    repetition_penalty=2)
+                    top_p=1.0)
 agent = actor.agent_ppo(update_interval=2, minibatch_size=2, epochs=10)
 
 print(actor.predict(observaton_list[0]))
 
 train_agent_with_evaluation(
     agent,
     env,
@@ -485,16 +483,15 @@
 
 ```python
 actor = TextRLActor(env, model, tokenizer,
                     act_deterministically=False,  # select the max probability token for each step or not
                     temperature=1,                # temperature for sampling
                     compare_sample=2,             # num of sample to rank
                     top_k=0,                      # top k sampling
-                    top_p=1.0,                    # top p sampling
-                    repetition_penalty=2)         # repetition penalty from CTRL paper (https://arxiv.org/abs/1909.05858)
+                    top_p=1.0,)                    # top p sampling
 ```
 
 When training a reinforcement learning (RL) model, several key parameters need to be tuned to ensure optimal performance. Here is a list of important parameters and their descriptions:
 
 1. **Update Interval**: This determines how often the RL agent updates its policy based on collected experiences. A smaller update interval means the agent learns more frequently from recent experiences, while a larger interval allows more experiences to accumulate before learning. In the example above, the update interval is set to 10.
 
 ```python
```

