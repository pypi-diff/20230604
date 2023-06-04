# Comparing `tmp/henxel-0.1.8.tar.gz` & `tmp/henxel-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henxel-0.1.8.tar", last modified: Thu May 18 16:13:31 2023, max compression
+gzip compressed data, was "henxel-0.1.9.tar", last modified: Sun Jun  4 11:13:06 2023, max compression
```

## Comparing `henxel-0.1.8.tar` & `henxel-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-05-18 16:13:31.968646 henxel-0.1.8/
--rw-r--r--   0 samuel    (1000) samuel    (1000)    34801 2023-02-23 18:22:17.000000 henxel-0.1.8/LICENSE
--rw-r--r--   0 samuel    (1000) samuel    (1000)       50 2023-05-18 15:46:16.000000 henxel-0.1.8/MANIFEST.in
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5051 2023-05-18 16:13:31.968646 henxel-0.1.8/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)     4406 2023-03-13 09:44:43.000000 henxel-0.1.8/README.md
--rw-r--r--   0 samuel    (1000) samuel    (1000)       98 2023-05-18 15:46:24.000000 henxel-0.1.8/pyproject.toml
--rw-r--r--   0 samuel    (1000) samuel    (1000)      765 2023-05-18 16:13:31.968646 henxel-0.1.8/setup.cfg
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-05-18 16:13:31.948645 henxel-0.1.8/src/
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-05-18 16:13:31.968646 henxel-0.1.8/src/henxel/
--rw-r--r--   0 samuel    (1000) samuel    (1000)    95376 2023-05-18 15:58:22.000000 henxel-0.1.8/src/henxel/__init__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     6358 2023-03-31 11:12:00.000000 henxel-0.1.8/src/henxel/changefont.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      359 2022-12-03 19:17:18.000000 henxel-0.1.8/src/henxel/editor.png
--rw-r--r--   0 samuel    (1000) samuel    (1000)     7218 2023-04-22 15:10:52.000000 henxel-0.1.8/src/henxel/fdialog.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     7523 2023-05-18 15:44:42.000000 henxel-0.1.8/src/henxel/help.txt
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-05-18 16:13:31.968646 henxel-0.1.8/src/henxel.egg-info/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5051 2023-05-18 16:13:31.000000 henxel-0.1.8/src/henxel.egg-info/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)      302 2023-05-18 16:13:31.000000 henxel-0.1.8/src/henxel.egg-info/SOURCES.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2023-05-18 16:13:31.000000 henxel-0.1.8/src/henxel.egg-info/dependency_links.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2023-05-18 16:13:31.000000 henxel-0.1.8/src/henxel.egg-info/top_level.txt
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-04 11:13:06.959526 henxel-0.1.9/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    34801 2023-02-23 18:22:17.000000 henxel-0.1.9/LICENSE
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       50 2023-05-18 15:46:16.000000 henxel-0.1.9/MANIFEST.in
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5074 2023-06-04 11:13:06.959526 henxel-0.1.9/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4429 2023-06-04 10:58:22.000000 henxel-0.1.9/README.md
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       98 2023-06-04 10:54:28.000000 henxel-0.1.9/pyproject.toml
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      765 2023-06-04 11:13:06.959526 henxel-0.1.9/setup.cfg
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-04 11:13:06.955526 henxel-0.1.9/src/
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-04 11:13:06.955526 henxel-0.1.9/src/henxel/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    98446 2023-06-04 10:53:55.000000 henxel-0.1.9/src/henxel/__init__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     6358 2023-05-24 09:37:41.000000 henxel-0.1.9/src/henxel/changefont.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      359 2022-12-03 19:17:18.000000 henxel-0.1.9/src/henxel/editor.png
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     7223 2023-06-04 10:51:13.000000 henxel-0.1.9/src/henxel/fdialog.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     7837 2023-06-04 10:51:13.000000 henxel-0.1.9/src/henxel/help.txt
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-04 11:13:06.955526 henxel-0.1.9/src/henxel.egg-info/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5074 2023-06-04 11:13:06.000000 henxel-0.1.9/src/henxel.egg-info/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      302 2023-06-04 11:13:06.000000 henxel-0.1.9/src/henxel.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2023-06-04 11:13:06.000000 henxel-0.1.9/src/henxel.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2023-06-04 11:13:06.000000 henxel-0.1.9/src/henxel.egg-info/top_level.txt
```

### Comparing `henxel-0.1.8/LICENSE` & `henxel-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `henxel-0.1.8/PKG-INFO` & `henxel-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henxel
-Version: 0.1.8
+Version: 0.1.9
 Summary: GUI-editor for Python development.
 Home-page: https://github.com/SamuelKos/henxel
 Author: SamuelKos
 Author-email: koskinens371@gmail.com
 Project-URL: Bug Tracker, https://github.com/SamuelKos/henxel/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -30,14 +30,15 @@
 * Show git-branch
 * Run current file
 * Search - Replace
 * Indent - Unindent
 * Comment - Uncomment
 * Syntax highlighting
 * Click to open errors
+* Parenthesis checking
 * Persistent configuration
 * Near persistent contents
 
 # Lacking
 * Auto-completion
 * Hinting
```

