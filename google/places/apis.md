# Google Places API

地理的データをロケーション情報として提供する。

* [Places API](#places-api)
  * [Nearby Search requests](#nearby-search-requests)
  * [Place Details Requests](#place-details-requests)
  * [Place Photo Requests](#place-photo-requests)

## Places API

ロケーションに関する最新情報を取得する。(https://developers.google.com/places/web-service/intro)

## Nearby Search requests

指定したエリア内の場所を検索する。

### APIパラメータ

```
https://maps.googleapis.com/maps/api/place/nearbysearch/json
?location=-33.8670522,151.1957362&radius=500&type=food&key={APIキー}
```

* loation: 検索するロケーション (緯度,経度)
* key: APIキー
* radius: 結果を返す領域の半径(m) (最大50,000m)
* type: 結果を返すロケーションの種別 (https://developers.google.com/places/web-service/supported_types)

### 料金

1,000リクエスト当たり$32.00(USD)。1ヶ月$200(USD)分の無料クレジット利用可能。

### 制限

* 1秒あたりの最大クエリ数(QPS): 100

### 導入

1. APIライブラリ -> Places APIを選択。
2. 有効にするをクリック。

## Place Details Requests

place_idを使用してロケーションの詳細情報を取得する。

### APIパラメータ

```
https://maps.googleapis.com/maps/api/place/details/json?
place_id=ChIJN1t_tDeuEmsRUsoyG83frY4&key={APIキー}
```

* place_id: Place Searchから返されたロケーションの識別子
* key: APIキー

### 料金

1,000リクエスト当たり$17.00(USD)。1ヶ月$200(USD)分の無料クレジット利用可能。

### 制限

* 1秒あたりの最大クエリ数(QPS): 100

### 導入

1. APIライブラリ -> Places APIを選択。
2. 有効にするをクリック。

## Place Photo Requests

Placesデータベースに保存されている写真コンテンツを取得する。

### APIパラメータ

```
https://maps.googleapis.com/maps/api/place/photo?
photoreference=CnRtAAAATLZNl354RwP_9UKbQ_5Psy40texXePv4oAlgP4qNEkdIrkyse7rPXYGd9D_Uj1rVsQdWT4oRz4QrYAJNpFX7rzqqMlZw2h2E2y5IKMUZ7ouD_SlcHxYq1yL4KbKUv3qtWgTK0A6QbGh87GB3sscrHRIQiG2RrmU_jF4tENr9wGS_YxoUSSDrYjWmrNfeEHSGSc3FyhNLlBU&maxwidth=800&key={APIキー}
```

* photoreference: 写真の識別子
* maxheight/maxwidth: 写真の高さまたは幅
* key: APIキー

### 料金

1,000リクエスト当たり$7.00(USD)。1ヶ月$200(USD)分の無料クレジット利用可能。

### 制限

* 1秒あたりの最大クエリ数(QPS): 100

### 導入

1. APIライブラリ -> Places APIを選択。
2. 有効にするをクリック。
