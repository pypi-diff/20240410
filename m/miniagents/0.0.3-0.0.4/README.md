# Comparing `tmp/miniagents-0.0.3.tar.gz` & `tmp/miniagents-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniagents-0.0.3.tar", max compression
+gzip compressed data, was "miniagents-0.0.4.tar", max compression
```

## Comparing `miniagents-0.0.3.tar` & `miniagents-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.3/LICENSE
--rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.3/miniagents/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.3/miniagents/ext/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.3/miniagents/ext/llms/__init__.py
--rw-r--r--   0        0        0     2900 2024-04-05 18:15:16.114673 miniagents-0.0.3/miniagents/ext/llms/anthropic.py
--rw-r--r--   0        0        0     5170 2024-04-04 17:06:05.253979 miniagents-0.0.3/miniagents/miniagents.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.726367 miniagents-0.0.3/miniagents/promisegraph/__init__.py
--rw-r--r--   0        0        0      563 2024-04-02 17:38:48.000619 miniagents-0.0.3/miniagents/promisegraph/errors.py
--rw-r--r--   0        0        0     2228 2024-03-27 07:32:21.726518 miniagents-0.0.3/miniagents/promisegraph/node.py
--rw-r--r--   0        0        0    12613 2024-04-03 21:42:22.426837 miniagents-0.0.3/miniagents/promisegraph/promise.py
--rw-r--r--   0        0        0      307 2024-04-02 17:38:48.002385 miniagents-0.0.3/miniagents/promisegraph/sentinels.py
--rw-r--r--   0        0        0     1748 2024-04-02 21:38:18.181306 miniagents-0.0.3/miniagents/promisegraph/sequence.py
--rw-r--r--   0        0        0     1482 2024-04-03 21:42:22.427374 miniagents-0.0.3/miniagents/promisegraph/typing.py
--rw-r--r--   0        0        0      694 2024-04-05 16:29:22.896313 miniagents-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.4/LICENSE
+-rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.4/miniagents/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.4/miniagents/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.4/miniagents/ext/llms/__init__.py
+-rw-r--r--   0        0        0     3749 2024-04-10 07:17:04.828930 miniagents-0.0.4/miniagents/ext/llms/anthropic.py
+-rw-r--r--   0        0        0     5545 2024-04-10 07:17:04.829863 miniagents-0.0.4/miniagents/miniagents.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.726367 miniagents-0.0.4/miniagents/promisegraph/__init__.py
+-rw-r--r--   0        0        0      563 2024-04-02 17:38:48.000619 miniagents-0.0.4/miniagents/promisegraph/errors.py
+-rw-r--r--   0        0        0     2228 2024-03-27 07:32:21.726518 miniagents-0.0.4/miniagents/promisegraph/node.py
+-rw-r--r--   0        0        0    17291 2024-04-10 07:17:04.830362 miniagents-0.0.4/miniagents/promisegraph/promise.py
+-rw-r--r--   0        0        0      337 2024-04-10 07:17:04.830846 miniagents-0.0.4/miniagents/promisegraph/sentinels.py
+-rw-r--r--   0        0        0     1838 2024-04-10 07:17:04.831287 miniagents-0.0.4/miniagents/promisegraph/sequence.py
+-rw-r--r--   0        0        0     1972 2024-04-10 07:17:04.831723 miniagents-0.0.4/miniagents/promisegraph/typing.py
+-rw-r--r--   0        0        0      694 2024-04-05 18:27:53.768905 miniagents-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.4/PKG-INFO
```

### Comparing `miniagents-0.0.3/LICENSE` & `miniagents-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.3/miniagents/ext/llms/anthropic.py` & `miniagents-0.0.4/miniagents/ext/llms/anthropic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,85 @@
 """
 This module integrates Anthropic language models with MiniAgents.
 """
 
 import typing
-from typing import AsyncIterator, Any, Optional
-
-from anthropic.types import ContentBlockDeltaEvent
+from typing import AsyncIterator, Any, Optional, Union
 
 from miniagents.miniagents import MessagePromise, MessageType, MessageSequence, Message
