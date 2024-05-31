# Comparing `tmp/icx_reward-0.5.0.tar.gz` & `tmp/icx_reward-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icx_reward-0.5.0.tar", last modified: Thu Feb  8 06:13:31 2024, max compression
+gzip compressed data, was "icx_reward-0.6.0.tar", last modified: Fri May 31 05:51:11 2024, max compression
```

## Comparing `icx_reward-0.5.0.tar` & `icx_reward-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:13:31.522782 icx_reward-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-08 06:13:18.000000 icx_reward-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-08 06:13:31.522782 icx_reward-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-02-08 06:13:18.000000 icx_reward-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-02-08 06:13:18.000000 icx_reward-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 06:13:31.522782 icx_reward-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:13:31.518782 icx_reward-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:13:31.518782 icx_reward-0.5.0/src/icx_reward/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/penalty.py
--rw-r--r--   0 runner    (1001) docker     (127)    13444 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/reward.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:13:31.522782 icx_reward-0.5.0/src/icx_reward/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/argparse_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/reward_fund.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/rlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/term.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/types/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-02-08 06:13:18.000000 icx_reward-0.5.0/src/icx_reward/vote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:13:31.522782 icx_reward-0.5.0/src/icx_reward.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-08 06:13:31.000000 icx_reward-0.5.0/src/icx_reward.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-08 06:13:31.000000 icx_reward-0.5.0/src/icx_reward.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 06:13:31.000000 icx_reward-0.5.0/src/icx_reward.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-08 06:13:31.000000 icx_reward-0.5.0/src/icx_reward.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-08 06:13:31.000000 icx_reward-0.5.0/src/icx_reward.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:51:11.084417 icx_reward-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-31 05:51:03.000000 icx_reward-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-31 05:51:11.084417 icx_reward-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-31 05:51:03.000000 icx_reward-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-31 05:51:03.000000 icx_reward-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 05:51:11.084417 icx_reward-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:51:11.080417 icx_reward-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:51:11.080417 icx_reward-0.6.0/src/icx_reward/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/penalty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:51:11.084417 icx_reward-0.6.0/src/icx_reward/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/argparse_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/reward_fund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/rlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-05-31 05:51:03.000000 icx_reward-0.6.0/src/icx_reward/vote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:51:11.084417 icx_reward-0.6.0/src/icx_reward.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-31 05:51:11.000000 icx_reward-0.6.0/src/icx_reward.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-31 05:51:11.000000 icx_reward-0.6.0/src/icx_reward.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 05:51:11.000000 icx_reward-0.6.0/src/icx_reward.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 05:51:11.000000 icx_reward-0.6.0/src/icx_reward.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 05:51:11.000000 icx_reward-0.6.0/src/icx_reward.egg-info/top_level.txt
```

### Comparing `icx_reward-0.5.0/LICENSE` & `icx_reward-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/PKG-INFO` & `icx_reward-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icx_reward
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tools for ICON reward
 Author-email: ICON Foundation <foo@icon.foundation>
 Project-URL: Homepage, https://github.com/icon-project/icx-reward
 Project-URL: Bug Tracker, https://github.com/icon-project/icx-reward/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `icx_reward-0.5.0/README.md` & `icx_reward-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/pyproject.toml` & `icx_reward-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icx_reward"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
     { name = "ICON Foundation", email = "foo@icon.foundation" },
 ]
 description = "Tools for ICON reward"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `icx_reward-0.5.0/src/icx_reward/cli.py` & `icx_reward-0.6.0/src/icx_reward/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     subparser.add_argument("--address", type=IconAddress(), help="address of account", required=required, default=None)
 
 
 def add_address_optional(subparser):
     add_address(subparser, False)
 
 
+def add_height(subparser):
+    subparser.add_argument("--height", type=non_negative_num_type, default=None, help="height of block")
+
+
 def add_time(subparser):
     subparser.add_argument("--height", type=non_negative_num_type, default=None, help="height of block")
     subparser.add_argument("--term", type=num_type, default=None,
                            help="Sequence of Term. Negative value N means last + N sequence")
 
 
 def add_export_vote(subparser, required: bool = False):
@@ -38,24 +42,34 @@
 
 
 def add_import_vote(subparser, required: bool = False):
     subparser.add_argument("--import", help="import vote events from file",
                            type=argparse.FileType('r'), default=None, required=required)
 
 
+def add_count(subparser, required: bool = False):
+    subparser.add_argument("--count", help="count", type=num_type, default=None, required=required)
+
+
+def add_krw(subparser, required: bool = False):
+    subparser.add_argument("--krw", help="korea won", type=num_type, default=None, required=required)
+
+
 parser = ArgumentParser(prog="icx-reward")
 subparsers = parser.add_subparsers(dest="command", help="Command to execute")
 
 cmds = [
     ("check", "check I-Score of account", [add_uri, add_address, add_time, add_export_vote, add_import_vote]),
     ("estimate", "estimate reward of current Term", [add_uri, add_address]),
+    ("apy", "get the APY of voters who voting for Main/Sub P-Reps", [add_uri, add_time, add_count]),
     ("fetch-vote", "fetch all vote events in given Term", [add_uri, add_time, add_address_optional, add_export_vote]),
     ("fetch-penalty", "fetch penalties of account in given Term", [add_uri, add_address_optional, add_time]),
-    ("query", "query I-Score of account", [add_uri, add_address, add_time]),
+    ("query-iscore", "query I-Score of account", [add_uri, add_address, add_height]),
     ("term", "get Term information", [add_uri, add_time]),
+    ("wage", "calculate P-Rep wage", [add_uri, add_time, add_krw]),
 ]
 for cmd in cmds:
     p = subparsers.add_parser(cmd[0], help=cmd[1])
     for add_arg_func in cmd[2]:
         add_arg_func(p)
```

