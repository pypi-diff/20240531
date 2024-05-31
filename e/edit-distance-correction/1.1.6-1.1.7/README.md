# Comparing `tmp/edit_distance_correction-1.1.6-py3-none-any.whl.zip` & `tmp/edit_distance_correction-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,16 @@
-Zip file size: 19537 bytes, number of entries: 16
+Zip file size: 17134 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      139 b- defN 24-Feb-05 09:12 edit_distance_correction/__init__.py
 -rw-r--r--  2.0 unx     1256 b- defN 24-Feb-23 02:50 edit_distance_correction/correction.csv
--rw-r--r--  2.0 unx    11821 b- defN 24-Apr-12 07:13 edit_distance_correction/correction.py
--rw-r--r--  2.0 unx     9578 b- defN 24-Mar-19 02:11 edit_distance_correction/correction_copy.py
+-rw-r--r--  2.0 unx    11311 b- defN 24-May-31 07:19 edit_distance_correction/correction.py
 -rw-r--r--  2.0 unx     1089 b- defN 24-Feb-27 08:37 edit_distance_correction/heteronym.txt
--rw-r--r--  2.0 unx     6741 b- defN 24-Apr-16 05:36 edit_distance_correction/same_stroke.txt
--rw-r--r--  2.0 unx     1765 b- defN 24-Mar-25 11:40 edit_distance_correction/target_words
--rw-r--r--  2.0 unx      546 b- defN 24-Mar-05 08:16 edit_distance_correction/temp.py
+-rw-r--r--  2.0 unx     6801 b- defN 24-May-30 03:28 edit_distance_correction/same_stroke.txt
+-rw-r--r--  2.0 unx     1784 b- defN 24-May-30 05:59 edit_distance_correction/target_words
 -rw-r--r--  2.0 unx      391 b- defN 24-Mar-20 06:47 edit_distance_correction/test.py
--rw-r--r--  2.0 unx     2339 b- defN 24-Mar-25 11:40 edit_distance_correction/test_file
--rw-r--r--  2.0 unx     8819 b- defN 24-Mar-25 11:38 edit_distance_correction/utils.py
+-rw-r--r--  2.0 unx     2439 b- defN 24-May-30 06:55 edit_distance_correction/test_file
+-rw-r--r--  2.0 unx    11892 b- defN 24-May-30 09:34 edit_distance_correction/utils.py
 -rw-r--r--  2.0 unx     1676 b- defN 24-Jan-25 06:28 edit_distance_correction/valid_pinyin
--rw-r--r--  2.0 unx      291 b- defN 24-Apr-16 05:40 edit_distance_correction-1.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 05:40 edit_distance_correction-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 24-Apr-16 05:40 edit_distance_correction-1.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1486 b- defN 24-Apr-16 05:40 edit_distance_correction-1.1.6.dist-info/RECORD
-16 files, 48054 bytes uncompressed, 17029 bytes compressed:  64.6%
+-rw-r--r--  2.0 unx      291 b- defN 24-May-31 09:24 edit_distance_correction-1.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 09:24 edit_distance_correction-1.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 24-May-31 09:24 edit_distance_correction-1.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1299 b- defN 24-May-31 09:24 edit_distance_correction-1.1.7.dist-info/RECORD
+14 files, 40485 bytes uncompressed, 14928 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -3,47 +3,41 @@
 
 Filename: edit_distance_correction/correction.csv
 Comment: 
 
 Filename: edit_distance_correction/correction.py
 Comment: 
 
-Filename: edit_distance_correction/correction_copy.py
-Comment: 
-
 Filename: edit_distance_correction/heteronym.txt
 Comment: 
 
 Filename: edit_distance_correction/same_stroke.txt
 Comment: 
 
 Filename: edit_distance_correction/target_words
 Comment: 
 
-Filename: edit_distance_correction/temp.py
-Comment: 
-
 Filename: edit_distance_correction/test.py
 Comment: 
 
 Filename: edit_distance_correction/test_file
 Comment: 
 
 Filename: edit_distance_correction/utils.py
 Comment: 
 
 Filename: edit_distance_correction/valid_pinyin
 Comment: 
 