+from miniagents.promisegraph.promise import PromiseContext
+from miniagents.promisegraph.sentinels import Sentinel, DEFAULT
 
 if typing.TYPE_CHECKING:
     import anthropic as anthropic_original
 
 
 def anthropic(
     messages: MessageType,
-    schedule_immediately: bool = True,
-    collect_as_soon_as_possible: bool = True,
-    stream: bool = True,
+    schedule_immediately: Union[bool, Sentinel] = DEFAULT,
+    stream: Union[bool, Sentinel] = DEFAULT,
     async_client: Optional["anthropic_original.AsyncAnthropic"] = None,
     **kwargs,
 ) -> MessagePromise:
     """
     Run text generation with Anthropic.
     """
     if not async_client:
         # pylint: disable=import-outside-toplevel
+        # noinspection PyShadowingNames
         import anthropic as anthropic_original
 
         # TODO Oleksandr: instantiate the client only once (but still don't import `anthropic` at the module level)
         async_client = anthropic_original.AsyncAnthropic()
 
-    async def message_piece_producer(_: dict[str, Any]) -> AsyncIterator[str]:
-        # TODO Oleksandr: collect metadata_so_far
-        collected_messages = await MessageSequence.aflatten_and_collect(messages)
+    if stream is DEFAULT:
+        stream = PromiseContext().stream_llm_tokens_by_default
+
+    async def message_token_producer(metadata_so_far: dict[str, Any]) -> AsyncIterator[str]:
+        collected_messages = await MessageSequence.acollect_messages(messages)
         message_dicts = [_message_to_anthropic_dict(msg) for msg in collected_messages]
 
+        metadata_so_far["agent_call"] = {
+            "anthropic": {
+                "message_hash_keys": tuple(msg.hash_key for msg in collected_messages),
+                "stream": stream,
+                **kwargs,
+            },
+        }
+
         if stream:
-            response = await async_client.messages.create(messages=message_dicts, stream=True, **kwargs)
-            async for token in response:
-                if isinstance(token, ContentBlockDeltaEvent):
-                    yield token.delta.text
-            # # TODO Oleksandr: switch back to the version below when PromptLayer supports `text_stream`
-            # # pylint: disable=not-async-context-manager
-            # async with async_client.messages.stream(messages=message_dicts, **kwargs) as response:
-            #     async for token in response.text_stream:
-            #         yield token
+            # pylint: disable=not-async-context-manager
+            async with async_client.messages.stream(messages=message_dicts, **kwargs) as response:
+                async for token in response.text_stream:
+                    yield token
+                anthropic_final_message = await response.get_final_message()
+            # # TODO Oleksandr: if PromptLayer support is needed, but `text_stream` is still not supported by
+            # #  PromptLayer, switch back to the version of the code below. Here is a link to the related GitHub
+            # #  issue comment:
+            # #  - https://github.com/MagnivOrg/prompt-layer-library/issues/126#issuecomment-2040436402
+            # response = await async_client.messages.create(messages=message_dicts, stream=True, **kwargs)
+            # async for token in response:
+            #     if isinstance(token, ContentBlockDeltaEvent):
+            #         yield token.delta.text
         else:
-            response = await async_client.messages.create(messages=message_dicts, stream=False, **kwargs)
-            if len(response.content) != 1:
+            anthropic_final_message = await async_client.messages.create(
+                messages=message_dicts, stream=False, **kwargs
+            )
+            if len(anthropic_final_message.content) != 1:
                 raise RuntimeError(
-                    f"exactly one message should have been returned by Anthropic, "
-                    f"but {len(response.content)} were returned instead"
+                    f"exactly one TextBlock was expected from Anthropic, "
+                    f"but {len(anthropic_final_message.content)} were returned instead"
                 )
-            yield response.content[0].text  # yield the whole text as one "piece"
+            yield anthropic_final_message.content[0].text  # yield the whole text as one "piece"
+
+        metadata_so_far["anthropic"] = anthropic_final_message.model_dump(exclude={"content"})
 
     return MessagePromise(
-        message_piece_producer=message_piece_producer,
+        message_token_producer=message_token_producer,
         schedule_immediately=schedule_immediately,
-        collect_as_soon_as_possible=collect_as_soon_as_possible,
     )
 
 
 def _message_to_anthropic_dict(message: Message) -> dict[str, Any]:
     # TODO Oleksandr: introduce a lambda function to derive roles from messages ?
     try:
         role = message.role
