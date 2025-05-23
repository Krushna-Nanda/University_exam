# extend
```java
  public class SimpleThread{
    public static void main(String[] args) {
        // System.out.println("hello");
        myThread t1 = new myThread("hello");
        t1.start();
        myThread t2 = new myThread("world");
        t2.start();
        // System.out.println(Thread.currentThread().getState());
    }
}

class myThread extends Thread{
    String message;
    myThread(String m){
        message = m;
    }
    public void run(){
        for(int i = 0; i<5;i++){

            System.out.println(message);
            try{

                Thread.sleep(1000);
            }catch(Exception e){
                System.out.println(e);
            }
        }
    }
}
```

# runnable
```java
public class SimpleThread{
    public static void main(String[] args) {

        myThread t1 = new myThread("krushna");
        Thread thread1 = new Thread(t1);
        thread1.start();
        myThread t2 = new myThread("nanda");
        Thread thread2 = new Thread(t2);
        thread2.start();
     
   
    }
}

class myThread implements Runnable{
    String message;

    myThread(String m){
        message = m;
    }

    public void run (){
        for(int i = 0; i< 5 ; i++){
            System.out.println(message);
            try{
                Thread.sleep(1000);
            }catch(Exception e){
                System.out.println(e);
            }
            
        }
    }
    
 }

```
# sunchronized

```java
class Printer {
   synchronized void print(String msg) {
        for (int i = 1; i <= 3; i++) {
            System.out.print("[ " + msg);
            try{ Thread.sleep(500);
             } catch (Exception e){
                
             }
            System.out.println(" ]");
        }
    }
}

class MyThread extends Thread {
    Printer p;
    String msg;

    MyThread(Printer p, String msg) {
        this.p = p;
        this.msg = msg;
    }

    public void run() {
        p.print(msg);
    }
}

public class Test {
    public static void main(String[] args) {
        Printer p = new Printer();
        MyThread t1 = new MyThread(p, "Krushna");
        MyThread t2 = new MyThread(p, "Nanda");

        t1.start();
        t2.start();
    }
}

```


Below are clear, concise answers and super-simple Java examples for **all** the thread-related questions across 2024, 2023, and 2022. You can copy–paste and run each snippet as-is.

---

## 1. What is a thread? Describe the complete life cycle of a thread.

A **thread** is a lightweight unit of execution within a process. Java programs by default start with a single “main” thread; you can create additional threads to do work in parallel.

### Thread Life Cycle

A Java thread goes through these states:

1. **New** – Thread object created, `start()` not yet called.
2. **Runnable** – After `start()`, ready to run; the scheduler may pick it.
3. **Running** – Scheduler gives CPU to the thread; it executes `run()`.
4. **Blocked/Waiting** – Waiting for I/O, timing (`sleep()`/`wait()`), or lock (`synchronized`).
5. **Terminated** – `run()` completes or thread is interrupted.

```java
class LifeCycleDemo extends Thread {
    public void run() {
        System.out.println("Running...");
        // simulate work
        try { Thread.sleep(200); } catch (InterruptedException e) {}
        System.out.println("Finished.");
    }
    public static void main(String[] args) {
        LifeCycleDemo t = new LifeCycleDemo();  // New
        System.out.println("State after creation: " + t.getState());
        t.start();                                // Runnable -> Running
        System.out.println("State after start(): " + t.getState());
        try {
            t.join();                            // Wait for t to finish
        } catch (InterruptedException e) {}
        System.out.println("State after completion: " + t.getState()); // TERMINATED
    }
}
```

---

## 2. What is thread synchronization? Different ways, and a simple `synchronized`-method example.

**Thread synchronization** ensures that only one thread at a time accesses shared data, preventing race conditions.

### Ways to synchronize

1. **`synchronized` method** – whole method locked on the instance.
2. **`synchronized` block** – lock only a section on a given object.
3. **Static `synchronized`** – lock on the `.class` object.
4. **`java.util.concurrent.locks.Lock`** – explicit lock/unlock.

### Simple `synchronized`-method example

