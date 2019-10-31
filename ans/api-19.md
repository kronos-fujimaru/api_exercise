#### ApiMain9.java
```java
package jp.kronos.main;

import java.util.Calendar;

public class ApiMain10 {

    public static void main(String[] args) {
    	String[] dayOfWeek = {"日曜日", "月曜日", "火曜日", "水曜日", "木曜日", "金曜日", "土曜日"};
        Calendar cal = Calendar.getInstance();

        // 日付の設定（※月は0から始まる）
        cal.set(1986,  7, 19);

        int numWeek = cal.get(Calendar.DAY_OF_WEEK);
        System.out.println(dayOfWeek[numWeek - 1]);
    }

}
```
