# 名刺ラボ アプリ版

このフォルダをそのままWebに置くと、スマホのホーム画面に入れて使えるアプリになります（PWA）。

- `index.html` … 名刺ラボ（自分の名刺をつくる）
- `cards.html` … 名刺ポケット（もらった名刺をしまう）
- `manifest.webmanifest`・`sw.js`・`icons/` … アプリとして入れるためのファイル

無料・登録なしで使えます。作った名刺やもらった名刺は、使っている端末の中だけに保存され、どこにも送られません。

名刺ポケットのQR読み取りには jsQR 1.4.0（Copyright Cosmo Wolfe、Apache License 2.0、https://github.com/cozmo/jsQR）を、名刺ラボのQR作成には QR Code Generator（Copyright Kazuhiko Arase、MIT License）を使っています。どちらもファイルの中に入っているので、ネットにつながっていなくても動きます。

名刺ポケットの「写真の文字を読む」には Tesseract.js 5.1.1 と tesseract.js-core 5.1.1（Apache License 2.0）、文字データ @tesseract.js-data/jpn・eng 1.0.0（tessdata、Apache License 2.0）を使っています。`ocr/` フォルダに入っていて、はじめて使ったときに読み込まれ、そのあとはネットなしでも動きます。
