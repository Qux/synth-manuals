# vco_revision_2
電圧で周波数を制御できるオシレータです。CV入力端子に`0~5V`の電圧を印加した場合、それに応じた周波数の矩形波もしくは三角波を出すことができます。

以前のVCOからの主な変更点は下記です。
* XHコネクタを追加し、電源の接続をしやすくしました。
* また、一部の部品を表面実装にしました。

## 回路図
![回路図](https://raw.githubusercontent.com/Qux/schematics/master/vco_revision_2/vco_revision_2.svg)

## 部品
|記号|名前|数量|備考|
|---|-----------|-------|-------|
|P101|基板用マイクロUSBコネクタ（電源専用）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10398/)|
|P102|ピンソケットなど自由に|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|P103,P104|XHコネクタ ベース付ポスト サイド型|2|[秋月電子](https://akizukidenshi.com/catalog/g/gC-12262/)|
|C101|セラミックコンデンサ 0.01uF|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10398/)|
|C102|電解コンデンサ 47uF|1|[秋月電子](https://akizukidenshi.com/catalog/g/gP-04627/)|
|IC101, IC102|ICソケット2x4|2|[秋月電子](https://akizukidenshi.com/catalog/g/gP-00017/)|
|IC101, IC102|NJU7043D|2|[秋月電子](https://akizukidenshi.com/catalog/g/gI-06840/)|
|J101|PJ324M (スイッチ付きオーディオジャック)|1|[マルツ](https://www.marutsu.co.jp/pc/i/46705/)|
|J102|MJ-352W-O（オーディオジャック）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-08958/)|
|Q101|2SC1815（NPNトランジスタ）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gI-17089/)|
|R101,R103,R104,R108,R109|抵抗器 51kΩ|5|[秋月電子](https://akizukidenshi.com/)|
|R102,R106,R107|抵抗器 100kΩ|3|[秋月電子](https://akizukidenshi.com/)|
|R105|抵抗器 10kΩ|1|[秋月電子](https://akizukidenshi.com/)|
|RV101|可変抵抗器 10kΩ（Aカーブ）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gP-14773/)|
|SW101|SS12D01G4（1回路2接点スライドスイッチ）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gP-12723/)|


## 使い方
`CV-Emitter`や他のオシレータなどを`CV IN`に接続します。入力された電圧に応じて発振の周波数が変わり、音の高さが変動します。 スライドスイッチを切り替えることによって、発振の波形を矩形波もしくは三角波に設定することができます。

XHコネクタの端子は、それぞれ電源(5V)とGNDです。外部からこの基板に電源を供給したり、この基板から外部に電源を出力するのに使用可能です。

### 応用編
C1の大きさに応じて、最大周波数が変わります。最大周波数が高くなると、全体的に音域が高くなる印象になります。C1の値が２倍になると、最大周波数は半分になります。

#### C1の大きさとおよその最大周波数
|C1の値|最大周波数|
|:--- |:-----------:|
|220pF|16kHz程度|
|470pF|8kHz程度|
|1000pF|4kHz程度|
|2200pF|2kHz程度|
|4700pF|1kHz程度|



## Licence
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。
