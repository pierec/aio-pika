1.5.0
-----

* `Channel.is_closed` property
* `Channel.close` just return `None` when channel already closed
* `Connection` might be used in `async with` expression
* `Queue` might be used in `async with` and returns `QueueIterator`
* Changing examples
* `Queue.iterator()` method
* `QueueIterator.close()` returns `asyncio.Future` instead of `asyncio.Task`
* Ability to use `QueueIterator` in `async for` expression
* `connect_robust` is a `coroutine` instead of function which returns a coroutine 
(PyCharm type checking display warning instead)
* add tests


1.4.2
-----

* Improve documentation. Add examples for connection and channel
* `Conneciton.close` returns `asyncio.Task` instead coroutine.
* `connect_robust` now is function instead of `partial`.