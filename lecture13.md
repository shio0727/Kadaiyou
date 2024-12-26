## 第十三回課題  
### 課題内容  
- circleciにansibleとserverspecを追加して実行する。  
[課題に使用したリポジトリはこちら]()  

### 1 circleciに環境変数とSSH Keysを設定  
- 環境変数「AWS_ACCESS_KEY_ID」「AWS_DEFAULT_REGION」「AWS_SECRET_ACCESS_KEY」を設定  
![環境変数]()
- 「SSH Keys」を設定  
![SSH]()


### 2 cloudformationの実施  
RDSのパスワードはシークレットマネージャーで事前に決めたものを使用  
![cloudformation]()  
[cloudformationテンプレートファイル]()

### 3 ansibleの実施  
circleciをコントロールノード、AWSのEC2（前工程で作成）をターゲットノードとして、第三回講義の際に配布されたサンプルアプリケーションのデプロイを行った。 
![ansible]()  
![deploy]()  
[ansibleのテンプレートファイル]()  

### 4 serverspecの実施  
circleci上でserverspecを実施した。  
![serverspec]()
[ansibleのテンプレートファイル]()   
### 5 感想  
ansibleの成功までかなり時間を要してしまった。cloudformationで作成したリソースの値をansibleに渡す設定に手間取ってしまった。環境変数とは何かもう一度見直す良い機会になった。  
手動でアプリケーションを起動させる時とは違った難しさがあったが、一度起動できてしまえば再現性が高いので、タイムパフォーマンス的には良いのではないかと思った。