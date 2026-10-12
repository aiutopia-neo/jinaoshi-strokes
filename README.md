# jinaoshi-strokes（字なおし 手本データ）

美文字・ペン字の練習アプリ「字なおし」が使う、字の筆順の線のデータです。
[KanjiVG](https://kanjivg.tagaini.net) の筆順の線を、書体 [Klee One](https://github.com/fontworks-fonts/Klee) の字形に重なるように変形したものです。

- 元のデータ: KanjiVG r20260714 — Copyright (C) 2009-2026 Ulrich Apel
- ライセンス: [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)（元のデータと同じ条件で公開します）
- KanjiVG の作者は、このデータやアプリを推薦・保証するものではありません。

## 変えたところ

- 各画の線（点の列）を、Klee One の字形の中に収まるように位置・大きさ・形を合わせた
- 画の終わり方（とめ・はね・はらい）の印（`end`）を足した
- 重ね合わせの基準に届かなかった字は `ok: false` とし、線を入れていない
- 書体の輪郭（Klee One の字形そのもの）は入れていない（書体は SIL OFL 1.1 で、別に配布されています）

## ファイル

| ファイル | 中身 |
| --- | --- |
| `data/v1/templates-basic.json` | ひらがな・カタカナ・よく使う漢字 |
| `data/v1/templates-names.json` | 名前・住所によく使う字 |
| `data/v1/manifest.json` | 版・大きさ・SHA-256 |

座標は、Klee One の em 正方形を 0〜1 にしたもの（左上が原点・下向きが +y）。各画は筆順どおりに並びます。

---

## English

Stroke data used by the handwriting practice app "Jinaoshi". Derived from [KanjiVG](https://kanjivg.tagaini.net)
(Copyright (C) 2009-2026 Ulrich Apel), adapted to fit the Klee One typeface, with stroke-ending labels added.
Licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Not endorsed by the KanjiVG author.
