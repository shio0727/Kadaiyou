# RaiseTech AWSフルコース　学習状況
## 学習概要  
2024年5月よりAWS講座の学習を開始いたしました。  
現時点で、学習した内容を振り返りとともにまとめていこうと思います。  
### 実施内容  
- EC2上でサンプルアプリケーションをデプロイ  
- CloudFormationを用いて環境構築を自動化
### 現時点でのインフラ構成図  
![構成図](/readmeimg/kouseizu.drawio.png)  
### 学習記録  


|講座|概要|提出課題|備考|
|:---:|:---|:----|:---|
|1|**導入**<ul><li> AWSアカウントの作成<li> IAMユーザーの作成<li> MFAの設定<li> Cloud9の作成|discordにて提出|
|2|**バージョン管理システムGitHub**<ul><li>GitHub基礎<li> Markdown|[lecture02](lecture02.md)|PRデモンストレーション有|
|3|**Webアプリケーション**<ul><li>Webアプリケーションとは<li> GemとBundler|[lecture03](lecture03.md)|Railsによるアプリケーション起動デモンストレーション有|
|4|**AWS環境の完成イメージ**<ul><li>AWSでの権限管理<li> VPC、サブネット構築<li> EC2インスタンスの作成<li> RDSの作成|[lecture04](lecture04.md)|
|5|**EC2にアプリケーションデプロイ**<ul><li>冗長化・負荷分散<li> アプリケーションデータの保存先の変更<li> S3の役割<li> インフラ構成図の書き方|[lecture05](mdfail5)
|6|**システムの安定稼働のために行うこと**<ul><li>証跡・ロギング<li> 監視・通知<li> コスト管理|[lecture06](lecture06/lecture06.md)|ALBアラーム通知デモンストレーション有|
|7|**システムにおけるセキュリティの基礎**<ul><li>脆弱性<li> 認証情報の流出<li> 人為的な過負荷<li> その他知っておくべきサービス|[lecture07](lecture07.md)|
|8|**第五回課題環境構築の実演前編**|課題なし|環境構築のデモンストレーション有|
|9|**第五回課題環境構築の実演後編**|課題なし|環境構築のデモンストレーション有|
|10|**インフラ自動化**<ul><li>インフラの自動化のメリット<li> 全自動と半自動<li> 自動化の範囲<li> CloudFormationについて<li> テンプレートの解説|[lecture10](lecture10/lecture10.md)|テンプレートのデモンストレーション有|
|11|**インフラコード化支援ツール**<ul><li> インフラのコード化を支援するツール<li> インフラのテストとは<li> テスト駆動開発<li> ServerSpec|[lecture11](lecture11.md)|
|12|**Terraformについて**<ul><li> Terraformの解説<li> DevOps<li> CI/CDツールとは<li> イベントトリガーの設定や連携|[lecture12](lecture12.md)|
|13|**構成管理ツール**<ul><li> 構成管理ツールとは<li> Ansible<li> Ansibleの導入<li> Opsworks<li> CircleCiとの併用|[lecture13](lecture13.md)|
|14|**ライブコーディング**|課題なし|AnsibleやCircleCIの導入のデモンストレーション有|
|15|**ライブコーディング**|課題なし|AnsibleやCircleCIの導入のデモンストレーション有|
|16|**現場での心構え**<ul><li> 1月受講予定
