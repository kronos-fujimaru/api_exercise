#### ApiMain8.java
```java
package jp.kronos.main;

import java.time.LocalDateTime;
import java.time.format.DateTimeFormatter;

public class ApiMain8 {
    
    public static void main(String[] args) {
        LocalDateTime now = LocalDateTime.now();
        DateTimeFormatter fmt = DateTimeFormatter.ofPattern("yyyy年M月dd日 HH時mm分");
        System.out.println(fmt.format(now));
    }
}
```
