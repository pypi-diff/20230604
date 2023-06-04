# Comparing `tmp/crispy-forms-foundation-0.9.0.tar.gz` & `tmp/crispy-forms-foundation-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispy-forms-foundation-0.9.0.tar", last modified: Sun Oct 23 00:46:18 2022, max compression
+gzip compressed data, was "crispy-forms-foundation-1.0.0.tar", last modified: Sun Jun  4 15:40:56 2023, max compression
```

## Comparing `crispy-forms-foundation-0.9.0.tar` & `crispy-forms-foundation-1.0.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.879779 crispy-forms-foundation-0.9.0/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1056 2022-10-22 13:41:48.000000 crispy-forms-foundation-0.9.0/LICENCE.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      468 2022-10-22 13:41:48.000000 crispy-forms-foundation-0.9.0/MANIFEST.in
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2173 2022-10-23 00:46:18.879779 crispy-forms-foundation-0.9.0/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      869 2022-10-23 00:45:26.000000 crispy-forms-foundation-0.9.0/README.rst
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.875779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      758 2022-10-23 00:45:26.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6575 2022-10-23 00:45:26.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/forms.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.879779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1571 2022-10-22 13:41:48.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1222 2022-10-23 00:45:26.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/base.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6833 2022-10-23 00:45:26.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/buttons.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     8226 2022-10-23 00:45:26.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/containers.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6756 2022-10-23 00:45:26.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/fields.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3428 2022-10-23 00:45:26.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/grid.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.875779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.875779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/de/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.879779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/de/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      563 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      884 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.875779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/fr/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.879779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      562 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      811 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       15 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/models.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      430 2022-10-23 00:45:26.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/settings.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.875779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/static/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.875779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/static/js/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.879779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/static/js/crispy_forms_foundation/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3706 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/static/js/crispy_forms_foundation/plugins.js
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.875779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.879779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      731 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/betterform.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      280 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/display_form.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      406 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/errors.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      467 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/errors_formset.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2048 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/field.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1210 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/field.strict.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2084 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/inline_switch.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.879779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       95 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/accordion-holder.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      317 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/accordion-item.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      479 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/basebutton.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      385 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/baseinput.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      280 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/buttongroup.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      199 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/buttonholder.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      563 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/checkboxselectmultiple.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      168 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/div.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      288 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/fieldset.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1553 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/inline_field.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1135 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/multifield.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1249 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/splitdatetime_field.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      261 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/tab-holder.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      208 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/tab-item.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      310 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/tab-link.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      685 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/multifield.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1728 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/switch.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      359 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/uni_form.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      245 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/uni_formset.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      579 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/whole_uni_form.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      786 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/whole_uni_formset.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.879779 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templatetags/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-10-22 13:41:49.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templatetags/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4414 2022-10-23 00:45:26.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation/templatetags/crispy_forms_foundation_field.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2022-10-23 00:46:18.875779 crispy-forms-foundation-0.9.0/crispy_forms_foundation.egg-info/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2173 2022-10-23 00:46:18.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation.egg-info/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3028 2022-10-23 00:46:18.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation.egg-info/SOURCES.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2022-10-23 00:46:18.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation.egg-info/dependency_links.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      166 2022-10-23 00:46:18.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation.egg-info/requires.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       32 2022-10-23 00:46:18.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation.egg-info/top_level.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2022-10-23 00:41:04.000000 crispy-forms-foundation-0.9.0/crispy_forms_foundation.egg-info/zip-safe
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2012 2022-10-23 00:46:18.883779 crispy-forms-foundation-0.9.0/setup.cfg
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       60 2022-10-23 00:45:26.000000 crispy-forms-foundation-0.9.0/setup.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.869202 crispy-forms-foundation-1.0.0/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1056 2022-10-22 13:41:48.000000 crispy-forms-foundation-1.0.0/LICENCE.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      468 2022-10-22 13:41:48.000000 crispy-forms-foundation-1.0.0/MANIFEST.in
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2263 2023-06-04 15:40:56.869202 crispy-forms-foundation-1.0.0/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      869 2022-10-23 00:45:26.000000 crispy-forms-foundation-1.0.0/README.rst
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.861202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      758 2022-10-23 00:45:26.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6518 2023-06-04 15:40:27.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/forms.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.865202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1531 2023-06-04 15:40:27.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1222 2022-10-23 00:45:26.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/base.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6785 2023-06-04 15:40:27.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/buttons.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     8154 2023-06-04 15:40:27.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/containers.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6660 2023-06-04 15:40:27.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/fields.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3428 2022-10-23 00:45:26.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/grid.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.861202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.861202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/de/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.865202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      563 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      884 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.861202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/fr/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.865202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      562 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      811 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       15 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/models.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      430 2022-10-23 00:45:26.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/settings.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.861202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/static/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.861202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/static/js/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.865202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/static/js/crispy_forms_foundation/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3706 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/static/js/crispy_forms_foundation/plugins.js
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.861202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.865202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      731 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/betterform.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      280 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/display_form.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      406 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/errors.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      467 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/errors_formset.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2048 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/field.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1210 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/field.strict.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2084 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/inline_switch.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.869202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       95 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/accordion-holder.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      317 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/accordion-item.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      479 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/basebutton.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      385 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/baseinput.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      280 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/buttongroup.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      199 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/buttonholder.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      563 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/checkboxselectmultiple.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      168 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/div.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      258 2023-06-04 15:40:27.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/fieldset.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1553 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/inline_field.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1135 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/multifield.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1249 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/splitdatetime_field.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      261 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/tab-holder.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      208 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/tab-item.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      310 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/tab-link.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      685 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/multifield.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1728 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/switch.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      230 2023-06-04 15:40:27.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/uni_form.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      245 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/uni_formset.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      579 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/whole_uni_form.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      786 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/whole_uni_formset.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.869202 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templatetags/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-10-22 13:41:49.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templatetags/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4348 2023-06-04 15:40:27.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation/templatetags/crispy_forms_foundation_field.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-04 15:40:56.861202 crispy-forms-foundation-1.0.0/crispy_forms_foundation.egg-info/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2263 2023-06-04 15:40:56.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation.egg-info/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3028 2023-06-04 15:40:56.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation.egg-info/SOURCES.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-06-04 15:40:56.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation.egg-info/dependency_links.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      164 2023-06-04 15:40:56.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation.egg-info/requires.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       32 2023-06-04 15:40:56.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation.egg-info/top_level.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-06-04 13:21:31.000000 crispy-forms-foundation-1.0.0/crispy_forms_foundation.egg-info/zip-safe
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2040 2023-06-04 15:40:56.869202 crispy-forms-foundation-1.0.0/setup.cfg
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       60 2022-10-23 00:45:26.000000 crispy-forms-foundation-1.0.0/setup.py
```

### Comparing `crispy-forms-foundation-0.9.0/LICENCE.txt` & `crispy-forms-foundation-1.0.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/PKG-INFO` & `crispy-forms-foundation-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: crispy-forms-foundation
-Version: 0.9.0
+Version: 1.0.0
 Summary: Django application to add 'django-crispy-forms' layout objects for 'Foundation for sites'
 Home-page: https://github.com/sveetch/crispy-forms-foundation
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Django,django-crispy-forms,foundation-site
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: quality
```

### Comparing `crispy-forms-foundation-0.9.0/README.rst` & `crispy-forms-foundation-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/__init__.py` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/__init__.py`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/forms.py` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import unicode_literals, absolute_import
 from copy import deepcopy
 
 from django import forms
 from django.forms.fields import FileField, ImageField
 from django.utils.translation import gettext_lazy as _
 from django.urls import reverse, NoReverseMatch
```

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/__init__.py` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 Layout items for Foundation components.
 
 Inherits from the default **crispy_forms** layout objects to force templates on
 the right ``TEMPLATE_PACK`` (defined from ``settings.CRISPY_TEMPLATE_PACK``)
 and implements Foundation components.
 """
-from __future__ import absolute_import
-
 from .base import Div, Callout, Layout, UneditableField, HTML
 from .grid import Row, RowFluid, Column
 
 from .fields import (  # noqa: F401
     MultiWidgetField, Field, MultiField,
     SplitDateTimeField, InlineField,
     InlineJustifiedField, SwitchField,
```

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/base.py` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/base.py`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/buttons.py` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/buttons.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,21 +69,21 @@
 
     def __init__(self, *fields, **kwargs):
         self.fields = list(fields)
         self.css_class = kwargs.get('css_class', None)
         self.css_id = kwargs.get('css_id', None)
         self.template = kwargs.get('template', self.template)
 
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK):
+    def render(self, form, context, template_pack=TEMPLATE_PACK):
         field_list = []
         template = self.get_template_name(template_pack)
 
         for field in self.fields:
             field_list.append(
-                render_field(field, form, form_style, context,
+                render_field(field, form, context,
                              template_pack=template_pack)
             )
 
         buttons = render_to_string(template, {
             'buttongroup': self,
             'field_list': field_list,
         })
@@ -196,17 +196,17 @@
     input_type = 'button'
     field_classes = 'button'
 
     def __init__(self, field, *args, **kwargs):
         self.content = kwargs.pop('content', None)
         super(ButtonElement, self).__init__(field, *args, **kwargs)
 
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK):
+    def render(self, form, context, template_pack=TEMPLATE_PACK):
         context['button_content'] = self.content
-        return super(ButtonElement, self).render(form, form_style, context,
+        return super(ButtonElement, self).render(form, context,
                                                  template_pack)
 
 
 class ButtonSubmit(ButtonElement):
     """
     Create a submit button following the ``ButtonElement`` behaviors:
```

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/containers.py` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/containers.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,23 +56,23 @@
 
     def get_active_css_class(self, template_pack):
         # Foundation-6 addon only which use unusual class name
         if template_pack == 'foundation-6':
             return "is-active"
         return self.active_css_class
 
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK,
+    def render(self, form, context, template_pack=TEMPLATE_PACK,
                **kwargs):
         active_classname = self.get_active_css_class(template_pack)
         if self.active:
             if active_classname and active_classname not in self.css_class:
                 self.css_class += ' ' + active_classname
         else:
             self.css_class = self.css_class.replace(active_classname, '')
-        return super(Container, self).render(form, form_style, context,
+        return super(Container, self).render(form, context,
                                              template_pack)
 
 
 class ContainerHolder(crispy_forms_bootstrap.ContainerHolder):
     pass
 
 
@@ -94,15 +94,15 @@
 
     The first ``TabItem`` containing a field error will be marked as
     *active* if any, else this will be just the first ``TabItem``.
     """
     template = "%s/layout/tab-holder.html"
     default_active_tab = None
 
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK):
+    def render(self, form, context, template_pack=TEMPLATE_PACK):
         """
         Re-implement almost the same code from crispy_forms but passing
         ``form`` instance to item ``render_link`` method.
         """
         links, content = '', ''
 
         # accordion group needs the parent div id to set `data-parent` (I don't
@@ -114,15 +114,15 @@
             tab.active = False
 
         # Activate item
         self.open_target_group_for_form(form)
 
         for tab in self.fields:
             content += render_field(
-                tab, form, form_style, context, template_pack=template_pack
+                tab, form, context, template_pack=template_pack
             )
             links += tab.render_link(form, template_pack)
 
         context.update({
             'tabs': self,
             'links': links,
             'content': content
@@ -197,15 +197,15 @@
     using ``css_id`` argument.
 
     The first ``AccordionItem`` containing a field error will be marked as
     *active* if any, else this will be just the first ``AccordionItem``.
     """
     template = "%s/layout/accordion-holder.html"
 
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK,
+    def render(self, form, context, template_pack=TEMPLATE_PACK,
                **kwargs):
         """
         Re-implement almost the same code from crispy_forms but using
         ``form`` instance to catch field errors.
         """
         content = ''
 
@@ -221,15 +221,15 @@
 
         for group in self.fields:
             group.data_parent = self.css_id
             group.item_has_errors = any([fieldname_error for fieldname_error in
                                          form.errors.keys()
                                          if fieldname_error in group])
             content += render_field(
-                group, form, form_style, context, template_pack=template_pack,
+                group, form, context, template_pack=template_pack,
                 **kwargs
             )
 
         template = self.get_template_name(template_pack)
         context.update({'accordion': self, 'content': content})
 
         return render_to_string(template, context.flatten())
```

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/fields.py` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
     passed to the template context.
 
     Actually the only difference with a ``Field`` is label element drops
     ``for`` attribute.
 
     You should use this field in last resort.
     """
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK):
+    def render(self, form, context, template_pack=TEMPLATE_PACK):
         context['fake_field'] = True
-        return super(FakeField, self).render(form, form_style, context,
+        return super(FakeField, self).render(form, context,
                                              template_pack)
 
 
 class Hidden(crispy_forms_layout.Hidden):
     """
     Hidden field. Work as basic Field except the ``hidden`` value for ``type``
     attribute.
@@ -110,23 +110,23 @@
         self.field = field
         self.label_column = label_column+' columns'
         self.input_column = input_column+' columns'
         self.label_class = label_class
 
         super(InlineField, self).__init__(field, *args, **kwargs)
 
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK):
+    def render(self, form, context, template_pack=TEMPLATE_PACK):
         context['label_column'] = self.label_column
         context['input_column'] = self.input_column
         context['label_class'] = self.label_class
 
         html = ''
         template = self.get_template_name(template_pack)
         for field in self.fields:
-            html += render_field(field, form, form_style, context,
+            html += render_field(field, form, context,
                                  template=template, attrs=self.attrs,
                                  template_pack=template_pack)
         return html
 
 
 class InlineJustifiedField(InlineField):
     """
@@ -157,17 +157,17 @@
 
     def __init__(self, field, *args, **kwargs):
         self.switch_class = ['switch'] + kwargs.pop('switch_class', '').split()
         kwargs['class'] = (kwargs.pop('class', '') + ' switch-input').strip()
 
         super(SwitchField, self).__init__(field, *args, **kwargs)
 
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK):
+    def render(self, form, context, template_pack=TEMPLATE_PACK):
         context['switch_class'] = " ".join(self.switch_class)
-        return super(SwitchField, self).render(form, form_style, context,
+        return super(SwitchField, self).render(form, context,
                                                template_pack)
 
 
 class InlineSwitchField(InlineField):
     """
     Like ``SwitchField`` it use Foundation form switches with checkbox field
     but within an ``InlineField``
@@ -199,11 +199,11 @@
         self.switch_class = ['switch']+kwargs.pop('switch_class', '').split()
         kwargs['label_column'] = kwargs.pop('label_column', 'large-8')
         kwargs['input_column'] = kwargs.pop('input_column', 'large-4')
         kwargs['class'] = (kwargs.pop('class', '') + ' switch-input').strip()
 
         super(InlineSwitchField, self).__init__(field, *args, **kwargs)
 
-    def render(self, form, form_style, context, template_pack=TEMPLATE_PACK):
+    def render(self, form, context, template_pack=TEMPLATE_PACK):
         context['switch_class'] = " ".join(self.switch_class)
-        return super(InlineSwitchField, self).render(form, form_style, context,
+        return super(InlineSwitchField, self).render(form, context,
                                                      template_pack)
```

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/layout/grid.py` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/layout/grid.py`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/de/LC_MESSAGES/django.mo` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/de/LC_MESSAGES/django.po` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/fr/LC_MESSAGES/django.mo` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/locale/fr/LC_MESSAGES/django.po` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/static/js/crispy_forms_foundation/plugins.js` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/static/js/crispy_forms_foundation/plugins.js`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/betterform.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/betterform.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/field.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/field.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/field.strict.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/field.strict.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/inline_switch.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/inline_switch.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/checkboxselectmultiple.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/checkboxselectmultiple.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/inline_field.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/inline_field.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/multifield.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/multifield.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/layout/splitdatetime_field.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/layout/splitdatetime_field.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/multifield.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/multifield.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/switch.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/switch.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/whole_uni_form.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/whole_uni_form.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templates/foundation-6/whole_uni_formset.html` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templates/foundation-6/whole_uni_formset.html`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation/templatetags/crispy_forms_foundation_field.py` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation/templatetags/crispy_forms_foundation_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
 Re implementation of ``crispy_forms.templatetags.crispy_forms_field`` needed to
 have correct Foundation6 error class on input element.
-
-TODO: Changes stand on ``CRISPY_CLASS_CONVERTERS`` usage so it may be included
-      in ``django-crispy-forms``, this needs a Pull request.
 """
 from django import template
 from django.conf import settings
 
-from crispy_forms.templatetags.crispy_forms_field import (is_checkbox,
-                                                          is_file,
-                                                          pairwise,
-                                                          CrispyFieldNode)
+from crispy_forms.templatetags.crispy_forms_field import (
+    is_checkbox,
+    is_file,
+    pairwise,
+    CrispyFieldNode,
+)
 
 register = template.Library()
 
 
 class CrispyFoundationFieldNode(CrispyFieldNode):
+    """
+    Override original Node object to manage field in a proper way for Foundation
+    classes.
+    """
     def __init__(self, field, attrs):
         self.field = field
         self.attrs = attrs
         self.html5_required = 'html5_required'
 
     def render(self, context):
         # Nodes are not threadsafe so we must store and look up our instance
@@ -79,15 +82,15 @@
                 if (
                     field.field.widget.__class__.__name__ != 'RadioSelect' and
                     field.field.widget.__class__.__name__ != 'CheckboxSelectMultiple'
                 ):
                     widget.attrs['required'] = 'required'
 
             for attribute_name, attribute in attr.items():
-                attribute_name = template.Variable(attribute_name).resolve(context)  # noqa: E501
+                attribute_name = template.Variable(attribute_name).resolve(context)
                 attributes = template.Variable(attribute).resolve(context)
 
                 if attribute_name in widget.attrs:
                     # multiple attribtes are in a single string, e.g.
                     # "form-control is-invalid"
                     for attr in attributes.split():
                         if attr not in widget.attrs[attribute_name].split():
@@ -97,15 +100,20 @@
 
         return str(field)
 
 
 @register.tag(name="crispy_field")
 def crispy_field(parser, token):
     """
-    {% crispy_field field attrs %}
+    Override original template filter to use the ``CrispyFoundationFieldNode``.
+
+    Usage is identical to the original one: ::
+
+        {% crispy_field field attrs %}
+
     """
     token = token.split_contents()
     field = token.pop(1)
     attrs = {}
 
     # We need to pop tag name, or pairwise would fail
     token.pop(0)
```

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation.egg-info/PKG-INFO` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: crispy-forms-foundation
-Version: 0.9.0
+Version: 1.0.0
 Summary: Django application to add 'django-crispy-forms' layout objects for 'Foundation for sites'
 Home-page: https://github.com/sveetch/crispy-forms-foundation
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Django,django-crispy-forms,foundation-site
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: quality
```

