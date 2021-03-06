====================
用語集
====================
用語
===================
Amandaではいくつか専門的な用語が出ます。
ここではその用語について説明をいたします。

* バックアップセット
   | Amandaではバックアップの定義や実行の単位をバックアップセットとして管理します。
   | デフォルトではDailySet1というバックアップセットを使用します。
   | 名前に制限はありません。

* テープライブラリ
   | 標準のデータ保存媒体はテープです。
   | ＨＤＤの任意の領域をテープとして利用することも可能です（仮想テープ：Virtual Tape）。
   | このテープを自動交換などに対応させたものがテープライブラリと呼ばれます。
   | 仮想テープを束ねたものをVTL（仮想テープライブラリ）と呼びます。

* ホールディングディスク
   | バックアップデータをサーバが受け取り、テープに記録するのに時間が必要なため、一時的な保存が必要です。
   | この一時的なデータ保存領域をホールディングディスクと呼びます。

* dumptype
   | バックアップデータの形式をdumptypeと呼びます。
   | データの作成形式、見積方法、などどの様にデータを作成するか定義された形式です。

* fullとincremental
   | fullは対象の部分全てをバックアップする方式で、incrementalはその差分のことです。
   | 差分はデータ量が小さくなるので、バックアップに費やす時間は短くなりますが、復旧の際にfullデータから順を追って復元しなければならないため、手順が増えます。
