#### PrefListSample.java
```java
package jp.kronos.sample;

import java.util.ArrayList;
import java.util.List;

public class PrefListSample {
    public void execute() {
        List<String> prefs = new ArrayList<>();
        prefs.add("大阪");
        prefs.add("東京");
        prefs.add("名古屋");
        prefs.add("福岡");
        
        for (String pref : prefs) {
            System.out.println(pref);
        }
    }
}
```
