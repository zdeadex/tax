*MISSION TAX*

The idea is to get few data by scrapping API of blockchains for tax purposes.
Four things needs to be extracted from a transaction hash:

```block_id``` | ```txhash```	| ```timestamp``` |	```withdraw_commission```

Other columns we'll be adding:

```real_token_amount``` | ```price_usd```	| ```price_<your_currency>``` |	```total_price```

The ```real_token_amount``` will be the ```withdraw_commission``` amount but with decimals adjustment (for most blockchains it will be 6 decimals)


*STEP 1: WHICH TRANSACTIONS I NEED?*

We need here to extract all transactions hash from the operator address with a ```cosmos-sdk/MsgWithdrawValidatorCommission``` function:

```#
```

*STEP 2: WHICH DATA I NEED?*

We need to extract the data in all the tranasction hash as mentioned earlier:

```#
``` 
