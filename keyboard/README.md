# Keyboard
電圧で制御する基板に CV 電圧を与える基板です。 8 つのボタンと出力電圧を設定するためのつまみ、 ポルタメント、CV/GATE 出力を搭載しています。

## 回路図
![回路図](https://blog.qux-jp.com/wp-content/uploads/2018/08/cropped-cropped-qux_logo_3_c-1.png)

## 部品
|記号|名前|数量|備考|
| :--- |:-----------:|-------:|-------:|
|P1|基板用マイクロUSBコネクタ（電源専用）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10398/)|
|P2|ピンソケットなど自由に|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|R1|10kΩ抵抗|1|[秋月電子](https://akizukidenshi.com/)|


## 仕様
各つまみで出力電圧を設定し、つまみの真下にあるスイッチ を押している間設定した電圧を CV OUT から出力します。
上段にあるつまみはポルタメントです。つまみを回すと、 CV OUT から出力される電圧が推移するのにかかる時間を 設定することができます。 右に回すほど推移時間が長くなります。
GATE 出力からは、どれか 1 つでもボタンを押している間 は 5V、1 つも押していないときは 0V を出力できます。 こちらはポルタメントの値に関わらず、瞬時に変化します。
複数の Keyboard を横に連結していくこともできます。 この場合連結した Keyboard のうち一番右の Keyboard のポルタメントが全体に適用されます。

## 調整方法
それぞれのボタンに対し、ボタンを押しながらつまみを回し てちょうど良い電圧になるようにつまみの位置を決めます。 ツマミの位置を決める際は . ポルタメントは 0(一番左)に しておくと良いでしょう。

## 繋げ方の例
1. VCO と繋げて音を出す
![繋げ方1](https://blog.qux-jp.com/wp-content/uploads/2019/04/image.png)
チューニングすれば 8 音階のモノフォニックシンセサイザー になります。ポルタメントを掛けると音程が下がりきるまで 音が鳴り続けます。

2. GATE出力をVCAに入れる
![繋げ方2](https://blog.qux-jp.com/wp-content/uploads/2019/04/image-2.png)
ボタンを押している間 VCA が 5V を受け取って音を出し、 離すと 0V を受けて音量が 0 になります。ポルタメントを 掛けるとアタックは音程が「ポオォ~ン」と上がって、ボタ ンを離した瞬間に音が途切れるようになります。


![画像](https://blog.qux-jp.com/wp-content/uploads/2019/04/190420_keyboard_003.jpg)

## Licence
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。
