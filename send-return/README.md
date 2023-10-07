# Send-Return
外部のエフェクタに接続し、エフェクトをかける前 後の音を混ぜることができます。フィードバックし て何度もエフェクタに音を入れることができます。

## 回路図
![回路図](https://raw.githubusercontent.com/Qux/schematics/master/send_return/send_return.svg)

## 部品
| 記号|名前|数量|備考|
|---|-----------|-------|-------|
|P1|基板用マイクロUSBコネクタ（電源専用）|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10398/)|
|P2|ピンソケットなど自由に|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|R1-5, 8, 11, 12, 15-17|抵抗10kΩ (茶黒橙金)|11|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|R6,7|抵抗100kΩ (茶黒黄金)|2|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|R9,10|抵抗4.7kΩ (茶黒黄金)|2|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|R13,14|抵抗47kΩ (茶黒橙金)|2|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|RV1,2|可変抵抗50kΩ (503)|2|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|C1,3-5|電解コンデンサ 3.3μF|4|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|C2|フィルムコンデンサ 0.1μF (104)|1|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|IC1-4|NJU7043(オペアンプ) ICソケット4x2|4|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|
|J1-4|オーディオジャック MJ-352-O|4|[秋月電子](https://akizukidenshi.com/catalog/g/gC-10097/)|


## 使い方
- 音源をINに入れます。`Send`をエフェクタの入力に入れ、 `Return`はエフェクタの出力を受けるように繋げます。
- IN に入ったそのままの音と、`Return`から入ってきた音の混ざり具合を`Dry/Wet`つまみで変えられます。
- `Feedback`つまみを回すと、`Return`から来た音を再びSendに送ることができます。右に大きく回すと、IN に音が入っていなくても Send-Return と外部のエフェクタだけで大きな音がなることがあります。

### 応用編
- Qux の Delay 基板と組み合わせ、Feedback つまみを回 すことでエコーがかかった音を出すことができます。  
__注意__  
Feedback つまみを右に大きく回すと大きな音が出 ることがあるのでご注意ください。

## Licence
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">クリエイティブ・コモンズ 表示 - 非営利 4.0 国際 ライセンス</a>の下に提供されています。
