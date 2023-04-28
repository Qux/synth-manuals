# CV-Shield
## 回路図
![回路図](https://github.com/Qux/schematics/blob/master/cv-shield/cv-shield.svg)

## 部品
|記号|名前|数量|備考|
|---|-----------|-------|-------|
|R1-10|抵抗器10kΩ（茶黒橙金|10|[秋月電子](https://akizukidenshi.com/catalog/g/gR-25103/)|
|C1-6|セラミックコンデンサ0.047uF[473]|6|[秋月電子](https://akizukidenshi.com/catalog/g/gP-12059/)|
|C7-8|セラミックコンデンサ10uF[106]|2|[秋月電子](https://akizukidenshi.com/catalog/g/gP-08155/)|
|J1-8|縦型オーディオジャックMJ354WSG|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-15403/)|
|P5（基板上記載なし）|ピンヘッダ1x10|1|[秋月電子](https://akizukidenshi.com/)|
|P6（基板上記載なし）|足の長いピンソケット1x8|1|[秋月電子](https://akizukidenshi.com/)|
|P7（基板上記載なし）|ピンヘッダ1x8|1|[秋月電子](https://akizukidenshi.com/)|
|P8（基板上記載なし）|足の長いピンソケット1x6|1|[秋月電子](https://akizukidenshi.com/)|
|P9（基板上記載なし）|ピンソケット or ピンヘッダ 1x10|1|[秋月電子](https://akizukidenshi.com/)|
|P10（基板上記載なし）|ピンソケット or ピンヘッダ 1x8|1|[秋月電子](https://akizukidenshi.com/)|
|5V / GND|ピンソケット or ピンヘッダ 2x6|1|[秋月電子](https://akizukidenshi.com/)|

※詳しい配置は別紙の配置図を参照してください。

※基板上の記載（シルク）が一部間違っています。[別紙](./fig_cv-shield.PNG)に詳しく記載しているので、注意してご使用のほどよろしくお願いいたします。

## 使い方
ArduinoのPWM可能なピン (3, 5, 6, 9, 10, 11) がそれぞれオーディオジャックのJ1 - J6に対応しています。

`analogWrite` を使ってPWM信号を出力すると、ローあすフィルターを通った信号がQuxのシンセサイザー用のCV信号として使えるようになります。

↓ライブラリはこちら↓
https://github.com/Qux/CV-Shield


## 応用編
A0, A1 はオーディオ入力用として設計されています。

入力信号を2.5Vを中心となるようにバイアスする回路が搭載されており、`analogRead` 関数で読むことができます。

2.5Vが基準となるようにバイアスされているということは、`analogRead` 関数は入力信号がないときは511を返すことになります。オーディオレートで入力信号を取得するのは少し厳しいかもしれませんが、もしかしたらMozziなどと組み合わせても使えるかもしれません。

## Licence
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。
