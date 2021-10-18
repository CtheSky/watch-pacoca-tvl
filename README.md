# watch-pacoca-tvl
A simple script to expose pacoca defi tvl data through prometheus. It gets data by:
- coingecko api
- bsc smart contract

The implementation is not ideal, but works.

# Example Output
Only pacoca pools are included:
```
bnb_price 473.78
pacoca_price 0.365985
cake_price 19.54
lp_locked_cnt{pool="pacoca_bnb_cafe"} 59924.06556769297
lp_total_cnt{pool="pacoca_bnb_cafe"} 60950.78713951532
pacoca_cnt{pool="pacoca_bnb_cafe"} 2230785.4383161995
bnb_cnt{pool="pacoca_bnb_cafe"} 1727.0442957597438
tvl{pool="pacoca_bnb_cafe"} 1634673.0550872055
lp_locked_cnt{pool="pacoca_bnb_ape"} 96962.15967139257
lp_total_cnt{pool="pacoca_bnb_ape"} 97354.801102866
pacoca_cnt{pool="pacoca_bnb_ape"} 3635700.880989473
bnb_cnt{pool="pacoca_bnb_ape"} 2804.695080770691
tvl{pool="pacoca_bnb_ape"} 2659420.42229647
lp_locked_cnt{pool="pacoca_busd_ape"} 1669822.8209508895
lp_total_cnt{pool="pacoca_busd_ape"} 1678946.7110309459
pacoca_cnt{pool="pacoca_busd_ape"} 2874260.413460098
busd_cnt{pool="pacoca_busd_ape"} 1047255.1318727472
tvl{pool="pacoca_busd_ape"} 2099191.3292929414
lp_locked_cnt{pool="pacoca_cake"} 272272.8040645397
lp_total_cnt{pool="pacoca_cake"} 275575.5429467876
pacoca_cnt{pool="pacoca_cake"} 39122.67534903381
cake_cnt{pool="pacoca_cake"} 2086146.8904167346
tvl{pool="pacoca_cake"} 1527955.546009289
pacoca_cnt{pool="auto_pacoca"} 30401867.38885753
tvl{pool="auto_pacoca"} 11126627.436311023
pacoca_cnt{pool="manual_pacoca"} 38741821.69559628
tvl{pool="manual_pacoca"} 14178925.613262804
```