### Comparing `icx_reward-0.5.0/src/icx_reward/commands.py` & `icx_reward-0.6.0/src/icx_reward/commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import sys
 from functools import wraps
+from typing import List
+
+from prettytable import PrettyTable
 
 from icx_reward.penalty import PenaltyFetcher
 from icx_reward.rpc import RPC
 from icx_reward.reward import PRepReward, Voter
-from icx_reward.types.term import Term
 from icx_reward.types.exception import InvalidParamsException
+from icx_reward.types.prep import PRep
+from icx_reward.types.rate import Rate
+from icx_reward.types.reward_fund import RewardFund
+from icx_reward.types.term import Term
 from icx_reward.utils import pprint
 from icx_reward.vote import VoteFetcher
 
+DENOM = 10000
+
 
 def time_info(f):
     @wraps(f)
     def wrapper(args):
         rpc = RPC(args["uri"])
         height = args.get("height", None)
         seq_in = args.get("term", None)
@@ -38,31 +46,49 @@
             height = int(term_["startBlockHeight"], 16)
 
         return f(args, height, term_)
 
     return wrapper
 
 
-@time_info
-def query(args: dict, height: int, term_: dict):
+def query_iscore(args: dict):
     rpc = RPC(args["uri"])
+    height = args["height"]
     resp = rpc.query_iscore(
         address=args["address"],
         height=height,
     )
     pprint(resp)
 
 
 @time_info
-def term(args: dict, height: int, term_: dict):
+def term(_args: dict, _height: int, term_: dict):
     pprint(term_)
 
 
 @time_info
-def fetch_vote(args: dict, height: int, term_: dict):
+def wage(args: dict, _height: int, term_: dict):
+    rpc = RPC(args["uri"])
+    t = Term.from_dict(rpc.term(height=int(term_["startBlockHeight"], 16)))
+    total = t.reward_fund.amount_by_key(RewardFund.IWAGE)
+    count = len(t.preps)
+    amount = total // count
+    krw = args["krw"]
+    tab = PrettyTable()
+    tab.title = f"Monthly P-Rep wage"
+    tab.add_column("Total wage", [format_int(total, True, 0)])
+    tab.add_column("P-Rep count", [count])
+    tab.add_column("Wage (icx)", [format_int(amount, True, 0)])
+    if krw is not None:
+        tab.add_column(f"KRW ({krw})", [format_int(amount * krw, True, 0)])
+    print(tab)
+
+
+@time_info
+def fetch_vote(args: dict, _height: int, term_: dict):
     uri = args["uri"]
     export_fp = args.get("export")
     address = args["address"]
     t = Term.from_dict(term_)
 
     if t.iiss_version < 4:
         pprint("Can't fetch vote. Support IISS 4 only.")
