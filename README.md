## Universal Cashback Protocol

**What is the Universal Cashback Protocol?**

Universal Cashback Protocol was born as a decentralized solution for the cashback service using smart contracts, without intermediaries, using UCP (Universal Cashback Protocol) as token.
The initial proposal developed works as follows: 
Affiliate companies can generate rewards with UCP tokens for the purchase of products, by accumulating UCP for purchases, it allows the user to exchange UCP tokens for USDT and buy more products.

**How does the UCP works?**

1.	Companies that wish to benefit from our Protocol must affiliate.
2.	Affiliated companies can create products with a certain amount of UCP tokens as a reward.
3.	Rewards must be greater than 1 UCP.
4.	Only users who wish to pay through our Protocol will receive the rewards.
5.	Users will accumulate UCP tokens which they can exchange for USDT and continue to buy more products.

**Actual infrastructure:**
![](https://i.imgur.com/VbWAzIu.png)

**Technical data:**
Describe below we will show some relevant functions of our code:
Function that calculates the price per number of tokens that an affiliated company requires for a promotion:

![](https://i.imgur.com/kW7Prr5.png)

Returns the price of the token (USDT) that we use in the functions calculatePricePerToken and calculateQtyTokenClaim

![](https://i.imgur.com/NTYdve3.png)



**Technologies we use:**
**Polygon:**
Contracts in beta phase have been deployed on the Polygon Mumbai network. Since our Protocol for this test phase only accepts USDT as a means of payment, we have used the AAVE faucet to test the functionalities of the Protocol.

AAVE Faucet: https://staging.aave.com/#/faucet 


**Metamask:**
The wallet that we use to manage assets is Metamask. Polygon Mumbai testnet should have been added.


**Moralis:**

was used for the following:

•	As a provider to interact with the Polygon network.
•	Its functionalities were used to instantiate the web3 provider.
•	Interaction with contracts.
•	Login with Metamask to monitor the activity of the associated account through the Moralis dashboard.
•	Execution of Call and Send functions (something we found was that there were problems when executing send functions, so the same Moralis library has been used to instantiate web3, this bug will be reported to the Moralis team once the project is finished).


**Alchemy:**

was used as a node provider to forke the Ethereum mainnet, along with Hardhat testing Chainlink's price feeds and interacting with the Tether USDT contract. We also use it for the deployment of contracts in Mumbai.


**Chainlink:**
We use Chainlink to obtain from a secure and decentralized source the current price of the USDT token so that both users and companies affiliated with the Protocol make the payment and exchange of tokens for the corresponding value.

**Main goal:**

Create a decentralized option with the use of Smart Contracts and Blockchain technologies, to streamline the cashback service, allowing companies to trust their clients and receive crypto without adding extra payment gateways, if not direct to their preferred wallet, streamlining your transactions and promoting the use of cryptocurrencies.

**General objectives:**


•	Promote the inclusion of people without technical knowledge in the Crypto economy through granting Cashback benefits in a simple way.

•	Adopt Blockchain technology in everyday use cases.

•	Expose to the general population the benefits and options obtained from decentralization.

**How did we come up with the idea?**

WIN-WIN-WIN: All parties that interact in the process win: Companies, consumers and the Universal Cashback Protocol. Users will benefit by receiving UCP tokens as a reward for making purchases in affiliated companies and thus the Protocol will become more secure and robust in its infrastructure, companies do not need to pay intermediaries, fees or a percentage of their sales. They will simply buy funds with the UCP token, offer them to promote more sales of their products and get happier customers in the process, increasing adoption in everyday transactions of the economy with cryptocurrencies.


**What does this project contribute to the community?**

We believe that everyone wins: The idea is that more people can approach the ecosystem of Blockchain and cryptocurrencies in a more friendly way. And all people make purchases of different products on a daily basis.
Consumers: they will be happy to make a profit on their purchases.
Companies: we provide the tools for a simple cashback process avoiding bureaucracy and technical knowledge.
It may sound utopian, but we believe that with this project we are contributing to build freedom, and for us that is priceless.


**What was the biggest challenge we faced?**
In the beta base we have decided to only accept the Tether USDT token, this by definition has 6 decimal places. At the same time, the Chainlink price feed for USDT contains 8 decimal places and our UCP Token contains 18 decimal places. Therefore, to perform the calculations corresponding to the final value to be paid by UCP, the purchase of products and the claim of the Cashback, we had to work with the decimals so that the final result is correct.
The formula for converting decimals is as follows:
To convert a uint256 of 18 decimal places into the necessary quantity, (in our case 6) we use the following formula: In which the value of decimals is the final result of decimals to be obtained.
amount / (10 ** (18 - decimals))
Continuing with our case, that we need 6 decimals, if we use the formula, the value of "18 - 6" is "12", which means that those "12" will be subtracted from the 18 decimals, resulting in "6 ”.

**What did we learn? What are we proud of?**

We learned to manage all the ideas that we gathered at the beginning to achieve harmony in them and create a solution that represents the complex concept of Blockchain in a simple everyday application, which the world is used to doing through the traditional method or in a centralized way. We are proud to have built an open option to this opportunity, demonstrating that blockchain technology really came to stay and above all to benefit us as a society.


**What are the next steps?**

Grow our network of users by the recommendations of those who benefit from using it so that we can cover more areas that are related to the service we offer, preserving the culture of Universal Cashback Protocol that is decentralization, open source and synergies, UCP will continue in development to achieve this purpose, so attracting the attention of collaborators would be a next step to continue progress and develop a higher quality web application in the experience and interface of all users involved in the UCP ecosystem.
In the short term, with the information obtained by the use of early adopters, we will build a web app that will include a marketplace of the products that are available to be exchanged with the UCP token.

![](https://i.imgur.com/SlbeaNk.png)


**Future infrastructure:**

![](https://i.imgur.com/1YXFMwS.png) 

**Smart Contract preferences:**

![](https://i.imgur.com/Eyzfk1K.png)


**How dApp works:**

![](https://i.imgur.com/unBkoQb.png)

![](https://i.imgur.com/DCxdx2u.png)




**What would we do if we were winners?**

1.	Develop the Smart Contracts much better with respect to a more adapted operation to the cashback service.

2.	Promote its use by presenting our Minimum Viable Product (MVP) to those involved in the operation of the UCP.

3.	Build a web application with the data collected from the use of early adopters.

4.	With the reward that we would receive for being the winners, we would use it to finance the development of a dApp to make the use of our Protocol friendly to anyone.


![](https://i.imgur.com/I1v7dHk.png)

![](https://i.imgur.com/TdZ5FQV.png)