```

### Comparing `miniagents-0.0.3/miniagents/miniagents.py` & `miniagents-0.0.4/miniagents/miniagents.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,114 +2,126 @@
 Split this module into multiple modules.
 """
 
 from typing import Protocol, AsyncIterator, Any, Union, Iterable, AsyncIterable, Optional
 
 from miniagents.promisegraph.node import Node
 from miniagents.promisegraph.promise import StreamedPromise
+from miniagents.promisegraph.sentinels import Sentinel, DEFAULT
 from miniagents.promisegraph.sequence import FlatSequence
 
 
 class Message(Node):
     """
     A message that can be sent between agents.
     """
 
     text: str
 
 
-class MessagePieceProducer(Protocol):
+class MessageTokenProducer(Protocol):
     """
     A protocol for message piece producer functions.
     """
 
     def __call__(self, metadata_so_far: dict[str, Any]) -> AsyncIterator[str]: ...
 
 
 class MessagePromise(StreamedPromise[str, Message]):
     """
     A promise of a message that can be streamed token by token.
     """
 
+    # pylint: disable=too-many-arguments
+
     def __init__(
         self,
-        schedule_immediately: bool = True,
-        collect_as_soon_as_possible: bool = True,
-        message_piece_producer: MessagePieceProducer = None,
+        schedule_immediately: Union[bool, Sentinel] = DEFAULT,
+        message_token_producer: MessageTokenProducer = None,
         prefill_message: Optional[Message] = None,
+        metadata_so_far: Optional[Node] = None,
     ) -> None:
-        # TODO Oleksandr: raise an error if both ready_message and message_piece_producer are not None
+        # TODO Oleksandr: raise an error if both ready_message and message_token_producer/metadata_so_far are not None
         #  (or both are None)
         if prefill_message:
             super().__init__(
                 schedule_immediately=schedule_immediately,
-                collect_as_soon_as_possible=collect_as_soon_as_possible,
                 prefill_pieces=[prefill_message.text],
                 prefill_whole=prefill_message,
             )
         else:
             super().__init__(
                 schedule_immediately=schedule_immediately,
-                collect_as_soon_as_possible=collect_as_soon_as_possible,
                 producer=self._producer,
                 packager=self._packager,
             )
-            self._message_piece_producer = message_piece_producer
-            self._metadata_so_far: dict[str, Any] = {}
+            self._message_token_producer = message_token_producer
+            self._metadata_so_far: dict[str, Any] = metadata_so_far.model_dump() if metadata_so_far else {}
 
     def _producer(self, _) -> AsyncIterator[str]:
-        return self._message_piece_producer(self._metadata_so_far)
+        return self._message_token_producer(self._metadata_so_far)
 
     async def _packager(self, _) -> Message:
         return Message(
             text="".join([token async for token in self]),
             **self._metadata_so_far,
         )
 
 
 # TODO Oleksandr: add documentation somewhere that explains what MessageType and SingleMessageType represent
 SingleMessageType = Union[str, dict[str, Any], Message, MessagePromise, BaseException]
 MessageType = Union[SingleMessageType, Iterable["MessageType"], AsyncIterable["MessageType"]]
 
 
+class MessageSequencePromise(StreamedPromise[MessagePromise, tuple[MessagePromise, ...]]):
+    """
+    A promise of a sequence of messages that can be streamed message by message.
+    """
+
+    async def acollect_messages(self) -> tuple[Message, ...]:
+        """
+        Collect all messages from the sequence and return them as a tuple of Message objects.
+        """
+        # pylint: disable=consider-using-generator
+        return tuple([await message_promise.acollect() async for message_promise in self])
+
+
 class MessageSequence(FlatSequence[MessageType, MessagePromise]):
     """
     TODO Oleksandr: produce a docstring for this class after you actually use it in real agents
     """
 
+    sequence_promise: MessageSequencePromise
+
     def __init__(
         self,
-        producer_capture_errors: bool,
-        schedule_immediately: bool = True,
-        collect_as_soon_as_possible: bool = False,
+        producer_capture_errors: Union[bool, Sentinel] = DEFAULT,
+        schedule_immediately: Union[bool, Sentinel] = DEFAULT,
     ) -> None:
-        self._schedule_immediately = schedule_immediately
-        self._collect_as_soon_as_possible = collect_as_soon_as_possible
         super().__init__(
             flattener=self._flattener,
             schedule_immediately=schedule_immediately,
-            collect_as_soon_as_possible=collect_as_soon_as_possible,
             producer_capture_errors=producer_capture_errors,
+            sequence_promise_class=MessageSequencePromise,
         )
 
     @classmethod
-    async def aflatten_and_collect(cls, messages: MessageType) -> list[Message]:
+    async def acollect_messages(cls, messages: MessageType) -> tuple[Message, ...]:
         """
         Convert an arbitrarily nested collection of messages of various types (strings, dicts, Message objects,
-        MessagePromise objects etc. - see `MessageType` definition for details) into a flat and uniform list of
+        MessagePromise objects etc. - see `MessageType` definition for details) into a flat and uniform tuple of
         Message objects.
         """
         message_sequence = cls(
             producer_capture_errors=True,
             schedule_immediately=False,
-            collect_as_soon_as_possible=False,
         )
         with message_sequence.append_producer:
             message_sequence.append_producer.append(messages)
-        return [await message_promise.acollect() async for message_promise in message_sequence.sequence_promise]
+        return await message_sequence.sequence_promise.acollect_messages()
 
     @staticmethod
     async def _flattener(_, zero_or_more_items: MessageType) -> AsyncIterator[MessagePromise]:
         if isinstance(zero_or_more_items, MessagePromise):
             yield zero_or_more_items
         elif isinstance(zero_or_more_items, Message):
             yield MessagePromise(prefill_message=zero_or_more_items)
@@ -117,15 +129,15 @@
             yield MessagePromise(prefill_message=Message(text=zero_or_more_items))
         elif isinstance(zero_or_more_items, dict):
             yield MessagePromise(prefill_message=Message(**zero_or_more_items))
         elif isinstance(zero_or_more_items, BaseException):
             raise zero_or_more_items
         elif hasattr(zero_or_more_items, "__iter__"):
             for item in zero_or_more_items:
-                async for message_promise in MessageSequence._flattener(None, item):
+                async for message_promise in MessageSequence._flattener(_, item):
                     yield message_promise
         elif hasattr(zero_or_more_items, "__aiter__"):
             async for item in zero_or_more_items:
-                async for message_promise in MessageSequence._flattener(None, item):
+                async for message_promise in MessageSequence._flattener(_, item):
                     yield message_promise
         else:
             raise TypeError(f"unexpected message type: {type(zero_or_more_items)}")
```

### Comparing `miniagents-0.0.3/miniagents/promisegraph/errors.py` & `miniagents-0.0.4/miniagents/promisegraph/errors.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.3/miniagents/promisegraph/node.py` & `miniagents-0.0.4/miniagents/promisegraph/node.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.3/miniagents/promisegraph/promise.py` & `miniagents-0.0.4/miniagents/promisegraph/promise.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,116 @@
 """
 The main class in this module is `StreamedPromise`. See its docstring for more information.
 """
 
 import asyncio
+import contextvars
+from asyncio import Task
+from contextvars import ContextVar
 from types import TracebackType
-from typing import Generic, AsyncIterator, Union, Optional, Iterable
+from typing import Generic, AsyncIterator, Union, Optional, Iterable, Awaitable, Any
 
 from miniagents.promisegraph.errors import AppendClosedError, AppendNotOpenError
-from miniagents.promisegraph.sentinels import Sentinel, NO_VALUE, FAILED, END_OF_QUEUE
-from miniagents.promisegraph.typing import PIECE, WHOLE, StreamedPieceProducer, StreamedWholePackager
+from miniagents.promisegraph.sentinels import Sentinel, NO_VALUE, FAILED, END_OF_QUEUE, DEFAULT
+from miniagents.promisegraph.typing import (
+    PIECE,
+    WHOLE,
+    StreamedPieceProducer,
+    StreamedWholePackager,
+    PromiseCollectedEventHandler,
+)
+
+
+class PromiseContext:
+    """
+    This is the main class for managing the context of promises. It is a context manager that is used to configure
+    default settings for promises and to handle the lifecycle of promises (attach `on_promise_collected` handlers).
+    TODO Oleksandr: explain this class in more detail
+    """
+
+    _current: ContextVar[Optional["PromiseContext"]] = ContextVar("PromiseContext._current", default=None)
+
+    def __init__(
+        self,
+        schedule_immediately_by_default: bool = True,
+        producer_capture_errors_by_default: bool = False,
+        stream_llm_tokens_by_default: bool = True,
+        on_promise_collected: Union[PromiseCollectedEventHandler, Iterable[PromiseCollectedEventHandler]] = (),
+    ) -> None:
+        self.parent = self._current.get()
+        self.on_promise_collected: list[PromiseCollectedEventHandler] = (
+            [on_promise_collected] if callable(on_promise_collected) else list(on_promise_collected)
+        )
+        self.child_tasks: set[Task] = set()
+
+        self.schedule_immediately_by_default = schedule_immediately_by_default
+        self.producer_capture_errors_by_default = producer_capture_errors_by_default
+        # TODO Oleksandr: move this setting to a child class (MiniAgents ?)
+        self.stream_llm_tokens_by_default = stream_llm_tokens_by_default
+
+        self._previous_ctx_token: Optional[contextvars.Token] = None
+
+    @classmethod
+    def get_current(cls) -> "PromiseContext":
+        """
+        Get the current context. If no context is currently active, raise an error.
+        """
+        current = cls._current.get()
+        if not current:
+            raise RuntimeError(
+                "No PromiseContext is currently active. Did you forget to do `async with PromiseContext():`?"
+            )
+        return current
+
+    def schedule_task(self, awaitable: Awaitable) -> Task:
+        """
+        Schedule a task in the current context. "Scheduling" a task this way instead of just creating it with
+        `asyncio.create_task()` allows the context to keep track of the child tasks and to wait for them to finish
+        before finalizing the context.
+        """
+
+        async def awaitable_wrapper() -> Any:
+            try:
+                return await awaitable
+            finally:
+                self.child_tasks.remove(task)
+
+        task = asyncio.create_task(awaitable_wrapper())
+        self.child_tasks.add(task)
+        return task
+
+    def activate(self) -> "PromiseContext":
+        """
+        Activate the context. This is a context manager method that is used to activate the context for the duration
+        of the `async with` block. Can be called as a regular method as well in cases where it is not possible to use
+        the `async with` block (e.g., if a PromiseContext needs to be activated for the duration of an async webserver
+        being up).
+        """
+        if self._previous_ctx_token:
+            raise RuntimeError("PromiseContext is not reentrant")
+        self._previous_ctx_token = self._current.set(self)  # <- this is the context switch
+        return self
+
+    async def afinalize(self) -> None:
+        """
+        Finalize the context (wait for all the child tasks to finish and reset the context). This method is called
+        automatically at the end of the `async with` block.
+        """
+        await asyncio.gather(
+            *self.child_tasks,
+            return_exceptions=True,  # this prevents waiting until the first exception and then giving up
+        )
+        self._current.reset(self._previous_ctx_token)
+        self._previous_ctx_token = None
+
+    async def __aenter__(self) -> "PromiseContext":
+        return self.activate()
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
+        await self.afinalize()
 
 
 class StreamedPromise(Generic[PIECE, WHOLE]):
     """
     A StreamedPromise represents a promise of a whole value that can be streamed piece by piece.
 
     The StreamedPromise allows for "replaying" the stream of pieces without involving the producer
