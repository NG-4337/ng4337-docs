# Social Media Login

Social media login allows users to log in to their wallets using existing email or social media accounts such as Facebook and Twitter. The process includes the following steps:

\
1\. User sends a login request to the back-end through the wallet.

2\. The back-end uses SDKs for social media login to communicate with relevant external services to enable login.

3\. The social media account information is saved on the back-end, and the login result is returned to the wallet to complete the login process.

4\. After a successful login, the wallet creates an EOA (Externally Owned Account) locally as a signing account. This process is transparent to the user, and the user does not need to record any EOA-related information, such as a private key or seed words.

5\. The wallet then constructs a User Operation (UO) to create a contract account (CA) using the EOA signature and sends it to the bundler.

6\. The bundler saves the UO to the mempool and, when it satisfies certain requirements, calls the entry point contract to verify and execute the UO and create a CA.



Additionally, 4337 I NG wallet also supports ERC20 payment of transaction fees completed through the paymaster contract.

\
