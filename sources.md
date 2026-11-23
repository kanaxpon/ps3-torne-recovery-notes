# 参照した公開資料

以下は調査で参照した一次資料です。各プロジェクトの対象機器・版・機能は異なり、この事例で録画の復号に成功したことを示すものではありません。

- [PS3 バックアップユーティリティー](https://manuals.playstation.net/document/jp/ps3/current/settings/backuputility.html)：バックアップ・復元の対象と制約。
- [PS3xport](https://github.com/kakaroto/ps3xport)：バックアップ層の索引・データ処理。参照した上流コミットは `95479d35c02be32a8034634f9455ca70f60498f7`。
- [torne 外付けHDDに関するサポート](https://www.playstation.com/ja-jp/support/hardware/accessories-torne-external-hdd/)：公式の録画ストレージ説明。
- [torne](https://www.playstation.com/ja-jp/torne/) と [uke-torne](https://manuals.playstation.net/document/jp/uketorne/)：公式の機能・対応機器。対応機器への転送と汎用動画ファイルへの復号は区別する。
- [PS3HENのプラグイン読込み実装](https://github.com/PS3Xploit/PS3HEN/blob/master/payload/modulespatch.c)：USB/HDDのboot_plugins.txtの探索・読込み。
- [webMAN MOD](https://github.com/aldostools/webMAN-MOD)：参照・配布物照合に用いたコミットは `6bd4425229544e60c5c8cfdcadb664dfb163d9f3`。
- [固定版のHTML生成処理](https://github.com/aldostools/webMAN-MOD/blob/6bd4425229544e60c5c8cfdcadb664dfb163d9f3/include/init/html.h)、[設定画面](https://github.com/aldostools/webMAN-MOD/blob/6bd4425229544e60c5c8cfdcadb664dfb163d9f3/include/setup.h)、[PS3MAPIサーバー](https://github.com/aldostools/webMAN-MOD/blob/6bd4425229544e60c5c8cfdcadb664dfb163d9f3/include/ps3mapi/ps3mapi_server.h)。
- [webMAN Setup Options](https://github.com/aldostools/webMAN-MOD/wiki/Setup-Options)：設定項目の説明。Wikiの記述と特定の実機表示が常に一致するとは限らない。
- [Ghidra](https://github.com/NationalSecurityAgency/ghidra)：静的解析。デコンパイル結果だけで分岐の有無を決めず、命令列も確認した。
- [coax](https://github.com/Till0196/coax/tree/63643f0019187e6fef80f0e17294bc7535207b6c)、[ghidra-fr60](https://github.com/aleph-void/ghidra-fr60/tree/cc91ae7f3085f2e64f9ce07a1038fd4b8ed5d477)：関連チップ・命令セットを調べる参考資料。今回の保存録画を復号できると確認したものではない。
- [PS3 セーフモード](https://www.playstation.com/ja-jp/support/hardware/ps3-safe-mode/)：USBコントローラー要求画面の照合用。中断時の実画面がセーフモードだったと確定する資料ではない。
