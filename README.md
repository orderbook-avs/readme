# AI-Orderbook

AI-Orderbook is a user-first orderbook matchmaking service that utilizes an AI agent to help user make the most efficient trades. 

In TradFi, companies specializing in matchmaking services will typically pocket any profits made when someone initiates a limit order that is above asking price or below bidding price. See example below:

//insert 

Our orderbook places all profits into a ERC20 "Reward" token, that gets distributed to users everytime they trade on our platform. 

//insert image

Besides distributing profits to users, we also provide an AI agent that actively works to make sure you make the best trade on our orderbook. The agent will query all of the most recent orders, and determine what price levels the user should trade at.

## System overview

The user submits a trade order on the frontend NextJS web3 website () which stores the order in an on chain smart contract.

The matchmaking service runs on Tangle AVS operators, where operators watch for new orders and try to match them to existing ones. Batches of matched orders are sent to a smart contract to be finalized on chain. 

The AI agent, using the ElizaOS framework and hosted on Autonome, queries the smart contract for the most recent trades and outstanding orders, and helps the user make the best possible trades based on that information.

A Gaia node (run locally on our machine) is used to host the DeepSeekR1 model for the AI agent.

//insert image

## Repositories

[AI Agent with custom orderbook plugin](https://github.com/orderbook-avs/eliza-orderbook-plugin)
[Tangle AVS System and Orderbook Smart Contract](https://github.com/orderbook-avs/orderbook_tangle)
[Frontend Website](https://github.com/orderbook-avs/frontend)
