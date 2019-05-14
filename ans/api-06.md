#### StringSample.java
```java
public class StringSample {

    public static void main(String[] args) {
        String str = "HelloWorld";
        String[] splitted = str.split("o");
        
        for(int i = 0; i < splitted.length; i++) {
            System.out.println(splitted[i]);
        }
    }

}
```
