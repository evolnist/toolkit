# Batch Toolkit

## 目的

PHP製のツール郡をHTML5化して、
ブラウザだけでオフラインアプリケーションとして実行できるようにする


## 方針

* PHP製のツールの移植ではなく、HTML5に最適な実装方法を模索する
* 動作環境はChromeなど実装が容易なものを指定してかまわない
* 動作するようになったら公開する


### AppCache
	window.applicationCache


### FileSystem

http://jsdo.it/kurukurupapa/kOKf

	fileEntry.createWriter()


### 複数ファイルの一括取得

JSZip
http://stuartk.com/jszip/


### WebSQL


### Web Workers


### JSON

	JSON.stringify([1,2])
	JSON.parse('[1,2]')


### Local Strage

	window.localStrage
