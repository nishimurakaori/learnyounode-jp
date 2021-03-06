拡張子のフィルタを使ってファイルリストをコンソールに出すアプリを書いてください。アプリの一つ目のアーギュメントはフォルダーのパスです（例えば `/あなた/の/フォルダー/`)。 拡張子は二つ目のアーギュメントです。

例えば：`"txt"`が二つ目のアーギュメントだったら*後ろに.txt*がついてあるだけファイルのリストを表示しないといけません。メモ：二つ目のアーギュメントは`"."`プレフィックスがありません。

コンソールにそのリストを出してください。一つのファイル名は一行。**ASYNC**I/Oが要件です。

----------------------------------------------------------------------
## HINTS

`fs.readdir()`というメソードの一つ目のアーギュメントはパスです。コールバップは二つ目です。コールバックはこのようになります：

```js
function callback (err, list) { /* ... */ }
```

`list`はファイル名のStringのArrayです。

`fs`のモジュールドキュメントはブラウザーを使ってこのリンクにアクセスできます:
  {rootdir:/node_apidoc/fs.html}

Nodeの `path` も役に立つかもしれません。とくに `extname` のメソード.

`path`のモジュールドキュメントはブラウザーを使ってこのリンクにアクセスできます:
  {rootdir:/node_apidoc/path.html}

----------------------------------------------------------------------
