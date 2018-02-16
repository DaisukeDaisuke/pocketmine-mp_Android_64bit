  # pocketmine-mp Android 64bit
phpバイナリです。<br />
Androidでお使いになる場合は、ターミナルエミュレータが必要です。<br />

## install

`7.2.2-Android-AArch64-x64_compile-GD.zip`をダウンロードし、解凍します。<br />
以下のアプリケーションをインストールします。<br />
https://play.google.com/store/apps/details?id=jackpal.androidterm <br />
アプリを起動し、以下のコマンドを入力します。<br />
なお[download]などは適切なも物に変えましょう。<br />
```
cp [download]/php /data/data/jackpal.androidterm/app_HOME/php
chmod 777 /data/data/jackpal.androidterm/app_HOME/php
```

## pmmp/Pocketmine-MPのダウンロード

最新版のPocketMine-MPもダウンロードし、`[storage]/PocketMine/`か任意のフォルダに展開しましょう。<br />
https://github.com/pmmp/PocketMine-MP/archive/master.zip

## Composerのダウンロード
composer.phar<br />
https://getcomposer.org/composer.phar<br />

## start
```
cd [storage]/PocketMine/
env TMPDIR='[storage]/PocketMine/tmp' /data/data/jackpal.androidterm/app_HOME/php [storage]/PocketMine/PocketMine-MP.phar
```
### php.iniを設定したい場合
`7.2.2-Android-AArch64-x64_compile-GD.zip`の中に`php.ini`が入っていますので、<br />
それを任意のフォルダにコピーして使いましょう。<br />
```
cd [storage]/PocketMine/
env TMPDIR='[storage]/PocketMine/tmp' /data/data/jackpal.androidterm/app_HOME/php  -c  [storage]/PocketMine/php.ini [storage]/PocketMine/PocketMine-MP.phar
```