### Comparing `crispy-forms-foundation-0.9.0/crispy_forms_foundation.egg-info/SOURCES.txt` & `crispy-forms-foundation-1.0.0/crispy_forms_foundation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crispy-forms-foundation-0.9.0/setup.cfg` & `crispy-forms-foundation-1.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crispy-forms-foundation
-version = 0.9.0
+version = 1.0.0
 description = Django application to add 'django-crispy-forms' layout objects for 'Foundation for sites'
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = David Thenon
 author_email = sveetch@gmail.com
 url = https://github.com/sveetch/crispy-forms-foundation
 license = MIT
@@ -12,31 +12,33 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 include_package_data = True
 install_requires = 
 	Django>=3.2
-	django-crispy-forms>=1.8.1
+	django-crispy-forms>=2.0
 packages = find:
 zip_safe = True
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-django
@@ -77,24 +79,23 @@
 addopts = -vv
 python_files = 
 	*.py
 testpaths = 
 	tests
 
 [tox:tox]
-envlist = py{38,39,310}-django{320,400,410}
+envlist = py{38,310,311}-django{320,400,420}
 minversion = 3.4.0
 
 [testenv]
 deps = 
 	django320: Django>=3.2,<4.0
 	django400: Django>=4.0,<4.1
 	django410: Django>=4.1,<4.2
-	
-	django320,django400,django410: django-crispy-forms>=1.9.0,<2.0.0
+	django420: Django>=4.2,<4.3
 commands = 
 	pip install -e .[test]
 	pytest -vv tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

