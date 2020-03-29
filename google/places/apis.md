# Google Places API

地理的データをロケーション情報として提供する。

* [Places API](#places-api)

## Places API

ロケーションに関する最新情報を取得する。

### Nearby Search requests

指定したエリア内の場所を検索する。

#### APIパラメータ

```
https://maps.googleapis.com/maps/api/place/nearbysearch/json
?location=-33.8670522,151.1957362&radius=500&type=food&key={APIキー}
```

* loation: 検索するロケーション (緯度,経度)
* key: APIキー
* radius: 結果を返す領域の半径(m) (最大値は50,000m)
* type: 結果を返すロケーションの種別 (https://developers.google.com/places/web-service/supported_types)
