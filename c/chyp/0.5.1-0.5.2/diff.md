# Comparing `tmp/chyp-0.5.1.tar.gz` & `tmp/chyp-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyp-0.5.1.tar", last modified: Wed May 31 16:16:07 2023, max compression
+gzip compressed data, was "chyp-0.5.2.tar", last modified: Sun Jun  4 15:44:54 2023, max compression
```

## Comparing `chyp-0.5.1.tar` & `chyp-0.5.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:16:07.586484 chyp-0.5.1/
--rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.5.1/LICENSE
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    16188 2023-05-31 16:16:07.586484 chyp-0.5.1/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    15651 2023-05-24 08:31:14.000000 chyp-0.5.1/README.md
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:16:07.582484 chyp-0.5.1/chyp/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      653 2023-05-22 22:21:15.000000 chyp-0.5.1/chyp/__init__.py
--rw-r--r--   0 aleger    (1000) aleger    (1000)      715 2023-05-22 22:21:24.000000 chyp-0.5.1/chyp/__main__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    17564 2023-05-31 13:33:25.000000 chyp-0.5.1/chyp/graph.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:16:07.586484 chyp-0.5.1/chyp/gui/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      651 2023-05-22 22:23:21.000000 chyp-0.5.1/chyp/gui/__init__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2537 2023-05-22 22:22:46.000000 chyp-0.5.1/chyp/gui/app.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4911 2023-05-22 22:22:48.000000 chyp-0.5.1/chyp/gui/codeview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4824 2023-05-22 22:20:22.000000 chyp-0.5.1/chyp/gui/colors.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2060 2023-05-22 22:22:54.000000 chyp-0.5.1/chyp/gui/completion.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4774 2023-05-22 22:23:00.000000 chyp-0.5.1/chyp/gui/document.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    11344 2023-05-31 12:57:08.000000 chyp-0.5.1/chyp/gui/editor.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3285 2023-05-22 22:23:06.000000 chyp-0.5.1/chyp/gui/errorlist.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     8146 2023-05-31 13:34:32.000000 chyp-0.5.1/chyp/gui/graphscene.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1281 2023-05-29 12:07:27.000000 chyp-0.5.1/chyp/gui/graphview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3307 2023-05-24 08:35:35.000000 chyp-0.5.1/chyp/gui/highlighter.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    13424 2023-05-22 22:23:18.000000 chyp-0.5.1/chyp/gui/mainwindow.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    10786 2023-05-23 21:40:13.000000 chyp-0.5.1/chyp/layout.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    11350 2023-05-22 22:20:49.000000 chyp-0.5.1/chyp/matcher.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    16896 2023-05-31 13:47:17.000000 chyp-0.5.1/chyp/parser.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3804 2023-05-22 22:21:44.000000 chyp-0.5.1/chyp/rewrite.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1806 2023-05-31 13:58:50.000000 chyp-0.5.1/chyp/rule.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.5.1/chyp/scraps.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     5504 2023-05-31 14:43:38.000000 chyp-0.5.1/chyp/state.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:16:07.586484 chyp-0.5.1/chyp/tactic/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     6140 2023-05-31 14:22:39.000000 chyp-0.5.1/chyp/tactic/__init__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1678 2023-05-31 13:45:24.000000 chyp-0.5.1/chyp/tactic/ruletac.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1551 2023-05-31 14:54:32.000000 chyp-0.5.1/chyp/tactic/simptac.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     6018 2023-05-23 23:17:32.000000 chyp-0.5.1/chyp/term.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:16:07.582484 chyp-0.5.1/chyp.egg-info/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    16188 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      700 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/SOURCES.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/dependency_links.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/entry_points.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/requires.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/top_level.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.5.1/pyproject.toml
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-31 16:16:07.586484 chyp-0.5.1/setup.cfg
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1076 2023-05-31 16:15:09.000000 chyp-0.5.1/setup.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-06-04 15:44:54.159491 chyp-0.5.2/
+-rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.5.2/LICENSE
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    20269 2023-06-04 15:44:54.159491 chyp-0.5.2/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    19732 2023-06-04 13:35:16.000000 chyp-0.5.2/README.md
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-06-04 15:44:54.155491 chyp-0.5.2/chyp/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      653 2023-05-22 22:21:15.000000 chyp-0.5.2/chyp/__init__.py
+-rw-r--r--   0 aleger    (1000) aleger    (1000)      715 2023-05-22 22:21:24.000000 chyp-0.5.2/chyp/__main__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    17564 2023-05-31 13:33:25.000000 chyp-0.5.2/chyp/graph.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-06-04 15:44:54.159491 chyp-0.5.2/chyp/gui/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      651 2023-05-22 22:23:21.000000 chyp-0.5.2/chyp/gui/__init__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2495 2023-06-03 17:49:15.000000 chyp-0.5.2/chyp/gui/app.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4812 2023-06-03 11:00:02.000000 chyp-0.5.2/chyp/gui/codeview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4824 2023-05-22 22:20:22.000000 chyp-0.5.2/chyp/gui/colors.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2060 2023-05-22 22:22:54.000000 chyp-0.5.2/chyp/gui/completion.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     5667 2023-06-03 11:34:02.000000 chyp-0.5.2/chyp/gui/document.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11824 2023-06-03 17:52:48.000000 chyp-0.5.2/chyp/gui/editor.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3285 2023-06-03 11:46:51.000000 chyp-0.5.2/chyp/gui/errorlist.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     8146 2023-05-31 13:34:32.000000 chyp-0.5.2/chyp/gui/graphscene.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1281 2023-05-29 12:07:27.000000 chyp-0.5.2/chyp/gui/graphview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3340 2023-06-02 20:02:50.000000 chyp-0.5.2/chyp/gui/highlighter.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    13816 2023-06-04 08:43:52.000000 chyp-0.5.2/chyp/gui/mainwindow.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10786 2023-05-23 21:40:13.000000 chyp-0.5.2/chyp/layout.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11350 2023-05-22 22:20:49.000000 chyp-0.5.2/chyp/matcher.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4317 2023-06-01 12:49:29.000000 chyp-0.5.2/chyp/parser.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3804 2023-05-22 22:21:44.000000 chyp-0.5.2/chyp/rewrite.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1806 2023-05-31 13:58:50.000000 chyp-0.5.2/chyp/rule.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.5.2/chyp/scraps.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    17091 2023-06-04 12:46:13.000000 chyp-0.5.2/chyp/state.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-06-04 15:44:54.159491 chyp-0.5.2/chyp/tactic/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11490 2023-06-04 13:06:07.000000 chyp-0.5.2/chyp/tactic/__init__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1678 2023-05-31 13:45:24.000000 chyp-0.5.2/chyp/tactic/ruletac.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1765 2023-06-04 13:21:30.000000 chyp-0.5.2/chyp/tactic/simptac.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     6018 2023-05-23 23:17:32.000000 chyp-0.5.2/chyp/term.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-06-04 15:44:54.155491 chyp-0.5.2/chyp.egg-info/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    20269 2023-06-04 15:44:54.000000 chyp-0.5.2/chyp.egg-info/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      700 2023-06-04 15:44:54.000000 chyp-0.5.2/chyp.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-06-04 15:44:54.000000 chyp-0.5.2/chyp.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-06-04 15:44:54.000000 chyp-0.5.2/chyp.egg-info/entry_points.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-06-04 15:44:54.000000 chyp-0.5.2/chyp.egg-info/requires.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-06-04 15:44:54.000000 chyp-0.5.2/chyp.egg-info/top_level.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.5.2/pyproject.toml
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-06-04 15:44:54.159491 chyp-0.5.2/setup.cfg
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1076 2023-06-04 15:44:14.000000 chyp-0.5.2/setup.py
```

### Comparing `chyp-0.5.1/LICENSE` & `chyp-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/PKG-INFO` & `chyp-0.5.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.5.1
+Version: 0.5.2
 Summary: An interactive theorem prover for string diagrams
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
@@ -130,21 +130,15 @@
     rewrite ba1_backwards :
       g * f ; id * id * g ; id * sw * id ; f * f ; g * id
       = id * f ; f ; g ; g * id by -bialg
       = f * id ; f ; g ; g * id by -assoc
 
 The golden rule of Chyp is that _only connectivity matters_. So, if two terms give the same diagram, like `a * b ; c * d` and `(a ; c) * (b ; d)`, Chyp treats them as identical. Since under the hood, Chyp does everything with graph rewriting and not term rewriting, the prover handles all of this extra book-keeping for you.
 
