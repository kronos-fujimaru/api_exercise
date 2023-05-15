#### SimpleListSample.java
```java
package jp.kronos.sample;

import java.util.ArrayList;
import java.util.List;

public class SimpleListSample {
    
    public void execute() {
        List<String> prefs = new ArrayList<>();
        prefs.add("大阪");
        prefs.add("東京");
        prefs.add("名古屋");
        prefs.add("福岡");
        
        for (int i = 0; i < prefs.size(); i++) {
            System.out.println(prefs.get(i));
        }
    }
}
```

#### ApiMain10.java
```java
package jp.kronos.main;

import jp.kronos.sample.PrefListSample;

public class ApiMain10 {

    public static void main(String[] args) {
        PrefListSample sample = new PrefListSample();
        sample.execute();
    }

}
```
