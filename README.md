# AI-Orderbook

AI-Orderbook is a orderbook matchmaking service that utilizes an AI agent to help user make the most efficient trades. 

In TradFi, companies specializing in matchmaking services 

## System overview

The user submits a trade order on the frontend NextJS web3 website () which stores the order in an on chain smart contract.

The matchmaking service runs on Tangle AVS operators, where operators watch for new orders and try to match them to existing ones. Batches of matched orders are sent to a smart contract to be finalized on chain. 

The AI agent, using the ElizaOS framework and hosted on Autonome, queries the smart contract for the most recent trades and outstanding orders, and helps the user make the best possible trades based on that information.

A Gaia node (run locally on our machine) is used to host the DeepSeekR1 model for the AI agent.

