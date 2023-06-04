# Comparing `tmp/autoviz-0.1.71.tar.gz` & `tmp/autoviz-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoviz-0.1.71.tar", last modified: Sun Jun  4 17:05:30 2023, max compression
+gzip compressed data, was "autoviz-0.1.72.tar", last modified: Sun Jun  4 17:07:29 2023, max compression
```

## Comparing `autoviz-0.1.71.tar` & `autoviz-0.1.72.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-06-04 17:05:30.769207 autoviz-0.1.71/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14259 2023-06-04 17:05:30.765206 autoviz-0.1.71/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12287 2023-06-04 16:49:22.000000 autoviz-0.1.71/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-06-04 17:05:30.625206 autoviz-0.1.71/autoviz/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    30562 2023-05-16 01:58:53.000000 autoviz-0.1.71/autoviz/AutoViz_Class.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    60800 2023-05-15 13:55:02.000000 autoviz-0.1.71/autoviz/AutoViz_Holo.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-10-02 14:52:48.000000 autoviz-0.1.71/autoviz/AutoViz_NLP.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   117958 2023-05-15 13:41:29.000000 autoviz-0.1.71/autoviz/AutoViz_Utils.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1323 2022-10-02 14:52:48.000000 autoviz-0.1.71/autoviz/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2023-05-16 02:18:27.000000 autoviz-0.1.71/autoviz/__version__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24678 2023-04-18 12:53:31.000000 autoviz-0.1.71/autoviz/classify_method.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-06-04 17:05:30.745205 autoviz-0.1.71/autoviz.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14259 2023-06-04 17:05:30.000000 autoviz-0.1.71/autoviz.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2023-06-04 17:05:30.000000 autoviz-0.1.71/autoviz.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-06-04 17:05:30.000000 autoviz-0.1.71/autoviz.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      257 2023-06-04 17:05:30.000000 autoviz-0.1.71/autoviz.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-06-04 17:05:30.000000 autoviz-0.1.71/autoviz.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-06-04 17:05:30.773238 autoviz-0.1.71/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1231 2023-06-04 17:04:10.000000 autoviz-0.1.71/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-06-04 17:07:29.406938 autoviz-0.1.72/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    14259 2023-06-04 17:07:29.402935 autoviz-0.1.72/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12287 2023-06-04 16:49:22.000000 autoviz-0.1.72/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-06-04 17:07:29.290941 autoviz-0.1.72/autoviz/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    34170 2023-06-04 16:19:08.000000 autoviz-0.1.72/autoviz/AutoViz_Class.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    60800 2023-05-15 13:55:02.000000 autoviz-0.1.72/autoviz/AutoViz_Holo.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-10-02 14:52:48.000000 autoviz-0.1.72/autoviz/AutoViz_NLP.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   117952 2023-06-04 16:41:05.000000 autoviz-0.1.72/autoviz/AutoViz_Utils.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      782 2023-06-04 15:27:11.000000 autoviz-0.1.72/autoviz/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      403 2023-06-04 17:06:30.000000 autoviz-0.1.72/autoviz/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    18331 2023-06-04 15:27:51.000000 autoviz-0.1.72/autoviz/classify_method.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-06-04 17:07:29.386937 autoviz-0.1.72/autoviz.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    14259 2023-06-04 17:07:28.000000 autoviz-0.1.72/autoviz.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2023-06-04 17:07:28.000000 autoviz-0.1.72/autoviz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-06-04 17:07:28.000000 autoviz-0.1.72/autoviz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      257 2023-06-04 17:07:28.000000 autoviz-0.1.72/autoviz.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-06-04 17:07:28.000000 autoviz-0.1.72/autoviz.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-06-04 17:07:29.410936 autoviz-0.1.72/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1231 2023-06-04 17:06:51.000000 autoviz-0.1.72/setup.py
```

### Comparing `autoviz-0.1.71/PKG-INFO` & `autoviz-0.1.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.71
+Version: 0.1.72
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](images/logo.png)
```

### Comparing `autoviz-0.1.71/README.md` & `autoviz-0.1.72/README.md`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.71/autoviz/AutoViz_Class.py` & `autoviz-0.1.72/autoviz/AutoViz_Class.py`

 * *Files 21% similar despite different names*

