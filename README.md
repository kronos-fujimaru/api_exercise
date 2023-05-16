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

### 演習11　※演習10のつづき

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

### 演習14　※演習13のつづき

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
Userクラス（パッケージ：jp.kronos.domain）
　ログインID、パスワード、姓、名のフィールドとそれぞれのgetter/setterを持つクラス。
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

**jp.kronos.dto.User.java**　※作成済み

```java
package jp.kronos.dto;

public class User {
    // ログインID
    private String loginId;
    
    // パスワード
    private String password;
    
    // 姓
    private String lastName;
    
    // 名
    private String firstName;
    
    /**
     * コンストラクタ
     * @param loginId ログインID
     * @param password パスワード
     * @param lastName 姓
     * @param firstName 名
     */
    public User(String loginId, String password, String lastName, String firstName) {
        this.loginId = loginId;
        this.password = password;
        this.lastName = lastName;
        this.firstName = firstName;
    }
    
    public String getLoginId() {
        return loginId;
    }
    public void setLoginId(String loginId) {
        this.loginId = loginId;
    }
    public String getPassword() {
        return password;
    }
    public void setPassword(String password) {
        this.password = password;
    }
    public String getLastName() {
        return lastName;
    }
    public void setLastName(String lastName) {
        this.lastName = lastName;
    }
    public String getFirstName() {
        return firstName;
    }
    public void setFirstName(String firstName) {
        this.firstName = firstName;
    }
}
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

<br>