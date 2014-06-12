Evaluates a script asynchronously. This means that the script will not
be executed atomically. Each time it does a redis "call", the coroutine
will be suspended, the command will be executed inside the event loop
and it will them be resumed. See more details on `EVAL` documentation.
