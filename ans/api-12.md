#### ApiMain3.java
```java
package jp.kronos.main;

import java.util.HashSet;
import java.util.Set;

public class ApiMain3 {
    public static void main(String[] args) {
        Set<String> courseSet = new HashSet<>();
        courseSet.add("CSS");
        courseSet.add("HTML");
        courseSet.add("JavaScript");
        courseSet.add("PHP");
        
        if(courseSet.contains("Java")) {
            System.out.println("Javaコースはあります。");
        } else {
            System.out.println("Javaコースはありません。");
        }
        
        // セットに「Java」の文字列を追加し、再度存在チェックをする。
        courseSet.add("Java");
        
        if(courseSet.contains("Java")) {
            System.out.println("Javaコースはあります。");
        } else {
            System.out.println("Javaコースはありません。");
        }    
    }
}
```
