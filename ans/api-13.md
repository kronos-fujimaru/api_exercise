#### SimpleMapSample.java
```java
package jp.kronos.sample;

import java.util.HashMap;
import java.util.Map;

public class SimpleMapSample {

    private Map<String, String> cities = new HashMap<>();

    public SimpleMapSample() {
        this.cities.put("001", "大阪");
        this.cities.put("002", "東京");
        this.cities.put("003", "名古屋");
        this.cities.put("004", "福岡");
    }

    public void execute(String key) {
        System.out.println(cities.get(key));
    }
}
```

#### ApiMain4.java
```java
package jp.kronos.main;

import jp.kronos.sample.SimpleMapSample;

public class ApiMain4 {

    public static void main(String[] args) {
        SimpleMapSample sample = new SimpleMapSample();
        sample.execute("001");

        // 実行時引数を使用する場合
        //sample.execute(args[0]);
    }
}
```
