# Social Recovery

The Social recovery process has the following steps:

\
1\. BlueWave Wallet sets up Guardians for the user's Contract Wallet and stores the Guardian information to the back-end for display during account recovery. The Guardian accounts are EOA that can belong to a friend and are used to sign recovery requests.

2\. Social recovery: Users can determine a list of EOAs (guardians) that can recover access to their wallet. This is extremely useful, giving the user the peace of mind of not having to worry about losing their keys. Guardians only need to sign the recovery signature to support the owner recovering his abstraction account by using the Security center, which is convenient and time-saving.

3\. The user needs to notify the owner of the Guardian account to log in to the recovery center webpage and use their Guardian account to sign in through the wallet (BlueWave Wallet, Metamask) to retrieve the recovery request from the back-end.

4\. Sign the request with the Guardian account and return it to the back-end.

5\. The user monitors the signature status of the recovery request using the BlueWave Wallet. If more than half of the Guardians have signed, the user can trigger the account recovery operation (UO), which is sent to the bundler.

6\. Similar to creating an account, the entry point contract verifies and executes the UO to complete the account recovery. At this point, the  Contract Wallet owner becomes the newly generated EOA account.

\


<figure><img src="https://lh3.googleusercontent.com/zgqTfKehSmaUd8Zrc_UqGmXvza_XvqXCwj3Sqi2equujDjGdH3SMBuAaklyk5h4zYrNIiW9_jovKrhY2UVIMYLedTBSL0FnGfdLKqp6R781TEivEpluAcuPiIcTKYAfNxQxcBJcvL309U9483JIcxuc" alt="4337NG Social Recovery Process Mechanism "><figcaption></figcaption></figure>

Furthermore, similar to other web3 wallets, the BlueWave wallet also supports features like token sending, token receiving, transaction records management, and contacts management. Among these, token sending is also implemented through the wallet contract, which follows a similar process to account creation and is done by sending a UO to the bundler.
