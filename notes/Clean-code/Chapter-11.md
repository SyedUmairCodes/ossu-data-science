Writing clean concurrent programs is hard sometimes very hard. It is much easier to write code that executes in a single thread.

> Concurrency is a decoupling strategy. It helps us decouple what gets done from when it gets done. 

In single-threaded applications what and when are so strongly coupled that the state of the entire application can often be determined by looking at the stack back trace.

Decoupling what from when can dramatically improve both the throughput and structures of an application. This can make the system easier to understand and offers some powerful ways to separate concerns.

Concurrency can sometimes improve performance, but only when there is a lot of wait time that can be shared between multiple threads or multiple processors.

The design of a concurrent algorithm can be remarkably different from the design of a single-threaded system because of all the decoupling.

Consider writing your threaded code such that each thread exists in its own world, sharing no data with any other thread. Each thread processes one client request, with all of its required data coming from an un-shared source and stored as local variables.

Write tests that have the potential to expose problems and then run them frequently, with different programmatic configurations and system configurations and load. If tests ever fail, track down the failure.

Don’t ignore a failure just because the tests pass on a subsequent run. Multi threaded code behaves differently in different environments. You should run your tests in every
potential deployment environment.