-Filename: edit_distance_correction-1.1.6.dist-info/METADATA
+Filename: edit_distance_correction-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: edit_distance_correction-1.1.6.dist-info/WHEEL
+Filename: edit_distance_correction-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: edit_distance_correction-1.1.6.dist-info/top_level.txt
+Filename: edit_distance_correction-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: edit_distance_correction-1.1.6.dist-info/RECORD
+Filename: edit_distance_correction-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edit_distance_correction/correction.py

```diff
@@ -8,24 +8,22 @@
 #import kenlm
 
 _get_module_path = lambda path: os.path.normpath(os.path.join(os.getcwd(),
                                                  os.path.dirname(__file__), path))
 class Corrector:
     def __init__(self):
         self.max_k = 0
-        #pinyin:set(word)
         self.pinyin_di = dict()
         self.target_word = dict()
-        #start:set(pinyin)
-        # self.start_pinyin_di = dict()
         self.start_word_di = dict()
         self.correction_dict = dict()
         self.original_dict = dict()
         self.same_stroke_dict = dict()
         self.same_stroke_head = set()
+        self.start_pinyin_di = dict()
         self.heteronym_dict = dict()
         self.gram = dict()
         self.lm = None
         self.valid_pinyin = set()
         self._load_correction()
         self._load_same_stroke()
         self._load_valid_pinyin()
@@ -61,33 +59,34 @@
                             if elem1 not in self.same_stroke_dict:
                                 self.same_stroke_dict[elem1] = set()
                             self.same_stroke_dict[elem1].add(elem2)
 
 
     def load_target_words(self, target_words):
         for word in target_words:
+            if len(word.strip()) == 0: continue
             #word = word.lower()
             if len(word) > self.max_k:
                 self.max_k = len(word)
             all_res = utils.get_pinyin(word, "all", True, self.heteronym_dict)
             for res in all_res:
                 if res["pinyin"] not in self.pinyin_di:
                     self.pinyin_di[res["pinyin"]] = set()
                 self.pinyin_di[res["pinyin"]].add(word)
-                # if re.match('^[\u4e00-\u9fa5]+$', word) is not None:
-                #     if res["start"] not in self.start_pinyin_di:
-                #         self.start_pinyin_di[res["start"]] = set()
-                #     self.start_pinyin_di[res["start"]].add(res["pinyin"])
                 if re.match('^[\u4e00-\u9fa5]+$', word) is not None:
                     if res["start"] not in self.start_word_di:
                         self.start_word_di[res["start"]] = set()
                     self.start_word_di[res["start"]].add(word)
                 if word not in self.target_word:
                     self.target_word[word] = set()
                 self.target_word[word].add(res["pinyin"])
+                for pinyin_comb in res["pinyin_comb"]:
+                    if pinyin_comb not in self.start_pinyin_di:
+                        self.start_pinyin_di[pinyin_comb] = set()
+                    self.start_pinyin_di[pinyin_comb].add(word)
             if len(word) > 0:
                 self.same_stroke_head.add(word[0])
 
             for i in range(len(word)):
                 if word[i] not in self.gram:
                     self.gram[word[i]] = set()
                 if i == len(word) - 1:
@@ -142,15 +141,14 @@
         res = []
         end = len(word_list)
         while end > 0:
             break_flag = False
             for i in range(max_k):
                 start = end - max_k + i
                 if start < 0: continue
-                # temp = "".join(word_list[start:end])
                 temps = utils.get_all_list(word_list[start:end])
                 for temp in temps:
                     temp = "".join(temp)
                     if temp in vocab:
                         res.append([temp, start, end])
                         break_flag = True
                 if break_flag:
@@ -158,41 +156,38 @@
             if not break_flag:
                 end -= 1
         res.reverse()
         return res
 
 
     def recall_word(self, query):
-        #temp_cuts = jieba.lcut(query)
         temp_cuts = utils.cut(query)
         cuts = []
         for cut in temp_cuts:
             if re.search("^[a-zA-Z]+$", cut) is not None:
                 res = utils.pinyin_split(cut, self.valid_pinyin)
                 if res is None:
                     cuts.append(cut)
                 else:
                     cuts.extend(res)
             else:
                 cuts.append(cut)
+        print(cuts)
         cuts_stroke = utils.get_stroke_replace(cuts, self.gram, self.same_stroke_dict, self.same_stroke_head)
-        #cuts_stroke = utils.get_all_list(cuts_stroke)
-        #print(len(cuts_stroke))
-
         query_pinyin, query_start_pinyin, query_pinyin_list = "", "", []
         for cut in cuts:
             qp = utils.get_pinyin(cut, mode="pinyin")
             query_pinyin_list.append(qp)
         res, second_res = self.max_backward_match_transform(query_pinyin_list, self.pinyin_di, max_k=self.max_k * 5)
         jianpin_res = utils.max_backward_match(cuts, self.start_word_di, max_k=1)
-        #stroke_res = [utils.max_backward_match(elem, self.target_word, max_k=10) for elem in cuts_stroke]
-        #stroke_res = list(chain(*stroke_res))
-        #todo:这里找到一个直接返回，实际上最好收集所有可能再比较最好的
+        print(cuts, self.start_word_di)
+        print(jianpin_res)
         stroke_res = self.max_backward_match_list(cuts, cuts_stroke, self.target_word, max_k=self.max_k)
         stroke_res = utils.combine_same_position(stroke_res)
+        jianpin_pinyin_res = utils.max_backward_match(cuts, self.start_pinyin_di, max_k=1)
         first_pinyin_r = []
         second_pinyin_r = []
         for elem in res:
             original = "".join(cuts[elem[1]:elem[2]])
             pinyin = "".join(query_pinyin_list[elem[1]:elem[2]])
             candidates = []
             for word in self.pinyin_di.get(pinyin, []):
@@ -227,51 +222,48 @@
                         break
             candidates = candidates[:i]
             if len(candidates) > 0:
                 second_pinyin_r.append([elem[1], elem[2], [word[0] for word in candidates]])
         jianpin_r = []
         for elem in jianpin_res:
             jianpin_r.append([elem[1], elem[2], self.start_word_di[elem[0]]])
-            # for e in self.start_word_di[elem[0]]:
-            #     jianpin_r.append([e, 0, elem[1], elem[2]])
-
+        jianpin_pinyin_r = []
+        for elem in jianpin_pinyin_res:
+            jianpin_pinyin_r.append([elem[1], elem[2], self.start_pinyin_di[elem[0]]])
         stroke_r = []
         for elem in stroke_res:
             start, end = elem[0], elem[1]
             original = query[start : end]
             candidates = []
             for correct in elem[2]:
-                #correct_pinyin = self.target_word[correct]
                 correct_pinyins = self.target_word[correct]
                 original_pinyin = utils.get_pinyin(original, mode="pinyin")
                 candidates.append([correct, Levenshtein.distance(correct, original) + min(
                     [Levenshtein.distance(correct_pinyin, original_pinyin) for correct_pinyin in correct_pinyins])])
-                # stroke_r.append([correct, Levenshtein.distance(correct, original) + min(
-                #     [Levenshtein.distance(correct_pinyin, original_pinyin) for correct_pinyin in correct_pinyins]),
-                #                  elem[1],
-                #                  elem[2]])
             candidates = list(filter(lambda x: x[0] != original, candidates))
             candidates = sorted(candidates, key=lambda x: x[1])
             i = len(candidates)
             if len(candidates) > 1:
                 for ii in range(1, len(candidates)):
                     if candidates[ii][1] > candidates[0][1]:
                         i = ii
                         break
             candidates = candidates[:i]
             if len(candidates) > 0:
                 stroke_r.append([start, end, [word[0] for word in candidates]])
 
         all_candidates = utils.check_conflict(first_pinyin_r, second_pinyin_r)
         all_candidates = utils.check_conflict(all_candidates, jianpin_r)
+        all_candidates = utils.check_conflict(all_candidates, jianpin_pinyin_r)
         all_candidates = utils.check_conflict(all_candidates, stroke_r)
 
         #all_candidates = list(filter(lambda x: x[0] != "".join(cuts[x[2]: x[3]]), all_candidates))
         res = utils.get_correct(all_candidates, cuts)
-        #暂时取第一个，实际可以算分比较
+        #todo:暂时取第一个，实际可以算分比较
+        print(res)
         res = res[0]
         return res
```

