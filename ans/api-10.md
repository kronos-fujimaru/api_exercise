#### SimpleListSample.java
```java
package jp.kronos.sample;

import java.util.ArrayList;
import java.util.List;

public class SimpleListSample {
    
    public void execute() {
        String[] prefs = {"大阪", "東京", "名古屋", "福岡"};
        List<String> prefList = new ArrayList<>();
        for(int i = 0; i < prefs.length; i++) {
            prefList.add(prefs[i]);
        }
        
        for (int i = 0; i < prefList.size(); i++) {
            System.out.println(prefList.get(i));
        }

        // 拡張for文の場合
        //for (String pref : prefList) {
        //    System.out.println(pref);
        //}
    }
}
```

#### ApiMain1.java
```java
package jp.kronos.main;

import jp.kronos.sample.SimpleListSample;

public class ApiMain1 {

    public static void main(String[] args) {
        SimpleListSample sample = new SimpleListSample();
        sample.execute();
    }
}

```
