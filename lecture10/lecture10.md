# 第10回課題  
## 課題内容  
CloudFormationを使用した環境構築の自動化  

## 1 ネットワーク環境の構築
[network](./yml/1network.yml)  

VPC  
![network](./network/vpc.png) 

パブリックサブネット  
![network](./network/pubsub1.png)   
![network](./network/pubsub2.png)  

プライベートサブネット  
![network](./network/prisub1.png)   
![network](./network/prisub2.png)  

ルートテーブル  
パブリック用  
![network](./network/pubrtb.png)  

プライベート用  
![network](./network/prirtb.png)

インターネットゲートウェイ  
![network](./network/igw.png)

## 2 セキュリティグループ  
[network](./yml/2security.yml)  

EC2のセキュリティグループ  
![network](./sec/secec2.png)  

RDSのセキュリティグループ  
![network](./sec/secrds.png)  

ALBのセキュリティグループ  
![network](./sec/secalb.png)  

## 3 EC2 
[application](./yml/3application.yml)  

作成したEC2  
![application](./app/ec2.png)  

IAMRole  
![application](./app/iamrole.png)  

## 4 RDS  
[application2](./yml/4pplication.yml)  

作成したRDS  
![application](./app/rds.png)  

## 5 ALB  
[application3](./yml/5application.yml)  

作成したALB  
![application](./app/alb.png)

ターゲットグループ  
![application](./app/tg.png)  

## 6 S3  
[application4](./yml/6application.yml)  

作成したS3 
![application](./app/s3.png)  

## 7 動作確認  

SSH接続  
![application](./dousakakuninn/ssh.png)　　

RDS確認  
![application](./dousakakuninn/RDS.png)　　

nginx起動確認  
![application](./dousakakuninn/nginx.png)  

S3バケット動作確認  
![application](./dousakakuninn/s3.png)  





## 感想　　
スタック作成時に何度もエラーを出された。その都度対応していくうちにエラー文を読むと、引っかかっている部分がわかり自力で解決できたことに成長を感じた。  
今回は初めてのクラウドフォーメーションを利用しての環境構築であった為、テンプレートファイルを細かく分けた方がやりやすいのでは？と考えたが、メンテナンスや管理のことを考えると、一つにまとめた方がよいのではないかと思った。




