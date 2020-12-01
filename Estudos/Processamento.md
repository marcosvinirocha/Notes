# Multithreading in Java

1. [Multithreading](https://www.javatpoint.com/multithreading-in-java#)
2. [Multitasking](https://www.javatpoint.com/multithreading-in-java#multitasing)
3. [Process-based multitasking](https://www.javatpoint.com/multithreading-in-java#multiprocessing)
4. [Thread-based multitasking](https://www.javatpoint.com/multithreading-in-java#multithreading)
5. [What is Thread](https://www.javatpoint.com/multithreading-in-java#thread)

**Multithreading in [Java](https://www.javatpoint.com/java-tutorial)** is a process of executing multiple threads simultaneously.

A thread is a lightweight sub-process, the smallest unit of processing. Multiprocessing and multithreading, both are used to achieve multitasking.

However, we use multithreading than multiprocessing because threads use a shared memory area. They don't allocate separate memory area so saves memory, and context-switching between the threads takes less time than process.

Java Multithreading is mostly used in games, animation, etc.



| S.N. | Modifier and Type                      | Method                                                       | Description                                                  |
| :--- | :------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| 1)   | void                                   | [start()](https://www.javatpoint.com/java-thread-start-method) | It is used to start the execution of the thread.             |
| 2)   | void                                   | [run()](https://www.javatpoint.com/java-thread-run-method)   | It is used to do an action for a thread.                     |
| 3)   | static void                            | [sleep()](https://www.javatpoint.com/java-thread-sleep-method) | It sleeps a thread for the specified amount of time.         |
| 4)   | static Thread                          | [currentThread()](https://www.javatpoint.com/java-thread-currentthread-method) | It returns a reference to the currently executing thread object. |
| 5)   | void                                   | [join()](https://www.javatpoint.com/java-thread-join-method) | It waits for a thread to die.                                |
| 6)   | int                                    | [getPriority()](https://www.javatpoint.com/java-thread-getpriority-method) | It returns the priority of the thread.                       |
| 7)   | void                                   | [setPriority()](https://www.javatpoint.com/java-thread-setpriority-method) | It changes the priority of the thread.                       |
| 8)   | String                                 | [getName()](https://www.javatpoint.com/java-thread-getname-method) | It returns the name of the thread.                           |
| 9)   | void                                   | [setName()](https://www.javatpoint.com/java-thread-setname-method) | It changes the name of the thread.                           |
| 10)  | long                                   | [getId()](https://www.javatpoint.com/java-thread-getid-method) | It returns the id of the thread.                             |
| 11)  | boolean                                | [isAlive()](https://www.javatpoint.com/java-thread-isalive-method) | It tests if the thread is alive.                             |
| 12)  | static void                            | [yield()](https://www.javatpoint.com/java-thread-yield-method) | It causes the currently executing thread object to pause and allow other threads to execute temporarily. |
| 13)  | void                                   | [suspend()](https://www.javatpoint.com/java-thread-suspend-method) | It is used to suspend the thread.                            |
| 14)  | void                                   | [resume()](https://www.javatpoint.com/java-thread-resume-method) | It is used to resume the suspended thread.                   |
| 15)  | void                                   | [stop()](https://www.javatpoint.com/java-thread-stop-method) | It is used to stop the thread.                               |
| 16)  | void                                   | [destroy()](https://www.javatpoint.com/java-thread-destroy-method) | It is used to destroy the thread group and all of its subgroups. |
| 17)  | boolean                                | [isDaemon()](https://www.javatpoint.com/java-thread-isdaemon-method) | It tests if the thread is a daemon thread.                   |
| 18)  | void                                   | [setDaemon()](https://www.javatpoint.com/java-thread-setdaemon-method) | It marks the thread as daemon or user thread.                |
| 19)  | void                                   | [interrupt()](https://www.javatpoint.com/java-thread-interrupt-method) | It interrupts the thread.                                    |
| 20)  | boolean                                | [isinterrupted()](https://www.javatpoint.com/java-thread-isinterrupted-method) | It tests whether the thread has been interrupted.            |
| 21)  | static boolean                         | [interrupted()](https://www.javatpoint.com/java-thread-interrupted-method) | It tests whether the current thread has been interrupted.    |
| 22)  | static int                             | [activeCount()](https://www.javatpoint.com/java-thread-activecount-method) | It returns the number of active threads in the current thread's thread group. |
| 23)  | void                                   | [checkAccess()](https://www.javatpoint.com/java-thread-checkaccess-method) | It determines if the currently running thread has permission to modify the thread. |
| 24)  | static boolean                         | [holdLock()](https://www.javatpoint.com/java-thread-holdlock-method) | It returns true if and only if the current thread holds the monitor lock on the specified object. |
| 25)  | static void                            | [dumpStack()](https://www.javatpoint.com/java-thread-dumpstack-method) | It is used to print a stack trace of the current thread to the standard error stream. |
| 26)  | StackTraceElement[]                    | [getStackTrace()](https://www.javatpoint.com/java-thread-getstacktrace-method) | It returns an array of stack trace elements representing the stack dump of the thread. |
| 27)  | static int                             | [enumerate()](https://www.javatpoint.com/java-thread-enumerate-method) | It is used to copy every active thread's thread group and its subgroup into the specified array. |
| 28)  | Thread.State                           | [getState()](https://www.javatpoint.com/java-thread-getstate-method) | It is used to return the state of the thread.                |
| 29)  | ThreadGroup                            | [getThreadGroup()](https://www.javatpoint.com/java-thread-getthreadgroup-method) | It is used to return the thread group to which this thread belongs |
| 30)  | String                                 | [toString()](https://www.javatpoint.com/java-thread-tostring-method) | It is used to return a string representation of this thread, including the thread's name, priority, and thread group. |
| 31)  | void                                   | [notify()](https://www.javatpoint.com/java-thread-notify-method) | It is used to give the notification for only one thread which is waiting for a particular object. |
| 32)  | void                                   | [notifyAll()](https://www.javatpoint.com/java-thread-notifyall-method) | It is used to give the notification to all waiting threads of a particular object. |
| 33)  | void                                   | [setContextClassLoader()](https://www.javatpoint.com/java-thread-setcontextclassloader-method) | It sets the context ClassLoader for the Thread.              |
| 34)  | ClassLoader                            | [getContextClassLoader()](https://www.javatpoint.com/java-thread-getcontextclassloader-method) | It returns the context ClassLoader for the thread.           |
| 35)  | static Thread.UncaughtExceptionHandler | [getDefaultUncaughtExceptionHandler()](https://www.javatpoint.com/java-thread-getdefaultuncaughtexceptionhandler-method) | It returns the default handler invoked when a thread abruptly terminates due to an uncaught exception. |
| 36)  | static void                            | [setDefaultUncaughtExceptionHandler()](https://www.javatpoint.com/java-thread-setdefaultuncaughtexceptionhandler-method) | It sets the default handler invoked when a thread abruptly terminates due to an uncaught exception. |