インストール（Cent OS 6)
**************************

サーバインストール
===================

Cent OS 6では標準リポジトリにAmandaが登録されています。
yumを使用する事で簡単にインストールが可能です。

# yum install amanda-server

上記コマンドで必要な多数のファイルがインストールされます。

クライアント側よりamrecoverコマンドでファイルの復元を行うためにamandadというコマンドがサーバ側に必要となります。
amandadはamanda-clientをインストールすると登録されます。

# yum install amanda-client


クライアントインストール
========================

サーバインストールの時と同様にyumコマンドでインストールします。

# yum install amanda-client


