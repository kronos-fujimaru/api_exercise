#### CustomExceptionSample.java
```java
package jp.kronos.sample;

import jp.kronos.exception.TooLongLengthException;

public class CustomExceptionSample {
    
    public void execute(String input) throws TooLongLengthException {
        if(input.length() >= 6) {
            throw new TooLongLengthException();
        }
    }
}
```

#### TooLongLengthException.java
```java
package jp.kronos.exception;

public class TooLongLengthException extends Exception {
}
```

#### ApiMain6.java
```java
package jp.kronos.main;

import java.util.Scanner;

import jp.kronos.exception.TooLongLengthException;
import jp.kronos.sample.CustomExceptionSample;

public class ApiMain6 {
    
    public static void main(String[] args) {
        CustomExceptionSample sample = new CustomExceptionSample();
        Scanner scan = new Scanner(System.in);
        String input = scan.nextLine();
        
        try {
            sample.execute(input);
        } catch(TooLongLengthException e) {
            System.out.println("文字列は5文字以内で入力してください");
        }
        
        scan.close();
    }
}
```
