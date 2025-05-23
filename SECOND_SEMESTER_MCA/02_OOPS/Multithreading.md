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
