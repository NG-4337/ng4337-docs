# Architecture

The BlueWave Wallet has three layers: front-end, back-end, and contract. The front-end layer serves as the user interface, with two main parts: the wallet and account recovery center. The wallet products include both a Chrome extension wallet and a mobile wallet.



&#x20;The back-end comprises two services: one that provides social media login and social recovery service, which also supplies social media login data storage, and the other is bundler, which is part of the ERC4337 protocol. \


The bundler verifies and packages user operations and sends them to the contract layer. The contact layer verifies and executes user operations and is also part of the ERC4337 protocol. The primary contracts include an entry point, contract wallet, and paymaster.

\


<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
