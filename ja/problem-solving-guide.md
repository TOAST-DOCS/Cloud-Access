
# Cloud Access トラブルシューティングガイド

**セキュリティ > Cloud Access > トラブルシューティングガイド**

<br>

## エージェントを接続したが、インスタンスにアクセスできません

ログイン後にインスタンスへアクセスするには、以下の設定を追加する必要があります。

* ルート設定
    * 詳細は [コンソール使用ガイド - はじめに](https://docs.nhncloud.com/ja/Security/Cloud%20Access/ja/console-user-guide/cloud-access-start/)を参照してください。
* ACLポリシー設定
    * 내부 인스턴스에 접근 시 적용되는 접근 제어 정책입니다. **ACL 정책** 탭에서 IP를 허용해야 합니다.
    * 内部インスタンスにアクセスする際に適用されるアクセス制御ポリシーです。**ACLポリシー**タブでIPを許可する必要があります。
* セキュリティグループ設定
    * インスタンスのセキュリティグループで送信元IPを許可する必要があります。

<br>

## Windowsユーザーですが、生体認証が使用できません

Cloud Accessの生体認証機能は、指紋認証や顔認証が可能なデバイスでのみ使用できます。
生体認証がない場合は、アカウント > サインインオプション メニューでPINを設定し、生体認証の代わりに使用できます。

<br>

## ユーザーアカウントは作成済みだが、「ユーザーオブジェクト追加」ボタンを押しても表示されません

以下の場合、ユーザーオブジェクト追加リストに表示されません。

* アカウント作成直後から認証完了前まで
    * 認証が完了しないとIPが確認できません。
* アカウント作成時にIPタイプを **動的IP(dynamic IP)** で設定した場合

<br>

## パスワードポリシーを有効にしたが、条件に合わないパスワードでもログインできます

パスワードポリシーを使用に設定して保存しても、既存ユーザーやすでにパスワードを変更したアカウントには適用されません。
パスワードポリシーは、初期パスワード強制変更オプションを選択して新しく作成されたアカウントにのみ適用されます。
この場合、該当アカウントのパスワードを初期化し、ポリシーに合ったパスワードを使用するよう案内してください。  

<br>

## 初期パスワード強制変更を設定したが、ログイン時に変更画面が表示されません

**初期パスワード強制変更**オプションは、設定後に新しく作成されたアカウントにのみ適用されます。
既に作成されたアカウントや、設定前に作成されたアカウントには適用されません。
該当アカウントのパスワードを初期化し、パスワードの変更を進めてください。

<br>

## 「アカウント連携」ボタンをクリックしたところ、アクティブなサービスがないというポップアップが表示されます

Cloud Accessサービスが非アクティブ状態の場合、アカウント連携はできません。
サービスを有効化してから再度連携を行うか、不要な連携は削除してください。

<br>

## 板橋と坪村の両リージョンでサービスを有効化した後、一方のみを無効にすることはできません

現在、すべてのリージョンが一括で無効化される仕様になっており、特定のリージョンのみを無効にする機能はサポートされていません。
特定のリージョンでのみ使用する場合は、一度サービスを無効化し、使用したいリージョンで再度有効化してください。
（個別リージョン削除機能は今後追加予定です）

<br>

!!! tip "問題が解決しない場合"
    トラブルシューティングガイドに従っても問題が解決しない場合は、NHN Cloudカスタマーセンターまでお問い合わせください。
    * [オンライン1:1お問い合わせはこちら](https://www.nhncloud.com/kr/support/inquiry?alias=tab16_15)
    * お問い合わせ電話: 1588-7967（受付時間: 月〜金 10:00〜19:00）