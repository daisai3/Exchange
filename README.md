# Exchange

Flama Exchange  is a modified Uniswap fork. Trading and flash loans have a 0.35% fee.

Flama Exchange rewards:
- 0.25% of trading fees to Liquidity Providers.
- 0.1% to Flama Staking Shares (FSS) holders. 

A protocol-wide charge of 0.1% per trade will take effect. This represents 2/7th (28.57%) of the 0.35% fee. Rather than calculating this charge on swaps, which would significantly increase gas costs for all users, the charge is instead calculated when liquidity is added or removed.

The feeTo recipient of the 0.1% charge is a smartcontract (FlappFeeConverter).

“FlappFeeConverter” converts FL (Flama Liquidity Tokens) to FLAPP (FLAP) through the Flama-Exchange and decentralized exchanges and protocols and distributes these FLAPP to the Flama Staking Shares (FSS) smartcontract through another smartcontract called “FlappFeeDistributor”.

**Code:**
- https://github.com/FlamaToken/Exchange
