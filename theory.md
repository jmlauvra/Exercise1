Exercise 1 - Theory questions
-----------------------------
 
 ### What is the difference between concurrency and parallelism?
 > Parallelism means doing multiple computations simultaneously while concurrency is about running multiple computations at the same time.
 When solving a task using concurrency we need to manage the time spent on each subtask because each subtask can not be computed simultaneously.
 
 ### Why have machines become increasingly multicore in the past decade?
 > Multicore allowes for parallelism which is faster than concurrency if your task can be solved using parallelism. In the past decade, developers have been trying to optimize programs for multicores.
 
 ### Why do we divide software (programs) into concurrently executing parts (like threads or processes)?
 (Or phrased differently: What problems do concurrency help in solving?)
 > Concurrency helps make it seem as different porcesses and threads are being executed simultaneously for the user when executed by a single core processor.
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > Concurrent programs make life harder, but it is necessary.
 
 ### What is the conceptual difference between threads and processes?
 > A process contains many threads.
 
 ### Some languages support "fibers" (sometimes called "green threads") or "coroutines"? What are they?
 > A "fiber" is a program proces that has the ability to share resourses and adresses.
 
 ### What is the Go-language's "goroutine"? A C/POSIX "pthread"?
 > A "goroutine" is a lightweight thread managed by Go runtime that runs concurrently to other threads in a program.
 
 ### In Go, what does `func GOMAXPROCS(n int) int` change? 
 > GOMAXPROCS decides the maximum number of threads that can execute simultaneously.