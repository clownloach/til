# Google Maps API

地理的データを地図情報として提供する。Styling Wizard: Google Maps APIsから抽出した描画スタイルのパラメータを使用し、独自のマップスタイルを設定可能。(https://mapstyle.withgoogle.com)

* [Maps Statc API](#maps-static-api)
* [Street View Static API](#street-view-static-api)

## Maps Static API

埋め込み可能な地図画像を取得する。(https://developers.google.com/maps/documentation/maps-static/intro)

### APIパラメータ

```
https://maps.googleapis.com/maps/api/staticmap
?center=37.62761,-122.42588&zoom=17&format=png&size=640x480&maptype=roadmap&key={APIキー}
```

* center: マップの中心 (緯度,経度)
* zoom: ズームレベル
* format: 結果の画像形式 (gif,jpeg,png etc.)
* key: APIキー
* size: マップ画像の寸法
* scale: ピクセル解像度の倍数 (1,2,4)
* maptype: 構築するマップのタイプ
  * roadmap: Webサイトに表示される標準のロードマップ画像
  * satellite: 衛星画像
  * hybrid: 衛星画像とロードマップ画像の混在指定
  * terrain: 地形と植生を表示するレリーフマップ画像
* sensor: アプリケーションがセンサーを使用してユーザの位置を特定するかどうか (現在は不要)

### 料金

1,000リクエスト当たり$2.00(USD)。1ヶ月$200(USD)分の無料クレジット利用可能。

### 制限

* 1秒あたりの最大クエリ数(QPS): 500
* 1日あたり25,000までのリクエストはAPIキーが必要。
* 1日あたり25,000を超えるリクエストはAPIキーとデジタル署名が必要。

### 導入

1. APIライブラリ -> Maps Static APIを選択。
2. 有効にするをクリック。

## Street View Static API

360度のパノラマ画像を取得する。(https://developers.google.com/maps/documentation/streetview/intro)

### APIパラメータ

```
https://maps.googleapis.com/maps/api/streetview
?location=37.62827,-122.4259&fov=80&heading=0&size=640x480&pitch=-4&key={APIキー}
```

* location: 検索するロケーション (緯度,経度)
* fov: 画像の視野角
* heading: コンパスの向き
* size: 出力画像の寸法
* pitch: ストリートビュー撮影車に対する上向きまたは下向きの角度
* key: APIキー

### 料金

1,000リクエスト当たり$７.00(USD)。1ヶ月$200(USD)分の無料クレジット利用可能。

### 制限

* 1秒あたりの最大クエリ数(QPS): 500
* 1日あたり25,000までのリクエストはAPIキーが必要。
* 1日あたり25,000を超えるリクエストはAPIキーとデジタル署名が必要。

### 導入

1. APIライブラリ -> Street View Static APIを選択。
2. 有効にするをクリック。