## edit_distance_correction/same_stroke.txt

```diff
@@ -341,8 +341,18 @@
 帅	师
 大	犬	夫	天
 固	涸
 格	恪
 檫	擦
 著	着	者
 （ (
-) ）
+) ）
+0 零
+1 一
+2 二
+3 三
+4 四
+5 五
+6 六
+7 七
+8 八
+9 九
```

## edit_distance_correction/target_words

```diff
@@ -1,10 +1,11 @@
 话费
 化肥
 充话费
+
 牛人
 六人行
 电脑
 长度
 最好
 贵州茅台
 卡费
@@ -128,8 +129,10 @@
 直销
 直销银行
 保险（分红型）
 华润信托悦财宝21号
 东吴新产业精选b
 红塔证券
 孩童证券
+360
+七七四十9
```

## edit_distance_correction/test_file

```diff
@@ -74,7 +74,20 @@
 东吴新产业精选b
 东吴新产业精选B
 冻吴新产业精选A国信安泰中短债A华润信托悦财宝21号财通够策略福鑫华安MSCI中国A役指数增强保险（分红刑）冻吴新产业精选A国信安泰中短债A华润信托悦财宝21号财通够策略福鑫华安MSCI中国A役指数增强保险（分红刑）
 冻吴新产业精选A国信安泰中短债a华润信托悦财宝21号责通够策略副鑫华安MSCI中国
 咖啡贵州maotai
 gzmt
 gzmt华妃swerwjrjweewjweqj害同振券
+haitongzq
+haitzq
+haitzhengq
+360
+三六零
+三60
+三六0
+774十9
+gzmttt
+gzmtp
+dgzmt
+gzmtai
+gzmt我tai
```

