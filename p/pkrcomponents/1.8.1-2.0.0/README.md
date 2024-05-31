# Comparing `tmp/pkrcomponents-1.8.1.tar.gz` & `tmp/pkrcomponents-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.8.1.tar", last modified: Thu May 30 09:36:59 2024, max compression
+gzip compressed data, was "pkrcomponents-2.0.0.tar", last modified: Fri May 31 18:46:10 2024, max compression
```

## Comparing `pkrcomponents-1.8.1.tar` & `pkrcomponents-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-30 09:36:59.064635 pkrcomponents-1.8.1/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-30 09:36:58.741027 pkrcomponents-1.8.1/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.8.1/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.8.1/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.8.1/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-30 09:36:59.060165 pkrcomponents-1.8.1/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.8.1/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1512 2024-05-30 09:17:12.000000 pkrcomponents-1.8.1/coverage.txt
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-30 09:36:58.986215 pkrcomponents-1.8.1/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.8.1/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.8.1/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      933 2024-05-27 23:40:01.000000 pkrcomponents-1.8.1/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.8.1/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4030 2024-05-29 18:47:23.000000 pkrcomponents-1.8.1/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1386 2024-05-29 10:10:09.000000 pkrcomponents-1.8.1/pkrcomponents/buy_in.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4409 2024-05-29 11:00:59.000000 pkrcomponents-1.8.1/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-27 17:30:11.000000 pkrcomponents-1.8.1/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1401 2024-05-29 11:06:38.000000 pkrcomponents-1.8.1/pkrcomponents/deck.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.8.1/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13075 2024-05-27 18:44:25.000000 pkrcomponents-1.8.1/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1586 2024-05-29 09:57:04.000000 pkrcomponents-1.8.1/pkrcomponents/level.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1382 2024-05-27 17:30:11.000000 pkrcomponents-1.8.1/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.8.1/pkrcomponents/lookup_table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3998 2024-05-29 10:44:39.000000 pkrcomponents-1.8.1/pkrcomponents/payout.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5171 2024-05-29 13:53:41.000000 pkrcomponents-1.8.1/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1429 2024-05-29 10:34:29.000000 pkrcomponents-1.8.1/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    16774 2024-05-29 11:06:38.000000 pkrcomponents-1.8.1/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    14787 2024-05-29 18:33:29.000000 pkrcomponents-1.8.1/pkrcomponents/table_player.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-29 09:25:32.000000 pkrcomponents-1.8.1/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-30 09:36:59.036416 pkrcomponents-1.8.1/pkrcomponents/utils/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:06:12.000000 pkrcomponents-1.8.1/pkrcomponents/utils/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      301 2024-05-27 18:51:06.000000 pkrcomponents-1.8.1/pkrcomponents/utils/converters.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      371 2024-05-27 20:12:18.000000 pkrcomponents-1.8.1/pkrcomponents/utils/validators.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-30 09:36:59.052345 pkrcomponents-1.8.1/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      693 2024-05-30 09:36:57.000000 pkrcomponents-1.8.1/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.8.1/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-30 09:36:59.065712 pkrcomponents-1.8.1/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1399 2024-05-27 22:58:49.000000 pkrcomponents-1.8.1/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 18:46:10.119210 pkrcomponents-2.0.0/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 18:46:09.745436 pkrcomponents-2.0.0/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-2.0.0/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-2.0.0/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-2.0.0/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-31 18:46:10.119210 pkrcomponents-2.0.0/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-2.0.0/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1512 2024-05-31 18:42:51.000000 pkrcomponents-2.0.0/coverage.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 18:46:10.023970 pkrcomponents-2.0.0/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-2.0.0/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-2.0.0/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4097 2024-05-31 18:42:39.000000 pkrcomponents-2.0.0/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-2.0.0/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4030 2024-05-29 18:47:23.000000 pkrcomponents-2.0.0/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1386 2024-05-29 10:10:09.000000 pkrcomponents-2.0.0/pkrcomponents/buy_in.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4409 2024-05-29 11:00:59.000000 pkrcomponents-2.0.0/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-27 17:30:11.000000 pkrcomponents-2.0.0/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1401 2024-05-29 11:06:38.000000 pkrcomponents-2.0.0/pkrcomponents/deck.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-2.0.0/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13075 2024-05-27 18:44:25.000000 pkrcomponents-2.0.0/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1586 2024-05-29 09:57:04.000000 pkrcomponents-2.0.0/pkrcomponents/level.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1382 2024-05-27 17:30:11.000000 pkrcomponents-2.0.0/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-2.0.0/pkrcomponents/lookup_table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3998 2024-05-29 10:44:39.000000 pkrcomponents-2.0.0/pkrcomponents/payout.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5171 2024-05-29 13:53:41.000000 pkrcomponents-2.0.0/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1429 2024-05-29 10:34:29.000000 pkrcomponents-2.0.0/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    18160 2024-05-31 17:25:18.000000 pkrcomponents-2.0.0/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13465 2024-05-31 18:42:39.000000 pkrcomponents-2.0.0/pkrcomponents/table_player.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3422 2024-05-31 18:42:39.000000 pkrcomponents-2.0.0/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 18:46:10.087520 pkrcomponents-2.0.0/pkrcomponents/utils/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:06:12.000000 pkrcomponents-2.0.0/pkrcomponents/utils/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      185 2024-05-31 18:09:47.000000 pkrcomponents-2.0.0/pkrcomponents/utils/converters.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      371 2024-05-27 20:12:18.000000 pkrcomponents-2.0.0/pkrcomponents/utils/validators.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-31 18:46:10.119210 pkrcomponents-2.0.0/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      693 2024-05-31 18:46:08.000000 pkrcomponents-2.0.0/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-2.0.0/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-31 18:46:10.119210 pkrcomponents-2.0.0/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1399 2024-05-27 22:58:49.000000 pkrcomponents-2.0.0/setup.py
```

### Comparing `pkrcomponents-1.8.1/LICENSE.txt` & `pkrcomponents-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/MANIFEST.in` & `pkrcomponents-2.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/PKG-INFO` & `pkrcomponents-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.8.1
+Version: 2.0.0
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.8.1/coverage.txt` & `pkrcomponents-2.0.0/coverage.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Name                                Stmts   Miss  Cover
 -------------------------------------------------------
 pkrcomponents/__init__.py               0      0   100%
 pkrcomponents/_common.py               48      0   100%
