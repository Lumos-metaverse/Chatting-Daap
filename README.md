
# Chatting DAPP on Avalanche chain

This is a chatting Daap similar to whatsapp, where you can chatt with your friends by adding their wallet id. All the chatts are stored on block chain which means your chatts are more secure.

![image](https://i.postimg.cc/bwBGxsj0/Screenshot-4.png)

![image](https://i.postimg.cc/prCrpdZF/Screenshot-5.png)


[_Chatting DAAP Hosted link_](https://jade-cupcake-c5c2fe.netlify.app/)
steps for using chatting dapp
- configure your metamask for fuji c test net
- click on connect to metamask button to connect your dapp with fuji c chain
- click on new chatt button then add your friends public wallet id (configured at fugi chain) and friends name
- now you can send message to your friends but each transaction will cost gas fees.

## How to execute Chatting DAPP locally  

clone this project locally

install dependencies for react 

 ```sh
npm install
```

configuration for adding fugi testnet inside metamask wallet
 ```sh
    Network Name: Avalanche FUJI C-Chain
    New RPC URL: https://api.avax-test.network/ext/bc/C/rpc
    ChainID: 43113
    Symbol: AVAX
    Explorer: https://testnet.snowtrace.io/
```
Since we are using block chain we need to pay tokens for sending every message because every activity on blockchain costs some token.Now we will bring some test tokens for avalanche network by using faucet, where we have to add our wallet address and request for avax coin.

 ```sh
https://faucet.avax.network/
```

Now start the react project which we have cloned locally
 ```sh
npm start
```
Now we can use this chatting dapp at http://localhost:3000/ 

connect your metamask wallet by pressing on connect to metamask button. we have already configured our wallet with fugi c chain so after pressing on, connect to metamask button, metamask will connect our daap with fuji c chain.

Now we need to add our friends name and public wallet address by pressing on add new chat button
(friends wallet need to be configured at fugi c chain).

for chatting with your friend we need to pay gas fees every time we send a message. When ever we send any message to any friend, our metamask will open with a transaction detail and ask for approval.

_you can find a .env file which consists deployed smart contract address. you can change it by deploying it by your self_