## edit_distance_correction/utils.py

```diff
@@ -52,14 +52,40 @@
         for line in f:
             line = line.strip()
             if use_list: res.append(line)
             else: res.add(line)
     return res
 
 
+def _pinyin_check(word_list, start, end):
+    if (start == 0 or re.match("[a-zA-Z]", word_list[start-1]) is False) and (end == len(word_list) or re.match("[a-zA-Z]", word_list[end]) is False):
+        return True
+    return False
+
+
+# def max_backward_match(word_list, vocab, max_k=10, no_pinyin_check=True):
+#     res = []
+#     end = len(word_list)
+#     while end > 0:
+#         break_flag = False
+#         for i in range(max_k):
+#             start = end - max_k + i
+#             if start < 0: continue
+#             temp = "".join(word_list[start:end])
+#             if temp in vocab and (no_pinyin_check or _pinyin_check(word_list, start, end)):
+#                 res.append([temp, start, end])
+#                 end = start
+#                 break_flag = True
+#                 break
+#         if not break_flag:
+#             end -= 1
+#     res.reverse()
+#     return res
+
+
 #最大后向匹配
 def max_backward_match(word_list, vocab, max_k=10):
     res = []
     end = len(word_list)
     while end > 0:
         break_flag = False
         for i in range(max_k):
@@ -190,14 +216,49 @@
             temp = set(original).union(heteronym_dict.get(ch, set()))
             li.append(list(temp).copy())
         else:
             li.append([ch])
     return li
 
 
+# def get_pinyin(word, mode="all", heteronym=False, heteronym_dict=None):
+#     if heteronym:
+#         if heteronym_dict is None:
+#             li = list(itertools.product(*pinyin(word.lower(), heteronym=heteronym, style=pypinyin.NORMAL)))
+#         else:
+#             li = list(itertools.product(*_heteronym_pinyin(word.lower(), heteronym_dict)))
+#         heteronym_res = []
+#         for one in li:
+#             if mode == "pinyin_list":
+#                 heteronym_res.append([elem for elem in one])
+#             elif mode == "pinyin":
+#                 heteronym_res.append("".join([elem for elem in one]))
+#             elif mode == "start":
+#                 heteronym_res.append("".join([elem[0] for elem in one]))
+#             else:
+#                 res = dict()
+#                 res["pinyin_list"] = [elem for elem in one]
+#                 res["pinyin"] = "".join(res["pinyin_list"])
+#                 res["start"] = "".join([elem[0] for elem in one])
+#                 heteronym_res.append(res.copy())
+#         return heteronym_res
+#     word_pinyin = pypinyin.pinyin(word.lower(), style=pypinyin.NORMAL)
+#     if mode == "pinyin_list":
+#         return [elem[0] for elem in word_pinyin]
+#     elif mode == "pinyin":
+#         return "".join([elem[0] for elem in word_pinyin])
+#     elif mode == "start":
+#         return "".join([elem[0][0] for elem in word_pinyin])
+#     res = dict()
+#     res["pinyin_list"] = [elem[0] for elem in word_pinyin]
+#     res["pinyin"] = "".join(res["pinyin_list"])
+#     res["start"] = "".join([elem[0][0] for elem in word_pinyin])
+#     return res
+
+
 def get_pinyin(word, mode="all", heteronym=False, heteronym_dict=None):
     if heteronym:
         if heteronym_dict is None:
             li = list(itertools.product(*pinyin(word.lower(), heteronym=heteronym, style=pypinyin.NORMAL)))
         else:
             li = list(itertools.product(*_heteronym_pinyin(word.lower(), heteronym_dict)))
         heteronym_res = []
@@ -209,30 +270,35 @@
             elif mode == "start":
                 heteronym_res.append("".join([elem[0] for elem in one]))
             else:
                 res = dict()
                 res["pinyin_list"] = [elem for elem in one]
                 res["pinyin"] = "".join(res["pinyin_list"])
                 res["start"] = "".join([elem[0] for elem in one])
+                #res["pinyin_comb"] = ["".join(res["pinyin_list"][:i]) + "".join([elem[0] for elem in one][i:]) for i in range(1, len(res["pinyin_list"]))]
+                res["pinyin_comb"] = ["".join(e) for e in get_all_list([list(set([elem, elem[0]])) for elem in one])]
                 heteronym_res.append(res.copy())
+
         return heteronym_res
     word_pinyin = pypinyin.pinyin(word.lower(), style=pypinyin.NORMAL)
     if mode == "pinyin_list":
         return [elem[0] for elem in word_pinyin]
     elif mode == "pinyin":
         return "".join([elem[0] for elem in word_pinyin])
     elif mode == "start":
         return "".join([elem[0][0] for elem in word_pinyin])
     res = dict()
     res["pinyin_list"] = [elem[0] for elem in word_pinyin]
     res["pinyin"] = "".join(res["pinyin_list"])
     res["start"] = "".join([elem[0][0] for elem in word_pinyin])
+    # res["pinyin_comb"] = ["".join([elem[0] for elem in word_pinyin][:i]) + "".join([elem[0][0] for elem in word_pinyin][i:]) for i in
+    #                       range(1, len(word_pinyin))]
+    res["pinyin_comb"] = ["".join(e) for e in get_all_list([list(set([elem[0][0], elem[0]])) for elem in word_pinyin])]
     return res
 
-
 #长串拼音分割，多种路径
 def pinyin_split(pinyin, valid_pinyin):
     res = []
     def split_helper(pinyin, pos, before_res):
         if pos >= len(pinyin):
             res.append(before_res)
         for i in range(pos, len(pinyin)+1):
```

