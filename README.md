# PolyQuilt(ポリキルト)
---
PolyQuiltはローポリモデリングをサポートするBlender2.8用アドオンです。シンプルでオーソドックスでオールドスクールな面張り機能に加えてドラッグや長押し等のマウスオペレーションに様々な機能を割り振ることでツールの切り替えを最小限にしてポリゴンモデリングを支援します。
またタブレットやデジタイザ付きタブレットPCとの相性も良く、操作量を減らしつつ直感的にモデリングを行う事ができます。

# 導入方法

ダウンロードは[こちら](https://github.com/sakana3/PolyQuilt/releases/download/1.0.3/PolyQuilt_v1.0.3.zip)から

ダウンロードして編集→設定→アドオン→インストールよりダウンロード先を指定してインストールしてください。インストールした段階ではまだ使えませんのでその後検索バーよりPolyQuiltを検索しチェックボックスをOnにしてください。

編集モードに入るとPolyBuildの下にアイコンが追加されているのでこれをクリックでPolyQuiltがアクティブツールになります。

# 機能一覧

各種機能はクリック、ドラッグ、長押し、長押し後ドラッグの操作に割り振られています。空間、点辺面の要素との組み合わせで以下の機能が割り振られています。

||クリック|ドラッグ|長押し|長押し後ドラッグ| 
|:-:|:-:|:-:|:-:|:-:|
|空間|[頂点作成](#頂点作成)<br>→[面張り](#面張り)<br>→[ループカット](#ループカット)|ビュー回転(暫定)||[ナイフ](#ナイフ)||
|点|[面張り](#面張り)|[移動(結合)](#移動)|[削除/融解](#削除/融解)|[扇カット](#扇カット)<br>[エッジ押し出し](#エッジ押し出し)|
|辺|[頂点挿入→面張り](#面張り)|[移動](#移動)|[削除/融解](#削除/融解)|[ループ挿入](#ループ挿入)<br>[エッジ押し出し](#エッジ押し出し)<br>[ループカット](#ループカット)|
|面||[移動](#移動)|[削除](#削除/融解)||

---
## 移動  

点、線、面の上でマウスドラッグでビュー平面状の移動ができます。エッジの頂点は別エッジの頂点に近づける事で結合する事ができます。

## 頂点作成
何もない空間をクリックで頂点が作成されます。通常はそのまま面張りモードになりますがジオメトリを点モードにすれば連続で点を作れます。

## 面張り

何もないエリアか点の上でクリックで面張りを開始します。クリックする度に点、線、面が追加されます。最後に配置した点の上でクリック(ダブルクリックと同意)か右クリックで終了しまた新たな面を作ることができます。

画面上部のツールメニューより作成するジオメトリを点、線、三角形、四角形、ポリゴンから選ぶ事ができます。

また同一面の頂点でクリックすると面の分断になります。  

## 削除/融解

点、線、面の上で長押しでその要素を消去or融解します。共有する線や面がある場合は融解、そうでない場合は削除になります。

## ナイフ

空間で長押し後にドラッグでナイフを実行できます。

## ループカット

辺の上で長押し後ドラッグで辺をループカットできます。

## 扇カット

点の上で長押し後ドラッグで辺を扇状にループカットできます。

## エッジ押し出し

辺または点の上で長押し後ドラッグでエッジの押し出しをします。

## ループ挿入

辺ループを挿入します

## ループカット

辺ループをカットします

# 環境設定

ドキュメント準備中

## Extra Setting
特別な設定群です。上級者向け

### Check PolyQuilt add-on update 

ポリキルトを更新をチェックし最新版にアップデートする事ができます。上手くいかない場合は従来通りの方法でお願いします。

### ゲームエンジン風キーマップをセットアップ

右マウスボタン＋ドラッグでの視点変更にキーマップをセットアップします。標準で割り振られているコンテキストメニューはクリックで開く為、操作が被る事なくUnityやUE4といった主要ゲームエンジン風の操作を行う事ができます。キーマップを書き換える為、独自カスタムや他のアドオンとの衝突する場合があるので注意してください。

# フィードバック

フィードバックはGithubの[Issues](https://github.com/sakana3/PolyQuilt/issues)かTwitterアカウント[sakana3](https://twitter.com/sakanaya) まで宜しくお願い致します。

# 実装予定

- [ ] 分離(Rip)
- [ ] LoopCutの末端三角形対応
- [ ] 選択
- [x] ハンドリトポ編集