@@ -75,15 +101,15 @@
         print(f"## Export result to {export_fp.name}")
         vf.export(export_fp)
     else:
         vf.print_result()
 
 
 @time_info
-def fetch_penalty(args: dict, height: int, term_: dict):
+def fetch_penalty(args: dict, _height: int, term_: dict):
     address = args["address"]
     t = Term.from_dict(term_)
 
     pprint(f"## Fetch penalties of {'all' if address is None else address} in {t.info()}")
     pf = PenaltyFetcher(args["uri"])
     try:
         penalties = pf.run(t.start_block_height, t.end_block_height, address, True)
@@ -93,15 +119,15 @@
 
     print()
     for height, penalty in penalties.items():
         pprint(f"{penalty}")
 
 
 @time_info
-def check(args: dict, height: int, term_: dict):
+def check(args: dict, _height: int, term_: dict):
     uri = args["uri"]
     address = args["address"]
     import_fp = args["import"]
     t = Term.from_dict(term_)
 
     if t.iiss_version < 4:
         pprint("Support IISS 4 only.")
@@ -156,15 +182,15 @@
     print(f"\n## Queried I-Score is{' not ' if reward != iscore else ' '}same with calculated value")
     if reward != iscore:
         print(f"\tcalculated {format_int(reward)}")
         print(f"\tqueried    {format_int(iscore)}")
 
 
 @time_info
-def estimate(args: dict, height: int, term_: dict):
+def estimate(args: dict, _height: int, term_: dict):
     uri = args["uri"]
     address = args["address"]
     t = Term.from_dict(term_)
     if t.iiss_version < 4:
         pprint("Support IISS 4 only.")
         return
 
@@ -213,26 +239,75 @@
     voter.calculate()
 
     print(f"## Estimated reward")
     prep = pr.get_prep(address)
     print_reward(prep, voter, total_votes, t.period)
 
 
+@time_info
+def apy(args: dict, _height: int, term_: dict):
+    uri = args["uri"]
+    count = args["count"]
+    t = Term.from_dict(term_)
+
+    rpc = RPC(uri)
+    network_info = rpc.get_network_info(t.start_block_height)
+    start_term = Term.from_dict(rpc.term(height=t.start_block_height))
+    rf: RewardFund = start_term.reward_fund
+    if "rewardFund2" in network_info:
+        rf = RewardFund.from_dict(network_info["rewardFund2"])
+
+    preps = []
+    total_power = 0
+    for p in start_term.preps:
+        prep = rpc.get_prep(p.address, to_obj=True)
+        preps.append(prep)
+        total_power += prep.power
+
+    for prep in preps:
+        prep.calculate_apy(
+            total_reward_for_preps=rf.amount_by_key(RewardFund.IPREP),
+            total_power=total_power,
+            br=start_term.bond_requirement,
+        )
+
+    apy_list = sorted(preps, key=lambda p: p.apy_sort_key(), reverse=True)
+    print_apy(apy_list, count)
+
+
 def print_reward(prep, voter, total_votes: int = 0, period: int = 0):
     reward = (0 if prep is None else prep.reward()) + voter.reward
     reward_loop = reward // 10 ** 3
     print(f"\t= PRep.commission + PRep.wage + Voter.reward")
     print()
     print(f"\t= {format_int(0 if prep is None else prep.commission)} # PRep.commission")
     print(f"\t+ {format_int(0 if prep is None else prep.wage)} # PRep.wage")
     print(f"\t+ {format_int(voter.reward)} # Voter.reward")
     print()
     print(f"\t= {format_int(reward)} iscore")
     print(f"\t= {format_int(reward_loop)} loop")
-    print(f"\t= {format_int(reward_loop / 10 ** 18)} icx")
+    print(f"\t= {format_int(reward_loop, to_icx=True)} icx")
     if total_votes > 0:
         apy = reward_loop * 365 * 100 * 43200 / (total_votes * period)
         print(f"\n## Estimated APY = {apy} %")
 
 
