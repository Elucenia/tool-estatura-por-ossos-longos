<!-- ELUCENIA technical documentation · estatura-por-ossos-longos · zh · no clinical/professional/rights approval -->

# 根据长骨估算身高（Trotter 与 Gleser）

[条件、来源与许可](https://elucenia.org/zh/tools/estatura-por-ossos-longos)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 性别

`sexo`

- `F` — 女性
- `M` — 男性

### 测量的骨

`osso`

- `fem` — 股骨（最大长度）
- `tib` — 胫骨
- `fib` — 腓骨
- `hum` — 肱骨
- `rad` — 桡骨
- `ulna` — 尺骨

### 骨长

`comp`

cm · 范围: 10–70

### 估计年龄（可选，用于校正）

`idade`

年 · 选填 · 范围: 18–100

## 方法版本

Trotter–Gleser 1952 American Whites；年龄校正1951 \>30岁0.06 cm/年；原始人群受限

## 已记录的公式

身高（cm）=系数×骨长度（cm）+常数，采用Trotter–Gleser（1952）“American Whites”组方程。

年龄校正：超过30岁，每年减去0.06 cm（Trotter–Gleser，1951）。

## 限制与适用人群

这些回归方程对应所选版本的历史研究人群及骨长度定义，并非适用于所有祖源或年龄。请以 cm 测量，并记录骨骼和测量方法。Jantz 1995 发现 Trotter 的胫骨测量未包括踝部骨性突起；使用标准长度会使身高估计平均偏高 2.5–3 cm。不要混用测量定义或自动修正骨长度。本次审查尚未完整核对原始系数表和年龄修正。

## 参考文献

- [Trotter M, Gleser GC. Estimation of stature from long bones of American Whites and Negroes. Am J Phys Anthropol, 1952.](https://doi.org/10.1002/ajpa.1330100407)

- [Trotter M, Gleser GC. The effect of ageing on stature. Am J Phys Anthropol, 1951.](https://doi.org/10.1002/ajpa.1330090307)

- [Jantz RL, Hunt DR, Meadows L. The measure and mismeasure of the tibia: implications for stature estimation. J Forensic Sci, 1995.](https://doi.org/10.1520/JFS15379J)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
