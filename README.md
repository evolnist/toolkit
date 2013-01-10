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


### File API

[FileSystem](http://jsdo.it/kurukurupapa/kOKf)

	fileEntry.createWriter()


### 複数ファイルの一括取得

[JSZip](http://stuartk.com/jszip/)

	var zip = new JSZip();
	zip.file("Hello.txt", "Hello World\n");
	var img = zip.folder("images");
	img.file("smile.gif", imgData, {base64: true});
	var content = zip.generate();
	location.href="data:application/zip;base64,"+content;


### WebSQL


### Web Workers


### JSON

	JSON.stringify([1,2])
	JSON.parse('[1,2]')


### Local Strage

	window.localStrage
