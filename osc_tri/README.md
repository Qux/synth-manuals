# Triangle Oscillator
三角波を出すオシレータです。左のツマミで周波数、 右のツマミで音量を変えられます。スマートフォンの 充電器とイヤホンだけで気軽に楽しめます。

## 回路図
![回路図](https://raw.githubusercontent.com/Qux/schematics/master/osc_tri/osc_tri.svg)

## 部品
|記号|名前|数量|備考|
|---|-----------|-------|-------|
|P1|基板用マイクロUSBコネクタ（電源専用）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10398/)|
|P2|ピンソケットなど自由に|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|R1|220Ω抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R2|510kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R3, R4|100kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R5|10kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R6|180kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|RV1|1MΩ可変抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|RV2|100kΩ可変抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|C1|セラミックコンデンサ0.15uF|1|[秋月電子](https://akizukidenshi.com/)|
|IC1|6回路シュミットトリガインバータ SN74HC14N, IC ソケット 2x7|1|[秋月電子](https://akizukidenshi.com/)|
|IC2|オペアンプ NJU7043D, IC ソケット 2x4|1|[秋月電子](https://akizukidenshi.com/)|
|Audio Jack|MJ-352W-O|1|[秋月電子](https://akizukidenshi.com/)|

## 使い方
- `Vol`つまみを一番左に回し、イヤホンやスピーカーを`Audio Jack` に刺します。その後、スマートフォンの充電器などとUSBケーブルで電源を繋ぎます。
- `Vol`つまみを右に回すと、次第に音が聞こえてきます。`Freq`つまみを回してみてください。音量が変わります。`Audio Jack`に別のモジュールなどをつなぐこともできます。

## 応用編
コンデンサーと抵抗の組み合わせによって、周波数域を
変えられます。
__LFO__
- R1: 10kΩ / C1: 10μF
__LFO + 可聴域 ( 約 0.5Hz~663Hz)__
- R1: 220Ω / C1: 10μF

### Caution
- 出力波形の振幅は約 0~3.5V です
- イヤホンを接続する前に音量ツマミを 0 にしてください

## Licence
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。
