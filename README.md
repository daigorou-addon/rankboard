# RankBoard（ランキング表メーカー）

ランキングのデータを打ち込むだけで、SNSにそのまま使える「かっこいい表付き画像」を作れるWebツールです。インストール不要、ブラウザだけで使えます。

**公開ページ：https://daigorou-addon.github.io/rankboard/**

## 特徴

- 国別・都道府県別・自由なテーマなど、ランキングならなんでも作れます
- 国名を入れると国旗を表示（日本語名または2文字コード。例：`jp`）
- 値は数字でなくてもOK（`S/A/B`、`★★★`、`〇×` など）
- 8種類の表のタイプ：A 順位表 / B ティア表 / C 表彰台 / D バーチャート / E カードグリッド / F ピラミッド / G ヒーロー（1位ポスター）/ H ネオン
- 配色：Green / Blue / Red / Dark
- 画像サイズ：自動／スマホ縦 9:16（1080×1920）／正方形 1:1（1080×1080）／横長 16:9（1280×720）
- 表のタイプごとに値の形（数値・★・S/A/B）と区分の有無を変えたサンプル（7テーマ：ペット・フルーツ・寿司ネタ・プログラミング言語・スポーツ・音楽ジャンル・面積が大きい国）
- 元に戻す（↶）／やり直す（↷）
- 作業内容を `.json` で保存・読み込み
- 表を PNG 画像で保存
- 6言語対応：日本語 / English / 한국어 / 简体中文 / 繁體中文 / Español
- ライト／ダーク表示の切り替え、スマホ・タブレット対応

## 使い方

1. **表のタイプを選ぶ**（見た目の形）
2. **サンプルを選ぶ**（中身のテーマ）。タイプは変わらず、中身だけが入れ替わります
3. **タイトル・データを編集する**
4. 「PNGで保存」で画像を保存

### データの書き方

1行に1件、`名前, 値, 区分` の形で入力します（区分は省略可）。

```
フランス,★★★★★,必見
日本,★★★★☆,人気
```

値は数字でも、★やS/A/Bなどの文字でもOKです。区分を入れると、どのタイプでもバッジなどで表示されます。

ティア表（B）は1行に1ティアで、`ティア名|項目,項目,…|説明` の形です（説明は省略可）。行を増やせば D・E・F… 何段でも作れます。

```
S|東京大学,京都大学|あらゆる分野で突出
A|一橋大学,大阪大学|高い水準で安定
```

### 順位の付け方

入力順 / 値が大きい順 / 値が小さい順 / 順位なし から選べます。数値の場合は同順位も扱います。

### 保存と読み込み

- ヘッダーの「保存」で、タイトル・データ・タイプ・配色などの作業内容を `rankboard.json` に書き出します
- 「読み込み」で、保存した `.json` を選ぶと続きから編集できます

## プライバシー

すべての処理はお使いの端末内で行われます。入力したデータやファイルはどこにも送信されません。

## サポート

daigoroutools：https://daigorou-addon.github.io/daigorou-tools/

気に入ったら応援してもらえると励みになります：https://buymeacoffee.com/daigorou

---

# RankBoard (English)

A web tool that turns your ranking data into a stylish table image, ready to post on social media. No installation required.

**Live: https://daigorou-addon.github.io/rankboard/**

- Rank anything: countries (with flags), prefectures, or free-form items
- Values can be non-numeric (S/A/B, ★, ○× …)
- 8 table types: Ranking table / Tier list / Podium / Bar chart / Card grid / Pyramid / Hero / Neon
- 4 color themes, 4 image sizes (auto, 9:16, 1:1, 16:9), 7 sample themes matched to each table type
- Undo / redo; save your work as `.json` and load it back; export the table as PNG
- 6 languages: 日本語 / English / 한국어 / 简体中文 / 繁體中文 / Español
- Light / dark mode, works on phones and tablets
- Everything runs on your device. Nothing is sent anywhere.

daigoroutools：https://daigorou-addon.github.io/daigorou-tools/

Support: https://buymeacoffee.com/daigorou

---

Copyright (C) 2026 daigorou-tools. All rights reserved.