## Comparing `edit_distance_correction-1.1.6.dist-info/RECORD` & `edit_distance_correction-1.1.7.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 edit_distance_correction/__init__.py,sha256=iEwR-MyXazzbaotC3qWLZykxG-cA4hyVlazXyWsxR2c,139
 edit_distance_correction/correction.csv,sha256=Z15Pkoxu0BqTse-b0Vx6p8VhDVRi_2ct3NjCB84OuTA,1256
-edit_distance_correction/correction.py,sha256=TgZ1nFHfFaMsCHD3KgyactBSefzxLBkV4tK1XdAHyAk,11821
-edit_distance_correction/correction_copy.py,sha256=uKZjntYbrVUc695RAZMId4lnnjgihl4Vg1_c-NhvIL8,9578
+edit_distance_correction/correction.py,sha256=4IXAoGC1YKuQM-4lMOrhZpZDza21Fw3krTQdJb-C6zc,11311
 edit_distance_correction/heteronym.txt,sha256=-cGHvlDxqZm9QuTUEClUx7kLDETYZaNGc8QhJqV1kyI,1089
-edit_distance_correction/same_stroke.txt,sha256=rOrgIlpqY-WJzUitqlzcDp5ei04RkyUPOIfxIC2fWM0,6741
-edit_distance_correction/target_words,sha256=BOmPlH8n0A7xsaD8S0n9f3JCzN7nm9IHMtRJltiu1XI,1765
-edit_distance_correction/temp.py,sha256=s35J407s6ap1dkWg0AKmeL_nLM059RwcwAR-GZqcOEw,546
+edit_distance_correction/same_stroke.txt,sha256=62B02Q62AJywUlQKmWwilF6j3BdCLBGd3uQXn3ChNXI,6801
+edit_distance_correction/target_words,sha256=_0stRwUiMqck-ByqC7-j-r-vaK03IzAk8gO1ur7N5QY,1784
 edit_distance_correction/test.py,sha256=oG_UfMwTOEBAFlLD_N7CJzmDwvNibktFNaDR1dcR0m0,391
