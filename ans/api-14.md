#### ExceptionSample.java
```java
package jp.kronos.sample;

import java.util.Scanner;

public class ExceptionSample {
    
    public void execute() {
        Scanner scan = new Scanner(System.in);
        
        try {
            String input = scan.nextLine();
            int number = Integer.parseInt(input);
            System.out.println(number);
        } catch(NumberFormatException e) {
            System.out.println("整数値以外が入力されました");
        } 
        
        scan.close();
    }
}
```

#### ApiMain5.java
```java
package jp.kronos.main;

import jp.kronos.sample.ExceptionSample;

public class ApiMain5 {
    
    public static void main(String[] args) {
        ExceptionSample sample = new ExceptionSample();
        sample.execute();
    }
}
```
