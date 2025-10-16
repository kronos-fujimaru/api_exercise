# Java API 演習問題

Eclipse上で java_api_exerciseプロジェクトを作成し、APIドキュメントを参照しながら課題に取り組んでください。

<br>

**APIドキュメント（JDK 21）**<br><a href="https://docs.oracle.com/javase/jp/21/docs/api/" target="_blank">https://docs.oracle.com/javase/jp/21/docs/api/</a>

<br>

### 演習1

**ApiMain1クラス（パッケージ：jp.kronos.main）**

任意の文字列内に 'r' が含まれていれば TRUE、含まれていなければ FALSE を表示してください。

<br>

**<期待結果>**　文字列 "HelloWorld" の場合

```
TRUE
```

<br>

[解答例](/ans/api-01.md)

<br><br>

### 演習2

**ApiMain2クラス（パッケージ：jp.kronos.main）**

"HelloWorld"内に "orl"が出現するインデックス位置を表示してください。

<br>

**<期待結果>**

```
6
```

<br>

[解答例](/ans/api-02.md)

<br><br>

### 演習3

**ApiMain3クラス（パッケージ：jp.kronos.main）**

"HelloWorld"内に 'l'が最後に出現するインデックス位置を表示してください。

<br>

**<期待結果>**

```
8
```

<br><br>

[解答例](/ans/api-03.md)

<br><br>

### 演習4

**ApiMain4クラス（パッケージ：jp.kronos.main）**

任意の文字列の文字数を表示してください。

<br>

**<期待結果>**　文字列 "HelloWorld" の場合

```
10
```

<br>

[解答例](/ans/api-04.md)

<br><br>

### 演習5

**ApiMain5クラス（パッケージ：jp.kronos.main）**

"HellaWarld"の'a'を'o'に置換して表示しなさい。

<br>

**<期待結果>**　文字列 "HellaWarld" の場合

```
HelloWorld
```

<br>

[解答例](/ans/api-05.md)

<br><br>

### 演習6

**ApiMain6クラス（パッケージ：jp.kronos.main）**

"HelloWorld"を'o'で区切った部分文字列を改行しながらすべて表示してください。

<br>

**<期待結果>**

```
Hell
W
rld
```

<br>

[解答例](/ans/api-06.md)

<br><br>

### 演習7

**ApiMain7クラス（パッケージ：jp.kronos.main）**

"HelloWorldJava"から "Hello" の部分を取り出して表示してください。

<br>

**<期待結果>**

```
World
```

<br>

[解答例](/ans/api-07.md)

<br><br>

### 演習8

**ApiMain8クラス（パッケージ：jp.kronos.main）**

任意の小文字半角英字を含む文字列をすべて大文字にして表示してください。

<br>

**<期待結果>**　文字列 "HelloWorld" の場合

```
HELLOWORLD
```

<br>

[解答例](/ans/api-08.md)

<br><br>

### 演習9

**ApiMain9クラス（パッケージ：jp.kronos.main）**

" HelloWorld "の前後の半角スペースを排除して表示してください。

<br>

**<期待結果>**

```
HelloWorld
```

<br>

[解答例](/ans/api-09.md)

<br><br>

### 演習10

**PrefListSampleクラス（パッケージ：jp.kronos.sample）**

executeメソッド（戻り値なし、引数なし）に以下の処理を記述する。
1. String型のArrayListインスタンスに「大阪」「東京」「名古屋」「福岡」の文字列を格納する。
2. 通常のfor文（拡張for文ではない）を使用してArrayListに格納されている値をすべてコンソールに出力する。

<br>

**ApiMain10クラス（パッケージ：jp.kronos.main）**

mainメソッドに以下の処理を記述する。
1. PrefListSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。

<br>

[解答例](/ans/api-10.md)

<br><br>

### 演習11　※演習10のつづき

演習10で、PrefListSampleクラスのexecuteメソッドの繰り返し処理を拡張for文に修正する。

<br>

[解答例](/ans/api-11.md)

<br><br>

### 演習12

**NumListSampleクラス（パッケージ：jp.kronos.sample）**

executeメソッド（戻り値なし、引数なし）に以下の処理を記述する。
1. Integer型のArrayListインスタンスに「1000」「500」「300」「2000」「700」の整数を格納する。
2. ArrayListに格納されている値の合計値をArrayListに追加する。
3. ArrayListに格納されている各値をコンソールに出力した後に、「合計: [合計値]」を出力する。

<br>

**ApiMain12クラス（パッケージ：jp.kronos.main）**

mainメソッドに以下の処理を記述する。
1. NumListSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。

<br>

**＜期待結果＞**

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

<br><br>

### 演習13


**PrefMapSampleクラス（パッケージ：jp.kronos.sample）**
1. HashMapフィールド（prefs）をprivateなフィールドとして定義する
2. コンストラクタでprefsに以下の情報をセットする。（すべてString型の文字列）<br>
　キー："001" 値："大阪"<br>　キー："002" 値："東京"<br>　キー："003" 値："名古屋"<br>　キー："004" 値："福岡"<br>
3. executeメソッドでStringの引数（キー）を受け取り、prefs内でキーに一致する値を取得し、コンソールに出力する。