### Comparing `henxel-0.1.8/README.md` & `henxel-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 * Show git-branch
 * Run current file
 * Search - Replace
 * Indent - Unindent
 * Comment - Uncomment
 * Syntax highlighting
 * Click to open errors
+* Parenthesis checking
 * Persistent configuration
 * Near persistent contents
 
 # Lacking
 * Auto-completion
 * Hinting
```

### Comparing `henxel-0.1.8/src/henxel/__init__.py` & `henxel-0.1.9/src/henxel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,17 +307,14 @@
 		self.y_extra_offset = self.contents['highlightthickness'] + self.contents['bd'] + self.contents['pady']
 		# Needed in update_linenums() and sbset_override()
 		self.bbox_height = self.contents.bbox('@0,0')[3]
 		self.text_widget_height = self.scrollbar.winfo_height()
 				
 		self.contents['yscrollcommand'] = lambda *args: self.sbset_override(*args)
 		
-		self.contents.tag_config('match', background='lightyellow', foreground='black')
-		self.contents.tag_config('focus', background='lightgreen', foreground='black')
-		
 		self.contents.bind( "<Alt-Return>", lambda event: self.btn_open.invoke())
 		
 		self.contents.bind( "<Alt-l>", self.toggle_ln)
 		self.contents.bind( "<Control-f>", self.search)
 		
 		self.contents.bind( "<Control-s>", self.goto_linestart)
 		self.contents.bind( "<Control-i>", self.move_right)
@@ -499,15 +496,16 @@
 				'keywords',
 				'numbers',
 				'bools',
 				'strings',
 				'comments',
 				'breaks',
 				'calls',
-				'selfs'
+				'selfs',
+				'mismatch'
 				]
 		
 		self.boldfont = self.font.copy()
 		self.boldfont.config(weight='bold')
 		
 		self.contents.tag_config('keywords', font=self.boldfont, foreground='deep sky blue')
 		#self.contents.tag_config('tests', font=self.boldfont, foreground='khaki3')
@@ -515,16 +513,19 @@
 		self.contents.tag_config('comments', font=self.boldfont, foreground=gray)
 		self.contents.tag_config('breaks', font=self.boldfont, foreground=orange)
 		self.contents.tag_config('calls', font=self.boldfont, foreground=cyan)
 		
 		self.contents.tag_config('bools', foreground=magenta)
 		self.contents.tag_config('strings', foreground=green)
 		self.contents.tag_config('selfs', foreground=gray)
+		self.contents.tag_config('mismatch', background='brown1', foreground='white')
 		
 		# search tags have highest priority
+		self.contents.tag_config('match', background='lightyellow', foreground='black')
+		self.contents.tag_config('focus', background='lightgreen', foreground='black')
 		self.contents.tag_raise('match')
 		self.contents.tag_raise('focus')
 		
 		
 		self.oldline = ''
 		self.token_err = False
 		self.token_can_update = False
