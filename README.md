realtime clock
===============

配信時の画面に現在時刻を表示します。

## 使い方
1. [ダウンロード](https://github.com/PRiMENON/realtime-clock/archive/master.zip)
1. 適当なフォルダに展開
1. `clock.html` を OBS などの配信ソフトのブラウザで開く
1. 表示位置を調整
1. 完了

## 初期設定

映像の手前に表示すると、黒文字が見ずらいので白文字になっています。  
そのために、何も表示されていないように見えます。

## カスタマイズ
### 日本語の年月日で表示したい
```
toFormat('yyyy-LL-dd HH:mm:ss')
👇
toFormat("yyyy'年'LL'年'dd'日' HH'時'mm'分'ss'秒'")
```

### 時刻の背景色をつけたい
```
<div id="time" class="style"></div>
👇
<div id="time" class="style style__background"></div>
```

色の指定は下記です。  
デフォルトは黒色になっていて、透明度を`.7`（0.7の省略指定）にしてあります。`1`が透明なしで、`0`に近ければ透明になります。
```
background: rgba(0,0,0,.7);
```

## ライブラリ
luxon.js という時刻表示ライブラリを使用しています。
* [Luxon](https://moment.github.io/luxon/) - MIT License

## 動作ブラウザ

* Google Chrome
* Mozilla Firefox

## ライセンス
MIT License
