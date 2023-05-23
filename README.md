### Hi there 👋
The token in the provided contract is called "OELON TOKEN" (symbol: OELON). Here are the details regarding its supply, tax, and tokenomics:

Supply:

Total supply: 500,000,000 OELON tokens (represented by the _tTotal variable).
Decimals: 9.
Tax and Tokenomics:

The token implements a buy and sell tax mechanism.
Initial Buy Tax: 6% (represented by the _initialBuyTax variable).
Initial Sell Tax: 7% (represented by the _initialSellTax variable).
Final Buy Tax: 0% (represented by the _finalBuyTax variable).
Final Sell Tax: 7% (represented by the _finalSellTax variable).
Reduce Buy Tax Threshold: 16 (represented by the _reduceBuyTaxAt variable).
Reduce Sell Tax Threshold: 37 (represented by the _reduceSellTaxAt variable).
Prevent Swap Before Threshold: 20 (represented by the _preventSwapBefore variable).
Max Transaction Amount: 0.1% of the total supply (represented by the _maxTxAmount variable).
Max Wallet Size: 0.1% of the total supply (represented by the _maxWalletSize variable).
Tax Swap Threshold: 0.02% of the total supply (represented by the _taxSwapThreshold variable).
Max Tax Swap: 0.02% of the total supply (represented by the _maxTaxSwap variable).
Other Features:

The contract implements the ERC-20 interface with standard functions such as totalSupply(), balanceOf(), transfer(), allowance(), approve(), and transferFrom().
The contract includes SafeMath library for arithmetic operations to prevent overflow and underflow.
The contract is Ownable, allowing the owner to manage ownership and certain functions through the onlyOwner modifier.
The contract includes functionality to create a Uniswap trading pair, add liquidity, and enable trading on Uniswap through the openTrading() function.
There is a delay mechanism (transferDelayEnabled) that limits transfers to one per block.
Bots can be added or removed from the bot list using the addBots() and delBots() functions.
The contract includes a manual swap function (manualSwap()) to convert token balance into ETH and send it to the tax wallet.
