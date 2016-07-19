# 4d-tips-auto-upgrade
Example of automated upgrade of 4D, using curl (FTP), zip, unzip

**注記**: コードの性格上，不可欠な情報がいくつか隠匿されており，そのままではサンプルが動きません。

* Enginesフォルダー内が空
* Licensesフォルダー内が空
* ライセンスファイルの場所が未指定

``BuildApps/desktop-mac.xml``内47-48行目

```
<Item1>:Licenses:{your_license_file}.license4D</Item1>
<Item2>:Licenses:{your_license_file}.license4D</Item2>
```
* アップロード先FTPユーザー名，パスワード，パスが空

``Resources/auto-update.xlf``内22, 25, 29行目

Windowsプラットフォームでは``StartElevated``キーの設定も必要かもしれません。

http://doc.4d.com/4Dv15/4D/15/Overview.300-2399981.ja.html
