# Square Oscillator
矩形波を出すオシレータです。左のつまみで周波数、右のつまみで音量を変えられます。スマートフォンの充電器とイヤホンだけで気軽に楽しめます。

## 回路図
![回路図](https://github.com/Qux/schematics/raw/master/osc_sqr/osc_sqr.svg)

## 部品
|記号|名前|数量|備考|
|---|-----------|-------|-------|
|P1|基板用マイクロUSBコネクタ（電源専用）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10398/)|
|P2|ピンソケットなど自由に|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|R1|220Ω抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R2|510kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|RV1|1MΩ可変抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|RV2|10kΩ可変抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|C1|積層セラミックコンデンサ0.15uF|1|[秋月電子](https://akizukidenshi.com/)|
|IC1|6回路シュミットトリガインバータ SN74HC14N, ICソケット 2x7|1|[秋月電子](https://akizukidenshi.com/)|
|IC2|NJU7043D, ICソケット 2x4|1|[秋月電子](https://akizukidenshi.com/)|
|Audio Jack|MJ-352W-O|1|[秋月電子](https://akizukidenshi.com/)|



## 使い方
1. `Vol`つまみを一番左に回し、イヤホンやスピーカーを`Audio Jack`に刺します。その後、スマートフォンの充電器 などと USBケーブルで電源を繋ぎます。
2. `Vol`つまみを右に回すと、次第に音が聞こえてきます。`Freq`つまみを回してみてください。音量が変わります。`Audio Jack`に別のモジュールなどをつなぐこともできます。

## 応用編
- 抵抗とコンデンサーの組み合わせによって、周波数域を変えられます。
__LFO( 約 1Hz~200Hz)__
- R1: 2.2kΩ / R2: 1MΩ / C1: 10μF
__LFO + 可聴域 ( 約 1Hz~20,000Hz)__
- R1: 10Ω / R2: 1MΩ / C1: 4.7μF

### Caution
- イヤホンを接続する前に音量ツマミを0にしてください。


## Licence
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。
