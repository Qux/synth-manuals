# Delay
入力した音を遅らせて出力するモジュールです。 つまみをまわすことによって遅らせる時間を自在に 変えることができます。

## 回路図
![回路図](https://github.com/Qux/schematics/raw/master/delay/delay.svg)

## 部品
|記号|名前|数量|備考|
|---|-----------|-------|-------|
|P1|基板用マイクロUSBコネクタ（電源専用）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10398/)|
|P2|ピンソケットなど自由に|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|R1, 10, 13|100kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R2, 4-6, 15,16|10kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R3, 14|39kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R7, 17|33kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R8|22kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R9|4.7kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R11-12|5.6kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|R18|68kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|
|RV1|可変抵抗器 200kΩ 204|1|[秋月電子](https://akizukidenshi.com/)|
|RV2|可変抵抗器 50kΩ 503|1|[秋月電子](https://akizukidenshi.com/)|
|C1, 3, 9, 11, 16|電解コンデンサ 3.3μF|1|[秋月電子](https://akizukidenshi.com/)|
|C2, 5-6, 12-14|積層セラミックコンデンサ 2200pF (222)|1|[秋月電子](https://akizukidenshi.com/)|
|C4, 7, 8, 15|積層セラミックコンデンサ 220pF (221)|1|[秋月電子](https://akizukidenshi.com/)|
|C10|電解コンデンサ 22uF|1|[秋月電子](https://akizukidenshi.com/)|
|IC1, 4|NJU7043D(オペアンプ)  ICソケット4x2|1|[秋月電子](https://akizukidenshi.com/)|
|IC2|V3102(ディレイのドライバ) ICソケット4x2|1|[秋月電子](https://akizukidenshi.com/)|
|IC3|V3205(ディレイ) ICソケット7x2|1|[秋月電子](https://akizukidenshi.com/)|
|J1-2|MJ-352-O|1|[秋月電子](https://akizukidenshi.com/)|

## 使い方
- iPhoneやAndroidの充電器、パソコンのUSB ポートなどと電源を接続します。
- 左のオーディオジャックに音源をつなぎます。スマートフォンでも他のQuxの基板でもOKです。
- 右のオーディオジャックにスピーカーをつなぎます。
- `Adjust`つまみを回して音が綺麗に出るように調整します。 
- `Delay Time`つまみを回すと遅延時間を変えられます。音を鳴らしながら回すとビデオテープの早送りや、スロー再生のようになります。

## 応用編
`Send Return`と組み合わせると、ディレイをかける前後の音を混ぜることができたり、エコーがかかった音を出したりできます。

### Caution
Adjust つまみでの調整をしていないと音が全く出ないことがあります。忘れずに調整をお願いします。

## Licence
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。
