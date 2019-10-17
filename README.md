# Java API 演習問題

#### APIドキュメント

<a href="https://docs.oracle.com/javase/jp/8/docs/api/" target="_blank">https://docs.oracle.com/javase/jp/8/docs/api/</a>

### 演習1

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"内に 'r' が含まれているかを T または F で表示しなさい。
```

[解答例](/ans/api-01.md)


### 演習2

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"内に "orl"が出現するインデックス位置を表示しなさい。
```

[解答例](/ans/api-02.md)


### 演習3

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"内に 'l'が最後に出現するインデックス位置を表示しなさい。
```

[解答例](/ans/api-03.md)


### 演習4

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"の文字数を表示しなさい。
```

[解答例](/ans/api-04.md)


### 演習5

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HellaWarld"の'a'を'o'に置換して表示しなさい。
```

[解答例](/ans/api-05.md)


### 演習6

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"を'o'で区切った部分文字列を改行しながらすべて表示しなさい。
```

[解答例](/ans/api-06.md)


### 演習7

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"のインデックス位置、3～7の部分文字列を表示しなさい。
```

[解答例](/ans/api-07.md)


### 演習8

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"をすべて大文字にして表示しなさい。
```

[解答例](/ans/api-08.md)


### 演習9

```
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
" HelloWorld "の前後のスペースを排除して、表示しなさい。
```

[解答例](/ans/api-09.md)


### 演習10

```
SimpleListSampleクラス（パッケージ：jp.kronos.sample）
　executeメソッドに以下の処理を記述する。
　①String型の配列に「大阪」「東京」「名古屋」「福岡」の文字列をセットする。
　②配列の値をすべてArrayListインスタンスに格納する。
　③ArryListに格納されている値をすべて標準出力する。
 
ApiMain1クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①SimpleListSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。
```

[解答例](/ans/api-10.md)


### 演習11

```
Dogクラス（パッケージ：jp.kronos.animal）
　①名前（name）を保持するprivateのString型フィールド
　②コンストラクタの引数で受け取った文字列をnameにセットする
　③showNameメソッドでは「私の名前は○○です。」と出力する

ListSampleクラス（パッケージ：jp.kronos.sample）
　executeメソッドに以下の処理を記述する。
　①繰り返し標準入力で犬の名前を入力させる。ブランクが入力された場合標準入力処理を終了する
　②入力された名前の数だけDogクラスのインスタンスを生成し、名前をセットする
　③生成したDogインスタンスをすべてArrayListインスタンスに格納する
　④ArrayListインスタンスを戻り値として返す

ApiMain2クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①ListSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。
　②戻り値で受け取ったList型のインスタンスからDogインスタンスを取得し、それぞれのshowNameメソッドを呼び出す。
```

[解答例](/ans/api-11.md)


### 演習12

```
ApiMain3クラス（パッケージ：jp.kronos.main）
　HashSetクラスのインスタンスを生成し、「CSS」「HTML」「JavaScript」「PHP」の文字列を格納する。
　HashSetクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
　「Java」がセットに存在する場合は「Javaコースはあります。」、存在しない場合は「Javaコースはありません。」と表示する。
　（存在しない想定）

　セットに「Java」の文字列を追加し、再度存在チェックをする。
```

[解答例](/ans/api-12.md)


### 演習13

```
SimpleMapSampleクラス（パッケージ：jp.kronos.sample）
　①HashMapフィールド（cities）をprivateで定義する
　②コンストラクタでcitiesに以下の情報をセットする。（すべてString型の文字列）
　　キー："001" 値："大阪"
　　キー："002" 値："東京"
　　キー："003" 値："名古屋"
　　キー："004" 値："福岡"
　③executeメソッドでStringの引数（キー）を受け取り、cities内でキーに一致する値を取得し、標準出力する。

ApiMain4クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①SimpleMapSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。
　　※キーは適当に入力する（実行時引数でも良い）
```

[解答例](/ans/api-13.md)


### 演習14

```
ExceptionSampleクラス（パッケージ：jp.kronos.sample）
　executeメソッドに以下の処理を記述する。
　①標準入力で整数値を入力させ,入力された値をint型に変換し標準出力する。
　②整数値以外が入力され、java.lang.NumberFormatExceptionが発生した場合は、「整数値以外が入力されました」と出力する。

ApiMain5クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①ExceptionSampleクラスのインスタンスを生成しexecuteメソッドを呼び出す。
```

[解答例](/ans/api-14.md)


### 演習15

```
CustomExceptionSampleクラス（パッケージ：jp.kronos.sample）
　executeメソッド(引数：String)
　　引数で受け取った文字列が5文字以内かチェックをし、6文字以上の場合はTooLongLengthExceptionをスローする。

TooLongLengthExceptionクラス（パッケージ：jp.kronos.exception）
　文字列の文字数が多すぎる際に発生する例外

ApiMain6クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①標準入力で文字列を入力させる
　②CustomExceptionSampleクラスのインスタンスを生成し、入力された文字列を引数にexecuteメソッドを呼び出す。
　③TooLongLengthExceptionが発生した場合は、「文字列は5文字以内で入力してください」と出力する。
```

[解答例](/ans/api-15.md)


### 演習16

```
SimpleFileReaderSampleクラス（パッケージ：jp.kronos.sample）
　executeメソッド(引数：なし、戻り値：List)
　　テキストファイル「sample.txt」から読み込んだ文字列をArrayList<String>に格納して返却する

sample.txt
　自由に作成しなさい

ApiMain7クラス（パッケージ：jp.kronos.main）
　mainメソッドに以下の処理を記述する。
　①SimpleFileReaderSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。
　②executeメソッドの戻り値を受け取り、すべて標準出力する。
```

[解答例](/ans/api-16.md)


### 演習17

```
ApiMain8クラス（パッケージ：jp.kronos.main）
　本日の日付を「2020年8月19日 09時15分」の形式で表示しなさい。
```

[解答例](/ans/api-17.md)


### 演習18

```
ApiMain9クラス（パッケージ：jp.kronos.main）
　CalendarクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
　あなたの生年月日の曜日を表示しなさい。
　（例）1986年8月19日なら「火曜日」と表示する。
```

[解答例](/ans/api-18.md)