@@ -20,58 +118,62 @@
     over the stream independently, and each consumer will receive all the pieces from the beginning,
     even if some pieces were produced before the consumer started iterating.
 
     :param producer: A callable that returns an async iterator yielding the pieces of the whole value.
     :param packager: A callable that takes an async iterable of pieces and returns the whole value
                      ("packages" the pieces).
     TODO Oleksandr: explain the `schedule_immediately` parameter
-    TODO Oleksandr: explain the `collect_as_soon_as_possible` parameter
     """
 
     # pylint: disable=too-many-instance-attributes,too-many-arguments
 
     def __init__(
         self,
-        schedule_immediately: bool,
-        collect_as_soon_as_possible: bool,
+        schedule_immediately: Union[bool, Sentinel] = DEFAULT,
         producer: Optional[StreamedPieceProducer[PIECE]] = None,
         packager: Optional[StreamedWholePackager[WHOLE]] = None,
         prefill_pieces: Optional[Iterable[PIECE]] = NO_VALUE,
         prefill_whole: Optional[WHOLE] = NO_VALUE,
     ) -> None:
-        # TODO Oleksandr: raise an error if both prefill_pieces/prefilled_whole pair and producer are set
+        # TODO Oleksandr: raise an error if both prefill_pieces/prefilled_whole and producer/packager are set
         #  (or both are not set)
         self.__producer = producer
         self.__packager = packager
 
         if prefill_pieces is NO_VALUE:
             self._pieces_so_far: list[Union[PIECE, BaseException]] = []
         else:
             self._pieces_so_far: list[Union[PIECE, BaseException]] = [*prefill_pieces, StopAsyncIteration()]
 
         if prefill_whole is NO_VALUE:
             # NO_VALUE is used because `None` is also a legitimate value for the "whole"
             self._whole: Union[WHOLE, Sentinel, BaseException] = NO_VALUE
         else:
             self._whole = prefill_whole
+            self._schedule_collected_event_handlers()
 
         self._all_pieces_consumed = prefill_pieces is not NO_VALUE
         self._producer_lock = asyncio.Lock()
         self._packager_lock = asyncio.Lock()
 
+        promise_context = PromiseContext.get_current()
+
+        if schedule_immediately is DEFAULT:
+            schedule_immediately = promise_context.schedule_immediately_by_default
+
         if schedule_immediately and prefill_pieces is NO_VALUE:
             # start producing pieces at the earliest task switch (put them in a queue for further consumption)
             self._queue = asyncio.Queue()
-            asyncio.create_task(self._aproduce_the_stream())
+            promise_context.schedule_task(self._aproduce_the_stream())
         else:
             # each piece will be produced on demand (when the first consumer iterates over it and not earlier)
             self._queue = None
 
-        if collect_as_soon_as_possible and prefill_whole is NO_VALUE:
-            asyncio.create_task(self.acollect())
+        if schedule_immediately and prefill_whole is NO_VALUE:
+            promise_context.schedule_task(self.acollect())
 
         self._producer_iterator: Union[Optional[AsyncIterator[PIECE]], Sentinel] = None
 
     def __aiter__(self) -> AsyncIterator[PIECE]:
         """
         This allows to consume the stream piece by piece. Each new iterator returned by `__aiter__` will replay
         the stream from the beginning.
