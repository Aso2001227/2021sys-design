# DB定義書

## ER図

## データベース詳細

### 購入テーブル　(d_purchase)
|和名|属性名（カラム名）|型|PK|NN|FK|
|---|-------|-------|---|---|---|
|オーダーID|order_id|bigint(20)|○|○||
|購入コード|customer_code|varchar(50)||○||
|購入日|purchase_date|date||○||
|総額|total_price|int(11)||○||

### 購入詳細テーブル　(d_purchase_detail)
|和名|属性名（カラム名）|型|PK|NN|FK|
|------|-------|-------|---|---|---|
|オーダー詳細ID|detail_id|bigint(20)|○|○||
|オーダーID|order_id|bigint(20)|○|○|○|
|商品コード|lite_code|int(11)||○||
|価格|price|int(11)||○||
|数量|num|int(11)||○||

### m_customers
|属性名|型|PK|NN|FK|
|-------|-------|---|---|---|
|customer_code|varchar(50)|○|○
|pass|varchar(50)|○|○|○|
|name|varchar(20)○
|address|varchar(100)○
|tel|varchar(20)○
|mail|varchar(100)○
|del_flag|int(11)
|reg_date|date○||
