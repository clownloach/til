# Google Places API

地理的データをロケーション情報として提供する。

* [Places API](#places-api)

## Places API

ロケーションに関する最新情報を取得する。(https://developers.google.com/places/web-service/intro)

* Nearby Search requests: 指定したエリア内の場所を検索する。

### APIパラメータ

#### Nearby Search requests

```
https://maps.googleapis.com/maps/api/place/nearbysearch/json
?location=-33.8670522,151.1957362&radius=500&type=food&key={APIキー}
```

* loation: 検索するロケーション (緯度,経度)
* key: APIキー
* radius: 結果を返す領域の半径(m) (最大50,000m)
* type: 結果を返すロケーションの種別 (https://developers.google.com/places/web-service/supported_types)

### 料金

#### Nearby Search requests

1ヶ月$200分の無料クレジットで最大62,500読み込み可能。

### 制限

* 1秒あたりの最大クエリ数(QPS): 100

### 導入

1. APIライブラリ -> Places APIを選択。
2. 有効にするをクリック。