-pkrcomponents/action.py                11      0   100%
+pkrcomponents/action.py                56      0   100%
 pkrcomponents/bitcard.py               68      0   100%
 pkrcomponents/board.py                 83      0   100%
 pkrcomponents/buy_in.py                14      0   100%
 pkrcomponents/card.py                  87      0   100%
 pkrcomponents/constants.py             71      0   100%
 pkrcomponents/deck.py                  26      1    96%
 pkrcomponents/evaluator.py             28      0   100%
 pkrcomponents/hand.py                 228      0   100%
 pkrcomponents/level.py                 17      0   100%
 pkrcomponents/listings.py              16      0   100%
 pkrcomponents/lookup_table.py         112      0   100%
 pkrcomponents/payout.py                37      0   100%
 pkrcomponents/players.py              109      0   100%
 pkrcomponents/pot.py                   13      0   100%
-pkrcomponents/table.py                327      4    99%
-pkrcomponents/table_player.py         181      2    99%
+pkrcomponents/table.py                345      2    99%
+pkrcomponents/table_player.py         157      1    99%
 pkrcomponents/tournament.py            46      0   100%
 pkrcomponents/utils/__init__.py         0      0   100%
-pkrcomponents/utils/converters.py       6      1    83%
+pkrcomponents/utils/converters.py       3      0   100%
 pkrcomponents/utils/validators.py       7      0   100%
 -------------------------------------------------------
