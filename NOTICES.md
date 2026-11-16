# 使用部品と出典

マインスイーパーの個人利用・内輪共有向け試遊版．ゲーム本体の出典と第三者部品のライセンスは区別する．

- Python 3.12.14（Windows），ブラウザで観測したPython 3.12.12．
- pygame-ce 2.5.8（Windows）／2.5.7（Web）：LGPL-2.1-or-later．本ゲームはpygame-ceを改変していない．Windows版は同梱DLL／拡張モジュールを外部配置する．対応する公開ソース配布物をthird_party/sourcesへ同梱する．
- PyInstaller 6.22.3：COPYINGの例外条項を含めて保持．
- pygbag 0.9.3：MIT．tools/web/default.tmplは取得済み公式テンプレートを利用する．音声はHTMLAudioElementで扱い，ゲーム内の入力で開始するため，pygbag独自のメディア操作待ちは使わない．
- SE7種・BGM：本ゲーム用にtools/generate_audio.pyで合成した音源．外部の楽曲・録音サンプルは使わない．assets/audio/README.mdとmanifest.jsonに生成方法・長さ・ハッシュを記録する．
- Noto Sans CJK JP：SIL OFL．assets/font-manifest.jsonとOFL原文を参照．
- atomicfile 1.0.0：本プロジェクトの共通部品．docs/reuse/ORIGIN.json参照．

third_partyには同版を使用した前作の保全済み原文・出典・pygameソース配布物を引き継いだ．docs/reuse/notices-origin.jsonにファイルごとのSHA-256を記録する．原文の前作向けREADME・manifestは取得時点の参考記録であり，本ゲームの検証結果を示さない．受入候補の検証範囲は同梱CHECK-STATUS.mdを参照する．上流ビルドの全経路を再調査したとは扱わない．

WebのCDN参照先は https://pygame-web.github.io/cdn/0.9.3/ である．同梱ソース配布物とライセンスはゲーム開始時のプリロードには含めない．

## この配信先での原文・ソースの取得

[出典・ライセンス・対応ソース一式](third-party-notices-and-sources.zip)をダウンロードして展開すると，元のthird_partyフォルダ構成で閲覧できる．受入候補の全原文・対応ソースを保持し，ゲーム開始時の通信量を増やさないため別ZIPで提供する．