@@ -600,26 +601,26 @@
 		return 'continue'
 		
 	
 	def ensure_idx_visibility(self, index):
 		
 		self.contents.mark_set('insert', index)
 		s = self.contents.bbox('%s - 2lines' % index)
-		e = self.contents.bbox('%s + 2lines' % index)
+		e = self.contents.bbox('%s + 4lines' % index)
 		
 		tests = [
 				not s,
 				not e,
 				( s and s[1] < 0 )
 				]
 				
 		if any(tests):
 			self.contents.see('%s - 2lines' % index)
 			self.update_idletasks()
-			self.contents.see('%s + 2lines' % index)
+			self.contents.see('%s + 4lines' % index)
 			
 		
 	def quit_me(self):
 	
 		self.save(forced=True)
 		self.save_config()
 		
@@ -660,35 +661,37 @@
 		
 		# More info in update_linenums()
 		self.bbox_height = self.contents.bbox('@0,0')[3]
 		self.text_widget_height = self.scrollbar.winfo_height()
 		
 		self.update_linenums()
 		
-		if self.token_can_update:
-		
-			#  tag alter triggers this event if font changes, like from normal to bold.
-			# --> need to check if line is changed to prevent self-trigger
-			line_idx = self.contents.index( tkinter.INSERT )
-			linenum = line_idx.split('.')[0]
-			#prev_char = self.contents.get( '%s - 1c' % tkinter.INSERT )
-			
-			
-			lineend = '%s lineend' % line_idx
-			linestart = '%s linestart' % line_idx
-			
-			tmp = self.contents.get( linestart, lineend )
-			
-			if self.oldline != tmp or self.oldlinenum != linenum:
-			
-				#print('sync')
-				#print('sync')
-				self.oldline = tmp
-				self.oldlinenum = linenum
-				self.update_tokens(start=linestart, end=lineend, line=tmp)
+		if self.tabs[self.tabindex].filepath:
+			if self.can_do_syntax():
+				if self.token_can_update:
+				
+					#  tag alter triggers this event if font changes, like from normal to bold.
+					# --> need to check if line is changed to prevent self-trigger
+					line_idx = self.contents.index( tkinter.INSERT )
+					linenum = line_idx.split('.')[0]
+					#prev_char = self.contents.get( '%s - 1c' % tkinter.INSERT )
+					
+					
+					lineend = '%s lineend' % line_idx
+					linestart = '%s linestart' % line_idx
+					
+					tmp = self.contents.get( linestart, lineend )
+					
+					if self.oldline != tmp or self.oldlinenum != linenum:
+					
+						#print('sync')
+						#print('sync')
+						self.oldline = tmp
+						self.oldlinenum = linenum
+						self.update_tokens(start=linestart, end=lineend, line=tmp)
 				
 
 ############## Linenumbers Begin
 
 	def no_copy_ln(self, event=None):
 		return 'break'
 		
@@ -927,16 +930,17 @@
 			self.entry.insert(0, self.tabs[self.tabindex].filepath)
 			
 		
 		self.token_can_update = False
 		self.contents.delete('1.0', tkinter.END)
 		self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
 	
-		if self.can_do_syntax():
-			self.update_tokens(start='1.0', end=tkinter.END, everything=True)
+		if self.tabs[self.tabindex].filepath:
+			if self.can_do_syntax():
+				self.update_tokens(start='1.0', end=tkinter.END, everything=True)
 
 		# set cursor pos
 		line = self.tabs[self.tabindex].position
 		self.contents.focus_set()
 		
 		try:
 			self.contents.mark_set('insert', line)
@@ -949,23 +953,24 @@
 
 		
 		self.contents.edit_reset()
 		self.contents.edit_modified(0)
 		
 		# Until update_title: avoiding viewsync messing when cursor
 		# position is in line with multiline string marker.
