# REST_JSON_sample
jQueryを使用してIRISからJSONデータを取得するサンプルです

使用手順は以下になります。

<b>1. USERネームスペースにjson.xmlをインポート・コンパイル</b>

<b>2. テスト用データの作成（ターミナルで以下のコマンドを実行する）</b>

      USER>do ##class(Sample.Person).Populate(200)

<b>3. 初期設定（REST用）</b>

     管理ポータル > セキュリティ管理 > ウェブ・アプリケーション

     新しいウェブ・アプリケーションを作成ボタンを押す

     名前　/csp/user/rest
     ネームスペース    user
     ディスパッチ・クラス　REST.Person

     保存ボタンを押す

<b>4. test_json.htmlをWEBサーバに配置する</b>

     例：
     
     C:\Inetpub\wwwroot          <-- IIS ルート
     
     C:\InterSystems\IRIS\CSP\user     <-- cspフォルダ

<b>5. test_json.htmlをブラウザで開く</b>

     例：
     
     http://localhost/test_json.html
     
     http://localhost:52773/csp/user/test_json.html
     
     ※サンプル内のクロスドメイン対応URLは、http://127.0.0.1:52773/ を使用(PWS用サンプル)

<b>6. テキストボックスに適当なID(1,2,100など)を入力し、検索ボタンを押して出力結果を確認する。</b>
