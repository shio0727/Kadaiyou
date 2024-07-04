#  第６回課題  
## 1 CloudTrailにてログを確認する（選んだイベントの内容を３つ取り上げる）  

- "event Time":"2024-07-01T14:01:44z"  
- "eventSource":"ec2.amazonaws.com"  
- "eventName": "StopInstances"  

![kiroku](lecture06/img/1kiroku.png)  
![kiroku2](lecture06/img/2event3.png)  

## 2 CloudWatchアラームを設定する（ALBのアラームの設定)  
対象およびメトリクス：ALB/UnhealtyHostCount  
閾値およびアクション：60 秒あたりに 1 以上/E メール通知（Amazon SNS を利用)  

- Railsアプリ停止状態  

![alarm](lecture06/img/4alarm.png)  
![alarm](lecture06/img/3alarm-email.png)  

- Railsアプリ起動状態  

![ok](lecture06/img/6ok.png)  
![ok](lecture06/img/5ok-email.png)  

## 3 AWS利用料の見積作成  
AWS Pricing Calculatorにて作成  
- URL:https://calculator.aws/#/estimate?id=ca25f0a2468c3755d2375583a66449dbc872f903  

## 4 現在の利用料金の確認  
- EC2はすでに無料利用枠を超えていた。  
- 最も高い請求額はRDSであった。理由としては、リージョンを間違えて作ってしまったRDSが起動していることに気が付かなかったことが原因である。

![6gatu](lecture06/img/8six.png)  
![utiwake](lecture06/img/9kakinn.png)
![ec2](lecture06/img/7ec2.png)