# 第4章: ビットコイン・ウォレット
ビットコインウォレットの主な機能
1. その人の暗号鍵の生成やバックアップやアドレス管理
1. 送金のためのトランザクションの生成
1. ブロックチェーン内にある自分に関連したトランザクション履歴
1. 自分が所持しているUTXOを簡単に把握できるようにすること

## ウォレットの初期化
### 新しいアドレスの生成
bitcoin-cli getnewaddress コマンドで新規生成できる

### アドレスにアカウントを設定できる
- アカウントの設定は必須ではない
- アカウントの設定
    - bitcoin-cli setaccount xxxxxxxxxxxxxxxxxxxxxxxxxxxx
- アカウントごとの所持金残高
    - bitcoin-cli listaccounts

### ウォレットの秘密鍵の暗号化
- bitcoin-cli encryptwallet <パスワード>

## ウォレット残高を確認する
- bitcoin-cli getbalance

### 自分宛のUTXOを確認する
- bitcoin-cli listunspent

### ビットコインを送金する
#### 取引手数料の規定値の設定
- 送金を実用的な時間で行うには手数料が必要
- BitcoinCoreでは1Kbあたりの取引手数料の規定値を設定できる
    - これを設定すると毎回送金ごとに取引手数料を設定する必要がなくなる
    - bitcoin-cli settxfee 0.00001
- bitcoin-cli sendfrom <送信アカウント名> <送信先ビットコインアドレス> <送金金額> で送信

## ビットコイン・ウォレットによる暗号鍵管理
### ウォレットのセキュリティレベルは「財布」と同じではない



