```diff
@@ -55,18 +55,25 @@
 import traceback
 import xgboost as xgb
 from xgboost.sklearn import XGBClassifier
 from xgboost.sklearn import XGBRegressor
 from sklearn.model_selection import train_test_split
 ##########################################################################################
 from autoviz.AutoViz_Holo import AutoViz_Holo
-from autoviz.AutoViz_Utils import *
+from autoviz.AutoViz_Utils import save_image_data, save_html_data, analyze_problem_type, draw_pivot_tables, draw_scatters
+from autoviz.AutoViz_Utils import draw_pair_scatters, plot_fast_average_num_by_cat, draw_barplots, draw_heatmap
+from autoviz.AutoViz_Utils import draw_distplot, draw_violinplot, draw_date_vars, catscatter, draw_catscatterplots
+from autoviz.AutoViz_Utils import list_difference, search_for_word_in_list, analyze_ID_columns, start_classifying_vars
+from autoviz.AutoViz_Utils import analyze_columns_in_dataset, find_remove_duplicates, load_file_dataframe, classify_print_vars
+from autoviz.AutoViz_Utils import marthas_columns, EDA_find_remove_columns_with_infinity, return_dictionary_list
+from autoviz.AutoViz_Utils import remove_variables_using_fast_correlation, count_freq_in_list, find_corr_vars, left_subtract
+from autoviz.AutoViz_Utils import convert_train_test_cat_col_to_numeric, return_factorized_dict, convert_a_column_to_numeric
+from autoviz.AutoViz_Utils import convert_all_object_columns_to_numeric, find_top_features_xgb, convert_a_mixed_object_column_to_numeric
 from autoviz.AutoViz_NLP import draw_word_clouds
-from autoviz.classify_method import data_suggestions
-#####################################################
+#############################################################################################
 class AutoViz_Class():
     """
         ##############################################################################
         #############       This is not an Officially Supported Google Product! ######
         ##############################################################################
         #Copyright 2019 Google LLC                                              ######
         #                                                                       ######
@@ -203,34 +210,14 @@
         """
         if X is None:
             ### If there is nothing to add, leave it as it is.
             pass
         else:
             getattr(self,plotname)["subheading"].append(X)
 
-    def give_data_suggestions(self, X):
-        """
-        This is a simple program to give data cleaning and improvement suggestions in class AV. 
-        Make sure you send in a dataframe. Otherwise, this will give an error.
-        """
-        return self.get_data_suggestions(X)
-
-    def get_data_suggestions(self, X):
-        """
-        This is a simple program to give data cleaning and improvement suggestions in class AV. 
-        Make sure you send in a dataframe. Otherwise, this will give an error.
-        """
-        if isinstance(X, pd.DataFrame):
-            dfx = data_suggestions(X)
-            all_rows = dfx.shape[0]
-            ax = dfx.head(all_rows).style.background_gradient(cmap='Reds').set_properties(**{'font-family': 'Segoe UI'})
-            display(ax);
-        else:
-            print("Input must be a dataframe. Please check input and try again.")
-
     def AutoViz(self, filename, sep=',', depVar='', dfte=None, header=0, verbose=1,
                             lowess=False,chart_format='svg',max_rows_analyzed=150000,
                                 max_cols_analyzed=30, save_plot_dir=None):
         """
         ##############################################################################
         ##### AUTOVIZ PERFORMS AUTOMATIC VISUALIZATION OF ANY DATA SET WITH ONE CLICK.
         #####    Give it any input file (CSV, txt or json) and AV will visualize it.##
@@ -312,14 +299,19 @@
         try:
             dft, depVar,IDcols,bool_vars,cats,continuous_vars,discrete_string_vars,date_vars,classes,problem_type,selected_cols = classify_print_vars(
                                                 filename,sep,max_rows_analyzed, max_cols_analyzed,
                                                 depVar,dfte,header,verbose)
         except:
             print('Not able to read or load file. Please check your inputs and try again...')
             return None
+        ###########  This is where perform data quality checks on data ################
+        if verbose >= 1:
+            print('To fix data quality issues automatically, import FixDQ from autoviz...')
+            data_cleaning_suggestions(dft, target=depVar)
+
         ##### This is where we start plotting different kinds of charts depending on dependent variables
         if depVar == None or depVar == '':
          ##### This is when No dependent Variable is given #######
             if len(continuous_vars) > 1:
                 try:
                     svg_data = draw_pair_scatters(dft,continuous_vars,problem_type,verbose,chart_format,
                                                     depVar,classes,lowess, mk_dir)
@@ -549,7 +541,65 @@
         else:
             print('All Plots are saved in %s' %mk_dir)
         print('Time to run AutoViz = %0.0f seconds ' %(time.time()-start_time))
         if verbose <= 1:
             print ('\n ###################### AUTO VISUALIZATION Completed ########################')
         return dft
 #############################################################################################
+from pandas_dq import Fix_DQ
+# Create a new class FixDQ by inheriting from Fix_DQ
+class FixDQ(Fix_DQ):
+    """
+    FixDQ is a great way to clean an entire train data set and apply the same steps in 
+    an MLOps pipeline to a test dataset. FixDQ can be used to detect most issues in 
+    your data (similar to data_cleaning_suggestions but without the `target` 
+    related issues) in one step. Then it fixes those issues it finds during the 
+    `fit` method by the `transform` method. This transformer can then be saved 
+    (or "pickled") for applying the same steps on test data either at the same 
+    time or later.
+
+    FixDQ will perform following data quality cleaning steps:
+        It removes ID columns from further processing
+        It removes zero-variance columns from further processing
+        It identifies rare categories and groups them into a single category 
+                    called "Rare"
+        It finds infinite values and replaces them with an upper bound based on 
+                    Inter Quartile Range
+        It detects mixed data types and drops those mixed-type columns from 
+                    further processing
+        It detects outliers and suggests to remove them or use robust statistics.
+        It detects high cardinality features but leaves them as it is.
+        It detects highly correlated features and drops one of them (whichever 
+                    comes first in the column sequence)
+        It detects duplicate rows and drops one of them or keeps only one copy 
+                    of duplicate rows
+        It detects duplicate columns and drops one of them or keeps only one copy
+        It detects skewed distributions and applies log or box-cox 
+                    transformations on them
+        It detects imbalanced classes and leaves them as it is
+        It detects feature leakage and drops one of those features if 
+                    they are highly correlated to target
+    """
+    def __init__(self, quantile=0.87, cat_fill_value = 'missing', 
+                num_fill_value = 9999, rare_threshold = 0.01, 
+                correlation_threshold = 0.9):
+        super().__init__()  # Call the parent class constructor
+        # Additional initialization code here
+        self.quantile = quantile
+        self.cat_fill_value = cat_fill_value
+        self.num_fill_value = num_fill_value
+        self.rare_threshold = rare_threshold
+        self.correlation_threshold = correlation_threshold
+
+###################################################################################
+from pandas_dq import dq_report
+def data_cleaning_suggestions(df, target=None):
+    """
+    This is a simple program to give data cleaning and improvement suggestions in class AV.
+    Make sure you send in a dataframe. Otherwise, this will give an error.
+    """
+    if isinstance(df, pd.DataFrame):
+        dqr = dq_report(data=df, target=target, html=False, csv_engine="pandas", verbose=1)
+    else:
+        print("Input must be a dataframe. Please check input and try again.")
+    return dqr
+###################################################################################
```