<br>

**ApiMain13クラス（パッケージ：jp.kronos.main）**

mainメソッドに以下の処理を記述する。
1. PrefMapSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。<br>※キーは適当に指定する

<br>

[解答例](/ans/api-13.md)

<br><br>

### 演習14　※演習13のつづき

**PrefMapSampleクラス（パッケージ：jp.kronos.sample）**

executeメソッドを以下のように修正する。
1. 引数（キー）でHashMapフィールド（prefs）から取得した値がNullの場合は、以下のメッセージを追加してNullPointerExceptionをスローする。<br>
　「指定した都道府県IDは存在しません。」

<br>

**ApiMain13クラス（パッケージ：jp.kronos.main）**

mainメソッドを以下のように修正する。
1. NullPointerExceptionをキャッチし、例外オブジェクトのメッセージをコンソールに出力する。<br>
※getMessage()メソッドで例外オブジェクトのメッセージを取得できる

<br>

**＜期待結果＞**　※キーに "005" を指定した場合

```
指定した都道府県IDは存在しません。
```

<br>

[解答例](/ans/api-14.md)

<br><br>

### 演習15

**ApiMain15クラス（パッケージ：jp.kronos.main）**

Scannerクラスを使用した標準入力でジャンケンをするプログラムである。0（グー）、1（チョキ）、2（パー）のいずれかを入力してもらい、コンピュータと勝負する。ただし、整数以外（文字列など）を入力すると例外が発生するため以下のように例外の対応をする。
1. 発生する例外の種類を調べる。
2. 該当する例外をキャッチし、以下のメッセージをコンソールに表示する。
「メッセージ: 入力値が不正です。」
3. ジャンケンプログラムを終了する。

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

**＜期待結果＞**　※"a"を入力した場合

```
0:グー、1:チョキ、2:パー
a
入力値が不正です。
```

<br>

[解答例](/ans/api-15.md)

<br><br>


### 演習16

**ApiMain16クラス（パッケージ：jp.kronos.main）**

LocalDateクラスを使用し、ある任意の日付と現在日付が同日であれば "Same."、異なる日であれば "Not Same." と表示してください。

<br>

**<期待結果>**　※任意の日付と現在日付が同日の場合

```
Same.
```

<br>

[解答例](/ans/api-16.md)

<br><br>

### 演習17

**ApiMain17クラス（パッケージ：jp.kronos.main）**

LocalDateクラスを使用し、現在日付が任意の開始日と終了日の範囲内であれば "OK"、範囲外であれば "NG" と表示してください。なお、開始日または終了日と同日も範囲内とする。

<br>

**<期待結果>**　※それぞれの日付が以下の場合

- 現在日：2023/05/10
- 開始日：2023/05/07
- 終了日：2023/05/10

```
OK
```

<br>

[解答例](/ans/api-17.md)

<br><br>

<!-- ### 演習18

```
Userクラス（パッケージ：jp.kronos.dto）
　①ログインID、パスワード、姓、名のフィールドとそれぞれのgetter/setterを定義する。
　②ログインID、パスワード、姓、名を引数を取り、それぞれのフィールドに設定するコンストラクタを定義する。
UserSampleクラス（パッケージ：jp.kronos.sample）
　①ArrayListフィールド（users）をprivateなフィールドとして定義する
　②コンストラクタでusersに以下の情報をセットする。
　　以下の情報を持つUserインスタンス
　　　ログインID："user01"、パスワード："pass01"、姓："Yamada"、名："Taro"
　　以下の情報を持つUserインスタンス
　　　ログインID："user02"、パスワード："pass02"、姓："Suzuki"、名："Hanako"
　　以下の情報を持つUserインスタンス
　　　ログインID："user03"、パスワード："pass03"、姓："Tanaka"、名："Gonzalez"
　③showUsersメソッドでusersに格納されている各Userインスタンスの姓と名をコンソールに出力する。

ApiMain18クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①UserSampleクラスのインスタンスを生成し、showUsersメソッドを呼び出す。
```

<br>

**＜出力結果＞**

```
Yamada Taro
Suzuki Hanako
Tanaka Gonzalez
```

<br>

[解答例](/ans/api-18.md)

<br>

### 演習19　※演習18のつづき

```
UserSampleクラス（パッケージ：jp.kronos.sample）
　loginメソッドを定義し、以下の処理を記述する。
　①引数と戻り値は以下のように定義する。
　　引数：String（ログインID）、String（パスワード）
　　戻り値：boolean
　②引数のログインIDとパスワードに一致するUserインスタンスがArrayListフィールド（users）内に存在すれば戻り値としてtrueを返す。
　③Userインスタンスが存在しなければ戻り値としてfalseを返す。

ApiMain19クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①UserSampleクラスのインスタンスを生成し、loginメソッドを呼び出す。
　②戻り値がtrueの場合は「Login Success!」、falseの場合は「Login Failure!」とコンソールに出力する。
```

<br>

[解答例](/ans/api-19.md)

<br> -->