-		if self.can_do_syntax():
-			pos = self.tabs[self.tabindex].position
-			lineend = '%s lineend' % pos
-			linestart = '%s linestart' % pos
-			tmp = self.contents.get( linestart, lineend )
-			self.oldline = tmp
-			self.oldlinenum = pos.split('.')[0]
-				
-			self.token_can_update = True
+		if self.tabs[self.tabindex].filepath:
+			if self.can_do_syntax():
+				pos = self.tabs[self.tabindex].position
+				lineend = '%s lineend' % pos
+				linestart = '%s linestart' % pos
+				tmp = self.contents.get( linestart, lineend )
+				self.oldline = tmp
+				self.oldlinenum = pos.split('.')[0]
+					
+				self.token_can_update = True
 			
 		
 		self.update_title()
 		
 		return 'break'
 
 ########## Tab Related End
@@ -1255,14 +1260,16 @@
 			
 		linenum = int(start_idx.split('.')[0])
 		flag_err = False
 		#print(self.token_err)
 		
 		
 		try:
+			par_err = None
+			
 			with io.BytesIO( tmp.encode('utf-8') ) as fo:
 			
 				tokens = tokenize.tokenize( fo.readline )
 			
 				# Remove old tags:
 				for tag in self.tagnames:
 					self.contents.tag_remove( tag, start_idx, end_idx )
@@ -1337,26 +1344,82 @@
 
 			# This Error needs info about whole block, one line is not enough, so quite rare.
 			#print( e.args[0], '\nIndentation errline: ', self.contents.index(tkinter.INSERT) )
 			
 			flag_err = True
 			self.token_err = True
 
-			
+		
 		except tokenize.TokenError as ee:
-			
-			# This could be used with something
-			#print( ee.args[0], '\nerrline: ', self.contents.index(tkinter.INSERT) )
-			#print(ee.args)
-			
+		
+			self.contents.tag_remove('mismatch', '%s linestart' % start_idx, '%s lineend' % start_idx )
+				
+			if 'EOF in multi-line statement' in ee.args[0]:
+				# Check for parenthes mismatch only in the scope of
+				# the current token update call. And not whole file
+				# all the time. When the first mismatch is corrected
+				# all mismatch-tags are removed later below.
+				par_err = ee
+			
+				# count pars
+				# if more lpar: show first lpar
+				# if more rpar: show last rpar
+				lpar = list()
+				rpar = list()
+				bra = list()
+				ket = list()
+				
+				for i in range(len(token.line)):
+					if token.line[i] == '(':
+						lpar.append(i)
+					elif token.line[i] == ')':
+						rpar.append(i)
+					elif token.line[i] == '[':
+						bra.append(i)
+					elif token.line[i] == ']':
+						ket.append(i)
+				
+				if len(lpar) > len(rpar):
+					ln = idx_start.split('.')[0]
+					col = token.line.index('(')
+					err_idx = '%s.%i' % (ln, col)
+					
+					self.contents.tag_add('mismatch', err_idx, '%s +1c' % err_idx)
+				
+					
+				elif len(lpar) < len(rpar):
+					ln = idx_start.split('.')[0]
+					col = token.line.rindex(')')
+					err_idx = '%s.%i' % (ln, col)
+					
+					self.contents.tag_add('mismatch', err_idx, '%s +1c' % err_idx)
+				
+				elif len(bra) > len(ket):
+					ln = idx_start.split('.')[0]
+					col = token.line.index('[')
+					err_idx = '%s.%i' % (ln, col)
+					
+					self.contents.tag_add('mismatch', err_idx, '%s +1c' % err_idx)
+				
+				elif len(bra) < len(ket):
+					ln = idx_start.split('.')[0]
+					col = token.line.rindex(']')
+					err_idx = '%s.%i' % (ln, col)
+					
+					self.contents.tag_add('mismatch', err_idx, '%s +1c' % err_idx)
+				
+				
 			if 'multi-line string' in ee.args[0]:
 				flag_err = True
 				self.token_err = True
 			
-																				
+		if not par_err:
+			# not always checking whole file for par mismatches, so clear
+			self.contents.tag_remove('mismatch', '1.0', tkinter.END)
+																					
 ##		if flag_err:
 ##			print('err')
 			
 
 		if not flag_err and ( start_idx == '1.0' and end_idx == tkinter.END ):
 			#print('ok')
 			self.token_err = False
