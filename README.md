# Movement-deploy

個人的な備忘録です。

Movementのテストネットがあり、興味があったのでdeployしてみました。

# １．Metamaskの設定
- 手動でネットワークを追加
    - Network Name: Move-EVM
    - Network RPC: https://mevm.devnet.m1.movementlabs.xyz/v1
    - Network ID: 0x0150
    - Network Currency: MOV
<br>
- ID：0x150　画像で確認すると0150ではない。0150でやるとエラーになる。

# ２．faucet
以下のリンクよりアクセス。<br>
    <https://faucet.movementlabs.xyz/?network=testnet>
<br>M1 faucetにMove-EVMのウォレットアドレスを入力し、faucetを押す。<br>
<br>1 MOV貰えます。

# 3.hardhatとFractalを使用してM1へのコントラクトをデプロイする
１．プロジェクトディレクトリの作成する<br>
```　mkdir hardhat-move-evm　```

```　cd hardhat-move-evm　```


２．hardhatのプロジェクトを作成<br>
 ```npx hardhat init ```

 今回は、JSを選択しました。

```
npm install --save-dev "hardhat@^2.19.0" "@nomicfoundation/hardhat-toolbox@^3.0.0"
```







