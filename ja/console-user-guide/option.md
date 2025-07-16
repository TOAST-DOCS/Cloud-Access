# 設定

**Security > Cloud Access > コンソール使用ガイド > 設定**

**設定**タブでは、Cloud Accessの運用に必要なさまざまな設定を行うことができます。

<br>

## ログ設定

### 基本ブロックポリシーログ設定

Cloud Accessサービスを有効にすると、**ポリシー - ACLポリシー** タブにdefault-denyポリシーが表示され、**使用**に設定した場合、該当するポリシーに一致するブロックログが保存されます。

### ログの遠隔送信設定

Cloud Access運用中に発生したトラフィックログを遠隔地に自動送信し、長期保存できるように、Syslog、Object Storage、Log & Crash Searchによる遠隔送信機能を提供します。

* Syslog:最大2つのIPアドレスを入力してトラフィックログを送信します。

![syslog.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_cloud_access/2025.06.24/syslog.png)

* Object Storage: NHN Cloudが提供するObject Storageサービスにログを送信します。

![OBS.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_cloud_access/2025.06.24/OBS.png)

* Log & Crash Search: NHN Cloudが提供するLog & Crash Searchサービスにログを送信します。

![LNCS.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_cloud_access/2025.06.24/LNCS.png)

<br>

!!! tip 「参考情報」

    * Syslogは単一のIPアドレスのみを設定でき、IP範囲または帯域はサポートしていません。
    * Object StorageおよびLog & Crash Searchにログを送信するには、該当するサービスが事前に有効化されている必要があります。
    * Object Storage設定に必要な入力情報は[Object Storageユーザーガイド](https://docs.nhncloud.com/ko/Storage/Object%20Storage/ko/s3-api-guide/#aws-sdk)を参照してください。

<br>

## 一般設定

### 接続設定

* 接続設定では、Cloud Accessサービスを有効化した際に入力した情報を確認でき、そのうち顧客名とアルゴリズムは変更可能です。
    * アルゴリズムはAES-256とChaCha20をサポートします。

### ログインセキュリティ設定

* ログインセキュリティ設定では、ログイン失敗回数、パスワード有効期限、パスワードポリシーを設定できます。
    * ログイン失敗：ユーザーが認証を試行する際の最大失敗回数を設定します。
        * 最小1回から最大5回まで設定できます。
    * パスワード有効期限:アカウント作成後のパスワードの有効期間を設定します。
        * 最小1日から最大180日まで設定可能です。
    * パスワードポリシー:エージェント経由でアクセスするユーザーのパスワード作成基準を設定します。
        * 一部必須ポリシーは設定の有無に関わらず自動的に適用されます。

### 案内設定

* 案内設定では、ユーザーがエージェント経由で認証時に表示する通知メッセージを設定できます。
    * 案内フレーズは最大200文字まで入力可能です。

### ロゴ設定

* ロゴ設定では、ユーザーの法人ロゴなど、指定された条件に合う画像をアップロードし、ログイン認証画面にロゴを表示するように設定できます。

<br>

!!! tip 「参考情報」

    * 接続設定項目中のドメインと顧客キー、及び秘密鍵は、ユーザーがエージェント接続を追加する際に使用する情報です。外部に漏洩しないようご注意ください。
    * ログイン失敗またはパスワードの有効期限切れによりアカウントがロックされた場合は、Cloud Accessサービス権限を持つNHN Cloudコンソール管理者にお問い合わせください。
    * 案内メッセージは、ログイン後もトレイアイコンの機能を通じて確認できます。

!!! danger "注意"

    * ログインセキュリティ設定は、Cloud Accessエージェントを使用する全てのユーザーに共通で適用されますので、設定時にご注意ください。