-TOTAL                                1535      8    99%
+TOTAL                                1571      4    99%
```

### Comparing `pkrcomponents-1.8.1/pkrcomponents/_common.py` & `pkrcomponents-2.0.0/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/bitcard.py` & `pkrcomponents-2.0.0/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/board.py` & `pkrcomponents-2.0.0/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/buy_in.py` & `pkrcomponents-2.0.0/pkrcomponents/buy_in.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/card.py` & `pkrcomponents-2.0.0/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/constants.py` & `pkrcomponents-2.0.0/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/deck.py` & `pkrcomponents-2.0.0/pkrcomponents/deck.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/evaluator.py` & `pkrcomponents-2.0.0/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/hand.py` & `pkrcomponents-2.0.0/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/level.py` & `pkrcomponents-2.0.0/pkrcomponents/level.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/listings.py` & `pkrcomponents-2.0.0/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/lookup_table.py` & `pkrcomponents-2.0.0/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/payout.py` & `pkrcomponents-2.0.0/pkrcomponents/payout.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/players.py` & `pkrcomponents-2.0.0/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/pot.py` & `pkrcomponents-2.0.0/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/pkrcomponents/table.py` & `pkrcomponents-2.0.0/pkrcomponents/table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from functools import cached_property
 from pkrcomponents.board import Board
 from pkrcomponents.deck import Deck
 from pkrcomponents.constants import Street
 from pkrcomponents.players import Players
 from pkrcomponents.pot import Pot
 from pkrcomponents.tournament import Level, Tournament
 from pkrcomponents.evaluator import Evaluator
 
 
 class Table:
     """Class representing a poker table"""
-    _ident: str
     _board: Board
     _deck: Deck
     _players: Players
     _pots: [Pot]
     _max_players: int
     _is_mtt: bool
     _tournament: Tournament
@@ -133,17 +131,22 @@
         """Returns the list of the indexes of players on the table, with order depending on current street"""
         if self._street == Street.PREFLOP:
             return self.players.preflop_ordered_seats
         else:
             return self.players.postflop_ordered_seats
 
     @property
-    def players_waiting(self) -> list:
+    def players_order(self):
+        """Returns the players in playing order"""
+        return [self.players[i] for i in self.playing_order]
+
+    @property
+    def players_waiting(self):
         """Returns the list of players on the table that are waiting to play"""
-        return [self.players[i] for i in self.playing_order if self.players[i].can_play]
+        return [player for player in self.players_order if player.can_play]
 
     @property
     def street_ended(self) -> bool:
         """Returns True if the street has ended"""
         return len(self.players_waiting) == 0 or (
                 self.nb_waiting == 1
                 and self.nb_in_game == 1
@@ -151,25 +154,25 @@
                 and self.street != Street.SHOWDOWN) or (
                 self.street == Street.SHOWDOWN and len(self.unrevealed_players) == 0
         )
 
     @property
     def players_in_game(self) -> list:
         """Returns the list of players on the table that are still in the game (they can make an action)"""
-        return [self.players[i] for i in self.playing_order if self.players[i].in_game]
+        return [player for player in self.players_order if player.in_game]
 
     @property
     def players_involved(self) -> list:
         """Returns the list of players on the table that didn't fold yet"""
-        return [self.players[i] for i in self.playing_order if not self.players[i].folded]
+        return [player for player in self.players_order if not player.folded]
 
     @property
     def hand_ended(self) -> bool:
         """Returns True if the hand has ended"""
-        return len(self.players_involved) == 1 or self.street == Street.SHOWDOWN
+        return self.nb_involved == 1 or self.street == Street.SHOWDOWN
 
     @property
     def next_street_ready(self) -> bool:
         """Returns True if the next street is ready to be played"""
         return self.street_ended and not self.hand_ended
 
     @property
@@ -223,46 +226,54 @@
         c3 = self._deck.draw(c3)
         self._board.add(c1)
         self._board.add(c2)
         self._board.add(c3)
 
     def flop(self, c1=None, c2=None, c3=None):
         """Draw a flop and steps to this new street"""
+        if not (self.next_street_ready and self.street == Street.PREFLOP):
+            raise ValueError("The PREFLOP must be ended before we can draw a flop")
         self.draw_flop(c1=c1, c2=c2, c3=c3)
         self.street = "flop"
         self.street_reset()
 
     def draw_turn(self, card=None):
         """For the turn, draws a card in the deck and adds it on the board as turn card"""
         if len(self._board) != 3:
             raise ValueError("Board size must be 3 before we can draw a turn")
         card = self._deck.draw(card)
         self._board.add(card)
 
     def turn(self, card=None):
         """Draw a turn and steps to this new street"""
+        if not (self.next_street_ready and self.street == Street.FLOP):
+            raise ValueError("The FLOP must be ended before we can draw a turn")
         self.draw_turn(card)
         self.street = "turn"
         self.street_reset()
 
     def draw_river(self, card=None):
         """For the river, draws a card in the deck and adds it on the board as river card"""
         if len(self._board) != 4:
             raise ValueError("Board size must be 4 before we can draw a turn")
         card = self._deck.draw(card)
         self._board.add(card)
 
     def river(self, card=None):
         """Draw a river and steps to this new street"""
