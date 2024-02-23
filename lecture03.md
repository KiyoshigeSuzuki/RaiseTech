# AWSコース Lecture03 課題
## サンプルアプリケーションの起動
[サンプルアプリケーション「Listing fluits」](.RaiseTech/images/cloud9_Listingfruits.png)

1. APサーバーについて調べる。  
    - APサーバーの名前とバージョン  
      APサーバー:puma  
      バージョン:5.6.8   
      [Version](./images/version.png)

    - APサーバー終了後アクセスできるか、また再起動後アクセスできるか。  
      APサーバー終了後、"Oops No application seems to be running here!"  
      と表示されアクセスできなくなった。  
      再度、"bin/cloud9_dev"でAPサーバーを起動し、アクセスできることを確認した。  
      [NoApplication Server](./images/cloud9_noAP.png)

2. DBサーバーについて調べる。
    - DBサーバーの名前とバージョン  
      DBサーバー:mysql  
      バージョン:8.0.36  
      [Version](./images/version.png)
    - DBサーバーを終了後アクセスできるか。  
      DBサーバーを終了する(Database.yml内のPasswordを空欄にしてDBサーバーにアクセスできないようにした)と、
      "ActiveRecord::DatabaseConnectionError"によりアクセスできなくなった。  
      [NoDataBase Server](./images/cloud9_noDB.png)  

     - Railsの構成管理ツール  
      Bundler(ver 2.3.14)  
      [Version](./images/version.png)


3. 感想  
- Webアプリケーションはブラウザ上で表示される全てのコンテンツやサービスであることを学んだ。 
- 利用者にアウトプットされる情報だけではなく、利用者がインプットする情報を取り扱うのもWebアプリケーションであると理解した。
- システム開発のワークフローは、何か問題が発生すること前提で遂行するべきである。