-def format_int(value):
-    return f"{value:40,}"
+def format_int(value, to_icx: bool = False, width: int = 40):
+    return f"{value // 10 ** 18 if to_icx else value:{width},}"
+
+
+def print_apy(apy_list: List[PRep], count: int = None):
+    tab = PrettyTable(["name", "APY", "commission %", "bond %", "remain_vote(icx)", "address"])
+    for i, p in enumerate(apy_list):
+        if count != 0 and count == i:
+            break
+        tab.add_row(
+            [
+                p.name,
+                p.apy,
+                p.commission_rate.percent(),
+                p.bond_rate(),
+                format_int(p.remain_vote, to_icx=True, width=10),
+                str(p.address),
+            ]
+        )
+    print(tab)
```

### Comparing `icx_reward-0.5.0/src/icx_reward/penalty.py` & `icx_reward-0.6.0/src/icx_reward/penalty.py`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/src/icx_reward/reward.py` & `icx_reward-0.6.0/src/icx_reward/reward.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from __future__ import annotations
 
 import sys
 from typing import Dict, List, Optional
 
-from icx_reward.penalty import Penalty, PenaltyFetcher
+from prettytable import PrettyTable
+
+from icx_reward.penalty import Penalty
 from icx_reward.rpc import RPC
 from icx_reward.types.constants import ICX_TO_ISCORE_RATE, MONTH_BLOCK, RATE_DENOM
 from icx_reward.types.exception import InvalidParamsException
 from icx_reward.types.prep import JailInfo, PRep as PRepResp
+from icx_reward.types.rate import Rate
+from icx_reward.types.reward_fund import RewardFund
+from icx_reward.types.term import Term
 from icx_reward.vote import Vote, Votes
 
 
 class PRep:
     def __init__(self, enable: bool, address: str, bonded: int, delegated: int, power: int, commission_rate: int):
         self.__enable = enable
         self.__address = address
@@ -90,22 +95,22 @@
 
     def update_penalty(self, penalties: Dict[int, Penalty]):
         for k, v in penalties.items():
             p = v.get_by_address(self.address)
             if not p.is_empty():
                 self.penalties[k] = p
 
-    def apply_vote_diff(self, type_: int, value: int, period: int, br: int):
+    def apply_vote_diff(self, type_: int, value: int, period: int, br: Rate):
         if type_ == Vote.TYPE_BOND:
             self.__bonded += value
         else:
             self.__delegated += value
         self.__accumulated_voted += value * period
 
-        power = min(self.__bonded * 100 // br, self.__bonded + self.__delegated)
+        power = min(br.divide_int(self.__bonded), self.__bonded + self.__delegated)
         power_diff = power - self.__power
         self.__power = power
         self.__accumulated_power += power_diff * period
 
     def calculate_reward(self, total_prep_reward: int, total_accum_power: int, wage: int, min_bond: int):
         if self.rewardable():
             reward = total_prep_reward * self.__accumulated_power // total_accum_power
@@ -130,14 +135,24 @@
             address=prep["address"],
             bonded=int(prep["bonded"], 16),
             delegated=int(prep["delegated"], 16),
             power=int(prep["power"], 16),
             commission_rate=int(prep.get("commissionRate", "0x0"), 16),
         )
 
+    @classmethod
+    def table_header(cls):
+        return ['address', 'enable', 'accum_voted', 'accum_power', 'commission', 'wage', 'voter_reward']
+
+    def table_value(self):
+        return [
+            self.__address, self.__enable, self.__accumulated_voted, self.__accumulated_power,
+            self.__commission, self.__wage, self.__voter_reward,
+        ]
+
 
 class Voter:
     def __init__(self, address: str, votes: Votes, start_height: int, offset_limit: int, preps: Dict[str, PRep],
                  file=None):
         self.__address = address
         self.__votes = votes
         self.__start_height = start_height
@@ -209,34 +224,32 @@
 
     def _print(self, msg: str):
         if self.__file is not None:
             print(msg, file=self.__file)
 
 
 class PRepReward:
-    def __init__(self, uri: str, start: int, end: int, br: int, validator_count: int, min_bond: int, preps: dict,
-                 iglobal: int, iprep: int, iwage: int):
+    def __init__(self, uri: str, start: int, end: int, br: Rate, validator_count: int, min_bond: int, preps: dict,
+                 rf: RewardFund):
         self.__start_height: int = start
         self.__end_height: int = end
         self.__height = self.__end_height
-        self.__br: int = br
+        self.__br: Rate = br
         self.__validator_count: int = validator_count
         self.__min_bond: int = min_bond
         self.__preps: Dict[str, PRep] = preps
         self.__rpc = RPC(uri)
 
-        self.__total_prep_reward: int = self._reward_iscore_of_term(iglobal, iprep, self.period())
-        self.__total_wage: int = self._reward_iscore_of_term(iglobal, iwage, self.period())
+        self.__total_prep_reward: int = self._reward_iscore_of_term(rf.amount_by_key(RewardFund.IPREP), self.period())
+        self.__total_wage: int = self._reward_iscore_of_term(rf.amount_by_key(RewardFund.IWAGE), self.period())
         self.__total_accumulated_power: int = 0
 
-
-
     @staticmethod
-    def _reward_iscore_of_term(iglobal: int, rate: int, term_period: int) -> int:
-        return (iglobal * rate // RATE_DENOM) * ICX_TO_ISCORE_RATE * term_period // MONTH_BLOCK
+    def _reward_iscore_of_term(icx_amount: int, term_period: int) -> int:
+        return icx_amount * ICX_TO_ISCORE_RATE * term_period // MONTH_BLOCK
 
     @property
     def start_height(self) -> int:
         return self.__start_height
 
     @property
     def end_height(self) -> int:
@@ -315,15 +328,16 @@
         preps_addr = self.__preps.keys()
         # update accumulated value in PRep
         for vote in vote_diff_list:
             for to, value in vote.values.items():
                 if to not in preps_addr:
                     continue
                 prep = self.__preps[to]
-                prep.apply_vote_diff(vote.type, value, self.offset_limit() - vote.offset(self.__start_height), self.__br)
+                prep.apply_vote_diff(vote.type, value, self.offset_limit() - vote.offset(self.__start_height),
+                                     self.__br)
                 self.__preps[to] = prep
 
         # update total_accumulated_power
         total_accum_power = 0
         for prep in self.__preps.values():
             total_accum_power += prep.accumulated_power
         self.__total_accumulated_power = total_accum_power
@@ -347,35 +361,41 @@
         self.calculate_reward()
 
     def print_summary(self, file=sys.stdout):
         print(f"<< PRep reward summary. {self.__start_height} ~ {self.__end_height}", file=file)
         print(f"Total PRep reward: {self.__total_prep_reward}, Total wage: {self.__total_wage}", file=file)
         print(f"Total accumulated power: {self.__total_accumulated_power}", file=file)
         print(f"Elected PReps", file=file)
+        header = ["rand"]
+        header.extend(PRep.table_header())
+        tab = PrettyTable(header)
         for i, prep in enumerate(self.__preps.values()):
-            print(f"\t#{i}: {prep}", file=file)
+            value = [i]
+            value.extend(prep.table_value())
+            tab.add_row(value)
+        print(tab)
 
     @staticmethod
     def from_network(uri: str, height: int) -> PRepReward:
         return PRepReward.from_term(uri, RPC(uri).term(height))
 
     @staticmethod
     def from_term(uri: str, term: dict) -> PRepReward:
-        if term["startBlockHeight"] != term["blockHeight"]:
+        t = Term.from_dict(term)
+        if t.start_block_height != t.block_height:
             raise InvalidParamsException(f"term must be value at term start height")
+
         preps: Dict[str, PRep] = {}
         for p in term["preps"]:
             prep = PRep.from_get_prep(p)
             preps[prep.address] = prep
 
         return PRepReward(
             uri=uri,
-            start=int(term["startBlockHeight"], 0),
-            end=int(term["endBlockHeight"], 0),
-            br=int(term["bondRequirement"], 0),
-            validator_count=len(term["preps"]),
+            start=t.start_block_height,
+            end=t.end_block_height,
+            br=t.bond_requirement,
+            validator_count=len(preps),
             preps=preps,
-            iglobal=int(term["rewardFund"]["Iglobal"], 0),
-            iprep=int(term["rewardFund"]["Iprep"], 0),
-            iwage=int(term["rewardFund"].get("Iwage", "0x0"), 0),
-            min_bond=int(term.get("minimumBond", "0x0"), 0),
+            min_bond=t.minimum_bond,
+            rf=t.reward_fund,
         )
```

