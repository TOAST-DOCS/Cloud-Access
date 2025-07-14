# ログ

**セキュリティ > Cloud Access > コンソール使用ガイド > ログ**

**ログ**タブでは、Cloud Accessサービスの運用中に発生するさまざまなログをリアルタイムで検索できます。

<br>

## トラフィック

![traffic_log.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_cloud_access/2025.06.24/traffic_log.png)

ユーザーがエージェントを使用してCloud Access経由でインスタンスに接続する際に発生する通信トラフィックログを検索できます。
* 過去最大3か月間、1か月単位でログを検索可能です。

<br>

## 監査（Audit）

![audit_log.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_cloud_access/2025.06.24/audit_log.png)

ポリシーの作成や削除など、Cloud Accessサービスの変更履歴に関するログを検索できます。
* 最大1か月単位で検索可能で、組織サービスである CloudTrail からも検索できます。

<br>

## ユーザー

![audit_log.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_cloud_access/2025.06.24/user_log.png)

ユーザーがCloud Accessを使用している間に、エージェントで発生したすべてのログを検索できます。

<br>

## Excelダウンロード

検索結果をExcelファイルとしてダウンロードできます。

<br>

!!! tip "ポイント"
    * トラフィックログは最大7日間または5万件まで保存され、いずれかの条件を超えると、古いログから順に削除（上書き）されます。
        * ログを長期間保存する必要がある場合は、**設定**タブの**ログのリモート送信設定**を利用することをおすすめします。