@@ -96,18 +198,27 @@
             async with self._packager_lock:
                 if self._whole is NO_VALUE:
                     try:
                         self._whole = await self.__packager(self)
                     except BaseException as exc:  # pylint: disable=broad-except
                         self._whole = exc
 
+                    self._schedule_collected_event_handlers()
+
         if isinstance(self._whole, BaseException):
             raise self._whole
         return self._whole
 
+    def _schedule_collected_event_handlers(self):
+        promise_ctx = PromiseContext.get_current()
+        while promise_ctx:
+            for handler in promise_ctx.on_promise_collected:
+                promise_ctx.schedule_task(handler(self, self._whole))
+            promise_ctx = promise_ctx.parent
+
     async def _aproduce_the_stream(self) -> None:
         while True:
             piece = await self._aproducer_iterator_next()
             self._queue.put_nowait(piece)
             if isinstance(piece, StopAsyncIteration):
                 break
 
@@ -190,19 +301,22 @@
     This is a special kind of `producer` that can be fed into `StreamedPromise` constructor. Objects of this class
     implement the context manager protocol and an `append()` method, which allows for passing such an object into
     `StreamedPromise` constructor while also keeping a reference to it in the outside code in order to `feed` the
     pieces into it (and, consequently, into the `StreamedPromise`) later using `append()`.
     TODO Oleksandr: explain the `capture_errors` parameter
     """
 
-    def __init__(self, capture_errors: bool) -> None:
+    def __init__(self, capture_errors: Union[bool, Sentinel] = DEFAULT) -> None:
         self._queue = asyncio.Queue()
         self._append_open = False
         self._append_closed = False
-        self._capture_errors = capture_errors
+        if capture_errors is DEFAULT:
+            self._capture_errors = PromiseContext.get_current().producer_capture_errors_by_default
+        else:
+            self._capture_errors = capture_errors
 
     def __enter__(self) -> "AppendProducer":
         return self.open()
 
     def __exit__(
         self,
         exc_type: Optional[type[BaseException]],
```

### Comparing `miniagents-0.0.3/miniagents/promisegraph/sequence.py` & `miniagents-0.0.4/miniagents/promisegraph/sequence.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 """
 The main class in this module is `FlatSequence`. See its docstring for more information.
 """
 
-from typing import Generic, AsyncIterator
+from typing import Generic, AsyncIterator, Union
 
 from miniagents.promisegraph.promise import StreamedPromise, AppendProducer
+from miniagents.promisegraph.sentinels import Sentinel, DEFAULT
 from miniagents.promisegraph.typing import SequenceFlattener, IN, OUT
 
 
 class FlatSequence(Generic[IN, OUT]):
     """
     TODO Oleksandr: produce a docstring for this class after you use it in the MiniAgents framework
     """
 
     append_producer: AppendProducer[IN]
     sequence_promise: StreamedPromise[OUT, tuple[OUT, ...]]
 
     def __init__(
         self,
         flattener: SequenceFlattener[IN, OUT],
-        schedule_immediately: bool,
-        collect_as_soon_as_possible: bool,
-        producer_capture_errors: bool,
+        schedule_immediately: Union[bool, Sentinel] = DEFAULT,
+        producer_capture_errors: Union[bool, Sentinel] = DEFAULT,
+        sequence_promise_class: type[StreamedPromise[OUT, tuple[OUT, ...]]] = StreamedPromise[OUT, tuple[OUT, ...]],
     ) -> None:
         self.__flattener = flattener
         self._input_promise = StreamedPromise(
             producer=self._producer,
             packager=lambda _: None,
-            schedule_immediately=schedule_immediately,
-            collect_as_soon_as_possible=False,
+            schedule_immediately=False,
         )
 
         self.append_producer = AppendProducer(capture_errors=producer_capture_errors)
-        self.sequence_promise = StreamedPromise(
+        self.sequence_promise = sequence_promise_class(
             producer=self._input_promise,
             packager=self._packager,
-            schedule_immediately=False,
-            collect_as_soon_as_possible=collect_as_soon_as_possible,
+            schedule_immediately=schedule_immediately,
         )
 
     async def _producer(self, _) -> AsyncIterator[OUT]:
         async for zero_or_more_items in self.append_producer:
             async for item in self.__flattener(self, zero_or_more_items):
                 yield item
```

### Comparing `miniagents-0.0.3/miniagents/promisegraph/typing.py` & `miniagents-0.0.4/miniagents/promisegraph/typing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Types for the PromiseGraph part of the library.
 """
 
