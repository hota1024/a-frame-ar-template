# A-Frame AR template
このリポジトリは手っ取り早く[A-Frame](https://aframe.io/)でARを始めるためのリポジトリです。

# ファイル構成

- assets/
  - 画像やマーカーファイル(patt)用です。
- index.html
  - HTMLの雛形です。

# セットアップ
まずこのリポジトリをダウンロードし展開してください。

次に[こちら](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html)でマーカーを作成してください。
作成したら`DOWNLOAD MARKER`と`DOWNLOAD IMAGE`をクリックしマーカーのパターンファイル(patt)と画像ファイル(png)をダウンロードしてください。

先程ダウンロードしたマーカーのパターンファイル(patt)を`assets`フォルダに移動し、名前を`marker.patt`に変更してください。

以上でセットアップが完了します。

`index.html`にオブジェクトの情報などを書き込めばAR空間でもオブジェクトが表示されるはずです。

では、AR開発を楽しんでください。

# トラブルシューティング

- 画像が表示されない
  - ファイルのパスは合っていますか？
  - 角度(`rotation`)を`-90 0 0`にする
- マーカーを認識しない
  - マーカーファイルの名前は`maker.patt`になっていますか？この雛形ではデフォルトで`maker.patt`を読み込むようにしてあります。
  - マーカーファイルは`assets`フォルダに入っていますか？
  - マーカーの黒い縁にある程度の幅がないと認識しない可能性があります。パターンジェネレーターの`Pattern Ratio`を調整してみてください。
- カメラが起動しない
  - デバイスが対応していない可能性があります。
  - ドメインをSSLに対応させてますか？
  - iosのbeta版を使っていませんか？最新のbeta版にアップデートしましょう。
  - iosではARはSafariでしか表示されないようです
