==============================
Amandaについて
==============================
Amandaとは
==============================

Amanda（Amanda Network Backup）とはアメリカ、カリフォルニア州にあるzmanda社により開発された、クライアント-サーバ型のバックアップソリューションです。
amandaはオープンソースで公開され、ライセンスはBSD Licenceを採用されています。
オープンソース版のamandaのほか商用製品として、Amanda Enterprizeを開発されており、Amanzon S3へのバックアップや日常作業用の管理コンソール、データベース製品のホットバックアップ、対応ＯＳやプラットホームの充実などがコミュニティ版（オープンソース版）との差違にになります。

特徴
==============================
Amandaは、１〜複数のAmandaクライアントと通信を行い、バックアップデータを集約してテープに保管します。
テープをＨＤＤに置き換えて保管することも可能です。これをVTL = Virtual Tape Libraryと呼びます。
バックアップデータは一般的なdumpやtar、gzip形式ですので、専用のクライアントが無くてもデータの展開、復旧が可能です。

バックアップの仕組み
==========================
Amandaでは、

   #. サーバからバックアップの指示を対象のクライアントへ一斉に指示
   #. クライアントは指示を受け、バックアップに関する見積を実行
   #. 見積に従いバックアップデータを作成し、サーバへ送信
   #. サーバはクライアントより受け取ったデータを保存対象のテープへ保管

という流れでデータの保存を行います。

