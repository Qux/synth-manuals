# NoiseGen
## 回路図
![回路図](https://github.com/Qux/schematics/blob/master/noisegen/noisegen.svg)
![DCDC Converterの回路図](https://github.com/Qux/schematics/blob/master/noisegen/noisegen-DCDC%20Converter.svg)

## 部品
|記号|名前|数量|備考|
|---|-----------|-------|-------|
|C1|セラミックコンデンサ 0.1u|1|[秋月電子](https://akizukidenshi.com/catalog/g/g113582/)|
|C2, C3, C5|電解コンデンサ 10u|3|無極性<br>[秋月電子](https://akizukidenshi.com/catalog/g/g104621/)|
|C4|セラミックコンデンサ 2200p|1|[秋月電子](https://akizukidenshi.com/catalog/g/g112060/)|
|C6|チップコンデンサ 10u|1|実装済み|
|C7|チップコンデンサ 680p|1|実装済み|
|C8|チップコンデンサ 3.3u|1|実装済み|
|D1|チップダイオード 1N5819W|1|実装済み|
|J1|オーディオジャック MJ-352W-O|1|[秋月電子](http://akizukidenshi.com/catalog/g/gC-08958/)|
|L1|チップインダクタ 100u|1|実装済み|
|P1|USB-Cコネクタ|1|実装済み|
|P2, P3|-|2||
|Q1, Q2|NPNトランジスタ 2SC1815|2|[秋月電子](https://akizukidenshi.com/catalog/g/g106477/)|
|R1, R8, R9, R10|リード抵抗器 10kΩ|4|茶黒橙金|
|R2, R3|リード抵抗器 51kΩ|2|緑茶橙金|
|R4|リード抵抗器 220Ω|1|赤赤茶金|
|R5|リード抵抗器 2.2kΩ|1|赤赤赤金|
|R6, R7|リード抵抗器 4.7kΩ|2|黄紫赤金|
|R11|リード抵抗器 100kΩ|1|茶黒黄金|
|R12|チップ抵抗器 180Ω|1|実装済み|
|R13|チップ抵抗器 8.6kΩ|1|実装済み|
|R14|チップ抵抗器 1kΩ|1|実装済み|
|R15, R16|チップ抵抗器 5.1kΩ|2|実装済み|
|Rsc1|チップ抵抗器 560m|1|実装済み|
|RV1, RV2|可変抵抗器 100k|2|104<br>[秋月電子](https://akizukidenshi.com/catalog/g/g108014/)|
|U1|ICソケット 2x4|1|取付向き注意<br>[秋月電子](https://akizukidenshi.com/catalog/g/g100017/)|
|U1|オペアンプ NJU7043D|1|取付向き注意<br>[秋月電子](https://akizukidenshi.com/catalog/g/g106840/)|
|U2|電源IC MC34063AD|1|実装済み|


## 使い方
ノイズを出す基板です。
ホワイトノイズ（”サー”）やピンクノイズ（”ゴー”）のような音を出すことができます。
また、タッチ部分を触るとノイズの音が変わります。

<!-- ## 応用編 -->

## 回路について
３つのブロックで構成されています。
* 昇圧回路（電源電圧を5V→12Vに変換する）
* ノイズ発生回路
* フィルター＋増幅回路（ノイズの音や大きさを変える）

## Licence
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。
