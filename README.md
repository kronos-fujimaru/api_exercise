# Java API

### 演習1

<pre>
StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"内に 'r' が含まれているかを T または F で表示しなさい。
</pre>


### 演習2

StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"内に "orl"が出現するインデックス位置を表示しなさい。


### 演習3

StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"内に 'l'が最後に出現するインデックス位置を表示しなさい。


### 演習4

StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"の文字数を表示しなさい。


### 演習5

StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HellaWarld"の'a'を'o'に置換して表示しなさい。


### 演習6

StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"を'o'で区切った部分文字列を改行しながらすべて表示しなさい。


### 演習7

StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"のインデックス位置、3～7の部分文字列を表示しなさい。


### 演習8

StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
"HelloWorld"をすべて大文字にして表示しなさい。


### 演習9

StringクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
" HelloWorld "の前後のスペースを排除して、表示しなさい。


### 演習10

SimpleListSampleクラス（パッケージ：jp.kronos.sample）を作成する。
executeメソッドに以下の処理を記述する。
　① String型の配列に「大阪」「東京」「名古屋」「福岡」の文字列をセットする。
　② 配列の値をすべてArrayListインスタンスに格納する。
　③ ArryListに格納されている値をすべて標準出力する。
 
ApiMain1クラス（パッケージ：jp.kronos.main）を作成する。
mainメソッドに以下の処理を記述する。
　① SimpleListSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。


### 演習11

Dog（パッケージ：jp.kronos.animal）
　①名前（name）を保持するprivateのString型フィールド
　②コンストラクタの引数で受け取った文字列をnameにセットする
　③showNameメソッドでは「私の名前は○○です。」と出力する

ListSample（パッケージ：jp.kronos.sample）
executeメソッドに以下の処理を記述する。
　①繰り返し標準入力で犬の名前を入力させる。ブランクが入力された場合標準入力処理を終了する
　②入力された名前の数だけDogクラスのインスタンスを生成し、名前をセットする
　③生成したDogインスタンスをすべてArrayListインスタンスに格納する
　④ArrayListインスタンスを戻り値として返す

ApiMain2クラス（パッケージ：jp.kronos.main）
　①ListSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。
　②戻り値で受け取ったList型のインスタンスからDogインスタンスを取得し、それぞれのshowNameメソッドを呼び出す。


### 演習12

ApiMain3
HashSetクラスのインスタンスを生成し、「CSS」「HTML」「JavaScript」「PHP」の文字列を格納する。
HashSetクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
「Java」がセットに存在する場合は「Javaコースはあります。」、存在しない場合は「Javaコースはありません。」と表示する。（存在しない想定）
セットに「Java」の文字列を追加し、再度存在チェックをする。


### 演習13

SimpleMapSample（パッケージ：jp.kronos.sample）
　①HashMapフィールド（cities）をprivateで定義する
　①コンストラクタでcitiesに以下の情報をセットする。（すべてString型の文字列）
　　キー："001" 値："大阪"
　　キー："002" 値："東京"
　　キー："003" 値："名古屋"
　　キー："004" 値："福岡"
 
　②executeメソッドでStringの引数（キー）を受け取り、cities内でキーに一致する値を取得し、標準出力する。

ApiMain4（パッケージ：jp.kronos.main）
　①SimpleMapSampleクラスのインスタンスを生成し、executeメソッドを呼び出す。
　※キーは適当に入力する（実行時引数でも良い）
 

### 演習14

ExceptionSample（jp.kronos.sample）
executeメソッド
　標準入力で整数値を入力させ,入力された値をint型に変換し標準出力する。
　整数値以外が入力され、java.lang.NumberFormatExceptionが発生した場合は、「整数値以外が入力されました」と出力する。

ApiMain5（jp.kronos.main）
　ExceptionSampleクラスのインスタンスを生成しexecuteメソッドを呼び出す。


### 演習15

CustomExceptionSample（パッケージ：jp.kronos.sample）
execute(String str)
　引数で受け取った文字列が5文字以内かチェックをし、6文字以上の場合はTooLongLengthExceptionをスローする。

TooLongLengthException（パッケージ：jp.kronos.exception）
　文字列の文字数が多すぎる際に発生する例外

ApiMain6（jp.kronos.main）
　標準入力で文字列を入力させる
　CustomExceptionSampleクラスのインスタンスを生成し入力された文字列を引数にexecuteメソッドを呼び出す。
　TooLongLengthExceptionが発生した場合は「文字列は5文字以内で入力してください」と出力する。


### 演習16

SimpleFileReaderSample（jp.kronos.sample）
List execute()メソッド
　テキストファイル「sample.txt」から読み込んだ文字列をArrayList<String>に詰めて返却する

sample.txt
　自由に作成しなさい

ApiMain7（jp.kronos.main）
　SimpleFileReaderSampleクラスのインスタンスを生成しexecuteメソッドを呼び出す。
　executeメソッドの戻り値を受け取り、すべて標準出力する。


### 演習17

ApiMain8
　本日の日付を「2019年3月15日 10時35分」の形式で表示しなさい。


### 演習18

ApiMain9
　CalendarクラスのAPIドキュメントを参照し、以下の課題を解きなさい。
　指定した日付の曜日を表示しなさい。
　（例）2019年3月15日なら「金曜日」と表示する。
