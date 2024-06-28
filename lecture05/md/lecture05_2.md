## 2 組み込みサーバーとunixsocket使用の動作確認 

2.1 pumaの設定
 ```bash:title 
 ##config/puma.rbの設定変更 
 # 下の一行を削除
 port   ENV.fetch("PORT") { 3000 }　

 # アプリケーションのpathを確認
 bind "unix:///home/ec2-user/raisetech-live8-sample-app/tmp/sockets/puma.sock"
 ```
2.2 pumaを起動させリッスンを確認、curlを使用してunixsocket通信でアクセス 
```bash:title
curl --unix-socket /home/ec2-user/raisetech-live8-sample-app/tmp/sockets/puma.sock http://localhost/
``` 



