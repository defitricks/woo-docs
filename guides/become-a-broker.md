# Become a Broker

### What are WOOFi brokers?

WOOFi's bespoken sPMM algorithm provides deep liquidity and MEV proof trade execution on assets such as BTC, ETH, BNB, AVAX, FTM and predominant stablecoins on each blockchain. We aim to be the liquidity layer across DeFi, Web3 and GameFi spaces.

WOOFi has the lowest swap fee in the market with only 2.5bps on each transaction, in which 0.02% is used to buy back WOO tokens and reward WOO onchain stakers. WOOFi brokers are the applications or sites that route trades to WOOFi smart contracts. A whitelisted broker is eligible to receive 0.5bps of each trade that is sent to WOOFi via the broker's application as rebates in the form of quote tokens i.e. stablecoins.&#x20;

### How to enroll as a broker to receive rebates?

Any application such as DEX aggregators, wallets, web3 apps or websites that integrate WOOFi's sPMM liquidity can enroll as a broker to receive rebates. Fill out the enrollment form below and we will get in touch with you shortly.&#x20;

:point\_right: [**Enrollment Form**](https://docs.google.com/forms/d/e/1FAIpQLSdTTfytZmcKLwGTl6MUxGiaou1gAXhd83roAGgNCiIkBeYtFQ/viewform?usp=sf\_link)****

Once the enrollment information is reviewed, our team will get in contact with you and the provided broker rebate address will be added to the whitelist in `WooRebateManager.sol` on corresponding blockchains.

In order to receive rebates, the broker needs to integrate WOOFi as a liquidity source following [integration docs](integrate-woofi-as-liquidity-source.md).  For a trade to be eligible for rebates, the whitelisted rebate address must be included in the field `address rebateTo` in the transaction that is sent to WOOFi smart contracts.&#x20;

### How to check and claim the rebates?

The rebate is processed on a daily basis via smart contracts, the broker can check the eligible rebates and claim anytime you want on the chain that WOOFi liquidity is integrated.

| Network   | Smart Contract Address                                                                                                                |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| BNB Chain | [0x0208D735576B3D974024237393F4617285bf0563](https://bscscan.com/address/0x0208d735576b3d974024237393f4617285bf0563#readContract)     |
| Avalanche | [0xbF401edBb0265D037BfC89DfFeB7dbDa10b57C22](https://snowtrace.io/address/0xbf401edbb0265d037bfc89dffeb7dbda10b57c22#readContract)    |
| Fantom    | [0x0D37e768c3eD8a3FA494d03AF69605C5bE9a68e4](https://ftmscan.com/address/0x0d37e768c3ed8a3fa494d03af69605c5be9a68e4#readContract)     |
| Polygon   | [0x3d605fA64595Dba86f7780E128816ADAAeCA8A2b](https://polygonscan.com/address/0x3d605fa64595dba86f7780e128816adaaeca8a2b#code)         |
| Arbitrum  | [0x505ac728645d2ef84380961F72bAea500b3efa3f](https://arbiscan.io/address/0x505ac728645d2ef84380961f72baea500b3efa3f#code)             |
| Optimism  | [0x36b680fB76Dad86bcB2Cefc83fAE05e3Fe147706](https://optimistic.etherscan.io/address/0x36b680fb76dad86bcb2cefc83fae05e3fe147706#code) |

#### Check eligible rebates

* Step 1 - go to the `WooRebateManager` smart contract address using the corresponding blockchain explorer (click the link above)
* Step 2 - click 'Read Contract' under the "Contract" tab

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

* Step 3 - go to the 'pendingRebate' function, input your whitelisted rebate address and click 'Query', and you will see the current amount of claimable rebates in the quote token. i.e. stablecoins

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

#### Claim rebates

* Step 1  - visit the `WooRebateManager` smart contract address via the blockchain explorer and click the 'Write Contract' under the 'Contract' tab.

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

* Step 2 - click 'Connect to web3' and sign in with your whitelisted rebate address.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

* Step 3 - Claim your pending rebate by clicking the 'Write' button under the 'claimRebate' function, sign the transaction in your wallet to receive the rebates.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>



{% hint style="info" %}
With respect to the rebates provided to WOOFi brokers, WOO Network reserves the right to modify, suspend or discontinue any and all of the rules in the program at any time without the consensus of WOOFi brokers.
{% endhint %}