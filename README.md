##MISSION TAX

The idea is to get few data by scrapping API of blockchains for tax purposes.
Four things needs to be extracted from a block hash:
```block_id``` | ```txhash```	| ```timestamp``` |	```withdraw_commission```

Others column we gonna add:
```real_token_amount``` | ```price_usd```	| ```price_<your_currency>``` |	```total_price```

Basicaly, the ```real_token_amount``` is the decimals change from the ```withdraw_commission``` amount (for most blockchains it will be 6 decimals)
