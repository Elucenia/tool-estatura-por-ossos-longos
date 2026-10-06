<!-- ELUCENIA technical documentation · estatura-por-ossos-longos · ja · no clinical/professional/rights approval -->

# 長管骨による身長推定（Trotter・Gleser）

[条件・出典・許諾](https://elucenia.org/ja/tools/estatura-por-ossos-longos)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 性別

`sexo`

- `F` — 女性
- `M` — 男性

### 測定した骨

`osso`

- `fem` — 大腿骨（最大長）
- `tib` — 脛骨
- `fib` — 腓骨
- `hum` — 上腕骨
- `rad` — 橈骨
- `ulna` — 尺骨

### 骨長

`comp`

cm · 範囲: 10–70

### 推定年齢（補正用、任意）

`idade`

年 · 任意 · 範囲: 18–100

## 方法の版

Trotter–Gleser 1952 American Whites；年齢補正1951 \>30歳0.06 cm/年；元の対象集団に制限

## 記載された計算式

身長（cm）=係数×骨長（cm）+定数。Trotter–Gleser（1952）の「American Whites」群の式を使用。

年齢補正：30歳を超える年数につき0.06 cmを差し引く（Trotter–Gleser，1951）。

## 限界・対象集団

これらの回帰式は、選択した版の歴史的研究集団と骨長の定義に基づき、すべての祖先集団や年齢に普遍的なものではありません。cm で測定し、骨と手技を記録してください。Jantz 1995 は Trotter の脛骨測定が果部を含まず、標準的な長さを用いると身長を平均 2.5–3 cm 過大推定することを指摘しました。測定定義を混在させたり、骨長を自動補正したりしないでください。原始係数表と年齢補正は、この審査で完全には確認されていません。

## 参考文献

- [Trotter M, Gleser GC. Estimation of stature from long bones of American Whites and Negroes. Am J Phys Anthropol, 1952.](https://doi.org/10.1002/ajpa.1330100407)

- [Trotter M, Gleser GC. The effect of ageing on stature. Am J Phys Anthropol, 1951.](https://doi.org/10.1002/ajpa.1330090307)

- [Jantz RL, Hunt DR, Meadows L. The measure and mismeasure of the tibia: implications for stature estimation. J Forensic Sci, 1995.](https://doi.org/10.1520/JFS15379J)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

推定身長 168.5 ± 3.27 cm（1標準誤差）

| 結果の詳細 | |
| --- | --- |
| 式（大腿骨） | 2.38 × 45.0 + 61.41 = 168.5 cm |
| 範囲 ± 2標準誤差（~95%） | 162.0 〜 175.0 cm |


### 2

推定身長 163.0 ± 3.66 cm（1標準誤差）

| 結果の詳細 | |
| --- | --- |
| 式（脛骨） | 2.90 × 35.0 + 61.53 = 163.0 cm |
| 範囲 ± 2標準誤差（~95%） | 155.7 〜 170.4 cm |


### 3

推定身長 170.3 ± 4.05 cm（1標準誤差）

| 結果の詳細 | |
| --- | --- |
| 式（上腕骨） | 3.08 × 33.0 + 70.45 = 172.1 cm |
| 年齢補正（30歳超で0.06 cm/年） | −1.8 cm |
| 範囲 ± 2標準誤差（~95%） | 162.2 〜 178.4 cm |


### 4

推定身長 159.2 ± 4.24 cm（1標準誤差）

| 結果の詳細 | |
| --- | --- |
| 式（橈骨） | 4.74 × 22.0 + 54.93 = 159.2 cm |
| 範囲 ± 2標準誤差（~95%） | 150.7 〜 167.7 cm |

