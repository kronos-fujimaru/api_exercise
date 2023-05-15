#### ApiMain16.java
```java
package jp.kronos.main;

import java.text.SimpleDateFormat;
import java.util.Date;

public class ApiMain16 {

    public static void main(String[] args) {
        Date date = new Date();
        SimpleDateFormat sdf = new SimpleDateFormat("yyyy年M月dd日 HH時mm分");
        System.out.println(sdf.format(date));
    }

}
```
