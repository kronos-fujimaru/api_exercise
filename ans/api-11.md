#### Dog.java
```java
package jp.kronos.animal;

public class Dog {
    private String name;
    
    public Dog(String name) {
        this.name = name;
    }
    
    public void showName() {
        System.out.println("私の名前は" + name + "です。");
    }
}
```

#### ListSample.java
```java
package jp.kronos.sample;

import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;

import jp.kronos.animal.Dog;

public class ListSample {

    public List<Dog> execute() {
        Scanner scan = new Scanner(System.in);
        List<Dog> dogList = new ArrayList<>();
        
        while (true) {
            String input = scan.nextLine();
            if ("".equals(input)) {
                break;
            } else {
                dogList.add(new Dog(input));
            }
        }
        
        scan.close();
        return dogList;
    }
}
```

#### ApiMain2.java
```java
package jp.kronos.main;

import java.util.List;

import jp.kronos.animal.Dog;
import jp.kronos.sample.ListSample;

public class ApiMain2 {

    public static void main(String[] args) {
        ListSample sample = new ListSample();
        List<Dog> dogList = sample.execute();
        for (Dog dog : dogList) {
            dog.showName();
        }
    }
}
```
