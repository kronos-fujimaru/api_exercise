#### PrefMapSample.java
```java
package jp.kronos.sample;

import java.util.HashMap;
import java.util.Map;

public class PrefMapSample {
    private Map<String, String> prefs = new HashMap<>();
    
    public PrefMapSample() {
        this.prefs.put("001", "大阪");
        this.prefs.put("002", "東京");
        this.prefs.put("003", "名古屋");
        this.prefs.put("004", "福岡");
    }
    
    public void execute(String key) {
        String pref = prefs.get(key);
        if (pref == null) {
            throw new NullPointerException("指定した都道府県IDは存在しません。");
        }
    }
}
```

#### ApiMain13.java
```java
package jp.kronos.main;

import jp.kronos.sample.PrefMapSample;

public class ApiMain13 {

    public static void main(String[] args) {
        try {
            PrefMapSample sample = new PrefMapSample();
            sample.execute("005");
        } catch (NullPointerException e) {
            System.out.println(e.getMessage());
        }
    }

}
```
