# Comparing `tmp/asynkit-0.9.0.tar.gz` & `tmp/asynkit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynkit-0.9.0.tar", max compression
+gzip compressed data, was "asynkit-0.9.1.tar", max compression
```

## Comparing `asynkit-0.9.0.tar` & `asynkit-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1081 2023-06-03 12:49:45.045481 asynkit-0.9.0/LICENSE
--rw-r--r--   0        0        0    21296 2023-06-03 12:49:45.045481 asynkit-0.9.0/README.md
--rw-r--r--   0        0        0     2078 2023-06-03 12:49:45.045481 asynkit-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      124 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/compat.py
--rw-r--r--   0        0        0    17091 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/coroutine.py
--rw-r--r--   0        0        0        0 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/experimental/__init__.py
--rw-r--r--   0        0        0     4293 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/experimental/anyio.py
--rw-r--r--   0        0        0        0 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/__init__.py
--rw-r--r--   0        0        0     4164 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/default.py
--rw-r--r--   0        0        0     4815 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/eventloop.py
--rw-r--r--   0        0        0     2981 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/extensions.py
--rw-r--r--   0        0        0     2922 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/schedulingloop.py
--rw-r--r--   0        0        0      281 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/types.py
--rw-r--r--   0        0        0    10720 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/monitor.py
--rw-r--r--   0        0        0        0 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/py.typed
--rw-r--r--   0        0        0     5352 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/scheduling.py
--rw-r--r--   0        0        0     1209 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/tools.py
--rw-r--r--   0        0        0    22246 1970-01-01 00:00:00.000000 asynkit-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-04 21:35:04.612865 asynkit-0.9.1/LICENSE
+-rw-r--r--   0        0        0    22751 2023-06-04 21:35:04.612865 asynkit-0.9.1/README.md
+-rw-r--r--   0        0        0     2078 2023-06-04 21:35:04.616865 asynkit-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/compat.py
+-rw-r--r--   0        0        0    17639 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/coroutine.py
+-rw-r--r--   0        0        0        0 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/experimental/__init__.py
+-rw-r--r--   0        0        0     4293 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/experimental/anyio.py
+-rw-r--r--   0        0        0        0 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/__init__.py
+-rw-r--r--   0        0        0     4164 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/default.py
+-rw-r--r--   0        0        0     4815 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/eventloop.py
+-rw-r--r--   0        0        0     2981 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/extensions.py
+-rw-r--r--   0        0        0     2922 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/schedulingloop.py
+-rw-r--r--   0        0        0      281 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/types.py
+-rw-r--r--   0        0        0    10720 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/monitor.py
+-rw-r--r--   0        0        0        0 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/py.typed
+-rw-r--r--   0        0        0     5352 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/scheduling.py
+-rw-r--r--   0        0        0     1209 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/tools.py
+-rw-r--r--   0        0        0    23701 1970-01-01 00:00:00.000000 asynkit-0.9.1/PKG-INFO
```

### Comparing `asynkit-0.9.0/LICENSE` & `asynkit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.0/README.md` & `asynkit-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -108,30 +108,31 @@
 just as would happen if it were directly turned into a `Task`.
 
 `func_eager()` is a decorator which automatically applies `coro_eager()` to the coroutine returned by an async function.
 
 ## `coro_sync()` - Running coroutines synchronously
 
 If you are writing code which should work both synchronously and asynchronously,
-you can now write the code fully _async_ and then syn it _synchronously_ in the absence
-of an event loop.  Should the code cause any async features to be triggered, an exception is raised.  This helps avoid writing duplicate code.
+you can now write the code fully _async_ and then run it _synchronously_ in the absence
+of an event loop.  As long as the code doesn't _block_ (await unfinished _futures_) and doesn't try to access the event loop, it can successfully be executed.  This helps avoid writing duplicate code.
 
 ```python
-async def get_processed_data(datagetter):
+async def async_get_processed_data(datagetter):
     data = datagetter()  # could be an async callback
     data = await data if isawaitable(data) else data
     return process_data(data)
 
 
-# will raise SynchronousError if it datagetter to be async
+# raises SynchronousError if datagetter blocks
 def sync_get_processed_data(datagetter):
-    return asynkit.coro_sync(combine_stuff(cb1, cb2))
+    return asynkit.coro_sync(async_get_processed_data(datagetter))
 ```
 
 This sort of code might previously have been written thus:
