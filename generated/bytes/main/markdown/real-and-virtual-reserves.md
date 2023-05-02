## Real and Virtual Reserves


## Introduction

In Uniswap V3, real and virtual reserves manage liquidity. Real reserves are actual token amounts in a pool, while virtual reserves represent active liquidity within a specific price range.


    


---
## Real Reserves

Real reserves are affected by liquidity providers (LPs) adding or removing liquidity, and they are used to calculate the exchange rate between the two tokens in a pool.


    


---
## Virtual Reserves

Virtual reserves determine the available liquidity for trading within a price range, helping to calculate the effective exchange rate and slippage for trades within that range.


    


---
## Example - Virtual Reserves

Example: A liquidity provider (LP) adds 10 ETH and 20,000 USDC within the price range of 1,800 USDC/ETH to 2,200 USDC/ETH. These amounts become the virtual reserves for trades within that range.


    


---
## Virtual Reserves in Action

When a user wants to swap tokens within the specified price range, virtual reserves are used to determine the exchange rate and potential slippage for their trade.


    


---
## Impact on Trades Outside the Range

Trades outside of the specified price range won't have access to the virtual reserves and may experience higher slippage or fail due to lack of liquidity.


    
   