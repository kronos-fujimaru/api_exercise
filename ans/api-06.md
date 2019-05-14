#### StringSample.java
```java
public class StringSample {

    public static void main(String[] args) {
        String[] splitted = "HelloWorld".split("o");
        for(int i = 0; i < splitted.length; i++) {
            System.out.println(splitted[i]);
        }
    }

}
```