### Comparing `autoviz-0.1.71/autoviz/AutoViz_Holo.py` & `autoviz-0.1.72/autoviz/AutoViz_Holo.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.71/autoviz/AutoViz_NLP.py` & `autoviz-0.1.72/autoviz/AutoViz_NLP.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.71/autoviz/AutoViz_Utils.py` & `autoviz-0.1.72/autoviz/AutoViz_Utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,15 +780,15 @@
                 conti += [dep]
         ### Be very careful with the next line. we have used the plural "subplots" ##
         ## In this case, you have ax as an array and you have to use (row,col) to get each ax!
         ########## This is where you insert the logic for distplots ##############
         #sns.color_palette("Set1")
         sns.set_palette("Set1")
         ##### First draw all the numeric variables in row after row #############
-        if not len(conti) == 0:
+        if len(conti) > 0:
             cols = 3
             rows = len(conti)
             fig, axes = plt.subplots(rows, cols, figsize=(width_size,rows*height_size))
             fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows            
             k = 1
             binsize = 30
             for each_conti in conti:
@@ -815,15 +815,15 @@
                 ax3.set_title(each_conti + " | Probability Plot - Skew: "+str(skew_val), fontsize=9)
             ###### Save the plots to disk if verbose = 2 ############
             if verbose == 2:
                 imgdata_list.append(save_image_data(fig, chart_format,
                                 plot_name+'_Numeric', dep, mk_dir))
                 image_count += 1
         #####  Now draw each of the categorical variable distributions in each subplot ####
