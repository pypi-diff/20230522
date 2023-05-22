# Comparing `tmp/mathactive-0.0.6.tar.gz` & `tmp/mathactive-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathactive-0.0.6.tar", max compression
+gzip compressed data, was "mathactive-0.0.7.tar", max compression
```

## Comparing `mathactive-0.0.6.tar` & `mathactive-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    34336 2023-03-24 02:28:44.521708 mathactive-0.0.6/LICENSE.md
--rw-r--r--   0        0        0     2836 2023-05-17 03:54:46.693671 mathactive-0.0.6/README.md
--rw-r--r--   0        0        0      528 2023-05-17 04:08:11.946166 mathactive-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-07 16:23:10.191094 mathactive-0.0.6/src/mathactive/__init__.py
--rw-r--r--   0        0        0      820 2023-03-24 02:28:44.525707 mathactive-0.0.6/src/mathactive/data/difficulty_start_stop_step.csv
--rw-r--r--   0        0        0     1066 2023-03-24 02:28:44.525707 mathactive-0.0.6/src/mathactive/generators.py
--rw-r--r--   0        0        0      427 2023-03-24 02:28:44.525707 mathactive-0.0.6/src/mathactive/hints.py
--rw-r--r--   0        0        0     3470 2023-03-03 18:38:05.790120 mathactive-0.0.6/src/mathactive/machine.py
--rwxr-xr-x   0        0        0      663 2023-03-24 02:28:44.525707 mathactive-0.0.6/src/mathactive/manage.py
--rw-r--r--   0        0        0     2575 2023-03-24 02:28:44.525707 mathactive-0.0.6/src/mathactive/microlessons/num_one.py
--rw-r--r--   0        0        0      822 2023-03-24 02:28:44.525707 mathactive-0.0.6/src/mathactive/microlessons/utils.py
--rw-r--r--   0        0        0     2732 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/personalize.py
--rw-r--r--   0        0        0     1813 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/python_quiz.py
--rw-r--r--   0        0        0     1191 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/questions.py
--rw-r--r--   0        0        0     2594 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/utils.py
--rw-r--r--   0        0        0        0 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/webapp/__init__.py
--rw-r--r--   0        0        0       63 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/webapp/admin.py
--rw-r--r--   0        0        0      144 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/webapp/apps.py
--rw-r--r--   0        0        0        0 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/webapp/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/webapp/models.py
--rw-r--r--   0        0        0       60 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/webapp/tests.py
--rw-r--r--   0        0        0       63 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/webapp/views.py
--rw-r--r--   0        0        0        0 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/website/__init__.py
--rw-r--r--   0        0        0      402 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/website/asgi.py
--rw-r--r--   0        0        0     3224 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/website/settings.py
--rw-r--r--   0        0        0      749 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/website/urls.py
--rw-r--r--   0        0        0      391 2023-03-24 02:28:44.529707 mathactive-0.0.6/src/mathactive/website/wsgi.py
--rw-r--r--   0        0        0     3739 1970-01-01 00:00:00.000000 mathactive-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    34336 2023-03-20 03:29:53.959200 mathactive-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0      552 2023-05-22 01:44:00.793283 mathactive-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2924 2023-05-22 01:41:27.905365 mathactive-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-03-20 03:26:47.967820 mathactive-0.0.7/src/mathactive/__init__.py
+-rw-r--r--   0        0        0      875 2023-03-21 02:35:59.836638 mathactive-0.0.7/src/mathactive/data/difficulty_start_stop_step.csv
+-rw-r--r--   0        0        0     1099 2023-03-21 02:35:59.837638 mathactive-0.0.7/src/mathactive/generators.py
+-rw-r--r--   0        0        0      443 2023-03-21 02:35:59.838638 mathactive-0.0.7/src/mathactive/hints.py
+-rw-r--r--   0        0        0     3607 2023-03-20 03:26:47.971821 mathactive-0.0.7/src/mathactive/machine.py
+-rw-r--r--   0        0        0      685 2023-03-21 02:35:59.839639 mathactive-0.0.7/src/mathactive/manage.py
+-rw-r--r--   0        0        0     2646 2023-03-21 02:35:59.840638 mathactive-0.0.7/src/mathactive/microlessons/num_one.py
+-rw-r--r--   0        0        0      857 2023-03-22 06:13:54.278274 mathactive-0.0.7/src/mathactive/microlessons/utils.py
+-rw-r--r--   0        0        0     2806 2023-03-21 02:35:59.841638 mathactive-0.0.7/src/mathactive/personalize.py
+-rw-r--r--   0        0        0     1852 2023-03-21 02:35:59.842638 mathactive-0.0.7/src/mathactive/python_quiz.py
+-rw-r--r--   0        0        0     1223 2023-03-21 02:35:59.843639 mathactive-0.0.7/src/mathactive/questions.py
+-rw-r--r--   0        0        0     2667 2023-03-21 02:35:59.844639 mathactive-0.0.7/src/mathactive/utils.py
+-rw-r--r--   0        0        0        0 2023-03-21 02:35:59.844639 mathactive-0.0.7/src/mathactive/webapp/__init__.py
+-rw-r--r--   0        0        0       66 2023-03-21 02:35:59.845640 mathactive-0.0.7/src/mathactive/webapp/admin.py
+-rw-r--r--   0        0        0      150 2023-03-21 02:35:59.846639 mathactive-0.0.7/src/mathactive/webapp/apps.py
+-rw-r--r--   0        0        0        0 2023-03-21 02:35:59.847640 mathactive-0.0.7/src/mathactive/webapp/migrations/__init__.py
+-rw-r--r--   0        0        0       60 2023-03-21 02:35:59.847640 mathactive-0.0.7/src/mathactive/webapp/models.py
+-rw-r--r--   0        0        0       63 2023-03-21 02:35:59.848640 mathactive-0.0.7/src/mathactive/webapp/tests.py
+-rw-r--r--   0        0        0       66 2023-03-21 02:35:59.849640 mathactive-0.0.7/src/mathactive/webapp/views.py
+-rw-r--r--   0        0        0        0 2023-03-21 02:35:59.850640 mathactive-0.0.7/src/mathactive/website/__init__.py
+-rw-r--r--   0        0        0      418 2023-03-21 02:35:59.850640 mathactive-0.0.7/src/mathactive/website/asgi.py
+-rw-r--r--   0        0        0     3347 2023-03-21 02:35:59.851642 mathactive-0.0.7/src/mathactive/website/settings.py
+-rw-r--r--   0        0        0      770 2023-03-21 02:35:59.852641 mathactive-0.0.7/src/mathactive/website/urls.py
+-rw-r--r--   0        0        0      407 2023-03-21 02:35:59.852641 mathactive-0.0.7/src/mathactive/website/wsgi.py
+-rw-r--r--   0        0        0     3739 1970-01-01 00:00:00.000000 mathactive-0.0.7/PKG-INFO
```

### Comparing `mathactive-0.0.6/LICENSE.md` & `mathactive-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.6/README.md` & `mathactive-0.0.7/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-# "mathactive"
-
-<!--
-[![PyPI version](https://img.shields.io/pypi/pyversions/mathactive.svg)](https://pypi.or
-g/project/mathactive/)
-[![License](https://img.shields.io/pypi/l/mathactive.svg)](https://pypi.python.org/pypi/
-mathactive/)
-[![codecov](https://codecov.io/gl/tangibleai/mathactive/branch/master/graph/badge.svg)](
-https://codecov.io/gl/tangibleai/mathactive)
-[![Buy Us Tea](https://github.com/nlpia/nlpia-bot/raw/develop/docs/media/small-lea
-f-and-name-screenshot-31x80.png)](https://buymeacoffee.com/hobs)
-[![DigitalOcean Referral Badge](https://web-platforms.sfo2.digitaloceanspaces.com/
-WWW/Badge%202.svg)](https://www.digitalocean.com/?refcode=5bc34fba1bee&utm_campaig
-n=Referral_Invite&utm_medium=Referral_Program&utm_source=badge)
- -->
-Conversational math active learning.
-
-K-12 student can learn math from a chatbot that helps them actively solve math problems suitable to their skill level.
-
-## Quickstart
-
-If you have install python packages from source before, you will probably be able to follow these steps to get going quickly:
-
-```bash
-pip install --upgrade pip virtualenv poetry
-git clone git@gitlab.com:tangbileai/community/mathactive
-cd mathactive
-python -m virtualenv .venv
-source .venv/bin/activate || source .venv/Scripts/activate
-pip install --editable .
-```
-
-## Utilities
-
-```python
-def get_countq_start_step(difficulty=0.01):
-    """ Predict the parameters of a quiz question generator based on the desired difficulty
-    >>> get_start_step(difficulty=.02)
-    {'start': 0, 'step': 1}
-    >>> get_start_step(difficulty=.03)
-    {'start': 0, 'step': 1}
-    >>> get_start_step(difficulty=.04)
-    {'start': 10, 'step': 1}
-    """
-```
-
-## Directory structure
-
-```text
-├── docs
-│   ├── AIMA approaches to creating a chatbot.md
-│   ├── ...
-├── pyproject.toml
-├── README.md
-├── scripts
-│   ├── bump_version.py
-│   ├── release.sh
-│   └── requirements.txt
-└── src
-    └── mathactive
-        ├── data
-        │   └── difficulty_start_stop_step.csv
-        ├── data.csv
-        ├── db.sqlite3
-        ├── generators.py
-        ├── hints.py
-        ├── machine.py
-        ├── manage.py
-        ├── microlessons
-        │   ├── num_one.py
-        │   └── utils.py
-        ├── personalize.py
-        ├── python_quiz.py
-        ├── questions.py
-        ├── utils.py
-        ├── webapp
-        │   ├── admin.py
-        │   ├── apps.py
-        │   ├── migrations
-        │   ├── models.py
-        │   ├── tests.py
-        │   └── views.py
-        └── website
-            ├── asgi.py
-            ├── settings.py
-            ├── urls.py
-            └── wsgi.py
-```
+# "mathactive"
+
+<!--
+[![PyPI version](https://img.shields.io/pypi/pyversions/mathactive.svg)](https://pypi.or
+g/project/mathactive/)
+[![License](https://img.shields.io/pypi/l/mathactive.svg)](https://pypi.python.org/pypi/
+mathactive/)
+[![codecov](https://codecov.io/gl/tangibleai/mathactive/branch/master/graph/badge.svg)](
+https://codecov.io/gl/tangibleai/mathactive)
+[![Buy Us Tea](https://github.com/nlpia/nlpia-bot/raw/develop/docs/media/small-lea
+f-and-name-screenshot-31x80.png)](https://buymeacoffee.com/hobs)
+[![DigitalOcean Referral Badge](https://web-platforms.sfo2.digitaloceanspaces.com/
+WWW/Badge%202.svg)](https://www.digitalocean.com/?refcode=5bc34fba1bee&utm_campaig
+n=Referral_Invite&utm_medium=Referral_Program&utm_source=badge)
+ -->
+Conversational math active learning.
+
+K-12 student can learn math from a chatbot that helps them actively solve math problems suitable to their skill level.
+
+## Quickstart
+
+If you have install python packages from source before, you will probably be able to follow these steps to get going quickly:
+
+```bash
+pip install --upgrade pip virtualenv poetry
+git clone git@gitlab.com:tangbileai/community/mathactive
+cd mathactive
+python -m virtualenv .venv
+source .venv/bin/activate || source .venv/Scripts/activate
+pip install --editable .
+```
+
+## Utilities
+
+```python
+def get_countq_start_step(difficulty=0.01):
+    """ Predict the parameters of a quiz question generator based on the desired difficulty
+    >>> get_start_step(difficulty=.02)
+    {'start': 0, 'step': 1}
+    >>> get_start_step(difficulty=.03)
+    {'start': 0, 'step': 1}
+    >>> get_start_step(difficulty=.04)
+    {'start': 10, 'step': 1}
+    """
+```
+
+## Directory structure
+
+```text
+├── docs
+│   ├── AIMA approaches to creating a chatbot.md
+│   ├── ...
+├── pyproject.toml
+├── README.md
+├── scripts
+│   ├── bump_version.py
+│   ├── release.sh
+│   └── requirements.txt
+└── src
+    └── mathactive
+        ├── data
+        │   └── difficulty_start_stop_step.csv
+        ├── data.csv
+        ├── db.sqlite3
+        ├── generators.py
+        ├── hints.py
+        ├── machine.py
+        ├── manage.py
+        ├── microlessons
+        │   ├── num_one.py
+        │   └── utils.py
+        ├── personalize.py
+        ├── python_quiz.py
+        ├── questions.py
+        ├── utils.py
+        ├── webapp
+        │   ├── admin.py
+        │   ├── apps.py
+        │   ├── migrations
+        │   ├── models.py
+        │   ├── tests.py
+        │   └── views.py
+        └── website
+            ├── asgi.py
+            ├── settings.py
+            ├── urls.py
+            └── wsgi.py
+```
```

### Comparing `mathactive-0.0.6/src/mathactive/machine.py` & `mathactive-0.0.7/src/mathactive/machine.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-#!python3
-""" Infinite State Machine to implement a conversational Agent 
-
-Import and export from the v3.dialog.yaml format.
-
-### References
-
-* [python-statemaching](https://pypi.org/project/python-statemachine/)
-
-Example schema to start with (before migrating to `v2.dialog.yaml`
-
-#### *`schema`*
-```yaml
-- 
-  - activity
-  - state name and args 
-  - bot message
-    - human intent numerical answer: destination check answer state
-    - human intent command: destination action/eval state
-    - human intent question: destination FAQ answer state
-    - human intent conversation: destination conversation rapport state
-    - else: fallback destination state
-```
-
-#### *`example counting activity`*      
-```yaml
-- 
-  - count 1
-  - welcome 1 1 3
-  - Welcome! Lets count! Next number after 1, 2, 3 ?
-    - 4: question 1 6 3
-    - else: hint 1 1 3
-
-- 
-  - count 1
-  - hint 1 1 3
-  - what is 1 more than 3?
-    - 4: question 1 2 3
-    - else: hint 1 1 3
-    
-- 
-  - count 1
-  - question 1 1 3
-  - Next number after 1, 2, 3 ?
-    - 4: question 1 6 3
-    - else: hint 1 1 3
-
-- 
-  - count 1
-  - question 1 2 3
-  - Next number after 2, 3, 4?
-    - 5: question 1 6 3
-    - else: hint 1 2 3
-
-- 
-  - count 1
-  - hint 1 1 3
-  - what is 1 more than 3?
-    - 4: question 1 2 3
-    - else: hint 1 1 3
-```
-"""
-from statemachine import StateMachine, State
-
-
-class OrderControl(StateMachine):
-    """State machine for processing purchases of a single commodity item
-
-    >>> control = OrderControl()
-    >>> control.add_to_order(3)
-    3
-    >>> control.add_to_order(7)
-    10
-    >>> control.receive_payment(4)
-    [4]
-    >>> control.current_state.id
-    'waiting_for_payment'
-    """
-
-    waiting_for_payment = State("Waiting for payment", initial=True)
-    processing = State("Processing")
-    shipping = State("Shipping")
-    completed = State("Completed", final=True)
-
-    add_to_order = waiting_for_payment.to(waiting_for_payment)
-    receive_payment = waiting_for_payment.to(
-        processing, cond="payments_enough"
-    ) | waiting_for_payment.to(waiting_for_payment, unless="payments_enough")
-    process_order = processing.to(shipping, cond="payment_received")
-    ship_order = shipping.to(completed)
-
-    def __init__(self):
-        self.order_total = 0
-        self.payments = []
-        self.payment_received = False
-        super(OrderControl, self).__init__()
-
-    def payments_enough(self, amount):
-        return sum(self.payments) + amount >= self.order_total
-
-    def before_add_to_order(self, amount):
-        self.order_total += amount
-        return self.order_total
-
-    def before_receive_payment(self, amount):
-        self.payments.append(amount)
-        return self.payments
-
-    def after_receive_payment(self):
-        self.payment_received = True
-
-    def on_enter_waiting_for_payment(self):
-        self.payment_received = False
-
-
-if __name__ == "__main__":
-    print("control = OrderControl()")
-    control = OrderControl()
-
-    print("control.add_to_order(3)")
-    print(control.add_to_order(3))
-
-    print("control.add_to_order(7)")
-    print(control.add_to_order(7))
-
-    print("control.receive_payment(4)")
-    print(control.receive_payment(4))
-
-    print("control.current_state.id")
-    print(control.current_state.id)
-
-    from statemachine.contrib.diagram import DotGraphMachine
-
-    graph = DotGraphMachine(OrderControl)  # also accepts instances
-    dot = graph()
-    dot.to_string()
-    dot.write_png("docs/order_control_machine_initial.png")
+#!python3
+""" Infinite State Machine to implement a conversational Agent 
+
+Import and export from the v3.dialog.yaml format.
+
+### References
+
+* [python-statemaching](https://pypi.org/project/python-statemachine/)
+
+Example schema to start with (before migrating to `v2.dialog.yaml`
+
+#### *`schema`*
+```yaml
+- 
+  - activity
+  - state name and args 
+  - bot message
+    - human intent numerical answer: destination check answer state
+    - human intent command: destination action/eval state
+    - human intent question: destination FAQ answer state
+    - human intent conversation: destination conversation rapport state
+    - else: fallback destination state
+```
+
+#### *`example counting activity`*      
+```yaml
+- 
+  - count 1
+  - welcome 1 1 3
+  - Welcome! Lets count! Next number after 1, 2, 3 ?
+    - 4: question 1 6 3
+    - else: hint 1 1 3
+
+- 
+  - count 1
+  - hint 1 1 3
+  - what is 1 more than 3?
+    - 4: question 1 2 3
+    - else: hint 1 1 3
+    
+- 
+  - count 1
+  - question 1 1 3
+  - Next number after 1, 2, 3 ?
+    - 4: question 1 6 3
+    - else: hint 1 1 3
+
+- 
+  - count 1
+  - question 1 2 3
+  - Next number after 2, 3, 4?
+    - 5: question 1 6 3
+    - else: hint 1 2 3
+
+- 
+  - count 1
+  - hint 1 1 3
+  - what is 1 more than 3?
+    - 4: question 1 2 3
+    - else: hint 1 1 3
+```
+"""
+from statemachine import StateMachine, State
+
+
+class OrderControl(StateMachine):
+    """State machine for processing purchases of a single commodity item
+
+    >>> control = OrderControl()
+    >>> control.add_to_order(3)
+    3
+    >>> control.add_to_order(7)
+    10
+    >>> control.receive_payment(4)
+    [4]
+    >>> control.current_state.id
+    'waiting_for_payment'
+    """
+
+    waiting_for_payment = State("Waiting for payment", initial=True)
+    processing = State("Processing")
+    shipping = State("Shipping")
+    completed = State("Completed", final=True)
+
+    add_to_order = waiting_for_payment.to(waiting_for_payment)
+    receive_payment = waiting_for_payment.to(
+        processing, cond="payments_enough"
+    ) | waiting_for_payment.to(waiting_for_payment, unless="payments_enough")
+    process_order = processing.to(shipping, cond="payment_received")
+    ship_order = shipping.to(completed)
+
+    def __init__(self):
+        self.order_total = 0
+        self.payments = []
+        self.payment_received = False
+        super(OrderControl, self).__init__()
+
+    def payments_enough(self, amount):
+        return sum(self.payments) + amount >= self.order_total
+
+    def before_add_to_order(self, amount):
+        self.order_total += amount
+        return self.order_total
+
+    def before_receive_payment(self, amount):
+        self.payments.append(amount)
+        return self.payments
+
+    def after_receive_payment(self):
+        self.payment_received = True
+
+    def on_enter_waiting_for_payment(self):
+        self.payment_received = False
+
+
+if __name__ == "__main__":
+    print("control = OrderControl()")
+    control = OrderControl()
+
+    print("control.add_to_order(3)")
+    print(control.add_to_order(3))
+
+    print("control.add_to_order(7)")
+    print(control.add_to_order(7))
+
+    print("control.receive_payment(4)")
+    print(control.receive_payment(4))
+
+    print("control.current_state.id")
+    print(control.current_state.id)
+
+    from statemachine.contrib.diagram import DotGraphMachine
+
+    graph = DotGraphMachine(OrderControl)  # also accepts instances
+    dot = graph()
+    dot.to_string()
+    dot.write_png("docs/order_control_machine_initial.png")
```

### Comparing `mathactive-0.0.6/src/mathactive/microlessons/num_one.py` & `mathactive-0.0.7/src/mathactive/microlessons/num_one.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from ..generators import start_interactive_math
-from ..hints import generate_hint
-from .utils import load_user_data, dump_user, create_file
-
-FILE_PATH = "users.json"
-
-
-def process_user_message(user_id, message_text=""):
-    """
-    there are 2 possible states: question and hint, default is question
-    Algorithm:
-    1. load user by user id
-    2. create new user in case he doesn't exist
-    3. get student state, skill level and last answer result (right or wrong)
-    4.
-        4.1. If last state is question and last answer is wrong get user a hint
-        4.2. If last state is question and last answer is right increase the skill_score and get new question
-        4.3. If last state is hint and last answer is wrong decrease the skill_score and get user a new question
-        4.4. If last state is hint and last answer is right leave the skill_score on the same level, but generate new question with same skill_score
-    10. dump user
-    """
-
-    create_file(FILE_PATH)
-    user_data = load_user_data(user_id, FILE_PATH)
-    if len(user_data) == 0:
-        user_data = {"skill_score": 0.01, "state": "question"}
-    state = user_data["state"]
-    if (
-        state == "hint"
-        and "answer" in user_data
-        and user_data["answer"] == int(message_text)
-    ) or (
-        state == "question"
-        and (
-            message_text == ""
-            or "answer" in user_data
-            and user_data["answer"] == int(message_text)
-        )
-    ):
-        do_increase_skill_score = (
-            "leave"
-            if state == "hint" or state == "question" and message_text == ""
-            else "increase"
-        )
-        output = start_interactive_math(
-            user_data["skill_score"], do_increase_skill_score
-        )
-        user_data["state"] = "question"
-    elif "answer" in user_data and user_data["answer"] != int(message_text):
-        if state == "hint":
-            do_increase_skill_score = "decrease"
-            user_data["state"] = "question"
-        elif state == "question":
-            do_increase_skill_score = "leave"
-            user_data["state"] = "hint"
-        output = (
-            start_interactive_math(user_data["skill_score"], do_increase_skill_score)
-            if state == "hint"
-            else generate_hint(**user_data)
-        )
-
-    user_data.update(**output)
-
-    dump_user(user_id, user_data, FILE_PATH)
-    text = output["text"]
-    message_package = {
-        "messages": text.split(" "),
-        "input_prompt": message_text,
-        "state": user_data["state"],
-    }
-    return message_package
+from ..generators import start_interactive_math
+from ..hints import generate_hint
+from .utils import load_user_data, dump_user, create_file
+
+FILE_PATH = "users.json"
+
+
+def process_user_message(user_id, message_text=""):
+    """
+    there are 2 possible states: question and hint, default is question
+    Algorithm:
+    1. load user by user id
+    2. create new user in case he doesn't exist
+    3. get student state, skill level and last answer result (right or wrong)
+    4.
+        4.1. If last state is question and last answer is wrong get user a hint
+        4.2. If last state is question and last answer is right increase the skill_score and get new question
+        4.3. If last state is hint and last answer is wrong decrease the skill_score and get user a new question
+        4.4. If last state is hint and last answer is right leave the skill_score on the same level, but generate new question with same skill_score
+    10. dump user
+    """
+
+    create_file(FILE_PATH)
+    user_data = load_user_data(user_id, FILE_PATH)
+    if len(user_data) == 0:
+        user_data = {"skill_score": 0.01, "state": "question"}
+    state = user_data["state"]
+    if (
+        state == "hint"
+        and "answer" in user_data
+        and user_data["answer"] == int(message_text)
+    ) or (
+        state == "question"
+        and (
+            message_text == ""
+            or "answer" in user_data
+            and user_data["answer"] == int(message_text)
+        )
+    ):
+        do_increase_skill_score = (
+            "leave"
+            if state == "hint" or state == "question" and message_text == ""
+            else "increase"
+        )
+        output = start_interactive_math(
+            user_data["skill_score"], do_increase_skill_score
+        )
+        user_data["state"] = "question"
+    elif "answer" in user_data and user_data["answer"] != int(message_text):
+        if state == "hint":
+            do_increase_skill_score = "decrease"
+            user_data["state"] = "question"
+        elif state == "question":
+            do_increase_skill_score = "leave"
+            user_data["state"] = "hint"
+        output = (
+            start_interactive_math(user_data["skill_score"], do_increase_skill_score)
+            if state == "hint"
+            else generate_hint(**user_data)
+        )
+
+    user_data.update(**output)
+
+    dump_user(user_id, user_data, FILE_PATH)
+    text = output["text"]
+    message_package = {
+        "messages": text.split(" "),
+        "input_prompt": message_text,
+        "state": user_data["state"],
+    }
+    return message_package
```

### Comparing `mathactive-0.0.6/src/mathactive/microlessons/utils.py` & `mathactive-0.0.7/src/mathactive/microlessons/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import json
-import os
-
-FILE_PATH = "users.json"
-
-
-def create_file(file_path=FILE_PATH):
-    if not os.path.exists(file_path):
-        with open(file_path, "w") as f:
-            f.write()
-
-
-def load_user_data(user_id, file_path=FILE_PATH):
-    with open(file_path, "r") as f:
-        users = json.load(f)
-    try:
-        return users[user_id]
-    except KeyError:
-        return {}
-
-
-def dump_user(user_id, user_data, file_path=FILE_PATH):
-    user_attributes = ["skill_score", "state", "start", "stop", "step", "answer"]
-    with open(file_path, "r") as f:
-        users = json.load(f)
-    users[user_id] = {}
-    for attr in user_attributes:
-        try:
-            users[user_id][attr] = user_data[attr]
-        except KeyError:
-            pass
-    with open(file_path, "w") as f:
-        f.write(json.dumps(users))
+import json
+import os
+
+FILE_PATH = "users.json"
+
+
+def create_file(file_path=FILE_PATH):
+    if not os.path.exists(file_path):
+        with open(file_path, "w") as f:
+            f.write({})
+
+
+def load_user_data(user_id, file_path=FILE_PATH):
+    with open(file_path, "r") as f:
+        users = json.load(f)
+    try:
+        return users[user_id]
+    except KeyError:
+        return {}
+
+
+def dump_user(user_id, user_data, file_path=FILE_PATH):
+    user_attributes = ["skill_score", "state", "start", "stop", "step", "answer"]
+    with open(file_path, "r") as f:
+        users = json.load(f)
+    users[user_id] = {}
+    for attr in user_attributes:
+        try:
+            users[user_id][attr] = user_data[attr]
+        except KeyError:
+            pass
+    with open(file_path, "w") as f:
+        f.write(json.dumps(users))
```

### Comparing `mathactive-0.0.6/src/mathactive/personalize.py` & `mathactive-0.0.7/src/mathactive/personalize.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-# personalize.py
-import pandas as pd
-from pathlib import Path
-
-try:
-    DATA_DIR = Path(__file__).parent / 'data'
-except:
-    DATA_DIR = Path.cwd()
-
-
-DF = pd.read_csv(DATA_DIR / 'difficulty_start_stop.csv')
-
-
-def get_countq_params(difficulty=0.01, example_seq_len=3):
-    """ Predict the parameters of a quiz question generator based on the desired difficulty
-
-    >>> get_countq_params(.01)
-    {'difficulty': 0.01, 'start': 1, 'stop ': 6, 'step': 1, 'correct answer': 6, 'stop': 4}
-    >>> get_countq_params(.02)
-    {'difficulty': 0.02, 'start': 0, 'stop ': 3, 'step': 1, 'correct answer': 3, 'stop': 3}
-    >>> get_countq_params(.03)
-    {'difficulty': 0.03, 'start': 2, 'stop ': 8, 'step': 2, 'correct answer': 8, 'stop': 8}
-    >>> get_countq_params(.05)
-    {'difficulty': 0.05, 'start': 10, 'stop ': 13, 'step': 1, 'correct answer': 13, 'stop': 13}
-    """
-    global DF
-    response = DF[
-        (DF['difficulty'] > difficulty - .02) & (DF['difficulty'] < difficulty + .02)
-    ].sample(1).iloc[0].astype(int).to_dict()
-    response['difficulty'] = difficulty
-    response['stop'] = response['start'] + response['step'] * example_seq_len
-    return response
-
-
-def generate_countq(start=1, stop=None, step=1, example_seq_len=3, **unused_kwargs):
-    """ Generate the question text for a counting quiz question and answer 2-tuple
-
-    >>> generate_countq(start=1, step=1, example_seq_len=3)
-    {'question': 'What is the next number after 1, 2, 3?', 'answer': '4'}
-    """
-    if stop is None:
-        stop = start + example_seq_len * step
-    return {
-        'question': f'What is the next number after {", ".join([str(i) for i in range(start, stop, step)])}?',
-        'answer': f'{stop}',
-    }
-
-
-def generate_difficult_countq(difficulty):
-    """ Generate the question message (str) and answer (float or str) for a counting quiz question
-
-    >>> generate_difficult_countq(.02)
-    {'question': 'What is the next number after 0, 1, 2?', 'answer': '3'}
-    """
-    return generate_countq(**get_countq_params(difficulty))
-
-
-DF_STUDENTS = pd.DataFrame()
-STUDENTS = {}
-
-
-def set_student_skill(student_id, is_correct=1, question_category='counting'):
-    """ Record student's skill level improvement """
-    student_record = STUDENTS.get('student_id', dict(student_id=student_id))
-    k = question_category + '_num_answered'
-    student_record[k] = student_record.get(k, 0) + 1
-    k = question_category + '_num_correct'
-    student_record[k] = student_record.get(k, 0) + is_correct
-    k = question_category + '_skill_score'
-    latest_score = student_record[question_category + '_num_correct'] / \
-        student_record[question_category + '_num_answered']
-    student_record[k] = latest_score
-
-    return student_record
+# personalize.py
+import pandas as pd
+from pathlib import Path
+
+try:
+    DATA_DIR = Path(__file__).parent / 'data'
+except:
+    DATA_DIR = Path.cwd()
+
+
+DF = pd.read_csv(DATA_DIR / 'difficulty_start_stop.csv')
+
+
+def get_countq_params(difficulty=0.01, example_seq_len=3):
+    """ Predict the parameters of a quiz question generator based on the desired difficulty
+
+    >>> get_countq_params(.01)
+    {'difficulty': 0.01, 'start': 1, 'stop ': 6, 'step': 1, 'correct answer': 6, 'stop': 4}
+    >>> get_countq_params(.02)
+    {'difficulty': 0.02, 'start': 0, 'stop ': 3, 'step': 1, 'correct answer': 3, 'stop': 3}
+    >>> get_countq_params(.03)
+    {'difficulty': 0.03, 'start': 2, 'stop ': 8, 'step': 2, 'correct answer': 8, 'stop': 8}
+    >>> get_countq_params(.05)
+    {'difficulty': 0.05, 'start': 10, 'stop ': 13, 'step': 1, 'correct answer': 13, 'stop': 13}
+    """
+    global DF
+    response = DF[
+        (DF['difficulty'] > difficulty - .02) & (DF['difficulty'] < difficulty + .02)
+    ].sample(1).iloc[0].astype(int).to_dict()
+    response['difficulty'] = difficulty
+    response['stop'] = response['start'] + response['step'] * example_seq_len
+    return response
+
+
+def generate_countq(start=1, stop=None, step=1, example_seq_len=3, **unused_kwargs):
+    """ Generate the question text for a counting quiz question and answer 2-tuple
+
+    >>> generate_countq(start=1, step=1, example_seq_len=3)
+    {'question': 'What is the next number after 1, 2, 3?', 'answer': '4'}
+    """
+    if stop is None:
+        stop = start + example_seq_len * step
+    return {
+        'question': f'What is the next number after {", ".join([str(i) for i in range(start, stop, step)])}?',
+        'answer': f'{stop}',
+    }
+
+
+def generate_difficult_countq(difficulty):
+    """ Generate the question message (str) and answer (float or str) for a counting quiz question
+
+    >>> generate_difficult_countq(.02)
+    {'question': 'What is the next number after 0, 1, 2?', 'answer': '3'}
+    """
+    return generate_countq(**get_countq_params(difficulty))
+
+
+DF_STUDENTS = pd.DataFrame()
+STUDENTS = {}
+
+
+def set_student_skill(student_id, is_correct=1, question_category='counting'):
+    """ Record student's skill level improvement """
+    student_record = STUDENTS.get('student_id', dict(student_id=student_id))
+    k = question_category + '_num_answered'
+    student_record[k] = student_record.get(k, 0) + 1
+    k = question_category + '_num_correct'
+    student_record[k] = student_record.get(k, 0) + is_correct
+    k = question_category + '_skill_score'
+    latest_score = student_record[question_category + '_num_correct'] / \
+        student_record[question_category + '_num_answered']
+    student_record[k] = latest_score
+
+    return student_record
```

### Comparing `mathactive-0.0.6/src/mathactive/python_quiz.py` & `mathactive-0.0.7/src/mathactive/python_quiz.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import editdistance
-
-# Define the questions and their corresponding answers
-QA_DICT = {
-    "Step by step list of instructions that if followed exactly will solve the problem under consideration is called a/an ___": "algorithm",
-    "What is the command to print something in Python?": "print",
-    "___ is a notation that is more precise than English but generally not as precise as a programming language": "pseudocode",
-    "Which loop (in Python) would you use if you want to receive input from the user of your program but you don’t know how long it’ll take for them to be done with your code": "while",
-    "Comment 'this word' in Python": "#this word",
-    "How do you write 'snake code' in camel code": "SnakeCode",
-    "How can you determine the type of a variable?": "type",
-    "What is the data type of ‘this is what kind of data’?": "string",
-    "After the following statements, what is the value of y ? x = 15 y = x x = 2023": "15",
-    "What is a built-in Python function that returns the number of characters in a string?": "len"
-
-}
-
-# Define a function to ask a question and compare the user's answer to the correct answer
-
-
-def ask_question(question, answer):
-    user_answer = input(question + " ")
-    similarity_score = 1 - (editdistance.eval(user_answer, answer) / max(len(user_answer), len(answer)))
-    return similarity_score
-
-
-def main(qa_dict=QA_DICT):
-    # Ask each question and keep track of the user's total score
-    total_score = 0
-    for question, answer in qa_dict.items():
-        score = ask_question(question, answer)
-        total_score += score
-
-    return dict(total_score=total_score, num_questions=len(qa_dict))
-
-
-if __name__ == '__main__':
-    results = main()
-    print("Your score is: {total_score} or {total_score*100/num_questions}\%.".format(**results))
+import editdistance
+
+# Define the questions and their corresponding answers
+QA_DICT = {
+    "Step by step list of instructions that if followed exactly will solve the problem under consideration is called a/an ___": "algorithm",
+    "What is the command to print something in Python?": "print",
+    "___ is a notation that is more precise than English but generally not as precise as a programming language": "pseudocode",
+    "Which loop (in Python) would you use if you want to receive input from the user of your program but you don’t know how long it’ll take for them to be done with your code": "while",
+    "Comment 'this word' in Python": "#this word",
+    "How do you write 'snake code' in camel code": "SnakeCode",
+    "How can you determine the type of a variable?": "type",
+    "What is the data type of ‘this is what kind of data’?": "string",
+    "After the following statements, what is the value of y ? x = 15 y = x x = 2023": "15",
+    "What is a built-in Python function that returns the number of characters in a string?": "len"
+
+}
+
+# Define a function to ask a question and compare the user's answer to the correct answer
+
+
+def ask_question(question, answer):
+    user_answer = input(question + " ")
+    similarity_score = 1 - (editdistance.eval(user_answer, answer) / max(len(user_answer), len(answer)))
+    return similarity_score
+
+
+def main(qa_dict=QA_DICT):
+    # Ask each question and keep track of the user's total score
+    total_score = 0
+    for question, answer in qa_dict.items():
+        score = ask_question(question, answer)
+        total_score += score
+
+    return dict(total_score=total_score, num_questions=len(qa_dict))
+
+
+if __name__ == '__main__':
+    results = main()
+    print("Your score is: {total_score} or {total_score*100/num_questions}\%.".format(**results))
```

### Comparing `mathactive-0.0.6/src/mathactive/questions.py` & `mathactive-0.0.7/src/mathactive/questions.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from .utils import convert_sequence_to_string
-
-
-def generate_question_data(start, stop, step, question_num=1):
-    """returns question by provided number with filled parameters
-
-    parameters
-    ----------
-    :start: current number
-    :stop: stop value
-    :step: interval between current and next numbers
-    :question_num: question number"""
-    seq = convert_sequence_to_string(start, stop, step)
-    questions = [
-        f"Let's practice counting   {convert_sequence_to_string(start, stop, step, sep='... ')}   After {stop}, what is the next number you will count?\n{seq}",
-        f"What number comes {step} number after {stop}?\n{seq}",
-        f"We're counting by {step}s.  What number is 1 after {stop}?\n{seq}",
-        f"What is {step} number up from {stop}?\n{seq}",
-        f"If we count up {step} from {stop}, what number is next?\n{seq}",
-    ]
-    questions_data = []
-    for quest in questions:
-        questions_data.append(
-            {
-                "question": quest,
-                "answer": stop + step,
-                "start": start,
-                "stop": stop,
-                "step": step,
-            }
-        )
-    return questions_data[question_num]
+from .utils import convert_sequence_to_string
+
+
+def generate_question_data(start, stop, step, question_num=1):
+    """returns question by provided number with filled parameters
+
+    parameters
+    ----------
+    :start: current number
+    :stop: stop value
+    :step: interval between current and next numbers
+    :question_num: question number"""
+    seq = convert_sequence_to_string(start, stop, step)
+    questions = [
+        f"Let's practice counting   {convert_sequence_to_string(start, stop, step, sep='... ')}   After {stop}, what is the next number you will count?\n{seq}",
+        f"What number comes {step} number after {stop}?\n{seq}",
+        f"We're counting by {step}s.  What number is 1 after {stop}?\n{seq}",
+        f"What is {step} number up from {stop}?\n{seq}",
+        f"If we count up {step} from {stop}, what number is next?\n{seq}",
+    ]
+    questions_data = []
+    for quest in questions:
+        questions_data.append(
+            {
+                "question": quest,
+                "answer": stop + step,
+                "start": start,
+                "stop": stop,
+                "step": step,
+            }
+        )
+    return questions_data[question_num]
```

### Comparing `mathactive-0.0.6/src/mathactive/utils.py` & `mathactive-0.0.7/src/mathactive/utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import numpy
-import pandas
-import random
-from scipy.interpolate import interp1d
-from typing import Literal
-from pathlib import Path
-
-DATA_DIR = Path(__file__).parent.absolute() / 'data'
-
-def get_next_skill_score(
-    skill_score,
-    do_increase_skill_score: Literal["increase", "decrease", "leave"] = "leave",
-):
-    if do_increase_skill_score == "leave":
-        for i in numpy.arange(0.03, 1, 0.05):
-            i = round(i, 2)
-            if round(i - 0.02, 2) <= skill_score <= round(i + 0.02, 2):
-                i = 0.97 if str(i) == str(0.98) else i
-                next_skill_score = round(
-                    random.uniform(round(i - 0.02, 2), round(i + 0.02, 2)), 2
-                )
-                break
-    elif do_increase_skill_score == "increase":
-        if skill_score >= 0.95:
-            next_skill_score = round(random.uniform(0.95, 0.99), 2)
-        else:
-            next_skill_score = round(
-                random.uniform(skill_score + 0.01, skill_score + 0.05), 2
-            )
-    elif do_increase_skill_score == "decrease":
-        if skill_score <= 0.05:
-            next_skill_score = round(random.uniform(0.01, 0.05), 2)
-        else:
-            next_skill_score = round(
-                random.uniform(skill_score - 0.05, skill_score - 0.01), 2
-            )
-
-    return next_skill_score
-
-
-def generate_start_stop_step(
-    skill_score: float, path_to_csv_file: str = f'{DATA_DIR}/difficulty_start_stop_step.csv'
-):
-    """generate start and step values interpolating results to function built from data from file"""
-    df = pandas.read_csv(
-        path_to_csv_file, delimiter=",", header=0, names=['skill_score', 'start', 'stop', 'step']
-    )
-    all_rows = df.loc[:]
-
-    difficulties = [row_data["skill_score"] for _, row_data in all_rows.iterrows()]
-    starts = [row_data["start"] for _, row_data in all_rows.iterrows()]
-    stops = [row_data["stop"] for _, row_data in all_rows.iterrows()]
-
-    interp_start_func = interp1d(difficulties, starts)
-    interp_stop_func = interp1d(difficulties, stops)
-    generated_start = round(float(interp_start_func(skill_score)))
-    generated_stop = round(float(interp_stop_func(skill_score)))
-    if skill_score <= 0.3:
-        step = 1
-    elif skill_score > 0.6:
-        step = 10
-    else:
-        step = 5
-    return {
-        'start': generated_start,
-        'stop': generated_stop,
-        'step': step
-    }
-
-
-def convert_sequence_to_string(start, stop, step, sep=", "):
-    stop += 1  # increase by 1 to include stop value to sequence
-    return sep.join([str(num) for num in range(start, stop, step)])
+import numpy
+import pandas
+import random
+from scipy.interpolate import interp1d
+from typing import Literal
+from pathlib import Path
+
+DATA_DIR = Path(__file__).parent.absolute() / 'data'
+
+def get_next_skill_score(
+    skill_score,
+    do_increase_skill_score: Literal["increase", "decrease", "leave"] = "leave",
+):
+    if do_increase_skill_score == "leave":
+        for i in numpy.arange(0.03, 1, 0.05):
+            i = round(i, 2)
+            if round(i - 0.02, 2) <= skill_score <= round(i + 0.02, 2):
+                i = 0.97 if str(i) == str(0.98) else i
+                next_skill_score = round(
+                    random.uniform(round(i - 0.02, 2), round(i + 0.02, 2)), 2
+                )
+                break
+    elif do_increase_skill_score == "increase":
+        if skill_score >= 0.95:
+            next_skill_score = round(random.uniform(0.95, 0.99), 2)
+        else:
+            next_skill_score = round(
+                random.uniform(skill_score + 0.01, skill_score + 0.05), 2
+            )
+    elif do_increase_skill_score == "decrease":
+        if skill_score <= 0.05:
+            next_skill_score = round(random.uniform(0.01, 0.05), 2)
+        else:
+            next_skill_score = round(
+                random.uniform(skill_score - 0.05, skill_score - 0.01), 2
+            )
+
+    return next_skill_score
+
+
+def generate_start_stop_step(
+    skill_score: float, path_to_csv_file: str = f'{DATA_DIR}/difficulty_start_stop_step.csv'
+):
+    """generate start and step values interpolating results to function built from data from file"""
+    df = pandas.read_csv(
+        path_to_csv_file, delimiter=",", header=0, names=['skill_score', 'start', 'stop', 'step']
+    )
+    all_rows = df.loc[:]
+
+    difficulties = [row_data["skill_score"] for _, row_data in all_rows.iterrows()]
+    starts = [row_data["start"] for _, row_data in all_rows.iterrows()]
+    stops = [row_data["stop"] for _, row_data in all_rows.iterrows()]
+
+    interp_start_func = interp1d(difficulties, starts)
+    interp_stop_func = interp1d(difficulties, stops)
+    generated_start = round(float(interp_start_func(skill_score)))
+    generated_stop = round(float(interp_stop_func(skill_score)))
+    if skill_score <= 0.3:
+        step = 1
+    elif skill_score > 0.6:
+        step = 10
+    else:
+        step = 5
+    return {
+        'start': generated_start,
+        'stop': generated_stop,
+        'step': step
+    }
+
+
+def convert_sequence_to_string(start, stop, step, sep=", "):
+    stop += 1  # increase by 1 to include stop value to sequence
+    return sep.join([str(num) for num in range(start, stop, step)])
```

### Comparing `mathactive-0.0.6/src/mathactive/website/settings.py` & `mathactive-0.0.7/src/mathactive/website/settings.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-"""
-Django settings for website project.
-
-Generated by 'django-admin startproject' using Django 4.1.6.
-
-For more information on this file, see
-https://docs.djangoproject.com/en/4.1/topics/settings/
-
-For the full list of settings and their values, see
-https://docs.djangoproject.com/en/4.1/ref/settings/
-"""
-
-from pathlib import Path
-
-# Build paths inside the project like this: BASE_DIR / 'subdir'.
-BASE_DIR = Path(__file__).resolve().parent.parent
-
-
-# Quick-start development settings - unsuitable for production
-# See https://docs.djangoproject.com/en/4.1/howto/deployment/checklist/
-
-# SECURITY WARNING: keep the secret key used in production secret!
-SECRET_KEY = "django-insecure-ckr7!bk*ro1h*u(mgk5ky1-lnfeiog&_^5jchvuvoi*8lwy@2b"
-
-# SECURITY WARNING: don't run with debug turned on in production!
-DEBUG = True
-
-ALLOWED_HOSTS = []
-
-
-# Application definition
-
-INSTALLED_APPS = [
-    "django.contrib.admin",
-    "django.contrib.auth",
-    "django.contrib.contenttypes",
-    "django.contrib.sessions",
-    "django.contrib.messages",
-    "django.contrib.staticfiles",
-]
-
-MIDDLEWARE = [
-    "django.middleware.security.SecurityMiddleware",
-    "django.contrib.sessions.middleware.SessionMiddleware",
-    "django.middleware.common.CommonMiddleware",
-    "django.middleware.csrf.CsrfViewMiddleware",
-    "django.contrib.auth.middleware.AuthenticationMiddleware",
-    "django.contrib.messages.middleware.MessageMiddleware",
-    "django.middleware.clickjacking.XFrameOptionsMiddleware",
-]
-
-ROOT_URLCONF = "website.urls"
-
-TEMPLATES = [
-    {
-        "BACKEND": "django.template.backends.django.DjangoTemplates",
-        "DIRS": [],
-        "APP_DIRS": True,
-        "OPTIONS": {
-            "context_processors": [
-                "django.template.context_processors.debug",
-                "django.template.context_processors.request",
-                "django.contrib.auth.context_processors.auth",
-                "django.contrib.messages.context_processors.messages",
-            ],
-        },
-    },
-]
-
-WSGI_APPLICATION = "website.wsgi.application"
-
-
-# Database
-# https://docs.djangoproject.com/en/4.1/ref/settings/#databases
-
-DATABASES = {
-    "default": {
-        "ENGINE": "django.db.backends.sqlite3",
-        "NAME": BASE_DIR / "db.sqlite3",
-    }
-}
-
-
-# Password validation
-# https://docs.djangoproject.com/en/4.1/ref/settings/#auth-password-validators
-
-AUTH_PASSWORD_VALIDATORS = [
-    {
-        "NAME": "django.contrib.auth.password_validation.UserAttributeSimilarityValidator",
-    },
-    {
-        "NAME": "django.contrib.auth.password_validation.MinimumLengthValidator",
-    },
-    {
-        "NAME": "django.contrib.auth.password_validation.CommonPasswordValidator",
-    },
-    {
-        "NAME": "django.contrib.auth.password_validation.NumericPasswordValidator",
-    },
-]
-
-
-# Internationalization
-# https://docs.djangoproject.com/en/4.1/topics/i18n/
-
-LANGUAGE_CODE = "en-us"
-
-TIME_ZONE = "UTC"
-
-USE_I18N = True
-
-USE_TZ = True
-
-
-# Static files (CSS, JavaScript, Images)
-# https://docs.djangoproject.com/en/4.1/howto/static-files/
-
-STATIC_URL = "static/"
-
-# Default primary key field type
-# https://docs.djangoproject.com/en/4.1/ref/settings/#default-auto-field
-
-DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
+"""
+Django settings for website project.
+
+Generated by 'django-admin startproject' using Django 4.1.6.
+
+For more information on this file, see
+https://docs.djangoproject.com/en/4.1/topics/settings/
+
+For the full list of settings and their values, see
+https://docs.djangoproject.com/en/4.1/ref/settings/
+"""
+
+from pathlib import Path
+
+# Build paths inside the project like this: BASE_DIR / 'subdir'.
+BASE_DIR = Path(__file__).resolve().parent.parent
+
+
+# Quick-start development settings - unsuitable for production
+# See https://docs.djangoproject.com/en/4.1/howto/deployment/checklist/
+
+# SECURITY WARNING: keep the secret key used in production secret!
+SECRET_KEY = "django-insecure-ckr7!bk*ro1h*u(mgk5ky1-lnfeiog&_^5jchvuvoi*8lwy@2b"
+
+# SECURITY WARNING: don't run with debug turned on in production!
+DEBUG = True
+
+ALLOWED_HOSTS = []
+
+
+# Application definition
+
+INSTALLED_APPS = [
+    "django.contrib.admin",
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.messages",
+    "django.contrib.staticfiles",
+]
+
+MIDDLEWARE = [
+    "django.middleware.security.SecurityMiddleware",
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.middleware.common.CommonMiddleware",
+    "django.middleware.csrf.CsrfViewMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
+    "django.middleware.clickjacking.XFrameOptionsMiddleware",
+]
+
+ROOT_URLCONF = "website.urls"
+
+TEMPLATES = [
+    {
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": [],
+        "APP_DIRS": True,
+        "OPTIONS": {
+            "context_processors": [
+                "django.template.context_processors.debug",
+                "django.template.context_processors.request",
+                "django.contrib.auth.context_processors.auth",
+                "django.contrib.messages.context_processors.messages",
+            ],
+        },
+    },
+]
+
+WSGI_APPLICATION = "website.wsgi.application"
+
+
+# Database
+# https://docs.djangoproject.com/en/4.1/ref/settings/#databases
+
+DATABASES = {
+    "default": {
+        "ENGINE": "django.db.backends.sqlite3",
+        "NAME": BASE_DIR / "db.sqlite3",
+    }
+}
+
+
+# Password validation
+# https://docs.djangoproject.com/en/4.1/ref/settings/#auth-password-validators
+
+AUTH_PASSWORD_VALIDATORS = [
+    {
+        "NAME": "django.contrib.auth.password_validation.UserAttributeSimilarityValidator",
+    },
+    {
+        "NAME": "django.contrib.auth.password_validation.MinimumLengthValidator",
+    },
+    {
+        "NAME": "django.contrib.auth.password_validation.CommonPasswordValidator",
+    },
+    {
+        "NAME": "django.contrib.auth.password_validation.NumericPasswordValidator",
+    },
+]
+
+
+# Internationalization
+# https://docs.djangoproject.com/en/4.1/topics/i18n/
+
+LANGUAGE_CODE = "en-us"
+
+TIME_ZONE = "UTC"
+
+USE_I18N = True
+
+USE_TZ = True
+
+
+# Static files (CSS, JavaScript, Images)
+# https://docs.djangoproject.com/en/4.1/howto/static-files/
+
+STATIC_URL = "static/"
+
+# Default primary key field type
+# https://docs.djangoproject.com/en/4.1/ref/settings/#default-auto-field
+
+DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
```

### Comparing `mathactive-0.0.6/PKG-INFO` & `mathactive-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathactive
-Version: 0.0.6
+Version: 0.0.7
 Summary: Conversational math active learning.
 License: AGPLv3
 Author: hobs
 Author-email: hobson@totalgood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

