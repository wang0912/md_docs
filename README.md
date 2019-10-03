# terraformの使用
## 1. 環境準備  
### 1.1 ツールのインストール
###### ローカルPCで以下のツールをインストールします。  [InternetShortcut]
URL=https://github.com/wang0912/md_docs/settings

| 番号 | ツール名称 | 使用 | ダウンロードURL    
| :----------: | :----------: | :----------: | :----------:     
| 1 | Terraform | 生成とクラウド管理 | [https://www.terraform.io/downloads.html](https://www.terraform.io/downloads.html)
### 1.2 パラメータ設定（Windows側）
###### ローカルで実施するterraformパラメータを設定する。
### 1.3 アクセスKeyを作る  
###### “アクセスKey”を作って、自動ツールでAlicloudにアクセスする  
    1. Alicloudにログインする（IDとパスワードは別途連絡）  
    2. 検索“ram”-->“ram コントロールパネル”を選択 [コントロールパネルURL](https://ram.console.aliyun.com/overview)
    3. 左側パネル“ユーザグループ”-->“新規ユーザグループ”，グループ情報を入力し確定する，“アクセル権限を追加する（AdministratorAccess（すべてのAlicloudにアクセスできる最高権限を付与する））”確定する
    4. 左側パネル“ユーザ”-->“新規ユーザ”，ユーザ情報を入力し確定する（アクセスKeyを保存する,アクセスKeyはパラメータ設定に使われる），“ユーザグループに追加する（新規作成されたユーザグループに追加される）”確定する。  <br>  
## 2. 生成する
### 2.1 Terraform  
    1. 以下のフォルダの中で2のコマンドを実行する（ terraform init,plan,apply)
    cd alicloud\terraform\cn-shanghai\01_initial\03_develop\01_vpc  
    cd alicloud\terraform\cn-shanghai\02_common\03_develop\01_oss  
    cd alicloud\terraform\cn-shanghai\03_services\03_develop\01_ecs  
    2. 以下のコマンドを実行する  
    terraform init  
    terraform plan  
    terraform apply(確認画面でyesを入力する)
