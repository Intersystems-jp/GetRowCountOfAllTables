# GetRowCountOfAllTables

![image](https://user-images.githubusercontent.com/24215130/187606574-625d9e98-9632-40f6-8c12-a571d3416a51.png)
**このサンプルはInterSystemsで正式サポートしているものではありません。ご自身の責任においてご利用下さい  
　また、サンプル公開時の最新IRISバージョンで作成しておりますので、実際に使用されるIRISバージョン毎に動作確認をお願いします。**
 
*** 
ネームスペース内のテーブル情報を持つINFORMATION_SCHEMA.TABLESから情報を取得するクラスクエリをユーザコードで定義しています。
これを実行することで、全テーブル(もしくは条件に合う複数テーブル)の行数を一括で取得することが可能です。

[準備]<br>
GetRowCountOfTables.xmlをダウンロードし、処理を実行したいネームスペースにインポート&コンパイルします。

[実行]<br>
SQLのCall文で実行します。ODBC経由での実行も可能です。

(全テーブルの行数取得)<br>
call Sample.GetRowCountOfTables_TableRowCounts()

(テーブル名の一部を条件にして件数取得)<br>
call Sample.GetRowCountOfTables_TableRowCounts('%AAA%')