-Sometimes it can be helpful for readability to do a trivial proof step that does nothing but write the same string diagram differently. There is a special rule called `refl` (for reflexivity) for this. For example:
-
-    rewrite foo :
-      a * b ; c * d
-      = (a ; c) * (b ; d) by refl
-
-Formally, `refl` is defined as `id0 = id0`, i.e. the empty graph equals itself, which always matches exactly once on any graph. If we drop the `by` clause, Chyp automatically assumes `by refl`, so the following is equivalent:
+Sometimes it can be helpful for readability to do a trivial proof step that does nothing but write the same string diagram differently. We can do this just by dropping the `by` clause in a proof step:
 
     rewrite foo :
       a * b ; c * d
       = (a ; c) * (b ; d)
 
 
 The `def` statement introduced in the previous section is just syntactic sugar for a `gen` followed by a rule. That is:
@@ -184,14 +178,82 @@
       = g * f ; id * id * g ; id * sw * id ; f * f ; id * g by bialg
       = g * g * g ; id * id * id * sw * id ; id * id * f * f ; id * sw * id ; f * f ; id * g by bialg
       = g * g * g ; id * id * id * sw * id ; id * g * f * f ; sw * sw * id ; id * f * id * g ; sw * sw * id ; id * f * f by bialg
       = g * g * g ; id * id * id * sw * id ; id * g * f * g * g ; sw * sw * id * sw * id ; id * f * id * f * f ; sw * sw * id ; id * f * f by bialg
 
 How to we know it's a normal form? Pressing `CTRL+SHIFT+Enter` one more time will result in a red line that reads `  = ? by bialg`, which means Chyp wasn't able to find any more matchings of the `bialg` rule.
 
