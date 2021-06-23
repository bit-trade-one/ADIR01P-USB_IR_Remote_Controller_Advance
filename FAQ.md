# よくある質問

## USB接続の製品の場合には、下記の点についてお確かめください。

 - 使用しているケーブルがデータ通信可能であるか。
   - 電力供給のみのケーブルであることが多々ございます
 - ブートスイッチ等、ファームウェア書き込みモードになっていないか。
   - 説明書にブートスイッチについての記載がある製品が対象です
 - USBポートから十分な電力が供給されているか。
   - 念の為、PC本体のマザーボード側USBコネクタでお確かめください
 - 同時に接続している機器が干渉していないか。
   - できる限り最小構成での試行をお願い致します

## Q: 赤外線受信をフラグに自作アプリを動かしたいが赤外線信号を取りこぼしてしまう。

### A: 弊社公開の受信設定アプリの利用をご検討ください。  

公開されている赤外線取得用関数を使用し  
赤外線受信→一定時間待機→受信終了→受信内容読み出し のループをタイマ関数で  
一定間隔おきに呼び出すような処理は、決まった信号を取りこぼさず受信しアクションを起こすことに不向きです。  
決まった信号を受信したことをフラグに、自作アプリケーションを動かしたい場合  
弊社が公開している受信設定アプリを使用し、特定の赤外線信号を受信した際キーボード入力等を行うように設定し  
そのキーボード入力をフラグとして自作アプリケーションを動かすと赤外線受信信号を取りこぼしません。


## Q: 赤外線リモコンキットと比較したアドバンスの強みはなんですか

### A: 赤外線の送信強度やコード記憶方式の変更に伴うより多くの機器への対応、ファイルからのコード送信機能などが主な強化ポイントです。

----

## Q: 最長3秒の送信とはどういうものですか

### A: リモコンコードは機器によって長さなどが異なります。赤外線リモコンアドバンスは3秒までのコード長に対応します。

----

## Q: 赤外線リモコンアドバンスを納める外装などはありますか

### A: ホビー向け製品ということもあり、これといった指定はございません。基板むき出しのままでもご使用いただけますし、簡単な加工として清涼菓子フリスクのケースをそのまま流用して頂く等も可能です。

----

## Q: このボードは，パソコン側のソフトからコントロールできるものでしょうか

### A: [こちら](https://github.com/bit-trade-one/USB-IRRemocon-ADVANCE/tree/master/Library)で、USB赤外線リモコンアドバンスをPCから制御するためのC#用のライブラリ、並びに取り扱い説明書を公開しております。

----

## Q: コマンドライン経由での発信には対応していますか

### A: 対応しておりません。別途ライブラリの特注が必要です。


----
