#### ApiMain16.java

```java
package jp.kronos.main;

import java.text.SimpleDateFormat;
import java.util.Date;

public class ApiMain16 {

    public static void main(String[] args) {
        LocalDate today = LocalDate.now();
        LocalDate date = LocalDate.of(2023, 5, 10);
        
        if (date.isEqual(today)) {
            System.out.println("Same.");
        } else {
            System.out.println("Not Same.");
        }
    }

}
```
