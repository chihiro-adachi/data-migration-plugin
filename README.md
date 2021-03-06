# データ移行プラグイン for EC-CUBE4
ec-cube2系から出力出来るバックアップデータを利用して、2系から4系へのデータ移行をするプラグイン

https://www.ec-cube.net/products/detail.php?product_id=1804

## :sunny: 移行出来るデータ
### 会員データ
 - dtb_customer
 - dtb_customer_address
 - mtb_sex
 - mtb_job
### 管理者データ
 - dtb_member
 - mtb_authority
### 商品データ
 - dtb_product
 - dtb_product_class
 - dtb_class_category
 - dtb_class_name
 - mtb_sale_type
### カテゴリデータ
 - dtb_category
 - dtb_product_category
### 受注データ
 - dtb_order
 - dtb_shipping
 - dtb_order_item
### 支払い方法
 - dtb_payment ※データは移行するが非表示設定
### 配送方法
 - dtb_delivery ※データは移行するが非表示設定
 - dtb_delivery_fee
 - dtb_delivery_time
### 税設定
 - dtb_tax_rule
### :point_right: 他プラグイン連携
- 会員データ メールマガジン送付について [メルマガ管理プラグイン](https://www.ec-cube.net/products/detail.php?product_id=1760)

## :cloud: 移行出来ないデータ
### 商品画像
 - dtb_product_image
### カート
 - dtb_cart
 - dtb_cart_item
### 決済と配送の紐づけ
 - dtb_payment_option
### 決済モジュール

## :exclamation: 注意点
- アップロードファイルの最大容量はPHPの設定に依存します。(memory_limit, post_max_size, upload_max_filesize)
- PostgreSQLの場合は、super user権限が必要になります
- プラグイン内でcomposerを使用しているため、オーナーズストア経由のインストールが必要になります
- 新規に使う支払い方法と配送方法を設定する必要があります
- 複数配送は移行できません
- ダウンロード商品の受注データは移行できません
- ダウンロード商品も移行できません

## License
[LGPL](LICENSE)