@@ -1517,14 +1580,15 @@
 				self.fgcolor = self.fgdaycolor
 				self.bgcolor = self.bgdaycolor
 			
 			else:
 				self.fgcolor = self.fgnightcolor
 				self.bgcolor = self.bgnightcolor
 			
+			
 			self.contents.config(foreground=self.fgcolor, background=self.bgcolor,
 			insertbackground=self.fgcolor)
 			
 			self.ln_widget.config(foreground=self.fgcolor, background=self.bgcolor, selectbackground=self.bgcolor, selectforeground=self.fgcolor, inactiveselectbackground=self.bgcolor )
 			
 			
 	def chcolor(self, args, event=None):
@@ -1555,14 +1619,15 @@
 				self.fgdaycolor = tmpcolorfg
 				self.fgcolor = self.fgdaycolor
 			else:
 				self.fgnightcolor = tmpcolorfg
 				self.fgcolor = self.fgnightcolor
 		
 		try:
+		
 			self.contents.config(foreground=self.fgcolor, background=self.bgcolor,
 				insertbackground=self.fgcolor)
 				
 			self.ln_widget.config(foreground=self.fgcolor, background=self.bgcolor, selectbackground=self.bgcolor, selectforeground=self.fgcolor, inactiveselectbackground=self.bgcolor )
 		
 		except tkinter.TclError as e:
 			# because if closed editor, this survives
@@ -1979,29 +2044,33 @@
 		if len(tmp) > 1:
 			self.contents.tag_remove('sel', '1.0', tkinter.END)
 			
 			s = self.contents.index( '%s linestart' % line)
 			e = self.contents.index( 'insert lineend')
 			t = self.contents.get( s, e )
 			
-			if self.can_do_syntax():
-				self.update_tokens( start=s, end=e, line=t )
+			if self.tabs[self.tabindex].filepath:
+				if self.can_do_syntax():
+					self.update_tokens( start=s, end=e, line=t )
+					
 			
 			self.contents.tag_add('sel', line, tkinter.INSERT)
 			self.contents.mark_set('insert', line)
-	
+				
 			self.ensure_idx_visibility(line)
 			
+			
 		elif len(tmp) == 1 and tmp[-1][-1] == '\n':
 			s = self.contents.index( '%s linestart' % line)
 			e = self.contents.index( '%s lineend' % line)
 			t = self.contents.get( s, e )
 			
-			if self.can_do_syntax():
-				self.update_tokens( start=s, end=e, line=t )
+			if self.tabs[self.tabindex].filepath:
+				if self.can_do_syntax():
+					self.update_tokens( start=s, end=e, line=t )
 				
 		
 		return 'break'
 
 
 	def undo_override(self, event=None):
 		if self.state != 'normal':
@@ -2066,15 +2135,15 @@
 		
 		try:
 			tmp = self.contents.selection_get()
 			self.indent(event)
 			return 'break'
 			
 		except tkinter.TclError:
-			# No selection, continue to next bindtag
+			# No selection
 			return
 
 	
 	def backspace_override(self, event):
 		""" for syntax highlight
 		"""
 		
@@ -2083,14 +2152,16 @@
 			
 		try:
 			# Is there a selection?
 			self.contents.delete( tkinter.SEL_FIRST, tkinter.SEL_LAST )
 			
 			self.do_syntax()
 			
+			return 'break'
+			
 				
 		except tkinter.TclError:
 			# Deleting one letter
 		
 			# Rest is multiline string check
 			chars = self.contents.get( '%s - 3c' % tkinter.INSERT, '%s + 2c' % tkinter.INSERT )
 			
@@ -2706,14 +2777,29 @@
 				
 				if self.tabs[self.tabindex].filepath != None:
 					self.entry.delete(0, tkinter.END)
 					self.entry.insert(0, self.tabs[self.tabindex].filepath)
 					
 					
 					self.do_syntax()
+			
+				
+				# set cursor pos
+				try:
+					line = self.tabs[self.tabindex].position
+					self.contents.focus_set()
+					self.contents.mark_set('insert', line)
+					self.ensure_idx_visibility(line)
+					
+				except tkinter.TclError:
+					self.tabs[self.tabindex].position = '1.0'
+				
+				self.contents.edit_reset()
+				self.contents.edit_modified(0)
+				
 					
 				
 			# want to create new file with same contents:
 			else:
 				try:
 					with open(fpath_in_entry, 'w', encoding='utf-8') as f:
 						pass
