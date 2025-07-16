# ログ

**Security > Cloud Access > コンソール使用ガイド > ログ**

**ログ** タブでは、Cloud Accessサービスを運用中に発生する様々なログをリアルタイムで検索できます。

<br>

## トラフィック

![traffic_log.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_cloud_access/2025.06.24/traffic_log.png)

ユーザーがエージェントを接続してCloud Accessサービス経由でインスタンスに接続する際の通信トラフィックログを検索できます。
* 照会は1か月単位で、最大過去3か月分のデータまで検索可能です。

<br>

## Audit

![audit_log.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_cloud_access/2025.06.24/audit_log.png)

ユーザーポリシーの作成や削除など、Cloud Accessサービスに関する変更内容のログを検索できます。
* 照会は最大で1か月単位での検索が可能であり、組織サービスであるCloudTrailでも検索できます。

<br>

## ユーザー

![audit_log.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_cloud_access/2025.06.24/user_log.png)

ユーザーがエージェントにログイン後、Cloud Accessを使用している間にエージェントで発生するすべてのログを検索できます。

<br>

## Excelダウンロード

ログの検索結果をExcelでダウンロードできます。

<br>

!!! tip 「参考情報」

    * トラフィックログは最大7日間または50,000件まで保存され、いずれかの条件を満たすと、最も古いログから順に削除（上書き）されます。
        * 別途データ保存が必要な場合は、**設定** タブの **ログリモート送信設定** の使用を推奨します。