+
 ```python
 # may return an awaitable
 def get_processed_data(datagetter):
     data = datagetter()
     if isawaitable(data):
         # return an awaitable helper function
         async def helper():
@@ -156,27 +157,62 @@
 
 The above pattern, writing async methods as sync and returning async helpers,
 is common in library code which needs to work both in synchronous and asynchronous
 context.  Needless to say, it is very convoluted, hard to debug and contains a lot
 of code duplication where the same logic is repeated inside async helper methods.
 
 Using `coro_sync()` it is possible to write the entire logic as `async` methods and
-then selectively fail if the logic tries to invoke any truly async operations.
+then simply fail if the code tries to invoke any truly async operations.
+If the invoked coroutine blocks, a `SynchronousError` is raised _from_ a `SynchronousAbort` exception which
+contains a traceback.  This makes it easy to pinpoint the location in the code where the
+async code blocked.  If the code tries to access the event loop, e.g. by creating a `Task`, a `RuntimeError` will be raised.  
+
 
 `coro_sync()` can also be applied as a decorator:
 
-```python
-@asynkit.coro_sync
-async def sync_function():
-    return "look ma, no async!"
+```pycon
+>>> @asynkit.coro_sync
+... async def sync_function():
+...     async def async_function():
+...         return "look, no async!"
+...     return await async_function()
+...
+>>> sync_function()
+'look, no async!'
+>>>
+```
 
+the `ensure_corofunc()` utility can be used when passing callbacks to async
+code, to ensure that the callbacks are async.  This, with `coro_sync()`, can help integrate
+synchronous code with async middleware:
 
-assert sync_function().contains("look")
+```python
+def sync_client(sync_callback):
+    middleware = AsyncMiddleware(asynkit.ensure_corofunc(sync_callback))
+    return asynkit.coro_sync(middleware.run())
 ```
 
+Using this pattern, one can avoid writing special synchronous versions of middleware, or having
+_hybrid_ methods which _optionally_ return awaitables:
+
+```python
+# the hybrid method antipattern
+def hybrid_method(callable):
+    """A hybrid method, possibly returning awaitable"""
+    data = callable()
+    if isawaitable(data):
+        # inner async method with duplicate code
+        async def async_helper(data):
+            data2 = await data
+            return process_data(data2)
+
+        return async_helper
+    else:
+        return process_data(data)  # duplicate code
+```
 
 ## `CoroStart`
 
 This class manages the state of a partially run coroutine and is what what powers the `coro_eager()` and `coro_sync()` functions. 
 When initialized, it will _start_ the coroutine, running it until it either suspends, returns, or raises
 an exception.  It can subsequently be _awaited_ to retreive the result.
 
@@ -291,14 +327,15 @@
 
 async def runner():
     m = Monitor()
     c = coro(m)
     while True:
         try:
             print(await m.aawait(c))
+            break
         except OOBData as oob:
             print(oob.data)
 ```
 
 which will result in the output
 
 ```
@@ -317,15 +354,16 @@
 the syntax:
 
 ```python
 m = Monitor()
 a = m.awaitable(coro(m))
 while True:
     try:
-        return await a
+        await a
+        break
     except OOBData as oob:
         handle_oob(oob.data)
 ```
 The returned awaitable is a `MonitorAwaitable` instance, and it can also be created
 directly:
 
 ```python
```