-        if not len(cats) == 0:
+        if len(cats) > 0:
             cols = 2
             noplots = len(cats)
             rows = int((noplots/cols)+0.99 )
             k = 0
             fig = plt.figure(figsize=(width_size,rows*height_size))
             fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows            
             for each_cat in copy_cats:
@@ -1033,15 +1033,15 @@
     sns.set_palette("Set1")
     if modeltype == 'Regression' or dep == None or dep == '':
         image_count = 0
         if modeltype == 'Regression':
             nums = nums + [dep]
         numb = len(nums)
         if numb > number_in_each_row:
-            rows = int(numb/number_in_each_row)+1
+            rows = int((numb/number_in_each_row)+.99)
         else:
             rows = 1
         plot_index = 0
         for row in range(rows):
             plot_index += 1
             first_10 = number_in_each_row*row
             next_10 = first_10 + number_in_each_row
```

### Comparing `autoviz-0.1.71/autoviz/classify_method.py` & `autoviz-0.1.72/autoviz/classify_method.py`

 * *Files 20% similar despite different names*

```diff
@@ -284,19 +284,14 @@
         print("    Number of String-Boolean Columns = ", len(string_bool_vars))
         print("    Number of Numeric-Boolean Columns = ", len(num_bool_vars))
         print("    Number of Discrete String Columns = ", len(discrete_string_vars))
         print("    Number of NLP String Columns = ", len(nlp_vars))
         print("    Number of Date Time Columns = ", len(date_vars))
         print("    Number of ID Columns = ", len(id_vars))
         print("    Number of Columns to Delete = ", len(cols_delete))
-    if verbose >= 1:
-        dfx = data_suggestions(df_preds)
-        all_rows = dfx.shape[0]
-        ax = dfx.head(all_rows).style.background_gradient(cmap='Reds').set_properties(**{'font-family': 'Segoe UI'})#.hide(axis='index')
-        display(ax);
     if verbose >= 2:
         print('  Printing upto %d columns max in each category:' %max_cols_to_print)
         print("    Numeric Columns : %s" %continuous_vars[:max_cols_to_print])
         print("    Integer-Categorical Columns: %s" %int_vars[:max_cols_to_print])
         print("    String-Categorical Columns: %s" %cat_vars[:max_cols_to_print])
         print("    Factor-Categorical Columns: %s" %factor_vars[:max_cols_to_print])
         print("    String-Boolean Columns: %s" %string_bool_vars[:max_cols_to_print])
