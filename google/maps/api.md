# Google Maps API

地理的データを位置情報として提供する。

* [Maps Statc API](#maps-static-api)

## Maps Static API

埋め込み可能な地図画像を取得する。(例.https://maps.googleapis.com/maps/api/staticmap?key={APIキー}&center=37.62761,-122.42588&zoom=17&format=png&sensor=false&size=640x480&maptype=roadmap)

### 仕様

* center: マップの中心 (緯度,経度)
* zoom: ズームレベル
* format: 結果の画像形式 (gif,jpeg,png etc.)
* key: APIキー
* maptype: 構築するマップのタイプ
 * roadmap,satellite,hybrid,terrain
* sensor


### 料金

1ヶ月$200分の無料クレジットで最大100,000読み込み可能。
(https://developers.google.com/maps/documentation/maps-static/usage-and-billing?hl=ja)

### 制限

* 1日あたり25,000までのリクエストはAPIキーが必要。
* 1日あたり25,000を超えるリクエストはAPIキーとデジタル署名が必要。

### 導入

1. APIライブラリ -> Maps Static APIを選択。
2. 有効にするをクリック。