@@ -3012,33 +3098,49 @@
 	def indent(self, event=None):
 		if self.state != 'normal':
 			self.bell()
 			
 		try:
 			startline = int(self.contents.index(tkinter.SEL_FIRST).split(sep='.')[0])
 			endline = int(self.contents.index(tkinter.SEL_LAST).split(sep='.')[0])
+			
+			start_idx = self.contents.index(tkinter.SEL_FIRST)
+			end_idx = self.contents.index(tkinter.SEL_LAST)
+					
+			self.contents.tag_remove('sel', '1.0', tkinter.END)
+			self.contents.tag_add('sel', start_idx, end_idx)
+			
+			
 			for linenum in range(startline, endline+1):
 				self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
 				self.contents.insert(tkinter.INSERT, '\t')
 			
+			
 			self.contents.mark_set(tkinter.INSERT, tkinter.SEL_FIRST)
 			self.contents.edit_separator()
 			
 		except tkinter.TclError:
 			pass
 			
 
 	def unindent(self, event=None):
 		if self.state != 'normal':
 			self.bell()
 			return "break"
 			
 		try:
-			startline = int(self.contents.index(tkinter.SEL_FIRST).split(sep='.')[0])
-			endline = int(self.contents.index(tkinter.SEL_LAST).split(sep='.')[0])
+			# unindenting curline only:
+			if len(self.contents.tag_ranges('sel')) == 0:
+				startline = int( self.contents.index(tkinter.INSERT).split(sep='.')[0] )
+				endline = startline
+
+			else:
+				startline = int(self.contents.index(tkinter.SEL_FIRST).split(sep='.')[0])
+				endline = int(self.contents.index(tkinter.SEL_LAST).split(sep='.')[0])
+				
 			# Check there is enough space in every line:
 			flag_continue = True
 			
 			for linenum in range(startline, endline+1):
 				tmp = self.contents.get('%s.0' % linenum, '%s.0 lineend' % linenum)
 				
 				if len(tmp) != 0 and tmp[0] != '\t':
@@ -3046,18 +3148,24 @@
 					break
 				
 			if flag_continue:
 				for linenum in range(startline, endline+1):
 					tmp = self.contents.get('%s.0' % linenum, '%s.0 lineend' % linenum)
 				
 					if len(tmp) != 0:
-						self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
-						self.contents.delete(tkinter.INSERT, '%s+%dc' % (tkinter.INSERT, 1))
+						if len(self.contents.tag_ranges('sel')) != 0:
+							self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
+							self.contents.delete(tkinter.INSERT, '%s+%dc' % (tkinter.INSERT, 1))
 						
-				self.contents.mark_set(tkinter.INSERT, tkinter.SEL_FIRST)
+						else:
+							self.contents.delete( '%s.0' % linenum, '%s.0 +1c' % linenum)
+						
+				if len(self.contents.tag_ranges('sel')) != 0:
+					self.contents.mark_set(tkinter.INSERT, tkinter.SEL_FIRST)
+				
 				self.contents.edit_separator()
 		
 		except tkinter.TclError as e:
 			pass
 			
 		return "break"
```

### Comparing `henxel-0.1.8/src/henxel/changefont.py` & `henxel-0.1.9/src/henxel/changefont.py`

 * *Files identical despite different names*

### Comparing `henxel-0.1.8/src/henxel/fdialog.py` & `henxel-0.1.9/src/henxel/fdialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 					highlightthickness=0, bg='#d9d9d9')
 		self.files.configure(font=self.font, width=30, selectmode='single', bd=4,
 					highlightthickness=0, bg='#d9d9d9')
 		
 		self.dirsbar.configure(width=30, elementborderwidth=4)
 		self.filesbar.configure(width=30, elementborderwidth=4)
 		
