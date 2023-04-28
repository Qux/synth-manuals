# VCO
電圧で周波数を制御できるオシレータです。CV入力端子に`0~5V`の電圧を印加した場合、それに応じた周波数の矩形波もしくは三角波を出すことができます。

## 回路図
![回路図](https://blog.qux-jp.com/wp-content/uploads/2019/08/VCO_with_pot.png)

## 部品
|記号|名前|数量|備考|
|---|-----------|-------|-------|
|P1   |基板用マイクロUSBコネクタ（電源専用）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10398/)|
|P2   |ピンソケットなど自由に|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|R1, R6, R7|抵抗器 100kΩ|3|[秋月電子](https://akizukidenshi.com/catalog/g/gR-25104/)|
|R2, R3, R4, R8, R9|抵抗器 51kΩ|3|[秋月電子](https://akizukidenshi.com/catalog/g/gR-25513/)|
|R5|抵抗器 10kΩ|1|[秋月電子](https://akizukidenshi.com/catalog/g/gR-25103/)|
|RV1|抵抗器 100kΩ|1|[秋月電子](https://akizukidenshi.com/catalog/g/gP-06113/)|
|C1|セラミックコンデンサ 470pF|1|[秋月電子](https://akizukidenshi.com/catalog/g/gP-08130/)|
|Q1|2SC1815（NPNトランジスタ）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gI-17089/)|
|IC1, IC2|ICソケット2x4|1|[秋月電子](https://akizukidenshi.com/catalog/g/gP-00017/)|
|IC1, IC2|NJU7043D|1|[秋月電子](https://akizukidenshi.com/catalog/g/gI-06840/)|
|SW1|SS12D01G4（1回路2接点スライドスイッチ）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gP-12723/)|
|J1|スイッチ付きオーディオジャック|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-02384/)|
|J2|MJ-352W-O（オーディオジャック）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-08958/)|


## 使い方
`CV-Emitter`や他のオシレータなどを`CV IN`に接続します。入力された電圧に応じて発振の周波数が変わり、音の高さが変動します。 スライドスイッチを切り替えることによって、発振の波形を矩形波もしくは三角波に設定することができます。

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
