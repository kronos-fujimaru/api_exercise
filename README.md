# Java API 演習問題

**APIドキュメント**

<a href="https://docs.oracle.com/javase/jp/17/docs/api/" target="_blank">https://docs.oracle.com/javase/jp/17/docs/api/</a>

<br>

### 演習1

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"内に 'r' が含まれているかを T または F で表示しなさい。
```

<br>

[解答例](/ans/api-01.md)

<br>

### 演習2

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"内に "orl"が出現するインデックス位置を表示しなさい。
```

<br>

[解答例](/ans/api-02.md)

<br>

### 演習3

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"内に 'l'が最後に出現するインデックス位置を表示しなさい。
```

<br>

[解答例](/ans/api-03.md)

<br>

### 演習4

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"の文字数を表示しなさい。
```

<br>

[解答例](/ans/api-04.md)

<br>

### 演習5

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HellaWarld"の'a'を'o'に置換して表示しなさい。
```

<br>

[解答例](/ans/api-05.md)

<br>

### 演習6

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"を'o'で区切った部分文字列を改行しながらすべて表示しなさい。
```

<br>

[解答例](/ans/api-06.md)

<br>

### 演習7

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"のインデックス位置、3～7の部分文字列を表示しなさい。
```

<br>

[解答例](/ans/api-07.md)

<br>

### 演習8

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"をすべて大文字にして表示しなさい。
```

<br>

[解答例](/ans/api-08.md)

<br>

### 演習9

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
" HelloWorld "の前後のスペースを排除して、表示しなさい。
```

<br>

[解答例](/ans/api-09.md)

<br>

### 演習10

```
PrefListSampleクラス（パッケージ：jp.kronos.sample）
　executeメソッド（戻り値なし、引数なし）に以下の処理を記述する。
　①String型のArrayListインスタンスに「大阪」「東京」「名古屋」「福岡」の文字列を格納する。
　②通常のfor文（拡張for文ではない）を使用してArrayListに格納されている値をすべてコンソールに出力する。

ApiMain10クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①PrefListSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。
```

<br>

[解答例](/ans/api-10.md)

<br>

### 演習11

```
演習10で、PrefListSampleクラスのexecuteメソッドの繰り返し処理を拡張for文に修正する。
```

<br>

[解答例](/ans/api-11.md)

<br>

### 演習12

```
NumListSampleクラス（パッケージ：jp.kronos.sample）
　executeメソッド（戻り値なし、引数なし）に以下の処理を記述する。
　①Integer型のArrayListインスタンスに「1000」「500」「300」「2000」「700」の整数を格納する。
　②ArrayListに格納されている値の合計値をArrayListに追加する。
　③ArrayListに格納されている各値をコンソールに出力した後に、「合計: [合計値]」を出力する。

ApiMain12クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①NumListSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。
```

<br>

**＜出力結果＞**

```
1000
500
300
2000
700
合計: 4500
```

<br>

[解答例](/ans/api-12.md)

<br>

### 演習13

```
PrefMapSampleクラス（パッケージ：jp.kronos.sample）
　①HashMapフィールド（prefs）をprivateなフィールドとして定義する
　②コンストラクタでprefsに以下の情報をセットする。（すべてString型の文字列）
　　キー："001" 値："大阪"
　　キー："002" 値："東京"
　　キー："003" 値："名古屋"
　　キー："004" 値："福岡"
　③executeメソッドでStringの引数（キー）を受け取り、prefs内でキーに一致する値を取得し、コンソールに出力する。

ApiMain13クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①PrefMapSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。
　　※キーは適当に指定する
```

<br>

[解答例](/ans/api-13.md)

<br>

### 演習14

```
PrefMapSampleクラス（パッケージ：jp.kronos.sample）
　executeメソッドを以下のように修正する。
　①引数（キー）でHashMapフィールド（prefs）から取得した値がNullの場合は、以下のメッセージを追加してNullPointerExceptionをスローする。
　　メッセージ: 指定した都道府県IDは存在しません。

