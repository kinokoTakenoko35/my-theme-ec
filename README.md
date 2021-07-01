# my-theme-ec
Shopify theme開発用に遊ぶrepository

# shopify開発環境構築手順
## 1：Theme Kitをインストール(Mac)

```$ brew tap shopify/shopify```<br>
```$ brew install themekit```


## 2：Theme Kit pass を開発ストアから取得


## 3：既存のテーマに接続
```theme get --list --password=[your-password] --store="[your-store.myshopify.com]"```


## 4：設定ファイルを設定
```$ mkdir [your-theme-name]```<br>
```cd [your-theme-name]```<br>
```theme get --password=[your-password] --store="[your-store.myshopify.com]" --themeid=[your-theme-id]```


## 5：新しいテーマを作成する
```theme new --password=[your-password] --store="[your-store.myshopify.com]" --name=[theme name]```<br>
管理画面からテーマを複製して、ダウンロードするでもOK

## 6：テーマに更新をプッシュする
```theme watch --env=develop```<br>
```theme watch --env=production```

### 各種コマンド
編集内容の確認 ```$ theme open```<br>
Shopify側にあるテーマをローカル環境にダウンロード ```$ theme download```<br>
ローカル環境にあるデータをそのまま本番に反映する ```$ theme deploy```
