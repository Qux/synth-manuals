# Send-Return
外部のエフェクタに接続し、エフェクトをかける前 後の音を混ぜることができます。フィードバックし て何度もエフェクタに音を入れることができます。

## 回路図
![回路図](https://raw.githubusercontent.com/Qux/schematics/master/send_return/send_return.svg)

## 部品
| 記号|名前|数量|備考|
| :--- |:-----------:|-------:|-------:|
| R1   |10kΩ抵抗      |       1|[秋月電子](https://akizukidenshi.com/)|


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