ApiMain13クラス（パッケージ：jp.kronos.main）
　mainメソッドを以下のように修正する。
　①NullPointerExceptionをキャッチし、例外オブジェクトのメッセージをコンソールに出力する。
　　※getMessage()メソッドで例外オブジェクトのメッセージを取得できる
```

<br>

**＜出力結果＞**　※キーに "005" を指定した場合

```
指定した都道府県IDは存在しません。
```

<br>

[解答例](/ans/api-14.md)

<br>

### 演習15

```
ApiMain15クラス（パッケージ：jp.kronos.main）
　Scannerクラスを使用した標準入力でジャンケンをするプログラムである。
　0（グー）、1（チョキ）、2（パー）のいずれかを入力してもらい、コンピュータと勝負する。
　ただし、整数以外（文字列など）を入力すると例外が発生するため以下のように例外の対応をする。
　①発生する例外の種類を調べる。
　②該当する例外をキャッチし、以下のメッセージをコンソールに表示する。
　　メッセージ: 入力値が不正です。
　③ジャンケンプログラムを終了する。
　　※returnキーワードで終了できる
```

<br>

**ApiMain15.java**

```java
package jp.kronos.main;

import java.util.InputMismatchException;
import java.util.Random;
import java.util.Scanner;

public class ApiMain15 {

    public static void main(String[] args) {
        String[] signs = {"グー", "チョキ", "パー"};
        
        Scanner scan = new Scanner(System.in);
        System.out.println("0:グー、1:チョキ、2:パー");
        
        // プレイヤーの手を入力してもらう
        int player = scan.nextInt();
        
        if (!(player >= 0 && player <= 2)) {
            System.out.println("0～2の数値を入力してください。");
            return;
        }
        
        // コンピュータの手をランダムに決める
        int pc = new Random().nextInt(3);
        
        // それぞれの手を出力する
        System.out.println("PLAYER: " + signs[player]);
        System.out.println("COMPUTER: " + signs[pc]);
        
        // 結果を表示する
        if ((player == 0 && pc == 1) || (player == 1 && pc == 2) || (player == 2 && pc == 0)) {
            System.out.println("YOU WIN!");
        } else if ((player == 0 && pc == 2) || (player == 1 && pc == 0) || (player == 2 && pc == 1)) {
            System.out.println("YOU LOSE!");
        } else {
            System.out.println("DRAW!");
        }
    }

}
```

<br>

**＜出力結果＞**　※"a"を入力した場合

```
0:グー、1:チョキ、2:パー
a
入力値が不正です。
```

<br>

[解答例](/ans/api-15.md)

<br>


### 演習16

```
ApiMain16クラス（パッケージ：jp.kronos.main）
　本日の日付を「2020年8月19日 09時15分」のような形式で表示しなさい。
```

<br>

[解答例](/ans/api-16.md)

<br>

### 演習17

```
ApiMain17クラス（パッケージ：jp.kronos.main）
　CalendarクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
　あなたの生年月日の曜日を表示しなさい。
　（例）1986年8月19日なら「火曜日」と表示する。
```

> ヒント<br>Calendarクラスのget()メソッドで引数に「Calendar.DAY_OF_WEEK」を指定すると、1（日曜日）～ 7（土曜日）の数値が取得できます。

<br>

[解答例](/ans/api-17.md)

<br>

### 演習18

```
作成中
```

<br>

### 演習19

```
SimpleFileReaderSampleクラス（パッケージ：jp.kronos.sample）
　executeメソッド(引数：なし、戻り値：List)
　　テキストファイル「sample.txt」から読み込んだ文字列をArrayList<String>に格納して返却する

sample.txt
　自由に作成しなさい

ApiMain19クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①SimpleFileReaderSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。
　②executeメソッドの戻り値を受け取り、すべて標準出力する。
```

<br>

[解答例](/ans/api-19.md)

<br>

### 演習20

```
employee.csv
　以下の内容でCSVファイルを用意する。
　1,Yamada Taro,30,Male
　2,Tanaka Hanako,26,Female
　3,Yamamoto Kenji,42,Male
　4,Suzuki Ichiro,45,Male
　5,Yamada Chie,34,Female
　6,Goto Hajime,23,Male
　7,Tajima Kanako,31,Female
　8,Yamada Kotaro,27,Male
　9,Fukushige Yozo,52,Male
　10,Yamamoto Tetsuko,27,Female

ApiMain8クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①CSVファイル「employee.csv」から読み込んだ情報のうち、「Yamada」さんの情報のみ標準出力する。
```

<br>

[解答例](/ans/api-20.md)

<br>