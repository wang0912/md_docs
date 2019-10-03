# terraformの使用
## 1. 環境準備  
### 1.1 ツールのインストール
###### ローカルPCで以下のツールをインストールします。  
| 番号 | ツール名称 | 使用 | ダウンロードURL    
| :----------: | :----------: | :----------: | :----------:     
| 1 | Terraform | 生成とクラウド管理 | [https://www.terraform.io/downloads.html](https://www.terraform.io/downloads.html)
### 1.2 パラメータ設定（Windows側）
###### ローカルで実施するterraformパラメータを設定する。
    1.  terraformのローカルインストールアドレスをコピーする  
    2.  右クリック“PC”-->“プロパティ”-->“システムの詳細設定”-->“環境変数”-->“Path”を選択-->“編集”-->“新規”，最後、terraformのインストールアドレスを貼付け，全部確定する。    
# terraformの使用
## 1. 環境準備  
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
