#### ApiMain17.java

```java
package jp.kronos.main;

import java.util.Calendar;

public class ApiMain17 {

    public static void main(String[] args) {
        LocalDate today = LocalDate.now();
        LocalDate date1 = LocalDate.of(2023, 5, 7);
        LocalDate date2 = LocalDate.of(2023, 5, 10);
        
        if (today.isBefore(date1) || today.isAfter(date2)) {
            System.out.println("NG");
        } else {
            System.out.println("OK");
        }
    }

}
```
