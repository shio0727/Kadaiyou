## 第十一回課題  
### serverspecのテスト手順  
- 前提条件  
第十回で構築した環境、及びインストールしたサンプルアプリケーションを使用すること  
サンプルアプリケーションが起動できる事  

- 手順  
[公式ページ](https://serverspec.org/)の手順に従い作成  

#### 1 serverspecをインストール 
```bash:title
$ gem install serverspec  
#ec2-user配下でインストール  
```

#### 2 serverspecのテスト環境を設定  
```bash:title
$ serverspec-init  
#コマンドを入力すると以下写真のように選択肢が表示される  
#選択が終わるとspecディレクトリが表示される  
![syashinn1](img11/serverspec2.png)
```
#### 3 テストコードを記述    
今回は授業で配布された[テストコード]((https://github.com/MasatoshiMizumoto/raisetech_documents/tree/main/aws/samples/serverspec))を使用する。  
```bash:title
$ cd spec/localhost  
#local環境にてテストを実行  
$ vim sample_spec.rb  
#テストコードを打ち込む  
```
#### 4 テスト実行  
```bash:title
$ rake spec  
#localhostディレクトリにて  
```
成功した時  
![seikou](img11/seikou.png)  
失敗（テストコードで打ち込んだポート番号が違う）  
![shiltupai](img11/shiltupai.png)
