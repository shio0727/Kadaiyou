## 第七回課題  
### セキュリティ意識について（講義を受けての感想）  
今回講義を受けて、セキュリティ意識が甘かったと気づかされました。  
エンジニアの知識不足が脆弱性につながる可能性があると感じた為、勉強していかないといけないと思いました。  
また、AWSのシステムがアップデートされていくのにつれて、新たな脆弱性が見つかっていくと思うので、自分の知識もアップデートし続けなければならないと感じました。  


### 課題で構築したシステムにおけるセキュリティリスクについて  
- HTTP通信（脆弱性）  
http通信は、平文でネットワーク上を流れるため盗聴・改ざん・などの脅威にさらされる可能性がある。  
そのためSSL接続を利用して対策をとらなければいけないのがセオリー。AWSにもサービスが存在する。  
AWS Certificate Manager（ACM）はSSL証明書を発行するマネージドサービス。このサービスを利用するだけではなく必ず HTTPS（SSL)通信をを経由するよ
うに設定を行わなければいけない。 

- パスワードやアクセスキーの流出（認証情報の流出）  
一番原因として考えられやすいのは、課題をgithubに載せた際に誤って公開してしまう事（写真として載せてしまうことなど）だと思われる。  
対策としては、MFA認証で本人以外のログインを防ぐことや、アクセスキーを発行しないなどの対策が求められる。　　

- DDos攻撃（人為的な過負荷）  
多数のコンピューターから連続でリクエストを送り、停止に追いやる。  
対策としては AWS Shieldというサービスがあり、Standardは無料で適応されている。Advancedは超高額サービスである。  

