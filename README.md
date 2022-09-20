# GetRowCountOfAllTables

ユーザコードで定義したクラスクエリを使用して、全てのテーブルの行数を取得するサンプル

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
