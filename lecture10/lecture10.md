# 第10回課題  
## 課題内容  
CloudFormationを使用した環境構築の自動化  

## 1 ネットワーク環境の構築
[network](/yml/1network.yml)  

VPC  
![network](./network/VPC.png) 

パブリックサブネット  
![network](lecture10/network/pubsub1.png)   
![network](lecture10/network/pubsub2.png)  

プライベートサブネット  
![network](lecture10/network/prisub1.png)   
![network](lecture10/network/prisub2.png)  

ルートテーブル  
パブリック用  
![network](lecture10/network/rtb2.png)  

プライベート用  
![network](lecture10/network/rtb1.png)

インターネットゲートウェイ  
![network](lecture10/network/igw.png)

## 2 セキュリティグループ  
[network](lecture10/security.yml)  

EC2のセキュリティグループ  
![network](lecture10/sec/SECEC2.png)  

RDSのセキュリティグループ  
![network](lecture10/sec/SECRDS.png)  

ALBのセキュリティグループ  
![network](lecture10/sec/SECALB.png)  

## 3 EC2 
[application](lecture10/application.yml)  

作成したEC2とSSH接続の確認  
![application](lecture10/app/ec2.png)  

IAMRole  
![application](lecture10/app/IAMrole.png)  

## 4 RDS  
[application2](lecture10/application2.yml)  

作成したRDS  
![application](lecture10/app/RDS2.png)  

RDS接続確認  
![application](lecture10/app/RDS.png)  

## 5 ALB  
[application3](lecture10/application3.yml)  

作成したALB  
![application](lecture10/app/ALB.png)

ターゲットグループ  
![application](lecture10/app/tg.png)  

## 6 S3  
[application4](lecture10/application4.yml)  

作成したS3と動作確認  
![application](lecture10/app/s3.png)  


## 感想　　
スタック作成時に何度もエラーを出された。その都度対応していくうちにエラー文を読むと、引っかかっている部分がわかり自力で解決できたことに成長を感じた。　　
今回は初めてのクラウドフォーメーションを利用しての環境構築であった為、テンプレートファイルを細かく分けた方がやりやすいのでは？と考えたが、メンテナンスや管理のことを考えると、一つにまとめた方がよいのではないかと思った。