@@ -319,122 +314,8 @@
         flat_list = [item for sublist in ls for item in sublist]
         if len(left_subtract(list(train),flat_list)) == 0:
             print(' Missing columns = None')
         else:
             print(' Missing columns = %s' %left_subtract(list(train),flat_list))
     return sum_all_cols
 ####################################################################################
-from scipy.stats import probplot,skew
-def data_suggestions(data):
-    """
-    Modified by Ram Seshadri. Original idea for data suggestions module was a Kaggler.
-    Many thanks to: https://www.kaggle.com/code/itkin16/catboost-on-gpu-baseline
-    """
-    maxx = []
-    minn = []
-    all_cols = list(data)
-    cat_cols1 = data.select_dtypes(include='object').columns.tolist()
-    cat_cols2 = data.select_dtypes(include='category').columns.tolist()
-    cat_cols = list(set(cat_cols1+cat_cols2))
-    ### The next line may look odd but due to different versions of pandas which
-    ### treat the definition of float differently, I am forced to use this. Don't change it.
-    num_cols = data.select_dtypes(include='float16').columns.tolist() + data.select_dtypes(
-                    include='float32').columns.tolist() + data.select_dtypes(include='float64').columns.tolist()
-    non_num_cols = left_subtract(all_cols, num_cols)
-    for i in data.columns:
-        if i not in cat_cols:
-            ### for float and integer, no need to calculate this ##
-            minn.append(0)
-        else:
-            minn.append(data[i].value_counts().min())
-    length = len(data)
-    nunik = data.nunique()
-    nulls = data.isna().sum()
-    df = pd.DataFrame(
-        {
-         #'column': list(data),
-         'Nullpercent' : 100*(nulls/length),
-         'NuniquePercent': (100*(nunik/length)),
-         'dtype': data.dtypes,
-        'Nuniques': nunik,
-         'Nulls' : nulls,
-         'Least num. of categories':minn
-        },
-        columns = ['Nullpercent', 'NuniquePercent','dtype','Nuniques', 'Nulls',
-                       'Least num. of categories']).sort_values(by = 'Nullpercent',ascending = False)
-    newcol = 'Data cleaning improvement suggestions'
-    print('%s. Complete them before proceeding to ML modeling.' %newcol)
-    mixed_cols = [col for col in data.columns if len(data[col].apply(type).value_counts()) > 1]
-    df[newcol] = ''
-    df['first_comma'] = ''
-    if len(cat_cols) > 0:
-        mask0 = df['dtype'] == 'object'
-        mask1 = df['Least num. of categories']/df['Nuniques'] <= 0.05
-        mask4 = df['dtype'] == 'category'
-        df.loc[mask0&mask1,newcol] += df.loc[mask0&mask1,'first_comma'] + 'combine rare categories'
-        df.loc[mask4&mask1,newcol] += df.loc[mask4&mask1,'first_comma'] + 'combine rare categories'
-        df.loc[mask0&mask1,'first_comma'] = ', '
-        df.loc[mask4&mask1,'first_comma'] = ', '
-    mask2 = df['Nulls'] > 0
-    df.loc[mask2,newcol] += df.loc[mask2,'first_comma'] + 'fill missing values'
-    df.loc[mask2,'first_comma'] = ", "
-    mask3 = df['Nuniques'] == 1
-    df.loc[mask3,newcol] += df.loc[mask3,'first_comma'] + 'invariant values: drop'
-    df.loc[mask3,'first_comma'] = ", "
-    if len(non_num_cols) > 0:
-        for x in non_num_cols:
-            if df.loc[x, 'NuniquePercent'] == 100:
-                df.loc[x, newcol] += df.loc[x,'first_comma'] + 'possible ID column: drop'
-                df.loc[x,'first_comma'] = ", "
-    mask5 = df['Nullpercent'] >= 90
-    df.loc[mask5,newcol] += df.loc[mask5,'first_comma'] + 'very high nulls percent: drop'
-    df.loc[mask5,'first_comma'] = ", "
-    #### check for infinite values here #####
-    inf_cols1 = np.array(num_cols)[[(data.loc[(data[col] == np.inf)]).shape[0]>0 for col in num_cols]].tolist()
-    inf_cols2 = np.array(num_cols)[[(data.loc[(data[col] == -np.inf)]).shape[0]>0 for col in num_cols]].tolist()
-    inf_cols = list(set(inf_cols1+inf_cols2))
-    ### Check for infinite values in columns #####
-    if len(inf_cols) > 0:
-        for x in inf_cols:
-            df.loc[x,newcol] += df.loc[x,'first_comma'] + 'infinite values: drop'
-            df.loc[x,'first_comma'] = ", "
-    #### Check for skewed float columns #######
-    skew_cols1 = np.array(num_cols)[[(np.abs(np.round(data[col].skew(), 1)) >= 1
-                    ) & (np.abs(np.round(data[col].skew(), 1)) <= 5) for col in num_cols]].tolist()
-    skew_cols2 = np.array(num_cols)[[(np.abs(np.round(data[col].skew(), 1)) > 5) for col in num_cols]].tolist()
-    skew_cols = list(set(skew_cols1+skew_cols2))
-    ### Check for skewed values in columns #####
-    if len(skew_cols1) > 0:
-        for x in skew_cols1:
-            if data[x].skew() < 0:
-                df.loc[x,newcol] += df.loc[x,'first_comma'] + 'left skewed distribution: cap or drop outliers'
-            else:
-                df.loc[x,newcol] += df.loc[x,'first_comma'] + 'right skewed distribution: cap or drop outliers'
-            df.loc[x,'first_comma'] = ", "
-    if len(skew_cols2) > 0:
-        for x in skew_cols2:
-            if data[x].skew() < 0:
-                df.loc[x,newcol] += df.loc[x,'first_comma'] + 'highly left skewed distribution: drop outliers or do box-cox transform'
-            else:
-                df.loc[x,newcol] += df.loc[x,'first_comma'] + 'highly right skewed distribution: drop outliers or do box-cox transform'
-            df.loc[x,'first_comma'] = ", "
-    ##### Do the same for mixed dtype columns - they must be fixed! ##
-    if len(mixed_cols) > 0:
-        for x in mixed_cols:
-            df.loc[x,newcol] += df.loc[x,'first_comma'] + 'fix mixed data types'
-            df.loc[x,'first_comma'] = ", "
-    df.drop('first_comma', axis=1, inplace=True)
-    return df
-###################################################################################
-def data_cleaning_suggestions(df):
-    """
-    This is a simple program to give data cleaning and improvement suggestions in class AV.
-    Make sure you send in a dataframe. Otherwise, this will give an error.
-    """
-    if isinstance(df, pd.DataFrame):
-        dfx = data_suggestions(df)
-        all_rows = dfx.shape[0]
-        ax = dfx.head(all_rows).style.background_gradient(cmap='Reds').set_properties(**{'font-family': 'Segoe UI'})
-        display(ax);
-    else:
-        print("Input must be a dataframe. Please check input and try again.")
-###################################################################################
+
```

### Comparing `autoviz-0.1.71/autoviz.egg-info/PKG-INFO` & `autoviz-0.1.72/autoviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.71
+Version: 0.1.72
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](images/logo.png)
```

### Comparing `autoviz-0.1.71/setup.py` & `autoviz-0.1.72/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autoviz",
-    version="0.1.71",
+    version="0.1.72",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Automatically Visualize any dataset, any size with a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/AutoViz",
```

