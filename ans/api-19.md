#### SimpleFileReaderSample.java
```java
package jp.kronos.sample;

import java.io.BufferedReader;
import java.io.FileReader;
import java.io.IOException;
import java.util.ArrayList;
import java.util.List;

public class SimpleFileReaderSample {
    public List<String> execute() throws IOException {

        List<String> list = new ArrayList<>();

        String filePath = ""; // TODO 自分で設定したファイルのパスを設定する
        FileReader fr = new FileReader(filePath);

        BufferedReader br = new BufferedReader(fr);

        String line = br.readLine();
        while (line != null) {
            list.add(line);
            line = br.readLine();
        }
        br.close();

        return list;
    }
}
```

#### ApiMain19.java
```java
package jp.kronos.main;

import java.io.IOException;
import java.util.List;

import jp.kronos.sample.SimpleFileReaderSample;

public class ApiMain19 {

    public static void main(String[] args) throws IOException {
        SimpleFileReaderSample sample = new SimpleFileReaderSample();
        List<String> results = sample.execute();

        for (String result : results) {
            System.out.println(result);
        }
    }
}
```
