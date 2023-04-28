# template
## 回路図
![回路図](https://github.com/Qux/schematics/blob/master/adsr/adsr.svg)

## 部品
|記号|名前|数量|備考|
|---|-----------|-------|-------|
|P1|基板用マイクロUSBコネクタ（電源専用）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10398/)|
|P2, 3|ピンソケットなど自由に|2|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|C1|セラミックコンデンサ0.001uF|1|[秋月電子](https://akizukidenshi.com/)|
|C2|電解コンデンサ47uF|1|[秋月電子](https://akizukidenshi.com/)|
|D1-4|ダイオード1N914|4|[秋月電子](https://akizukidenshi.com/)|
|D5|LED|4|Vfが1.8V~4.0Vの範囲内にあるものを使用してください。[秋月電子](https://akizukidenshi.com/catalog/g/gI-09851/)|
|IC1|タイマーIC NE555|1|[秋月電子](https://akizukidenshi.com/)|
|J1|スイッチ付きオーディオジャック|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-02384/)|
|J2|オーディオジャック|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-08958/)|
|Q1-3, 5|NPNトランジスタ 2SC1815|1|[秋月電子](https://akizukidenshi.com/)|
|Q4|PNPトランジスタ 2SA1015|1|[秋月電子](https://akizukidenshi.com/)|
|R1, 2, 7, 10|抵抗器10kΩ(茶黒橙金)|1|[秋月電子](https://akizukidenshi.com/)|
|R3, 4, 6, 8|抵抗器2.2kΩ(赤赤赤金)|1|[秋月電子](https://akizukidenshi.com/)|
|R5|抵抗器47kΩ(黄紫橙金)|1|[秋月電子](https://akizukidenshi.com/)|
|R9|抵抗器4.7kΩ(黄紫赤金)|1|[秋月電子](https://akizukidenshi.com/)|
|R11, 12|抵抗器1kΩ(茶黒赤金)|1|[秋月電子](https://akizukidenshi.com/)|
|RV1-4|可変抵抗器10kΩ Aカーブ RK09D|1|[秋月電子](https://akizukidenshi.com/catalog/g/gP-14773/)|
|SW1|タクトスイッチ|1|[秋月電子](https://akizukidenshi.com/catalog/g/gP-03648/)|


## 使い方
【入力】

GATEに波形を入れるか、ボタンを押します。GATEにHighを入れることは、ボタンを押すことと同じです。GATEにLowを入れることは、ボタンを離すことと同じです。

【出力】

ボタンを押したとき、出力はHighを出そうとします。立ち上がりにかかる時間をAttackによって変えられます。

出力は立ち上がったあとすぐ、Sustainの電圧まで下がろうとします。Decayによって立ち下がる時間を変えられます。ボタンを押し続けていれば、出力は電圧を維持します。

ボタンを離したとき、出力はLowを出そうとします。立ち下がりにかかる時間をReleaseによって変えられます。

※Attack、Decay、Releaseは時間の設定です。Sustainは電圧の設定です。

【つなぎ方】

ADSRの出力をVCAのCVに接続するのが、最もわかりやすいです。VCAのINには別途音を入力しておきます。

ADSRのボタンを押すと、音がだんだん大きくなります。ボタンを離すと、音がだんだん小さくなります。この音量の変化を決めているのがAttack、Decay、Sustain、Releaseです。

## 応用編
GATEにLFOの矩形波を入れることもできます。

出力をVCFのCVにつなげることもできます。

その他いろいろ活用方法があります。基本的な動作が理解できたら挑戦してみてください。

## 注意事項
ボタンを押している間、DC電圧が出続けます。DC電圧をかけてはいけないところに接続しないように注意してください。

## Licence
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。