-from typing import TypeVar, AsyncIterator, Protocol, Union
+from typing import TypeVar, AsyncIterator, Protocol, Union, Any
 
 PIECE = TypeVar("PIECE")
 WHOLE = TypeVar("WHOLE")
 IN = TypeVar("IN")
 OUT = TypeVar("OUT")
 StreamedPromiseBound = TypeVar("StreamedPromiseBound", bound="StreamedPromise")
 FlatSequenceBound = TypeVar("FlatSequenceBound", bound="FlatSequence")
@@ -26,14 +26,24 @@
     A protocol for packagers of the whole value. A whole packager is a function that takes a `StreamedPromise`
     instance as an argument and returns the whole value.
     """
 
     async def __call__(self, streamed_promise: StreamedPromiseBound) -> WHOLE: ...
 
 
+class PromiseCollectedEventHandler(Protocol):
+    """
+    A protocol for StreamedPromise collection event handlers. A promise collection event is a function that is
+    scheduled to be called after StreamedPromise.acollect() finishes collecting the promise. "Scheduled" means
+    that the function is passed to the event loop for execution without blocking the current coroutine.
+    """
+
+    async def __call__(self, streamed_promise: StreamedPromiseBound, whole: Any) -> None: ...
+
+
 class SequenceFlattener(Protocol[IN, OUT]):
     """
     A protocol for sequence flatteners. A sequence flattener is a function that takes a single object of type `IN`
     and asynchronously converts it into zero or more objects of type `OUT`. In other words, it "flattens" a single
     `IN` into zero or more instances of `OUT`.
     """
```

### Comparing `miniagents-0.0.3/pyproject.toml` & `miniagents-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 119
 
 [tool.coverage.run]
 branch = true
 
 [tool.poetry]
 name = "miniagents"
-version = "0.0.3"
+version = "0.0.4"
 description = """\
 TODO Oleksandr\
 """
 authors = ["Oleksandr Tereshchenko <toporok@gmail.com>"]
 homepage = "https://github.com/teremterem/MiniAgents"
 readme = "README.md"
 license = "MIT"
```

### Comparing `miniagents-0.0.3/PKG-INFO` & `miniagents-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniagents
-Version: 0.0.3
+Version: 0.0.4
 Summary: TODO Oleksandr
 Home-page: https://github.com/teremterem/MiniAgents
 License: MIT
 Author: Oleksandr Tereshchenko
 Author-email: toporok@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