+        if not (self.next_street_ready and self.street == Street.TURN):
+            raise ValueError("The TURN must be ended before we can draw a river")
         self.draw_river(card)
         self.street = "river"
         self.street_reset()
 
     def advance_to_showdown(self):
         """Advance to showdown"""
+        if not (self.next_street_ready and self.street == Street.RIVER):
+            raise ValueError("The RIVER must be ended before we can advance to showdown")
         self.street = Street.SHOWDOWN
         self.street_reset()
 
     def add_tournament(self, tournament):
         """Associates table with a tournament"""
         self.tournament = tournament
         self._is_mtt = True
@@ -289,14 +300,22 @@
         """
         Set a player as the hero
         """
         for p in self.players:
             p.is_hero = False
         player.is_hero = True
 
+    def distribute_hero_cards(self, player_name, c1, c2):
+        """
+        Distribute hero cards
+        """
+        player = self.players[player_name]
+        self.set_hero(player)
+        player.distribute(f"{c1}{c2}")
+
     def set_bb_seat(self, player_seat: int):
         """
         Set the seat of the big blind player and redistribute positions
         """
         self.players.bb = player_seat
         if self.players.len > 1:
             self.players.distribute_positions()
@@ -376,15 +395,15 @@
     def pot_value(self):
         """Returns the pot's value"""
         return self.pot.value
 
     @property
     def pot_value_bb(self):
         """Returns the pot's value in big blinds"""
-        return self.pot_value/self.level.bb
+        return round(self.pot_value/self.level.bb, 2)
 
     @property
     def average_stack(self):
         """Returns the average stack of players on the table"""
         return sum(pl.init_stack for pl in self.players) / self.players.len
 
     @property
@@ -395,23 +414,29 @@
     @property
     def estimated_players_remaining(self):
         """Returns the estimated number of players remaining in the tournament"""
         return self.tournament.estimated_players_remaining(average_stack=self.average_stack)
 
     def advance_seat_playing(self):
         """Advances seat playing to next available player"""
-        player = self.current_player
-        while not player.can_play and self.nb_waiting > 0:
-            idx = self.playing_order.index(player.seat) + 1
-            try:
-                new_seat = self.playing_order[idx]
-            except IndexError:
-                new_seat = self.playing_order[0]
-            player = self.players[new_seat]
-        self._seat_playing = player.seat
+        self._seat_playing = self.next_seat
+        if not self.current_player.can_play and self.nb_waiting > 0:
+            self.advance_seat_playing()
+
+    @property
+    def next_player(self):
+        """ Returns the next player after the current player"""
+        current_player_index = self.players_order.index(self.current_player)
+        next_index = current_player_index + 1 if current_player_index < len(self.players_order) - 1 else 0
+        return self.players_order[next_index]
+
+    @property
+    def next_seat(self):
+        """ Returns the next seat to play after the current player"""
+        return self.next_player.seat
 
     def street_reset(self):
         """Reset status of players in game and betting status for a new street"""
         self.pot.highest_bet = 0
         self.cnt_bets = 0
         self._min_bet = self.level.bb
         self._seat_playing = self.players_in_game[0].seat
@@ -425,21 +450,28 @@
 
     @property
     def unrevealed_players(self) -> list:
         """Returns the list of players that have not revealed their cards"""
         return [pl for pl in self.players_involved if not pl.has_combo]
 
     @property
+    def nb_unrevealed(self) -> int:
+        """Returns the number of players that have not revealed their cards"""
+        return len(self.unrevealed_players)
+
+    @property
     def can_parse_winners(self) -> bool:
         """Returns True if the winners can be parsed"""
-        return self.hand_ended and len(self.unrevealed_players) == 0
+        return self.hand_ended and self.nb_unrevealed == 0 or self.nb_involved == 1
 
     @property
     def winners(self) -> dict[int, list]:
         """Current status of winners with associated scores"""
+        if not self.can_parse_winners:
+            raise ValueError("Winners can't be parsed yet")
         if self.nb_involved == 1:
             return {1: [self.players_involved[0]]}
         winners = {}
         for player in self.players_involved:
             pl_score = player.hand_score
             if not winners.get(pl_score):
                 winners[pl_score] = [player]
