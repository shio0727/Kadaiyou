## 第十一回課題  
### serverspecのテスト手順  
- 前提条件  
第十回で構築した環境、及びインストールしたサンプルアプリケーションを使用すること  
サンプルアプリケーションが起動できる事  

- 手順  
[公式ページ](https://serverspec.org/)の手順に従い作成  

1 serverspecをインストール  
$ gem install serverspec  
# ec2-user配下でインストール  

2 serverspecのテスト環境を設定  
$ serverspec-init  
#コマンドを入力すると以下写真のように選択肢が表示される  
#選択が終わるとspecディレクトリが表示される  
![syashinn1]()

3 テストコードを記述  
今回は授業で配布された[テストコード]((https://github.com/MasatoshiMizumoto/raisetech_documents/tree/main/aws/samples/serverspec))を使用する。  
$ cd spec/localhost  
# local環境にてテストを実行  
$ vim sample_spec.rb  
# テストコードを打ち込む  

4 テスト実行  
$ rake spec  
# localhostディレクトリにて  
成功した時  
![seikou]()  
失敗（ポート番号が違う）  
![shiltupai]()