### Comparing `asynkit-0.9.0/pyproject.toml` & `asynkit-0.9.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asynkit"
-version = "0.9.0"
+version = "0.9.1"
 description = "Async toolkit for advanced scheduling"
 authors = ["Kristján Valur Jónsson <sweskman@gmail.com>"]
 repository = "https://github.com/kristjanvalur/py-asynkit"
 readme = "README.md"
 keywords = ["asyncio", "eventloop"]
 license = "MIT"
 classifiers = [
```

### Comparing `asynkit-0.9.0/src/asynkit/compat.py` & `asynkit-0.9.1/src/asynkit/compat.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.0/src/asynkit/coroutine.py` & `asynkit-0.9.1/src/asynkit/coroutine.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,22 +30,23 @@
 __all__ = [
     "CoroStart",
     "awaitmethod",
     "coro_await",
     "coro_eager",
     "func_eager",
     "eager",
+    "ensure_corofunc",
     "coro_get_frame",
     "coro_is_new",
     "coro_is_suspended",
     "coro_is_finished",
     "coro_iter",
     "coro_sync",
     "SynchronousError",
-    "CoroutineAbort",
+    "SynchronousAbort",
 ]
 
 PYTHON_37 = sys.version_info.major == 3 and sys.version_info.minor == 7
 
 T = TypeVar("T")
 S = TypeVar("S")
 P = ParamSpec("P")
@@ -60,15 +61,15 @@
 class SynchronousError(RuntimeError):
     """
     An exception thrown when a coroutine does not complete
     synchronously.
     """
 
 
-class CoroutineAbort(BaseException):
+class SynchronousAbort(BaseException):
     """
     Exception thrown into coroutine to abort it.
     """
 
 
 # Helpers to find if a coroutine (or a generator as created by types.coroutine)
 # has started or finished
@@ -537,19 +538,35 @@
     start = CoroStart[T](coro)
     if start.done():
         return start.result()
     # kill the coroutine
     try:
         # we can't use GeneratorExit because that gets special handling and
         # a traceback is not collected.
-        start.throw(CoroutineAbort())
+        start.throw(SynchronousAbort())
     except BaseException as err:
         raise SynchronousError("coroutine failed to complete synchronously") from err
     else:
         raise SynchronousError(
             "coroutine failed to complete synchronously (caught BaseException)"
         )
     finally:
         try:
             start.close()
         except RuntimeError:
             pass
+
+
+def ensure_corofunc(
+    callable: Union[Callable[P, T], Callable[P, Coroutine[Any, Any, T]]]
+) -> Callable[P, Coroutine[Any, Any, T]]:
+    """Make a callable async, so that the result needs to be awaited.
+    Useful for adding synchronous callbacs to async code.
+    """
+    if inspect.iscoroutinefunction(callable):
+        return callable
+
+    async def helper(*args: P.args, **kwargs: P.kwargs) -> T:
+        callable2 = cast(Callable[P, T], callable)
+        return callable2(*args, **kwargs)
+
+    return helper
```

### Comparing `asynkit-0.9.0/src/asynkit/experimental/anyio.py` & `asynkit-0.9.1/src/asynkit/experimental/anyio.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.0/src/asynkit/loop/default.py` & `asynkit-0.9.1/src/asynkit/loop/default.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.0/src/asynkit/loop/eventloop.py` & `asynkit-0.9.1/src/asynkit/loop/eventloop.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.0/src/asynkit/loop/extensions.py` & `asynkit-0.9.1/src/asynkit/loop/extensions.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.0/src/asynkit/loop/schedulingloop.py` & `asynkit-0.9.1/src/asynkit/loop/schedulingloop.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.0/src/asynkit/monitor.py` & `asynkit-0.9.1/src/asynkit/monitor.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.0/src/asynkit/scheduling.py` & `asynkit-0.9.1/src/asynkit/scheduling.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.0/src/asynkit/tools.py` & `asynkit-0.9.1/src/asynkit/tools.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.0/PKG-INFO` & `asynkit-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asynkit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Async toolkit for advanced scheduling
 Home-page: https://github.com/kristjanvalur/py-asynkit
 License: MIT
 Keywords: asyncio,eventloop
 Author: Kristján Valur Jónsson
 Author-email: sweskman@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -132,30 +132,31 @@
 just as would happen if it were directly turned into a `Task`.
 
 `func_eager()` is a decorator which automatically applies `coro_eager()` to the coroutine returned by an async function.
 
 ## `coro_sync()` - Running coroutines synchronously
 
 If you are writing code which should work both synchronously and asynchronously,
-you can now write the code fully _async_ and then syn it _synchronously_ in the absence
-of an event loop.  Should the code cause any async features to be triggered, an exception is raised.  This helps avoid writing duplicate code.
+you can now write the code fully _async_ and then run it _synchronously_ in the absence
+of an event loop.  As long as the code doesn't _block_ (await unfinished _futures_) and doesn't try to access the event loop, it can successfully be executed.  This helps avoid writing duplicate code.
 
 ```python
-async def get_processed_data(datagetter):
+async def async_get_processed_data(datagetter):
     data = datagetter()  # could be an async callback
     data = await data if isawaitable(data) else data
     return process_data(data)
 
 
-# will raise SynchronousError if it datagetter to be async
+# raises SynchronousError if datagetter blocks
 def sync_get_processed_data(datagetter):
-    return asynkit.coro_sync(combine_stuff(cb1, cb2))
+    return asynkit.coro_sync(async_get_processed_data(datagetter))
 ```
 
 This sort of code might previously have been written thus:
+
 ```python
 # may return an awaitable
 def get_processed_data(datagetter):
     data = datagetter()
     if isawaitable(data):
         # return an awaitable helper function
         async def helper():
@@ -180,27 +181,62 @@
 
 The above pattern, writing async methods as sync and returning async helpers,
 is common in library code which needs to work both in synchronous and asynchronous
 context.  Needless to say, it is very convoluted, hard to debug and contains a lot
 of code duplication where the same logic is repeated inside async helper methods.
 
 Using `coro_sync()` it is possible to write the entire logic as `async` methods and
-then selectively fail if the logic tries to invoke any truly async operations.
+then simply fail if the code tries to invoke any truly async operations.
+If the invoked coroutine blocks, a `SynchronousError` is raised _from_ a `SynchronousAbort` exception which
+contains a traceback.  This makes it easy to pinpoint the location in the code where the
+async code blocked.  If the code tries to access the event loop, e.g. by creating a `Task`, a `RuntimeError` will be raised.  
+
 
 `coro_sync()` can also be applied as a decorator:
 
-```python
-@asynkit.coro_sync
-async def sync_function():
-    return "look ma, no async!"
+```pycon
+>>> @asynkit.coro_sync
+... async def sync_function():
+...     async def async_function():
+...         return "look, no async!"
+...     return await async_function()
+...
+>>> sync_function()
+'look, no async!'
+>>>
+```
 
+the `ensure_corofunc()` utility can be used when passing callbacks to async
+code, to ensure that the callbacks are async.  This, with `coro_sync()`, can help integrate
+synchronous code with async middleware:
 
-assert sync_function().contains("look")
+```python
+def sync_client(sync_callback):
+    middleware = AsyncMiddleware(asynkit.ensure_corofunc(sync_callback))
+    return asynkit.coro_sync(middleware.run())
 ```
 
+Using this pattern, one can avoid writing special synchronous versions of middleware, or having
+_hybrid_ methods which _optionally_ return awaitables:
+
+```python
+# the hybrid method antipattern
+def hybrid_method(callable):
+    """A hybrid method, possibly returning awaitable"""
+    data = callable()
+    if isawaitable(data):
+        # inner async method with duplicate code
+        async def async_helper(data):
+            data2 = await data
+            return process_data(data2)
+
+        return async_helper
+    else:
+        return process_data(data)  # duplicate code
+```
 
 ## `CoroStart`
 
 This class manages the state of a partially run coroutine and is what what powers the `coro_eager()` and `coro_sync()` functions. 
 When initialized, it will _start_ the coroutine, running it until it either suspends, returns, or raises
 an exception.  It can subsequently be _awaited_ to retreive the result.
 
@@ -315,14 +351,15 @@
 
 async def runner():
     m = Monitor()
     c = coro(m)
     while True:
         try:
             print(await m.aawait(c))
+            break
         except OOBData as oob:
             print(oob.data)
 ```
 
 which will result in the output
 
 ```
@@ -341,15 +378,16 @@
 the syntax:
 
 ```python
 m = Monitor()
 a = m.awaitable(coro(m))
 while True:
     try:
-        return await a
+        await a
+        break
     except OOBData as oob:
         handle_oob(oob.data)
 ```
 The returned awaitable is a `MonitorAwaitable` instance, and it can also be created
 directly:
 
 ```python
```

