#### ApiMain8.java
```java
package jp.kronos.main;

import java.io.BufferedReader;
import java.io.FileReader;
import java.io.IOException;

public class BufferedReaderSample6 {

    public static void main(String[] args) throws IOException {
        String path = "C:\\study\\employee.csv";

        BufferedReader br = new BufferedReader(new FileReader(path));

        String line = br.readLine();
        while (line != null) {
            String name = line.split(",")[1];
            if (name.contains("Yamada")) {
                System.out.println(line);
            }
            line = br.readLine();
        }
        br.close();
    }

}
```