+		
 		self.dirs.bind('<Double-ButtonRelease-1>', self.chdir)
 		self.dirs.bind('<Return>', self.chdir)
 		self.dirs.bind('<Tab>', self.nogoto_emptylist)
 		
 		self.dirs.bind('<Up>', self.carousel)
 		self.dirs.bind('<Down>', self.carousel)
 		self.files.bind('<Up>', self.carousel)
@@ -100,36 +101,36 @@
 		
 		self.entry.grid_configure(row=0, column = 0, columnspan=4, sticky='sew')
 		self.dirsbar.grid_configure(row=1, column = 0, sticky='nsw')
 		self.dirs.grid_configure(row=1, column = 1, sticky='nsew')
 		self.files.grid_configure(row=1, column = 2, sticky='nsew')
 		self.filesbar.grid_configure(row=1, column = 3, sticky='nse')
 		
+			
 		self.update_view()
 		
 		#################### init end ################
-		
+	
 	
 	def carousel(self, event=None):
-		
 		if event.widget.size() > 1:
-		
+			
 			idx = event.widget.index('active')
 			idx_last_file = event.widget.size() - 1
 			
 			if event.keysym == 'Up' and idx == 0:
 				event.widget.activate(idx_last_file)
 				event.widget.see(idx_last_file)
 				
 				return 'break'
 			
 			elif event.keysym == 'Down' and idx == idx_last_file:
 				event.widget.activate(0)
 				event.widget.see(0)
-				
+					
 				return 'break'
 				
 	
 	def nogoto_emptylist(self, event=None):
 		'''	prevent tabbing into empty file-box.
 			Tab to same line from dirs to files if possible.
 		'''
```

### Comparing `henxel-0.1.8/src/henxel/help.txt` & `henxel-0.1.9/src/henxel/help.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 		Ctrl-b  Move cursor left
 		Ctrl-n  Move cursor down
 		Ctrl-p  Move cursor up
 		Ctrl-e  Move cursor to lineend
 		Ctrl-s  Move cursor to linestart
 		Ctrl-k  Remove from cursor to lineend
 		
+		Ctrl-up		Move cursor one paragraph up
+		Ctrl-down	Move cursor one paragraph down
+		
 		Ctrl-left  		Move cursor one word left
 		Ctrl-right 		Move cursor one word right
 		Ctrl-shift-left 	Select one more word to left
 		Ctrl-shift-right	Select one more word to right
 		
 		Ctrl-plus 	Increase scrollbar-width
 		Ctrl-minus	Decrease scrollbar-width
@@ -147,15 +150,21 @@
 	  - When copying, select additional empty line before block.
 		This ensures indentation of whole block. If you do not do this,
 		and select for example from 'def' - word, which has indentation,
 		then indentation of this first line is wrong when pasted, compared
 		to other lines. But editor moves cursor at the start of block so
 		you can start fixing indenting that function definition line or
 		similar.
+	
 		
+	How to: hide blinking cursor
+	  - Sometimes one wants to focus on the code and blinking cursor is
+		not helping with that. Since there is no timer to turn it off one
+		have to click on linenumber-widget to hide the cursor.
+	
 	
 	How to: change indent-depth
 		For all files:
 	  - If you started editor with: import henxel and e=henxel.Editor(),
 		then to change indent-depth in python-console:
 		e.change_indentation_width(8)
```

### Comparing `henxel-0.1.8/src/henxel.egg-info/PKG-INFO` & `henxel-0.1.9/src/henxel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henxel
-Version: 0.1.8
+Version: 0.1.9
 Summary: GUI-editor for Python development.
 Home-page: https://github.com/SamuelKos/henxel
 Author: SamuelKos
 Author-email: koskinens371@gmail.com
 Project-URL: Bug Tracker, https://github.com/SamuelKos/henxel/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -30,14 +30,15 @@
 * Show git-branch
 * Run current file
 * Search - Replace
 * Indent - Unindent
 * Comment - Uncomment
 * Syntax highlighting
 * Click to open errors
+* Parenthesis checking
 * Persistent configuration
 * Near persistent contents
 
 # Lacking
 * Auto-completion
 * Hinting
```

