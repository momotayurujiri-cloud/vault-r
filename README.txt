VAULT//R v0.2 — Android「アプリっぽく使う」版

■ v0.2で変わったこと
・Androidのホーム画面からVAULT//R単体で起動できるPWA仕様を強化
・インストール後はブラウザの「タブ1」などのUIが消え、standalone表示
・ホーム画面用VAULT//Rアイコン追加
・オフライン起動対応（初回読み込み後）
・画面下のナビをAndroidの安全領域に合わせて調整
・v0.1のローカルデータが同じサイト/ブラウザにある場合は自動引き継ぎ
・バックアップ形式をv0.2に更新

■ まず中身だけ試す
ZIPを展開 → index.html をChrome等で開く。
この場合は「LOCAL PREVIEW MODE」なので、ブラウザのタブバー等は残ります。

■ 本命：ホーム画面に普通のアプリみたいに入れる
PWAのインストールには、VAULT//RをHTTPSまたはlocalhostで開く必要があります。

一番簡単な流れ：
1. このフォルダ一式をHTTPS対応の静的ホスティングに置く
2. AndroidのChromeでそのURLを開く
3. VAULT画面の「INSTALL VAULT//R」またはChromeメニューの「アプリをインストール」を押す
4. ホーム画面にVAULT//Rアイコンが追加される
5. 以後はアイコンから起動 → ブラウザのタブバーなしで使える

※ コレクション情報と写真は、インストールしたVAULT//Rのブラウザストレージに保存されます。
※ ブラウザデータ削除・端末故障に備えて、VAULT → EXPORT BACKUP を定期的に使ってください。

■ フォルダ構成
index.html                アプリ本体
manifest.webmanifest      PWA設定
sw.js                     オフラインキャッシュ
assets/vault-cover.png    表紙
assets/icon-192.png       アプリアイコン
assets/icon-512.png       アプリアイコン

VAULT//R — COLLECT. RECORD. REMEMBER.