@@ -449,16 +481,14 @@
 
     def split_pot(self, players):
         """Split pot between players"""
         while len(players) > 0 and self.pot.value > 0:
             min_reward = min([pl.max_reward for pl in players])
             reward = min(min_reward, self.pot.value/len(players))
             for player in players:
-                if not hasattr(player, "reward"):
-                    player.reward = 0
                 player.reward += reward
                 if player.reward >= player.max_reward:
                     players.remove(player)
                     player.win(reward)
 
     def distribute_rewards(self):
         """Distribute rewards between players"""
```

### Comparing `pkrcomponents-1.8.1/pkrcomponents/table_player.py` & `pkrcomponents-2.0.0/pkrcomponents/table_player.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     def invested(self) -> float:
         """The total amount already invested by a player in pot"""
         return self.init_stack - self.stack
 
     @property
     def to_call(self) -> float:
         """The amount to call to continue on the table"""
-        return min(self.table.pot.highest_bet - self.current_bet, self.stack)
+        return self.max_bet(self.table.pot.highest_bet - self.current_bet)
 
     @property
     def to_call_bb(self):
         """The amount to call to continue on the table in big blinds"""
         return self.to_call / self.table.level.bb
 
     @property
@@ -245,14 +245,16 @@
     def shows(self, combo: (Combo, str)):
         """
         The player shows a combo at showdown
 
         Args:
             combo (Combo, str): The combo to show
         """
+        if self.table.street != Street.SHOWDOWN:
+            raise ValueError("Player cannot show combo if it is not showdown")
         self.combo = Combo(combo)
         if self.has_table:
             self.table.deck.draw(self.combo.first)
             self.table.deck.draw(self.combo.second)
 
     def delete_combo(self):
         """Deletes a player's combo"""
@@ -294,62 +296,14 @@
         self.current_bet += self.max_bet(value)
         self.pay(value)
         if self.current_bet > self.table.pot.highest_bet:
             self.table.pot.highest_bet = self.current_bet
             self.table.cnt_bets += 1
         self.played = True
 
-    def bet(self, value: float):
-        """
-        Bet and step to next player
-
-        Args:
-            value (float): The amount to bet
-        """
-        if value >= self.table.min_bet:
-            self.table.min_bet = 2*value - self.table.pot.highest_bet
-            self.do_bet(value)
-        elif self.table.min_bet > self.stack:
-            self.bet(self.table.min_bet)
-        else:
-            raise ValueError(f"You cannot bet {value} if the minimum bet is {self.table.min_bet} "
-                             f"and your stack is {self.stack}")
-        self.table.advance_seat_playing()
-
-    def do_call(self):
-        """Action of calling"""
-        self.do_bet(self.to_call)
-
-    def call(self):
-        """Call and step to next player"""
-        self.do_call()
-        self.table.advance_seat_playing()
-
-    def do_check(self):
-        """Action of checking"""
-        if self.to_call != 0:
-            raise ValueError("A player cannot check if somebody bet before")
-        else:
-            self.played = True
-
-    def check(self):
-        """Check and step to next player"""
-        self.do_check()
-        self.table.advance_seat_playing()
-
-    def do_fold(self):
-        """Action of folding"""
-        self.folded = True
-        self.played = True
-
-    def fold(self):
-        """Fold and step to next player"""
-        self.do_fold()
-        self.table.advance_seat_playing()
-
     def post(self, value: float):
         """
         Action of posting
 
         Args:
             value (float): The amount to post
         """
```

### Comparing `pkrcomponents-1.8.1/pkrcomponents/tournament.py` & `pkrcomponents-2.0.0/pkrcomponents/tournament.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from attrs import define, field, asdict, Factory
-from attrs.validators import instance_of,  ge, gt, le
+from attrs import define, field, Factory
+from attrs.validators import instance_of, gt
 
 from pkrcomponents.constants import MoneyType
 from pkrcomponents.level import Level
 from pkrcomponents.payout import Payouts
 from pkrcomponents.buy_in import BuyIn
 from pkrcomponents.utils.validators import validate_players_remaining
```

### Comparing `pkrcomponents-1.8.1/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-2.0.0/pkrcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.8.1/setup.py` & `pkrcomponents-2.0.0/setup.py`

 * *Files identical despite different names*