```java
class Counter {
    private int count = 0;

    // only one thread at a time can run this on the same Counter instance
    public synchronized void increment() {
        int temp = count;
        temp = temp + 1;
        count = temp;
    }

    public int getCount() {
        return count;
    }
}

public class SyncDemo {
    public static void main(String[] args) throws InterruptedException {
        Counter c = new Counter();

        // create two threads that both increment the same counter 1000 times
        Thread t1 = new Thread(() -> {
            for (int i = 0; i < 1000; i++) c.increment();
        });
        Thread t2 = new Thread(() -> {
            for (int i = 0; i < 1000; i++) c.increment();
        });

        t1.start();
        t2.start();
        t1.join();
        t2.join();

        // Because increment() is synchronized, final count = 2000
        System.out.println("Final count: " + c.getCount());
    }
}
```

---

## 3. Discuss the concept of multithreading in Java. Advantages and challenges.

**Multithreading** means running multiple threads concurrently within one JVM process.

* **Advantages**

  1. **Improved performance** on multi-CPU/cores.
  2. **Better resource utilization** (e.g., background I/O).
  3. **Responsive UIs** (e.g., Swing/AWT move work off the Event-Dispatch thread).

* **Challenges**

  1. **Race conditions** if threads share mutable data without syncing.
  2. **Deadlock** if two threads each wait for locks the other holds.
  3. **Complexity** in reasoning, testing, and debugging concurrent code.

---

## 4. Compare the `Thread` class vs the `Runnable` interface for creating threads.

| Aspect                    | Extending `Thread`                  | Implementing `Runnable`                           |
| ------------------------- | ----------------------------------- | ------------------------------------------------- |
| Syntax                    | `class MyThread extends Thread`     | `class MyRunnable implements Runnable`            |
| Method to override        | `public void run()`                 | `public void run()`                               |
| Can extend another class? | **No** (Java single inheritance)    | **Yes** (you can extend something else)           |
| Sharing data              | Harder—each `Thread` has own object | Easier—pass same `Runnable` to multiple `Thread`s |
| Usage example             | `new MyThread().start();`           | `new Thread(new MyRunnable()).start();`           |

---

## 5. If you create two threads, how many threads actually run? Explain execution flow.

When you run:

```java
public class TwoThreads {
    public static void main(String[] args) {
        Thread t1 = new Thread(() -> System.out.println("T1"));
        Thread t2 = new Thread(() -> System.out.println("T2"));
        t1.start();
        t2.start();
    }
}
```

* **Threads running**: **3**

  1. **Main thread** (starts the others)
  2. **t1**
  3. **t2**

**Flow**:

1. JVM starts **main**.
2. `new Thread(...)` creates t1 and t2 in **New** state.
3. `t1.start()` → t1 goes to **Runnable**, scheduler picks it → it runs `run()`.
4. `t2.start()` → same for t2.
5. Meanwhile, **main** may continue or finish; JVM waits until all non-daemon threads finish.

---

## 6. What is thread priority? How to set it?

Each Java thread has a priority from **1** to **10**:

* `Thread.MIN_PRIORITY` = 1
* `Thread.NORM_PRIORITY` = 5 (default)
* `Thread.MAX_PRIORITY` = 10

Higher-priority threads are more likely to be scheduled before lower-priority ones (though this is OS-dependent).

```java
public class PriorityDemo {
    public static void main(String[] args) {
        Thread low = new Thread(() -> {
            System.out.println("Low priority running");
        }, "LowThread");
        Thread high = new Thread(() -> {
            System.out.println("High priority running");
        }, "HighThread");

        low.setPriority(Thread.MIN_PRIORITY);     // 1
        high.setPriority(Thread.MAX_PRIORITY);    // 10

        System.out.println(low.getName() + " priority: " + low.getPriority());
        System.out.println(high.getName() + " priority: " + high.getPriority());

        // Start both
        low.start();
        high.start();
    }
}
```

---

## 7. Write a Java program to implement `Runnable` and create a thread.

```java
class MyTask implements Runnable {
    @Override
    public void run() {
        System.out.println("Hello from MyTask on thread: " + Thread.currentThread().getName());
    }
}

public class RunnableDemo {
    public static void main(String[] args) {
        MyTask task = new MyTask();
        Thread t = new Thread(task, "WorkerThread");
        t.start();
        // main thread continues...
        System.out.println("Back in main on: " + Thread.currentThread().getName());
    }
}
```

---

With these explanations and bite-sized examples, you should have a solid grasp of Java threads, their life cycle, synchronization, priorities, and the two main ways to create them. Let me know if you need deeper digs or more examples!

