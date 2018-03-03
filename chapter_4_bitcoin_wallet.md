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
