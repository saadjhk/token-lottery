# Token Lottery Program on Solana

A simple token lottery system that crowdfunds lottery prizes.


## Requirements
- User should be able to buy lotteries
- The amount collect by users purchased tickets should be collected in a prize vault
- Specify an EPOCH for distributing rewards
- For each reward cycle there should be 3 prizes
- Future: We should be able to have multiple reward cycles. 
- NFT should not be valid after the distribution of rewards has started (perhaps have some sort of validation checks or have those NFTs be valid for entire lifespan)
- Smart contract should be able to determine first three winners
- Rewards should be transferred to first three winners
- Any amount remaining shall be rolled over for the next round of lottery winners
- Fees from the sale of NFT can be deducted but should be configurable


## Architecture

I want to keep this straight forward and as simple as possible for now. Will add more functionality as i achieve simple stuff first

- Lottery Tickets can be represented as NFTs
- Each NFT should be sold for specified amount of SPL Tokens