+## Tactics
+
+Tactics are the bread and butter of interactive theorem provers. These are routines that can be called to try to solve a given goal. In Chyp, a goal corresponds to a single proof step `LHS = RHS`. Chyp has three built in tactics: `refl`, `rule`, and `simp`. If you've been following along, you've actually been using the first two already.
+
+`refl`, which stands for "reflexivity of `=`", simply tries to prove `LHS` and `RHS` represent the same diagram, i.e. they are isomorphic cospans of hypergraphs. When you write a rewrite step without providing a rule, it is actually shorthand for applying the `refl` tactic. For example:
+
+    rewrite foo :
+      a * b ; c * d
+      = (a ; c) * (b ; d)
+
+is actually shorthand for:
+
+    rewrite foo :
+      a * b ; c * d
+      = (a ; c) * (b ; d) by refl()
+
+Note the parentheses tell Chyp that this is a tactic and not a rule name. They are empty because `refl` takes zero arguments.
+
+The `rule` tactic applies the given rewrite rule to the `LHS` in every possible way until it produces `RHS` (or fails). Most of the rewrites we have done so far have used the rule tactic, which can be applied either explicitly or implicitly just by giving a rule name. Namely, for a rule `R`, writing:
+
+    rewrite foo : lhs = rhs by R
+
+is actually shorthand for:
+
+    rewrite foo : lhs = rhs by rule(R)
+
+
+Finally, the `simp` tactic applies a list of given rules as much as possible to both the `LHS` and `RHS` then compares the resulting diagrams. It could be the case that the given set of rules is non-terminating (i.e. they can be applied forever without reaching a normal form), in which case `simp` gives up after 256 rule applications.
+
+This can be very useful if the set of rules provided actually yields unique normal forms, or in rewriting lingo the rules are [confluent and terminating](https://en.wikipedia.org/wiki/Rewriting). For example, the monoid laws:
+
+    gen u : 0 -> 1
+    gen m : 2 -> 1
+    rule unitL : u * id ; m = id
+    rule unitR : id * u ; m = id
+    rule assoc : m * id ; m = id * m ; m
+    
+always yield unique normal forms. So, we can prove any true equation involving a monoid in a single step using `simp`, e.g.
+
+    rewrite random_monoid_eq :
+      id * u * u * id ; m * m ; m
+      = id * u * id ; id * m ; m by simp(unitL, unitR, assoc)
+
+However, the beauty of interactive theorem provers is that sets of rules don't actually have to be that nice to benefit from automated tactics like `simp`, as long as they get a bit of help from a human when they get stuck.
+
+One more thing worth mentioning is the simplifier automatically unfolds definitions, i.e. any rule ending in `_def`, both to the term being simplified and in the LHS of all of the rules given. So something like this will also work:
+
+    def m2 = id * sw * id ; m * m
+    rewrite another_monoid_eq :
+      u * u * u * u ; m2
+      = u * u by simp(unitL)
+
+If you don't want this behaviour, you can pass the `+nodefs` flag as an argument to `simp`:
+
+    def m2 = id * sw * id ; m * m
+
+    rewrite another_monoid_eq1 :
+      u * u * u * u ; m2
+      = u * u by simp(+nodefs, unitL) # fails
+
+    rewrite another_monoid_eq2 :
+      u * u * u * u ; m2
+      = u * u by simp(+nodefs, m2_def, unitL) # succeeds again
+
+
+These three tactics are all implemented in the `chyp.tactic` module. [Tactic](https://github.com/akissinger/chyp/blob/master/chyp/tactic/__init__.py) implements `refl`, and the other tactics are implemented as subclasses of `Tactic` that should override the `check` method, which tries to close the current goal, and the `make_rhs` method, which returns an iterator over possible terms to fill in a hole `?`. Thanks to the API exposed by `Tactic`, the two tactics [RuleTac](https://github.com/akissinger/chyp/blob/master/chyp/tactic/ruletac.py) and [SimpTac](https://github.com/akissinger/chyp/blob/master/chyp/tactic/simptac.py) are very simple, and it shouldn't be too hard to implement more.
+
+In theory, if tactics only interact with the current goal via the public methods exposed by `Tactic`, it shouldn't be possible to prove anything that is not true. While this doesn't provide strong guarantees of soundness, like in the case of [LCF](https://en.wikipedia.org/wiki/Logic_for_Computable_Functions)-style theorem provers, it does attempt to provide some degree of assurance that (possibly very complex) tactics won't prove untrue statements.
 
 # Modules and importing
 
 As structures and proofs get more complicated, we may want to split them into multiple files. Every chyp file defines a module, which can be imported in other chyp files. Suppose for example we define the following file `monoid.chyp`:
 
     gen m : 2 -> 1
     gen u : 0 -> 1
```

### Comparing `chyp-0.5.1/README.md` & `chyp-0.5.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -114,21 +114,15 @@
     rewrite ba1_backwards :
       g * f ; id * id * g ; id * sw * id ; f * f ; g * id
       = id * f ; f ; g ; g * id by -bialg
       = f * id ; f ; g ; g * id by -assoc
 
 The golden rule of Chyp is that _only connectivity matters_. So, if two terms give the same diagram, like `a * b ; c * d` and `(a ; c) * (b ; d)`, Chyp treats them as identical. Since under the hood, Chyp does everything with graph rewriting and not term rewriting, the prover handles all of this extra book-keeping for you.
 
-Sometimes it can be helpful for readability to do a trivial proof step that does nothing but write the same string diagram differently. There is a special rule called `refl` (for reflexivity) for this. For example:
-
-    rewrite foo :
-      a * b ; c * d
-      = (a ; c) * (b ; d) by refl
-
-Formally, `refl` is defined as `id0 = id0`, i.e. the empty graph equals itself, which always matches exactly once on any graph. If we drop the `by` clause, Chyp automatically assumes `by refl`, so the following is equivalent:
+Sometimes it can be helpful for readability to do a trivial proof step that does nothing but write the same string diagram differently. We can do this just by dropping the `by` clause in a proof step:
 
     rewrite foo :
       a * b ; c * d
       = (a ; c) * (b ; d)
 
 
 The `def` statement introduced in the previous section is just syntactic sugar for a `gen` followed by a rule. That is:
@@ -168,14 +162,82 @@
       = g * f ; id * id * g ; id * sw * id ; f * f ; id * g by bialg
       = g * g * g ; id * id * id * sw * id ; id * id * f * f ; id * sw * id ; f * f ; id * g by bialg
       = g * g * g ; id * id * id * sw * id ; id * g * f * f ; sw * sw * id ; id * f * id * g ; sw * sw * id ; id * f * f by bialg
       = g * g * g ; id * id * id * sw * id ; id * g * f * g * g ; sw * sw * id * sw * id ; id * f * id * f * f ; sw * sw * id ; id * f * f by bialg
 
 How to we know it's a normal form? Pressing `CTRL+SHIFT+Enter` one more time will result in a red line that reads `  = ? by bialg`, which means Chyp wasn't able to find any more matchings of the `bialg` rule.
 
+## Tactics
+
+Tactics are the bread and butter of interactive theorem provers. These are routines that can be called to try to solve a given goal. In Chyp, a goal corresponds to a single proof step `LHS = RHS`. Chyp has three built in tactics: `refl`, `rule`, and `simp`. If you've been following along, you've actually been using the first two already.
+
+`refl`, which stands for "reflexivity of `=`", simply tries to prove `LHS` and `RHS` represent the same diagram, i.e. they are isomorphic cospans of hypergraphs. When you write a rewrite step without providing a rule, it is actually shorthand for applying the `refl` tactic. For example:
+
+    rewrite foo :
+      a * b ; c * d
+      = (a ; c) * (b ; d)
+
+is actually shorthand for:
+
+    rewrite foo :
+      a * b ; c * d
+      = (a ; c) * (b ; d) by refl()
+
+Note the parentheses tell Chyp that this is a tactic and not a rule name. They are empty because `refl` takes zero arguments.
+
+The `rule` tactic applies the given rewrite rule to the `LHS` in every possible way until it produces `RHS` (or fails). Most of the rewrites we have done so far have used the rule tactic, which can be applied either explicitly or implicitly just by giving a rule name. Namely, for a rule `R`, writing:
+
+    rewrite foo : lhs = rhs by R
+
+is actually shorthand for:
+
+    rewrite foo : lhs = rhs by rule(R)
+
+
+Finally, the `simp` tactic applies a list of given rules as much as possible to both the `LHS` and `RHS` then compares the resulting diagrams. It could be the case that the given set of rules is non-terminating (i.e. they can be applied forever without reaching a normal form), in which case `simp` gives up after 256 rule applications.
+
+This can be very useful if the set of rules provided actually yields unique normal forms, or in rewriting lingo the rules are [confluent and terminating](https://en.wikipedia.org/wiki/Rewriting). For example, the monoid laws:
+
+    gen u : 0 -> 1
+    gen m : 2 -> 1
+    rule unitL : u * id ; m = id
+    rule unitR : id * u ; m = id
+    rule assoc : m * id ; m = id * m ; m
+    
+always yield unique normal forms. So, we can prove any true equation involving a monoid in a single step using `simp`, e.g.
+
+    rewrite random_monoid_eq :
+      id * u * u * id ; m * m ; m
+      = id * u * id ; id * m ; m by simp(unitL, unitR, assoc)
+
+However, the beauty of interactive theorem provers is that sets of rules don't actually have to be that nice to benefit from automated tactics like `simp`, as long as they get a bit of help from a human when they get stuck.
+
+One more thing worth mentioning is the simplifier automatically unfolds definitions, i.e. any rule ending in `_def`, both to the term being simplified and in the LHS of all of the rules given. So something like this will also work:
+
+    def m2 = id * sw * id ; m * m
+    rewrite another_monoid_eq :
+      u * u * u * u ; m2
+      = u * u by simp(unitL)
+
+If you don't want this behaviour, you can pass the `+nodefs` flag as an argument to `simp`:
+
+    def m2 = id * sw * id ; m * m
+
+    rewrite another_monoid_eq1 :
+      u * u * u * u ; m2
+      = u * u by simp(+nodefs, unitL) # fails
+
+    rewrite another_monoid_eq2 :
+      u * u * u * u ; m2
+      = u * u by simp(+nodefs, m2_def, unitL) # succeeds again
+
+
+These three tactics are all implemented in the `chyp.tactic` module. [Tactic](https://github.com/akissinger/chyp/blob/master/chyp/tactic/__init__.py) implements `refl`, and the other tactics are implemented as subclasses of `Tactic` that should override the `check` method, which tries to close the current goal, and the `make_rhs` method, which returns an iterator over possible terms to fill in a hole `?`. Thanks to the API exposed by `Tactic`, the two tactics [RuleTac](https://github.com/akissinger/chyp/blob/master/chyp/tactic/ruletac.py) and [SimpTac](https://github.com/akissinger/chyp/blob/master/chyp/tactic/simptac.py) are very simple, and it shouldn't be too hard to implement more.
+
+In theory, if tactics only interact with the current goal via the public methods exposed by `Tactic`, it shouldn't be possible to prove anything that is not true. While this doesn't provide strong guarantees of soundness, like in the case of [LCF](https://en.wikipedia.org/wiki/Logic_for_Computable_Functions)-style theorem provers, it does attempt to provide some degree of assurance that (possibly very complex) tactics won't prove untrue statements.
 
 # Modules and importing
 
 As structures and proofs get more complicated, we may want to split them into multiple files. Every chyp file defines a module, which can be imported in other chyp files. Suppose for example we define the following file `monoid.chyp`:
 
     gen m : 2 -> 1
     gen u : 0 -> 1
```

### Comparing `chyp-0.5.1/chyp/__init__.py` & `chyp-0.5.2/chyp/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/__main__.py` & `chyp-0.5.2/chyp/__main__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/graph.py` & `chyp-0.5.2/chyp/graph.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/gui/__init__.py` & `chyp-0.5.2/chyp/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/gui/app.py` & `chyp-0.5.2/chyp/gui/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 import sys
-from PySide6.QtGui import QColor, QPalette
 from PySide6.QtWidgets import QApplication
 
 from .colors import apply_theme
 
-from .mainwindow import MainWindow
+from . import mainwindow
 
 
 cat_macchiato_p = {
   'rosewater':  '#f4dbd6',
   'flamingo':   '#f0c6c6',
   'pink':       '#f5bde6',
   'mauve':      '#c6a0f6',
@@ -76,15 +75,15 @@
     """
 
     def __init__(self) -> None:
         super().__init__(sys.argv)
         self.setApplicationName('chyp')
         self.setDesktopFileName("chyp")
         apply_theme()
-        self.main_window = MainWindow()
+        self.main_window = mainwindow.MainWindow()
         self.lastWindowClosed.connect(self.quit)
 
 
 def main() -> None:
     """Main entry point for chyp"""
 
     chyp = Chyp()
```

### Comparing `chyp-0.5.1/chyp/gui/codeview.py` & `chyp-0.5.2/chyp/gui/codeview.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,37 +9,35 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from sys import prefix
 from typing import Iterable, Optional, Tuple
 import re
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QKeyEvent, QTextCursor
 from PySide6.QtWidgets import QCompleter, QPlainTextEdit
 
 from .completion import CodeCompletionModel
 from .document import ChypDocument
 from .highlighter import BG, FG, NO_STATUS
 
 
 class CodeView(QPlainTextEdit):
     def __init__(self) -> None:
         super().__init__()
-        self.setStyleSheet("QPlainTextEdit {background-color: %s; color: %s}" % (BG, FG))
+        self.setStyleSheet("QTextEdit {background-color: %s; color: %s}" % (BG, FG))
         self.completer = QCompleter(self)
         self.completer.setCompletionMode(QCompleter.CompletionMode.PopupCompletion)
         self.completer.setCaseSensitivity(Qt.CaseSensitivity.CaseSensitive)
         self.completer.setModelSorting(QCompleter.ModelSorting.CaseSensitivelySortedModel)
         self.completer.setWidget(self)
         self.completion_model = CodeCompletionModel(self.completer)
-        # self.completion_model.set_completions(["foo", "bar", "baz"])
         self.completer.setModel(self.completion_model)
         self.completer.activated.connect(self.insert_completion)
 
     def popup_visible(self) -> bool:
         return self.completer.popup().isVisible()
 
     def set_completions(self, completions: Iterable[str]) -> None:
```

### Comparing `chyp-0.5.1/chyp/gui/colors.py` & `chyp-0.5.2/chyp/gui/colors.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/gui/completion.py` & `chyp-0.5.2/chyp/gui/completion.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/gui/editor.py` & `chyp-0.5.2/chyp/gui/editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,21 +15,24 @@
 
 from __future__ import annotations
 from typing import Callable, Dict, Optional, Tuple
 from PySide6.QtCore import QByteArray, QFileInfo, QObject, QThread, QTimer, Qt, QSettings
 from PySide6.QtGui import QTextCursor
 from PySide6.QtWidgets import QHBoxLayout, QSplitter, QTreeView, QVBoxLayout, QWidget
 
+
+from .. import parser
 from ..layout import convex_layout
 from ..graph import Graph
 from ..state import RewriteState, State
 # from ..term import graph_to_term
 # from ..matcher import match_rule
 # from ..rewrite import rewrite
 
+from . import mainwindow
 from .errorlist import ErrorListModel
 from .graphview import GraphView
 from .codeview import CodeView
 from .document import ChypDocument
 from .highlighter import STATUS_GOOD, STATUS_BAD
 
 class Editor(QWidget):
@@ -63,14 +66,15 @@
         # self.doc.documentReplaced.connect(self.reset_state)
 
         self.splitter.addWidget(self.code_view)
 
         self.error_view = QTreeView()
         self.error_view.setIndentation(0)
         self.error_view.setModel(ErrorListModel())
+        self.error_view.clicked.connect(self.jump_to_error)
         self.splitter.addWidget(self.error_view)
 
         splitter_state = conf.value("editor_splitter_state")
         if splitter_state and isinstance(splitter_state, QByteArray): self.splitter.restoreState(splitter_state)
 
         self.code_view.cursorPositionChanged.connect(self.show_at_cursor)
         self.code_view.textChanged.connect(self.invalidate_text)
@@ -129,14 +133,23 @@
         i += step
 
         if i >= 0 and i < len(self.state.parts):
             p1 = self.state.parts[i]
             cursor.setPosition(p1[1])
             self.code_view.setTextCursor(cursor)
             
+    def jump_to_error(self) -> None:
+        model = self.error_view.model()
+        window = self.window()
+        i = self.error_view.currentIndex().row()
+        if isinstance(model, ErrorListModel) and isinstance(window, mainwindow.MainWindow):
+            if i >= 0 and i < len(model.errors):
+                err = model.errors[i]
+                window.open(err[0], line_number=err[1])
+
     def show_errors(self) -> None:
         conf = QSettings('chyp', 'chyp')
         error_panel_size = conf.value('error_panel_size', 100)
         if isinstance(error_panel_size, str):
             error_panel_size = int(error_panel_size)
         if not isinstance(error_panel_size, int) or error_panel_size == 0:
             error_panel_size = 100
@@ -268,18 +281,17 @@
             else:
                 self.code_view.add_line_below(f'  = ? by {tactic}({args})')
 
             self.update_state()
             self.next_rewrite_at_cursor()
 
     def update_state(self) -> None:
-        self.state = State()
+        self.state = parser.parse(self.doc.toPlainText(), self.doc.file_name)
         self.code_view.set_current_region(None)
         
-        self.state.update(self.doc.toPlainText(), self.doc.file_name)
         model = self.error_view.model()
         if isinstance(model, ErrorListModel):
             model.set_errors(self.state.errors)
 
         if len(self.state.errors) == 0:
             self.parsed = True
             self.code_view.set_completions(self.state.rules.keys())
```

### Comparing `chyp-0.5.1/chyp/gui/errorlist.py` & `chyp-0.5.2/chyp/gui/errorlist.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/gui/graphscene.py` & `chyp-0.5.2/chyp/gui/graphscene.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/gui/graphview.py` & `chyp-0.5.2/chyp/gui/graphview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/gui/highlighter.py` & `chyp-0.5.2/chyp/gui/highlighter.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional, Tuple
 import re
-from PySide6.QtGui import QColor, QSyntaxHighlighter, QTextDocument
+from PySide6.QtGui import QColor, QSyntaxHighlighter, QTextBlockFormat, QTextCursor, QTextDocument
 
 from .colors import current_theme
 
 NO_STATUS = 0
 STATUS_GOOD = 1
 STATUS_BAD = 2
 
@@ -52,15 +52,15 @@
         ident = '[a-zA-Z_][\\.a-zA-Z0-9_]*'
         for m in re.finditer('(^|\\W)(let|def|gen|rule|by|rewrite|import|as|show)\\s+\\-?\\s*(%s)?' % ident, text):
             x,y = m.span(2)
             self.setFormat(x, y-x, QColor(KEYWORD))
             x,y = m.span(3)
             self.setFormat(x, y-x, QColor(IDENT))
 
-        for m in re.finditer('[?~.><:;*=\\-\\[\\]]', text):
+        for m in re.finditer('[?~<>(),:;*=\\-\\[\\]]', text):
             self.setFormat(m.start(), 1, QColor(OP))
 
         for m in re.finditer('(\\W|^)([0-9]+)(\\W|$)', text):
             x,y = m.span(2)
             self.setFormat(x, y-x, QColor(NUM))
 
         for m in re.finditer('"[^"]*"', text):
```

### Comparing `chyp-0.5.1/chyp/gui/mainwindow.py` & `chyp-0.5.2/chyp/gui/mainwindow.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 from typing import Callable, List, Optional
 from PySide6.QtCore import QByteArray, QDir, QFileInfo, QSettings, Qt
-from PySide6.QtGui import QActionGroup, QCloseEvent, QKeySequence
+from PySide6.QtGui import QActionGroup, QCloseEvent, QKeySequence, QTextCursor
 from PySide6.QtWidgets import QApplication, QFileDialog, QMainWindow, QMenuBar, QMessageBox, QTabWidget, QVBoxLayout, QWidget
 
-from .editor import Editor
+from . import editor
 
 
 class MainWindow(QMainWindow):
     def __init__(self) -> None:
         super().__init__()
         conf = QSettings('chyp', 'chyp')
 
@@ -41,37 +41,37 @@
         w.layout().addWidget(self.tabs)
         self.resize(1600, 800)
         
         geom = conf.value("editor_window_geometry")
         if geom and isinstance(geom, QByteArray): self.restoreGeometry(geom)
         self.show()
 
-        self.active_editor: Optional[Editor] = None
-        self.add_tab(Editor(), "Untitled")
+        self.active_editor: Optional[editor.Editor] = None
+        self.add_tab(editor.Editor(), "Untitled")
         self.update_file_name()
         self.build_menu()
 
 
     def remove_empty_editor(self) -> None:
         if self.active_editor:
             if self.active_editor.title() == 'Untitled' and self.active_editor.doc.toPlainText() == '':
                 self.tabs.removeTab(self.tabs.indexOf(self.active_editor))
                 self.active_editor = None
 
     def update_file_name(self) -> None:
         for i in range(self.tabs.count()):
             w = self.tabs.widget(i)
-            if isinstance(w, Editor):
+            if isinstance(w, editor.Editor):
                 self.tabs.setTabText(i, w.title())
         if self.active_editor:
             self.setWindowTitle('chyp - ' + self.active_editor.title())
 
     def tab_changed(self, i: int) -> None:
         w = self.tabs.widget(i)
-        if isinstance(w, Editor):
+        if isinstance(w, editor.Editor):
             self.active_editor = w
             self.active_editor.code_view.setFocus()
             self.update_file_name()
 
     def update_themes(self) -> None:
         conf = QSettings('chyp', 'chyp')
         theme_name = conf.value('theme')
@@ -111,75 +111,84 @@
 
         self.file_open_recent.clear()
         for f in self.recent_files():
             fi = QFileInfo(f)
             action = self.file_open_recent.addAction(fi.fileName())
             action.triggered.connect(open_recent(f))
 
-    def add_tab(self, editor: Editor, title: str) -> None:
-        self.tabs.addTab(editor, title)
-        editor.doc.fileNameChanged.connect(self.update_file_name)
-        editor.doc.modificationChanged.connect(self.update_file_name)
-        self.tabs.setCurrentWidget(editor)
-        editor.reset_state()
-
-    def close_tab(self, editor: Optional[Editor]=None) -> bool:
-        if editor is None:
-            editor = self.active_editor
-
-        if editor:
-            i = self.tabs.indexOf(editor)
-            if i != -1 and editor.doc.confirm_close():
-                editor.doc.fileNameChanged.disconnect(self.update_file_name)
-                editor.doc.modificationChanged.disconnect(self.update_file_name)
+    def add_tab(self, ed: editor.Editor, title: str) -> None:
+        self.tabs.addTab(ed, title)
+        ed.doc.fileNameChanged.connect(self.update_file_name)
+        ed.doc.modificationChanged.connect(self.update_file_name)
+        self.tabs.setCurrentWidget(ed)
+        ed.reset_state()
+
+    def close_tab(self, ed: Optional[editor.Editor]=None) -> bool:
+        if ed is None:
+            ed = self.active_editor
+
+        if ed:
+            i = self.tabs.indexOf(ed)
+            if i != -1 and ed.doc.confirm_close():
+                ed.doc.fileNameChanged.disconnect(self.update_file_name)
+                ed.doc.modificationChanged.disconnect(self.update_file_name)
                 self.tabs.removeTab(i)
 
                 if self.tabs.count() == 0:
                     app = QApplication.instance()
                     if app:
                         app.quit()
 
                 return True
 
         return False
 
     def new(self) -> None:
         self.remove_empty_editor()
-        editor = Editor()
-        self.add_tab(editor, "Untitled")
+        ed = editor.Editor()
+        self.add_tab(ed, "Untitled")
 
-    def open(self, file_name: str='') -> None:
+    def open(self, file_name: str='', line_number: int=-1) -> None:
         conf = QSettings('chyp', 'chyp')
 
         # if no file name provided, show open dialog
         if file_name == '':
             o = conf.value('last_dir')
             last_dir = o if isinstance(o, str) else QDir.home().absolutePath()
             file_name, _ = QFileDialog.getOpenFileName(self,
                                                        "Open File",
                                                        last_dir,
                                                        'chyp files (*.chyp)')
 
+        ed: Optional[editor.Editor] = None
+
         # if file is already open, just focus the tab
         for i in range(self.tabs.count()):
             w = self.tabs.widget(i)
-            if isinstance(w, Editor) and w.doc.file_name == file_name:
+            if isinstance(w, editor.Editor) and w.doc.file_name == file_name:
+                ed = w
                 self.tabs.setCurrentWidget(w)
-                return
 
-        try:
-            editor = Editor()
-            editor.doc.open(file_name)
-            conf.setValue('last_dir', QFileInfo(file_name).absolutePath())
-            self.remove_empty_editor()
-            self.update_recent_files()
-            editor.doc.fileNameChanged.connect(self.update_file_name)
-            self.add_tab(editor, editor.title())
-        except FileNotFoundError:
-            QMessageBox.warning(self, "File not found", "File not found: " + file_name)
+        if not ed:
+            try:
+                ed = editor.Editor()
+                ed.doc.open(file_name)
+                conf.setValue('last_dir', QFileInfo(file_name).absolutePath())
+                self.remove_empty_editor()
+                self.update_recent_files()
+                ed.doc.fileNameChanged.connect(self.update_file_name)
+                self.add_tab(ed, ed.title())
+            except FileNotFoundError:
+                QMessageBox.warning(self, "File not found", "File not found: " + file_name)
+
+        if ed and line_number != -1:
+            cur = QTextCursor(ed.code_view.document().findBlockByNumber(line_number - 1))
+            ed.code_view.moveCursor(QTextCursor.MoveOperation.End)
+            ed.code_view.setTextCursor(cur)
+            ed.code_view.setFocus()
 
 
     def save(self) -> None:
         if self.active_editor:
             self.active_editor.doc.save()
             self.update_recent_files()
 
@@ -247,15 +256,15 @@
             conf.setValue("editor_splitter_state", self.active_editor.splitter.saveState())
             sizes = self.active_editor.splitter.sizes()
             if sizes[2] != 0:
                 conf.setValue('error_panel_size', sizes[2])
 
         while self.tabs.count() > 0:
             w = self.tabs.widget(0)
-            if isinstance(w, Editor):
+            if isinstance(w, editor.Editor):
                 if not self.close_tab(w):
                     e.ignore()
                     return
             else:
                 raise RuntimeError("Unexpected widget in tab list")
 
         e.accept()
```

### Comparing `chyp-0.5.1/chyp/layout.py` & `chyp-0.5.2/chyp/layout.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/matcher.py` & `chyp-0.5.2/chyp/matcher.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/parser.py` & `chyp-0.5.2/chyp/state.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,96 +9,109 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import annotations
+from typing import Dict, List, Optional, Tuple
+
 import os.path
 from typing import Any, Dict, List, Optional, Tuple
-from lark import Lark, ParseTree, Transformer, UnexpectedInput, v_args
+import lark
+from lark import v_args
 from lark.tree import Meta
 
+from . import parser
 from .graph import Graph, GraphError, gen, perm, identity
 from .rule import Rule, RuleError
+from .tactic import Tactic
+from .tactic.simptac import SimpTac
+from .tactic.ruletac import RuleTac
+
+
+class RewriteState:
+    UNCHECKED = 0
+    CHECKING = 1
+    VALID = 2
+    INVALID = 3
+
+    def __init__(self,
+                 sequence: int,
+                 state: State,
+                 line_number: int = 0,
+                 term_pos: Tuple[int,int] = (0,0),
+                 equiv: bool=True,
+                 tactic: str='',
+                 tactic_args: Optional[List[str]]=None,
+                 lhs: Optional[Graph]=None,
+                 rhs: Optional[Graph]=None,
+                 lhs_match: Optional[Graph]=None,
+                 rhs_match: Optional[Graph]=None,
+                 stub: bool=False) -> None:
+
+        # store an integer representing my current location. This prevents cyclic dependencies of
+        # rules used inside of tactics. TODO: this doesn't work quite right for <= rules, since it
+        # doesn't store the location of the rule *and* its converse being proved.
+        self.sequence = sequence
+
+        self.state = state
+        self.status = RewriteState.UNCHECKED
+        self.line_number = line_number
+        self.term_pos = term_pos
+        self.equiv = equiv
+        self.lhs = lhs
+        self.rhs = rhs
+        self.lhs_match = lhs_match
+        self.rhs_match = rhs_match
+
+        tactic_args = [] if tactic_args is None else tactic_args
+
+        self.tactic : Tactic
+        if tactic == 'rule':
+            self.tactic = RuleTac(self, tactic_args)
+        elif tactic == 'simp':
+            self.tactic = SimpTac(self, tactic_args)
+        else:
+            self.tactic = Tactic(self, tactic_args)
+        self.stub = stub
 
-GRAMMAR = Lark("""
-    start : statement*
-    ?statement : import_statement | gen | let | def_statement | rule | rewrite | show
-    gen : "gen" var ":" num "->" num [ gen_color ]
-    def_statement : "def" var "=" term [ gen_color ]
-    gen_color : "\\\"" color "\\\"" | "\\\"" color "\\\"" "\\\"" color "\\\""
-    let : "let" var "=" term
-    rule : "rule" var ":" term (eq | le) term
-    rewrite : "rewrite" [converse] var ":" term rewrite_part*
-    rewrite_part : (eq | le) term_hole [ "by" tactic ]
-    converse : "-"
-
-    LPAREN: "("
-    tactic : [ converse ] IDENT | IDENT LPAREN [ TACTIC_ARG ("," TACTIC_ARG)* ] ")"
-    ?term  : par_term | seq
-    ?par_term : "(" term ")" | par | perm | id | id0 | term_ref
-    par : par_term "*" par_term
-    seq : term ";" term
-    perm : "sw" [ "[" num ("," num)* "]" ]
-    id : "id"
-    id0 : "id0"
-    show : "show" rule_ref
-
-    import_statement : "import" module_name [ "as" var ] [ "(" import_let ("," import_let)* ")" ]
-    import_let : var "=" term
-
-    eq : "=" | "=="
-    le : "<=" | "~>"
-    num : INT
-    module_name : IDENT
-    var : IDENT
-    term_ref : IDENT
-    rule_ref : IDENT
-    term_hole : term | "?"
-    color : HEXDIGIT HEXDIGIT HEXDIGIT HEXDIGIT HEXDIGIT HEXDIGIT
-    IDENT: ("_"|LETTER) ("_"|"."|LETTER|DIGIT)*
-    TACTIC_ARG: /[^(),]+/
-
-    %import common.LETTER
-    %import common.DIGIT
-    %import common.HEXDIGIT
-    %import common.INT
-    %import common.WS
-    %import common.SH_COMMENT
-    %ignore WS
-    %ignore SH_COMMENT
-    """,
-    parser='lalr',
-    propagate_positions=True,
-    maybe_placeholders=True)
-
+    def check(self) -> None:
+        self.tactic.run_check()
 
-source_cache: Dict[str, Tuple[float,str]] = dict()
 
-class ChypParseData(Transformer):
-    def __init__(self, namespace: str, file_name: str) -> None:
+class State(lark.Transformer):
+    def __init__(self, namespace: str='', file_name: str='') -> None:
         self.namespace = namespace
         self.file_name = file_name
         self.import_depth = 0
-
         self.sequence: int = 0
         self.graphs: Dict[str, Graph] = dict()
         self.rules: Dict[str, Rule] = {'refl': Rule(Graph(), Graph(), name="refl")}
         self.rule_sequence: Dict[str, int] = {'refl': 0}
-        self.rewrites: Dict[str, Tuple[int, int, int, bool, str, List[str],
-                                       Optional[Graph], Optional[Graph],
-                                       Optional[Graph], Optional[Graph]]] = dict()
+        self.rewrites: Dict[str, RewriteState] = dict()
         self.errors: List[Tuple[str, int, str]] = list()
         self.parts: List[Tuple[int, int, str, str]] = list()
         self.parsed = False
-    
-    # def start(self, items: List[List[Tuple[int,int,str,str]]]):
-    #     pass
+
+    def part_with_index_at(self, pos: int) -> Optional[Tuple[int, Tuple[int,int,str,str]]]:
+        p0 = (0, self.parts[0]) if len(self.parts) >= 1 else None
+        for (i,p) in enumerate(self.parts):
+            if p[0] <= pos:
+                p0 = (i,p)
+                if p[1] >= pos:
+                    return (i,p)
+        return p0
+
+    def part_at(self, pos: int) -> Optional[Tuple[int,int,str,str]]:
+        p = self.part_with_index_at(pos)
+        return p[1] if p else None
         
+
     def var(self, items: List[Any]) -> str:
         s = str(items[0])
         return self.namespace + '.' + s if self.namespace else s
 
     def module_name(self, items: List[Any]) -> str:
         return str(items[0])
     
@@ -237,14 +250,16 @@
                     self.rule_sequence[rule_name] = self.sequence
                 else:
                     lhs = self.graphs[name]
                     inp = len(lhs.inputs())
                     outp = len(lhs.outputs())
                     if inp == arity and outp == coarity:
                         self.rules[rule_name] = Rule(lhs, graph, rule_name, True)
+                        self.sequence += 1
+                        self.rule_sequence[rule_name] = self.sequence
                     else:
                         self.errors.append((self.file_name, meta.line, "Term '{}' already defined with incompatible type {} -> {}.".format(name, inp, outp)))
 
         else:
             self.errors.append((self.file_name, meta.line, "Rule '{}' already defined.".format(rule_name)))
         self.parts.append((meta.start_pos, meta.end_pos, 'rule', rule_name))
 
@@ -268,15 +283,15 @@
                     if graph:
                         self.graphs[name] = graph
                 else:
                     self.errors.append((self.file_name, meta.line, "Term '{}' already defined.".format(name)))
 
         file_name = module_filename(mod, self.file_name)
         try:
-            parse(file_name=file_name, namespace=namespace, parent=self)
+            parser.parse(file_name=file_name, namespace=namespace, parent=self)
         except FileNotFoundError:
             self.errors.append((self.file_name, meta.line, 'File not found: {}'.format(file_name)))
 
         self.parts.append((meta.start_pos, meta.end_pos, 'import', file_name))
 
     def import_let(self, items: List[Any]) -> Tuple[str, Graph]:
         return (items[0], items[1])
@@ -288,15 +303,15 @@
         name = '-' + base_name if converse else base_name
 
         term = items[2]
         rw_parts = items[3:]
 
         if len(rw_parts) == 0:
             self.parts.append((meta.start_pos, meta.end_pos, "rewrite", name))
-            self.rewrites[name] = (self.sequence, 0,0,False,"",[],term,None,None,None)
+            self.rewrites[name] = RewriteState(self.sequence, self, stub=True)
         else:
             start = meta.start_pos
             lhs = term
             rhs = None
             all_equiv = True
 
             if converse and base_name in self.rules:
@@ -304,21 +319,26 @@
                 rhs_match = self.rules[base_name].lhs
             else:
                 lhs_match = None
                 rhs_match = None
 
             last_i = len(rw_parts)-1
             for i, rw_part in enumerate(rw_parts):
-                end, t_start, t_end, equiv, tactic, tactic_args, rhs = rw_part
+                line_number, end, t_start, t_end, equiv, tactic, tactic_args, rhs = rw_part
                 all_equiv = all_equiv and equiv
-                self.rewrites[name + ":" + str(i)] = (self.sequence,
-                                                      t_start, t_end, equiv, tactic, tactic_args,
-                                                      lhs, rhs,
-                                                      lhs_match if i == 0 else None,
-                                                      rhs_match if i == last_i else None)
+                self.rewrites[name + ":" + str(i)] = RewriteState(
+                        self.sequence,
+                        self,
+                        line_number,
+                        (t_start, t_end),
+                        equiv,
+                        tactic, tactic_args,
+                        lhs, rhs,
+                        lhs_match if i == 0 else None,
+                        rhs_match if i == last_i else None)
                 lhs = rhs.copy() if rhs else None
                 self.parts.append((start, end, "rewrite", name + ":" + str(i)))
                 start = end
             if term and rhs:
                 try:
                     if converse:
                         if base_name in self.rules:
@@ -341,31 +361,31 @@
                             self.rule_sequence[name] = self.sequence
                         else:
                             self.errors.append((self.file_name, meta.line, "Rule '{}' already defined.".format(name)))
                 except RuleError as e:
                     self.errors.append((self.file_name, meta.line, str(e)))
 
     @v_args(meta=True)
-    def rewrite_part(self, meta: Meta, items: List[Any]) -> Tuple[int, int, int, bool, str, List[str], Optional[Graph]]:
+    def rewrite_part(self, meta: Meta, items: List[Any]) -> Tuple[int, int, int, int, bool, str, List[str], Optional[Graph]]:
         equiv = items[0]
         t_start,t_end,rhs = items[1]
         if items[2]:
             tactic, tactic_args = items[2]
         else:
-            tactic, tactic_args = ("rule", ["refl"])
+            tactic, tactic_args = ("refl", [])
 
         # converse = True if items[2] else False
 
         # rule = items[3] if items[3] else self.rules['refl']
         # if rule and converse:
         #     rule = rule.converse()
         # if equiv and rule and not rule.equiv:
         #     rule = None
 
-        return (meta.end_pos, t_start, t_end, equiv, tactic, tactic_args, rhs)
+        return (meta.line, meta.end_pos, t_start, t_end, equiv, tactic, tactic_args, rhs)
 
     def tactic(self, items: List[Any]) -> Tuple[str, List[str]]:
         if len(items) >= 2 and str(items[1]) == "(": #)
             args = items[2:] if not items[2] is None else []
             # arg_str = ', '.join(args)
             # print(f"got tactic: {items[0]}({arg_str})")
             return (items[0], args)
@@ -380,57 +400,41 @@
         t = items[0] if len(items) != 0 else None
         return (meta.start_pos, meta.end_pos, t)
 
 
 def module_filename(name: str, current_file: str) -> str:
     return os.path.join(os.path.dirname(current_file), *name.split('.')) + '.chyp'
 
-# cache parse trees for imported files and only re-parse if the file changes
-parse_cache: Dict[str, Tuple[float, ParseTree]] = dict()
-
-def parse(code: str='', file_name: str='', namespace: str='', parent: Optional[ChypParseData] = None) -> ChypParseData:
-    global parse_cache
-
-    if parent and parent.namespace:
-        if namespace != '':
-            namespace = parent.namespace + '.' + namespace
-        else:
-            namespace = parent.namespace
-
-    parse_data = ChypParseData(namespace, file_name)
-
-    if parent:
-        parse_data.graphs = parent.graphs
-        parse_data.rules = parent.rules
-        parse_data.errors = parent.errors
-        parse_data.rule_sequence = parent.rule_sequence
-        parse_data.sequence = parent.sequence
-        parse_data.import_depth = parent.import_depth + 1
-        if parse_data.import_depth > 255:
-            parse_data.errors += [(parent.file_name, -1, "Maximum import depth (255) exceeded. Probably a cyclic import.")]
-
-    try:
-        if file_name and not code:
-            mtime = os.path.getmtime(file_name)
-            if file_name in parse_cache and parse_cache[file_name][0] == mtime:
-                tree = parse_cache[file_name][1]
-            else:
-                with open(file_name) as f:
-                    tree = GRAMMAR.parse(f.read())
-                parse_cache[file_name] = (mtime, tree)
-        else:
-            tree = GRAMMAR.parse(code)
-        parse_data.transform(tree)
-        parse_data.parsed = True
-    except UnexpectedInput as e:
-        msg = 'Parse error: '
-        e_lines = e.get_context(code).splitlines()
-        if len(e_lines) >= 2:
-            parse_data.errors += [(file_name, e.line, msg + e_lines[0] + '\n' + len(msg)*' ' + e_lines[1])]
-        else:
-            parse_data.errors += [(file_name, e.line, msg + e_lines[0])]
-
-    if parent:
-        parent.sequence = parse_data.sequence
-
-    return parse_data
+# class State:
+#     def __init__(self) -> None:
+#         self.graphs: Dict[str, Graph] = dict()
+#         self.rules: Dict[str, Rule] = dict()
+#         self.rule_sequence: Dict[str, int] = dict()
+#         self.rewrites: Dict[str, RewriteState] = dict()
+#         self.parts: List[Tuple[int, int, str, str]] = list()
+#         self.errors: List[Tuple[str, int, str]] = list()
+
+#     def update(self, code: str, file_name: str) -> None:
+#         parse_data = parse(code, file_name)
+#         self.graphs = parse_data.graphs
+#         self.rules = parse_data.rules
+#         self.rule_sequence = parse_data.rule_sequence
+#         self.parts = parse_data.parts
+#         self.errors = parse_data.errors
+
+#         for name, (sequence, t_start, t_end, equiv, tactic, tactic_args, lhs, rhs, lhs_match, rhs_match) in parse_data.rewrites.items():
+#             stub = not (':' in name)
+#             self.rewrites[name] = RewriteState(sequence, self, (t_start, t_end), equiv, tactic, tactic_args, lhs, rhs, lhs_match, rhs_match, stub)
+
+#     def part_with_index_at(self, pos: int) -> Optional[Tuple[int, Tuple[int,int,str,str]]]:
+#         p0 = (0, self.parts[0]) if len(self.parts) >= 1 else None
+#         for (i,p) in enumerate(self.parts):
+#             if p[0] <= pos:
+#                 p0 = (i,p)
+#                 if p[1] >= pos:
+#                     return (i,p)
+#         return p0
+
+#     def part_at(self, pos: int) -> Optional[Tuple[int,int,str,str]]:
+#         p = self.part_with_index_at(pos)
+#         return p[1] if p else None
```

### Comparing `chyp-0.5.1/chyp/rewrite.py` & `chyp-0.5.2/chyp/rewrite.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/rule.py` & `chyp-0.5.2/chyp/rule.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/scraps.py` & `chyp-0.5.2/chyp/scraps.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/tactic/ruletac.py` & `chyp-0.5.2/chyp/tactic/ruletac.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp/tactic/simptac.py` & `chyp-0.5.2/chyp/tactic/simptac.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,42 +10,47 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
-from typing import Callable, Iterator
+from typing import Iterator, List
 
 
 from ..graph import Graph
 from . import Tactic
 
 
 class SimpTac(Tactic):
-    MAX_DEPTH = 256
-
     def name(self) -> str:
         return 'simp'
 
-    def __repeat(self, rw: Callable[[str], bool]):
-        got_match = True
-        i = 0
-        while got_match and i < SimpTac.MAX_DEPTH:
-            got_match = False
-            for r in self.args:
-                # print('rewriting: ' + r)
-                while rw(r) and i < SimpTac.MAX_DEPTH:
-                    # print('success')
-                    got_match = True
-                    i += 1
+    def __prepare_rules(self) -> List[str]:
+        flags = [a for a in self.args if a[:1] == '+']
+        rules = [a for a in self.args if a[:1] != '+']
+
+        if '+nodefs' in flags:
+            defs = [r for r in rules if r[-4:] == '_def']
+        else:
+            defs = [r for r in self.global_rules() if r[-4:]=='_def']
+
+        rest = [r for r in rules if r[-4:] != '_def']
+
+        for r in rest:
+            self.add_rule_to_context(r)
+            Tactic.repeat(lambda df: self.rewrite_lhs1(df, r), defs)
+
+        return defs + rest
 
     def make_rhs(self) -> Iterator[Graph]:
-        self.__repeat(self.rewrite_lhs1)
+        rules = self.__prepare_rules()
+        Tactic.repeat(self.rewrite_lhs1, rules)
         lhs = self.lhs()
         if lhs: yield lhs
 
     def check(self) -> None:
-        self.__repeat(self.rewrite_lhs1)
-        self.__repeat(self.rewrite_rhs1)
+        rules = self.__prepare_rules()
+        Tactic.repeat(self.rewrite_lhs1, rules)
+        Tactic.repeat(self.rewrite_rhs1, rules)
         self.validate_goal()
```

### Comparing `chyp-0.5.1/chyp/term.py` & `chyp-0.5.2/chyp/term.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/chyp.egg-info/PKG-INFO` & `chyp-0.5.2/chyp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.5.1
+Version: 0.5.2
 Summary: An interactive theorem prover for string diagrams
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
@@ -130,21 +130,15 @@
     rewrite ba1_backwards :
       g * f ; id * id * g ; id * sw * id ; f * f ; g * id
       = id * f ; f ; g ; g * id by -bialg
       = f * id ; f ; g ; g * id by -assoc
 
 The golden rule of Chyp is that _only connectivity matters_. So, if two terms give the same diagram, like `a * b ; c * d` and `(a ; c) * (b ; d)`, Chyp treats them as identical. Since under the hood, Chyp does everything with graph rewriting and not term rewriting, the prover handles all of this extra book-keeping for you.
 
-Sometimes it can be helpful for readability to do a trivial proof step that does nothing but write the same string diagram differently. There is a special rule called `refl` (for reflexivity) for this. For example:
-
-    rewrite foo :
-      a * b ; c * d
-      = (a ; c) * (b ; d) by refl
-
-Formally, `refl` is defined as `id0 = id0`, i.e. the empty graph equals itself, which always matches exactly once on any graph. If we drop the `by` clause, Chyp automatically assumes `by refl`, so the following is equivalent:
+Sometimes it can be helpful for readability to do a trivial proof step that does nothing but write the same string diagram differently. We can do this just by dropping the `by` clause in a proof step:
 
     rewrite foo :
       a * b ; c * d
       = (a ; c) * (b ; d)
 
 
 The `def` statement introduced in the previous section is just syntactic sugar for a `gen` followed by a rule. That is:
@@ -184,14 +178,82 @@
       = g * f ; id * id * g ; id * sw * id ; f * f ; id * g by bialg
       = g * g * g ; id * id * id * sw * id ; id * id * f * f ; id * sw * id ; f * f ; id * g by bialg
       = g * g * g ; id * id * id * sw * id ; id * g * f * f ; sw * sw * id ; id * f * id * g ; sw * sw * id ; id * f * f by bialg
       = g * g * g ; id * id * id * sw * id ; id * g * f * g * g ; sw * sw * id * sw * id ; id * f * id * f * f ; sw * sw * id ; id * f * f by bialg
 
 How to we know it's a normal form? Pressing `CTRL+SHIFT+Enter` one more time will result in a red line that reads `  = ? by bialg`, which means Chyp wasn't able to find any more matchings of the `bialg` rule.
 
+## Tactics
+
+Tactics are the bread and butter of interactive theorem provers. These are routines that can be called to try to solve a given goal. In Chyp, a goal corresponds to a single proof step `LHS = RHS`. Chyp has three built in tactics: `refl`, `rule`, and `simp`. If you've been following along, you've actually been using the first two already.
+
+`refl`, which stands for "reflexivity of `=`", simply tries to prove `LHS` and `RHS` represent the same diagram, i.e. they are isomorphic cospans of hypergraphs. When you write a rewrite step without providing a rule, it is actually shorthand for applying the `refl` tactic. For example:
+
+    rewrite foo :
+      a * b ; c * d
+      = (a ; c) * (b ; d)
+
+is actually shorthand for:
+
+    rewrite foo :
+      a * b ; c * d
+      = (a ; c) * (b ; d) by refl()
+
+Note the parentheses tell Chyp that this is a tactic and not a rule name. They are empty because `refl` takes zero arguments.
+
+The `rule` tactic applies the given rewrite rule to the `LHS` in every possible way until it produces `RHS` (or fails). Most of the rewrites we have done so far have used the rule tactic, which can be applied either explicitly or implicitly just by giving a rule name. Namely, for a rule `R`, writing:
+
+    rewrite foo : lhs = rhs by R
+
+is actually shorthand for:
+
+    rewrite foo : lhs = rhs by rule(R)
+
+
+Finally, the `simp` tactic applies a list of given rules as much as possible to both the `LHS` and `RHS` then compares the resulting diagrams. It could be the case that the given set of rules is non-terminating (i.e. they can be applied forever without reaching a normal form), in which case `simp` gives up after 256 rule applications.
+
+This can be very useful if the set of rules provided actually yields unique normal forms, or in rewriting lingo the rules are [confluent and terminating](https://en.wikipedia.org/wiki/Rewriting). For example, the monoid laws:
+
+    gen u : 0 -> 1
+    gen m : 2 -> 1
+    rule unitL : u * id ; m = id
+    rule unitR : id * u ; m = id
+    rule assoc : m * id ; m = id * m ; m
+    
+always yield unique normal forms. So, we can prove any true equation involving a monoid in a single step using `simp`, e.g.
+
+    rewrite random_monoid_eq :
+      id * u * u * id ; m * m ; m
+      = id * u * id ; id * m ; m by simp(unitL, unitR, assoc)
+
+However, the beauty of interactive theorem provers is that sets of rules don't actually have to be that nice to benefit from automated tactics like `simp`, as long as they get a bit of help from a human when they get stuck.
+
+One more thing worth mentioning is the simplifier automatically unfolds definitions, i.e. any rule ending in `_def`, both to the term being simplified and in the LHS of all of the rules given. So something like this will also work:
+
+    def m2 = id * sw * id ; m * m
+    rewrite another_monoid_eq :
+      u * u * u * u ; m2
+      = u * u by simp(unitL)
+
+If you don't want this behaviour, you can pass the `+nodefs` flag as an argument to `simp`:
+
+    def m2 = id * sw * id ; m * m
+
+    rewrite another_monoid_eq1 :
+      u * u * u * u ; m2
+      = u * u by simp(+nodefs, unitL) # fails
+
+    rewrite another_monoid_eq2 :
+      u * u * u * u ; m2
+      = u * u by simp(+nodefs, m2_def, unitL) # succeeds again
+
+
+These three tactics are all implemented in the `chyp.tactic` module. [Tactic](https://github.com/akissinger/chyp/blob/master/chyp/tactic/__init__.py) implements `refl`, and the other tactics are implemented as subclasses of `Tactic` that should override the `check` method, which tries to close the current goal, and the `make_rhs` method, which returns an iterator over possible terms to fill in a hole `?`. Thanks to the API exposed by `Tactic`, the two tactics [RuleTac](https://github.com/akissinger/chyp/blob/master/chyp/tactic/ruletac.py) and [SimpTac](https://github.com/akissinger/chyp/blob/master/chyp/tactic/simptac.py) are very simple, and it shouldn't be too hard to implement more.
+
+In theory, if tactics only interact with the current goal via the public methods exposed by `Tactic`, it shouldn't be possible to prove anything that is not true. While this doesn't provide strong guarantees of soundness, like in the case of [LCF](https://en.wikipedia.org/wiki/Logic_for_Computable_Functions)-style theorem provers, it does attempt to provide some degree of assurance that (possibly very complex) tactics won't prove untrue statements.
 
 # Modules and importing
 
 As structures and proofs get more complicated, we may want to split them into multiple files. Every chyp file defines a module, which can be imported in other chyp files. Suppose for example we define the following file `monoid.chyp`:
 
     gen m : 2 -> 1
     gen u : 0 -> 1
```

### Comparing `chyp-0.5.1/chyp.egg-info/SOURCES.txt` & `chyp-0.5.2/chyp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chyp-0.5.1/setup.py` & `chyp-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 
 data_files = []
 
 setuptools.setup(
     name="chyp",
-    version="0.5.1",
+    version="0.5.2",
     author="Aleks Kissinger",
     author_email="aleks0@gmail.com",
     description="An interactive theorem prover for string diagrams",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akissinger/chyp",
     project_urls={
```

