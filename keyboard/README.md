# Keyboard
電圧で制御する基板に CV 電圧を与える基板です。 8 つのボタンと出力電圧を設定するためのつまみ、 ポルタメント、CV/GATE 出力を搭載しています。

## 回路図
![回路図](https://github.com/Qux/schematics/raw/master/keyboard/keyboard.svg)

## 部品
|記号|名前|数量|備考|
| --- | -----------|-------|-------|
|P1|基板用マイクロUSBコネクタ（電源専用）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10398/)|
|P2|ピンソケットなど自由に|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|CON1|L字型ピンソケット 1x6|1|[秋月電子](https://akizukidenshi.com/)|
|CON2|L字型ピンヘッダ 1x6|1|[秋月電子](https://akizukidenshi.com/)|
|R1~8, R11|抵抗器 10kΩ|1|[秋月電子](https://akizukidenshi.com/)|
|R9|抵抗器 1MΩ|1|[秋月電子](https://akizukidenshi.com/)|
|R10|抵抗器 1kΩ|1|[秋月電子](https://akizukidenshi.com/)|
|RV1-9|可変抵抗器 100kΩ|1|[秋月電子](https://akizukidenshi.com/)|
|C1|電解コンデンサ 4.7μF|1|[秋月電子](https://akizukidenshi.com/)|
|Q1-8|NPN トランジスタ 2SC1815|1|[秋月電子](https://akizukidenshi.com/)|
|SW1-8|タクトスイッチ|1|[秋月電子](https://akizukidenshi.com/)|
|IC1-5|オペアンプ NJU7043D, ICソケット 2x4|1|[秋月電子](https://akizukidenshi.com/)|
|IC6,7|4回路OR TC74HC32AP, ICソケット 2x7|1|[秋月電子](https://akizukidenshi.com/)|
|J1,2|オーディオジャック MJ-352W-O|1|[秋月電子](https://akizukidenshi.com/)|

## 仕様
各つまみで出力電圧を設定し、つまみの真下にあるスイッチを押している間設定した電圧を`CV OUT`から出力します。
上段にあるつまみはポルタメントです。つまみを回すと、`CV OUT`から出力される電圧が推移するのにかかる時間を設定することができます。右に回すほど推移時間が長くなります。
`GATE`出力からは、どれか1つでもボタンを押している間は5V、1 つも押していないときは0Vを出力できます。こちらはポルタメントの値に関わらず、瞬時に変化します。
複数の `Keyboard` を横に連結していくこともできます。 この場合連結した `Keyboard` のうち一番右の `Keyboard` のポルタメントが全体に適用されます。

## 調整方法
それぞれのボタンに対し、ボタンを押しながらつまみを回してちょうど良い電圧になるようにつまみの位置を決めます。ツマミの位置を決める際にポルタメントは 0(一番左)にしておくと良いでしょう。

## 繋げ方の例
### 1.VCO と繋げて音を出す
![繋げ方1](https://blog.qux-jp.com/wp-content/uploads/2019/04/image.png)
チューニングすれば8音階のモノフォニックシンセサイザーになります。ポルタメントを掛けると音程が下がりきるまで 音が鳴り続けます。

### 2.GATE出力をVCAに入れる
![繋げ方2](https://blog.qux-jp.com/wp-content/uploads/2019/04/image-2.png)
ボタンを押している間、VCAが5Vを受け取って音を出し、離すと0V を受けて音量が0になります。ポルタメントを掛けるとアタックは音程が「ポオォ~ン」と上がって、ボタンを離した瞬間に音が途切れるようになります。


![画像](https://blog.qux-jp.com/wp-content/uploads/2019/04/190420_keyboard_003.jpg)

## Licence
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。