### Comparing `icx_reward-0.5.0/src/icx_reward/types/address.py` & `icx_reward-0.6.0/src/icx_reward/types/address.py`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/src/icx_reward/types/argparse_type.py` & `icx_reward-0.6.0/src/icx_reward/types/argparse_type.py`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/src/icx_reward/types/bloom.py` & `icx_reward-0.6.0/src/icx_reward/types/bloom.py`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/src/icx_reward/types/event.py` & `icx_reward-0.6.0/src/icx_reward/types/event.py`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/src/icx_reward/types/exception.py` & `icx_reward-0.6.0/src/icx_reward/types/exception.py`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/src/icx_reward/types/prep.py` & `icx_reward-0.6.0/src/icx_reward/types/prep.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from enum import auto, IntEnum, IntFlag
 
 from icx_reward.types.address import Address
+from icx_reward.types.rate import Rate
 
 
 class Status(IntEnum):
     """
     Enumerate of PRep status
     """
     Active = 0
@@ -28,14 +29,17 @@
     Sub = 1
     Candidate = 2
     NONE = 3
 
     def __str__(self) -> str:
         return repr(self)
 
+    def rewardable(self) -> bool:
+        return self < self.Candidate
+
     @staticmethod
     def from_string(grade: str):
         return Grade(int(grade, 16))
 
 
 class PenaltyFlag(IntFlag):
     """
@@ -165,24 +169,27 @@
         self._jail_info = jail_info
         self._status = status
         self._grade = grade
         self._penalty = penalty
         self._has_pub_key = has_pub_key
         self._bonded = int(bonded, 16)
         self._last_height = int(last_height, 16)
-        self._commission_rate = int(commission_rate, 16)
-        self._max_commission_rate = int(max_commission_rate, 16)
-        self._max_commission_change_rate = int(max_commission_change_rate, 16)
+        self._commission_rate = Rate(int(commission_rate, 16))
+        self._max_commission_rate = Rate(int(max_commission_rate, 16))
+        self._max_commission_change_rate = Rate(int(max_commission_change_rate, 16))
+
+        self._apy = 0
+        self._remain_vote = 0
 
     def __str__(self):
         return (f'PRep{{{self._status}, {self._grade}, {self._penalty}, bonded:{self._bonded}, '
                 f'last_height:{self._last_height}, '
-                f'commission_rate:{self._commission_rate}, '
-                f'max_commission_rate:{self._max_commission_rate}, '
-                f'max_commission_change_rate:{self._max_commission_change_rate}, '
+                f'commission_rate:{self._commission_rate.value}, '
+                f'max_commission_rate:{self._max_commission_rate.value}, '
+                f'max_commission_change_rate:{self._max_commission_change_rate.value}, '
                 f'{self._jail_info}, has_pub_key:{self._has_pub_key}, {super().__str__()}}}')
 
     @property
     def status(self) -> Status:
         return self._status
 
     @property
@@ -201,39 +208,66 @@
     def has_pub_key(self) -> bool:
         return self._has_pub_key
 
     @property
     def bonded(self) -> int:
         return self._bonded
 
+    def voted(self) -> int:
+        return self._bonded + self._delegated
+
     @property
     def last_height(self) -> int:
         return self._last_height
 
     @property
-    def commission_rate(self) -> int:
+    def commission_rate(self) -> Rate:
         return self._commission_rate
 
     @property
-    def max_commission_rate(self) -> int:
+    def max_commission_rate(self) -> Rate:
         return self._max_commission_rate
 
     @property
-    def max_commission_change_rate(self) -> int:
+    def max_commission_change_rate(self) -> Rate:
         return self._max_commission_change_rate
 
     def in_jail(self) -> bool:
         return self._jail_info.jail_flags.in_jail()
 
     def unjailing(self) -> bool:
         return self._jail_info.jail_flags.unjailing()
 
     def unjailable(self) -> bool:
         return self._jail_info.jail_flags.unjailable()
 
+    def bond_rate(self) -> float:
+        return round(self._bonded * 100 / self.voted(), 2)
+
+    @property
+    def remain_vote(self) -> int:
+        return self._remain_vote
+
+    @property
+    def apy(self) -> float:
+        return self._apy
+
+    def calculate_apy(self, total_reward_for_preps: int, total_power: int, br: Rate) -> float:
+        if self.grade.rewardable():
+            reward_for_prep = total_reward_for_preps * self._power * 12 // total_power
+            reward_for_voter = reward_for_prep * (1 - self._commission_rate.value / self._commission_rate.denom)
+            self._apy = round(reward_for_voter * 100 / self.voted(), 3)
+        else:
+            self._apy = float(0)
+        self._remain_vote = br.divide_int(self._bonded) - self.voted()
+        return self._apy
+
+    def apy_sort_key(self):
+        return (Grade.Candidate > self.grade), self._apy, self._remain_vote
+
     @staticmethod
     def from_dict(values: dict):
         return PRep(
             status=Status.from_string(values.get("status", "0x0")),
             grade=Grade.from_string(values.get("grade", "0x0")),
             penalty=PenaltyFlag.from_string(values.get("penalty", "0x0")),
             has_pub_key=True if values.get("hashPublicKey", "0x1") == "0x1" else False,
```

### Comparing `icx_reward-0.5.0/src/icx_reward/types/rlp.py` & `icx_reward-0.6.0/src/icx_reward/types/rlp.py`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/src/icx_reward/types/term.py` & `icx_reward-0.6.0/src/icx_reward/types/term.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import List
 
 from icx_reward.types.prep import PRep
+from icx_reward.types.rate import Rate
 from icx_reward.types.reward_fund import RewardFund
 
 
 class Term:
     def __init__(self,
                  block_height: int,
-                 bond_requirement: int,
+                 bond_requirement: Rate,
                  end_block_height: int,
                  iiss_version: int,
                  is_decentralized: bool,
                  main_prep_count: int,
                  minimum_bond: int,
                  period: int,
                  preps: List[PRep],
@@ -55,17 +56,21 @@
         return f"Term('sequence': {self.sequence}', start_height: {self.start_block_height}, 'end_block_height': {self.end_block_height})"
 
     def is_prep(self, address: str):
         return address in [str(p.address) for p in self.preps]
 
     @staticmethod
     def from_dict(values: dict):
+        if "bondRequirement" in values:
+            br = Rate(int(values["bondRequirement"], 16), Rate.DENOM_OLD)
+        else:
+            br = Rate(int(values["bondRequirementRate"], 16))
         return Term(
             block_height=int(values["blockHeight"], 16),
-            bond_requirement=int(values["bondRequirement"], 16),
+            bond_requirement= br,
             end_block_height=int(values["endBlockHeight"], 16),
             iiss_version=int(values["iissVersion"], 16),
             is_decentralized=bool(int(values["isDecentralized"], 16)),
             main_prep_count=int(values["mainPRepCount"], 16),
             minimum_bond=int(values.get("minimumBond", "0x0"), 16),
             period=int(values["period"], 16),
             preps=[PRep.from_dict(x) for x in values["preps"]],
```

### Comparing `icx_reward-0.5.0/src/icx_reward/types/utils.py` & `icx_reward-0.6.0/src/icx_reward/types/utils.py`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/src/icx_reward/utils.py` & `icx_reward-0.6.0/src/icx_reward/utils.py`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/src/icx_reward/vote.py` & `icx_reward-0.6.0/src/icx_reward/vote.py`

 * *Files identical despite different names*

### Comparing `icx_reward-0.5.0/src/icx_reward.egg-info/PKG-INFO` & `icx_reward-0.6.0/src/icx_reward.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icx_reward
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tools for ICON reward
 Author-email: ICON Foundation <foo@icon.foundation>
 Project-URL: Homepage, https://github.com/icon-project/icx-reward
 Project-URL: Bug Tracker, https://github.com/icon-project/icx-reward/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `icx_reward-0.5.0/src/icx_reward.egg-info/SOURCES.txt` & `icx_reward-0.6.0/src/icx_reward.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 src/icx_reward/types/address.py
 src/icx_reward/types/argparse_type.py
 src/icx_reward/types/bloom.py
 src/icx_reward/types/constants.py
 src/icx_reward/types/event.py
 src/icx_reward/types/exception.py
 src/icx_reward/types/prep.py
+src/icx_reward/types/rate.py
 src/icx_reward/types/reward_fund.py
 src/icx_reward/types/rlp.py
 src/icx_reward/types/term.py
 src/icx_reward/types/utils.py
```

