#### NumListSample.java

```java
package jp.kronos.sample;

import java.util.ArrayList;
import java.util.List;

public class NumListSample {
    public void execute() {
        List<Integer> nums = new ArrayList<>();
        nums.add(1000);
        nums.add(500);
        nums.add(300);
        nums.add(2000);
        nums.add(700);
        
        int total = 0;
        for (Integer num : nums) {
            total += num;
        }
        nums.add(total);
        
        for (int i = 0; i < nums.size() - 1; i++) {
            System.out.println(nums.get(i));
        }
        System.out.println("合計: " + nums.get(nums.size() - 1));
    }
    
}
```

#### ApiMain12.java

```java
package jp.kronos.main;

import jp.kronos.sample.NumListSample;

public class ApiMain12 {

    public static void main(String[] args) {
        NumListSample sample = new NumListSample();
        sample.execute();
    }

}
```
