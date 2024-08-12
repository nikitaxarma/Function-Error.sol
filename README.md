# Auction Smart Contract
## Overview
This project contains a smart contract for an auction system implemented in Solidity. The contract allows users to participate in a decentralized auction on the Ethereum blockchain.
## Features
* **Create Auction:** Allows the owner to create a new auction with specific details such as item description, starting bid, and duration.
* **Place Bid:** Enables users to place bids on active auctions.
* **Withdraw Bid:** Allows users to withdraw their bids before the auction ends.
* **End Auction:** Lets the owner end the auction and transfer the highest bid to the seller.
## Error Handling:
1. **Invalid Bidder:** The placeBid function will revert with "Invalid bidder" if the bidder's address is invalid.
2. **Zero Amount:** The placeBid function will revert with an assertion error if the bid amount is zero.
3. **Non-Existent Item:** The getCurrentBid and cancelItem functions will revert with "Item does not exist" if there is no bid for the specified address.
4. **Auction Cancellation:** The cancelItem function will revert with "Auction item cancelled. All bids will be refunded." to indicate the item has been canceled.
