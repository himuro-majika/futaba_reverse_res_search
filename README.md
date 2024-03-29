# futaba_reverse_res_search
被引用レスをポップアップ表示・自分の書き込みへのレスを通知しちゃう
## なにコレ
ブラウザ上で動くUserscriptです  

ふたば☆ちゃんねるのスレ内のレスを逆引き検索します  
- スレ内のレスが引用された件数(被引用数)を表示し、マウスオーバーでポップアップします  
- 自分の書き込みと自分の書き込みへのレスを強調表示・一覧表示できます  
- 自分の書き込みへのレスがあった場合は通知を表示します  

※このUserscriptは[赤福Firefox SP](http://toshiakisp.github.io/akahuku-firefox-sp/)と[ふたクロ](http://futakuro.com/)とKOSHIANに対応しています

## インストール
[Greasyfork](https://greasyfork.org/ja/scripts/444185-futaba-reverse-res-search)


ユーザースクリプトマネージャーがインストールされていない場合は先に使用しているブラウザに応じたアドオンをインストールしてください

- Firefoxの場合: [Tampermonkey](https://addons.mozilla.org/ja/firefox/addon/tampermonkey/)  
- Chromeの場合: [Tampermonkey](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)  
- Edgeの場合: [Tampermonkey](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpaadaobahmlepeloendndfphd)  


## 使い方
* レスNo.の横にレスの被引用数(そのレス以降に引用された回数)が表示されます
* 被引用数をマウスオーバーで引用先のレスがポップアップ表示されます
* ポップアップ内のレス番号をクリックすると該当レスにジャンプします
* レスを投稿すると自分の書き込みしたレスのレス番号を青でハイライト表示し、レスNo.の横にマーカーを表示します
* ハイライト表示したレス番号またはマーカーをクリックすると自分の書き込みが一覧表示されます(もう一度クリックすると閉じます)
* 自分の書き込みを引用したレスが有る場合に引用先のレスのレス番号を赤でハイライト表示します
* 自分の書き込みの引用先のレス番号をクリックすると自分の書き込みへのレスが一覧表示されます(もう一度クリックすると閉じます)
* 書き込みフォームの削除キーの下に表示される[自分の書き込み]ボタンをクリックすると自分の書き込みを一覧表示します(もう一度クリックすると閉じます)
* 同じく[書き込みへのレス]ボタンをクリックすると自分の書き込みへのレスを一覧表示します(もう一度クリックすると閉じます)
* 追加のレスを読み込んだときに自分の書き込みにレスが付いた場合にブラウザの通知を表示し、[書き込みへのレス]の色を変えます(クリックすると色が戻ります)

※書き込み履歴について  

自分の書き込みをハイライト表示する機能に必要なためブラウザ内にデフォルトで直近100スレ分のURL、本文、レスNo.を保存します  
保存されている内容はTampermonkeyのダッシュボード=>futaba reverse res search=>ストレージタブから確認することができます  
この内容がどこかに送信されたり他のスクリプトから見られることはありません  

※オプションについて  

通知のオンオフ、通知の表示時間、マーカーの文字を変更したい場合はソースの先頭付近のオプションを書き換えてください  

## 更新履歴
* v1.0.2 2022-11-23
	- 引用先ポップアップの階層が2つまでだったのを無制限に
	- 初期化のタイミングを調整
* v1.0.1 2022-05-15
	- ふたクロでレス投稿時にマーカーがつかない問題を修正
	- 被引用レスの検索方法を修正
* v1.0 2022-04-29
	- 公開