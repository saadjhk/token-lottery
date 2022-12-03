# Token Lottery Program on Solana

A simple token lottery system that crowdfunds lottery prizes.


## Requirements
- User should be able to buy lotteries as NFTs
- The amount collect by users purchased tickets should be collected by lottery contract
- Every fixed EPOCH winners will be choosen if any
- For each reward cycle there should be 3 prizes
- Rewards should be transferred to first three winners, any amount remaining shall be rolled over for the next round of lottery winners
- Fees from the sale of NFT can be deducted but should be configurable, transfer of NFTs should also deduct some fees (check if possible)

## Architecture

I want to keep this straight forward and as simple as possible for now. Will add more functionality as i achieve simple stuff first

- Lottery Tickets can be represented as NFTs
- Each NFT should be sold for specified amount of SPL Tokens
- Token Lottery Contract -> Select random NFT as the winner -> if owner Some -> Distribute else Rollover funds
- Collect NFT Sale in Lottery PDA