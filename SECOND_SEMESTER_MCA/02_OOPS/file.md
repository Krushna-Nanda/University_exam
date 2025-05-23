# cretion , redaing in same and also append 

---
```java
import java.io.*;
import java.util.Scanner;
public class Example1 {
    public static void main(String[] args) {
        // codeto crete a new file
        File myFile = new File("krushna.txt");
        try{
            myFile.createNewFile();
        }catch(Exception e){
            System.out.println(e);
        }
        try{

            FileWriter filewrite = new FileWriter("krushna.txt" , true);
            filewrite.write("hi i am krushana\nchandra nanda");
            filewrite.close();
            System.out.println("wrote succesfully");
        }catch(Exception e){
            System.out.println(e);
        }

        //read a file
        try{
            
            Scanner reader = new Scanner(myFile);
            while(reader.hasNextLine()){
                System.out.println(reader.nextLine());
            }
            reader.close();

        }catch(Exception e){
            System.out.println(e);
        }



    }

    // code to write

}

```
---


# if alreday exist

```java
import java.io.File;
import java.io.IOException;
import java.util.Scanner;

public class Hello {
    public static void main(String[] args) {
        
        File myFile = new File("krushna.txt");

        try{
            Scanner readFile = new Scanner(myFile);
            while(readFile.hasNextLine()){
                System.out.println(readFile.nextLine());
            }
            System.out.println("REDAING IS COMPLETE");
        }catch(IOException e){
            System.out.println(e + "\n" +  " a problem occured to read tyhe");
        }
    }
    
}

```
