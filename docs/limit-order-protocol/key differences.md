
#  Key Differences Between Limit Orders and RFQ Orders

## I. Limit orders
- A financial instrument that allows users to put up an ERC-20 token for sale at a fixed price
- Offers flexible trade management tools, such as partial fill, predicates, single and bunch cancellation, fullness check, and validation
- Executed by placing orders via the 1inch dApp and fetching signed orders via the 1inch Limit Orders Liquidity Source API to perform trades on-chain
- Integrated into the DeFi ecosystem as a liquidity source by the Pathfinder algorithm
- Extremely flexible order type and can be configured with order execution predicates, helper functions for asset price evaluation, and callbacks for maker notification.

## II. RFQ orders
- This order type mirrors a traditional business process called "request for quotation" where a customer requests a quote from a supplier (market maker) for the purchase of some tokens
- Optimized for gas efficiency and suitable for market makers who create a number of RFQ orders and expose them via the API
- Traders or platform algorithms can request market maker quotes and receive signed RFQ orders if the quotes match their needs
- Have restricted capabilities, such as supporting an expiration time, cancellation by order ID, and being filled only once

Limit Orders and RFQ Orders support ERC20, ERC721 and ERC1155 tokens. Other token standards could be supported via external extension in the future.


**Learn more about Limit Order and RFQ Order executions [here](https://docs.1inch.io/docs/limit-order-protocol/introduction)**
-   You can use Limit Orders and RFQ Orders right in [1inch dApp](https://app.1inch.io/#/1/limit-order/WETH/DAI)
-   Smart Contracts [repository](https://github.com/1inch/limit-order-protocol/)
-   Utils library [repository](https://github.com/1inch/limit-order-protocol-utils/)