-edit_distance_correction/test_file,sha256=_XlLhGNIFbjfQKmkkVmCIHl-izGjhGOXUUnsLbJTy6A,2339
-edit_distance_correction/utils.py,sha256=XtywpJdMVp_50kfMyqhEYo5UBhXk3E-3HejnfICCLPc,8819
+edit_distance_correction/test_file,sha256=f5Tf3POgV9F1YldCWF1ni1PHxARsZaKb2W38Xr7AGZs,2439
+edit_distance_correction/utils.py,sha256=dYZMbUigeCuKP5Try58HS8x19FubYTrKdqxnfiIMT6E,11892
 edit_distance_correction/valid_pinyin,sha256=6EqB5E8P3jAIukFOBvQtagZ4DCqQCjemjwo2bykSpJc,1676
-edit_distance_correction-1.1.6.dist-info/METADATA,sha256=3_NLo-DN9FU3oK8Bd21Vy79-9vLd5OAXCMervqaZoqE,291
-edit_distance_correction-1.1.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-edit_distance_correction-1.1.6.dist-info/top_level.txt,sha256=GzUwTYJvGTyxnBCc_IqRXlNzEQr5gg0oQ96jXfgwu2s,25
-edit_distance_correction-1.1.6.dist-info/RECORD,,
+edit_distance_correction-1.1.7.dist-info/METADATA,sha256=B6htWFp0QOCmMDtFA2vFdVgljqhpqlo_kpR44LGwb7w,291
+edit_distance_correction-1.1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+edit_distance_correction-1.1.7.dist-info/top_level.txt,sha256=GzUwTYJvGTyxnBCc_IqRXlNzEQr5gg0oQ96jXfgwu2s,25
+edit_distance_correction-1.1.7.dist-info/RECORD,,
```

