# Easy VCF with POT
モノラルのフィルターです。0から5Vの制御電圧かつまみによって、入力音声にローパス・ハイパス・ バンドパスフィルタをかけることができます。

## 回路図
![回路図](https://github.com/Qux/schematics/raw/master/easyvcf_with_pot/easyvcf_with_pot.svg)

## 部品
|記号|名前|数量|備考|
| :--- |:-----------:|-------:|-------:|
|P1|基板用マイクロUSBコネクタ MRUSB-2B-D14NI-S306|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10398/)|
|P2|ピンソケットなど自由に|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|R1, 2, 6-9|100kΩ抵抗 茶黒黄金|6|[秋月電子](https://akizukidenshi.com/)|
|R3|27kΩ抵抗 赤紫橙金|1|[秋月電子](https://akizukidenshi.com/)|
|R4|10kΩ抵抗 茶黒橙金|1|[秋月電子](https://akizukidenshi.com/)|
|R4|330Ω抵抗 橙橙茶金|1|[秋月電子](https://akizukidenshi.com/)|
|RV4|可変抵抗器 100kΩ (104) |1|[秋月電子](https://akizukidenshi.com/)|
|C1, 3, 5-6|電解コンデンサ 4.7μF|4|[秋月電子](https://akizukidenshi.com/)|
|C2, 4|セラミックコンデンサ 0.047μF|2|[秋月電子](https://akizukidenshi.com/)|
|IC1, 2|オペアンプ NJM7043D ICソケット2x4|2|[秋月電子](https://akizukidenshi.com/)|
|SW1, 2|2回路2接点スライドスイッチ IS-2235|2|[秋月電子](https://akizukidenshi.com/)|
|U1, 2|アナログフォトカプラ LCR0202|2|[秋月電子](https://akizukidenshi.com/)|
|J1, 3|オーディオジャック MJ-352W-O|2|[秋月電子](https://akizukidenshi.com/)|
|J2|スイッチ付オーディオジャック PJ324M|2|[秋月電子](https://akizukidenshi.com/)|

## 使い方
- 5VのUSBハブなどで電源を接続します。
- この回路には2つのRCフィルターが直列に入っています。 2つのスイッチを`LP`にすると強いローパスフィルタが、 `HP`にすると強いハイパスフィルタが、LPとHPにするとゆるやかなバンドパスフィルタがかかります。
- 右下のつまみをまわすか、0~5V の電圧を`CV IN`に入力することで、約30-20,000Hz のカットオフ周波数で入力音声をフィルタリングできます。
- スライドスイッチを切り替えてみてください。`LP(low-pass)`にするとカットオフ周波数より大きな周波数が、 `HP(hi-pass)` にすると小さな周波数がゆるやかにカットされます。

### 注意
- アナログフォトカプラ LCR-0202 は、部品上の□印 をフットプリントの□に合わせて配置してください。
- CV IN に何かが接続されているときには、つまみは 機能しません。ご注意ください。

## Licence
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。
