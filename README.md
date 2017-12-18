# Zenbot Helpers

These are unofficial helper scripts that may help in working with Zenbot.

## Backtesting CSVs
### Converting CSV row to Zenbot command

This browser-based script takes a pasted CSV row from the backtesting_xxxxxxx.csv files from Zenbot and converts them to ready-to-use parameters.

*Example Input*
```
"kraken.XXRP-ZEUR",0.46399714907997264,23.2,2.333,1,"crossover_vwap","taker",8551.59767761,6940.93556877,21,9,"9m",131,30,"module.exports = {""avg_slippage_pct"":0.045,""buy_stop_pct"":35,""emalen1"":17,""filename"":""none"",""markdown_buy_pct"":0.3288897092466354,""markup_sell_pct"":1.8085832043164172,""max_sell_loss_pct"":25,""max_slippage_pct"":5,""min_periods"":131,""order_type"":""taker"",""period"":""9m"",""profit_stop_enable_pct"":0,""profit_stop_pct"":11,""rsi_periods"":14,""selector"":""kraken.XXRP-ZEUR"",""sell_stop_pct"":50,""show_options"":true,""smalen1"":108,""smalen2"":60,""strategy"":""crossover_vwap"",""vwap_length"":81,""vwap_max"":787}"
````

*Example Output*
```
kraken.XXRP-ZEUR --avg_slippage_pct=0.045 --buy_stop_pct=35 --emalen1=17 --markdown_buy_pct=0.3288897092466354 --markup_sell_pct=1.8085832043164172 --max_sell_loss_pct=25 --max_slippage_pct=5 --min_periods=131 --order_type=taker --period=9m --profit_stop_enable_pct=0 --profit_stop_pct=11 --rsi_periods=14 --sell_stop_pct=50 --smalen1=108 --smalen2=60 --strategy=crossover_vwap --vwap_length=81 --vwap_max=787
````

Try it here: https://tiagosiebler.github.io/zenbot-helpers/csv_to_cmd.html

