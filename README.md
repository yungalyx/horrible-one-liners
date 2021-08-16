# horrible-one-liners
javascript but pythonic

```javascript
// creates a clean array with 'similar' duplicates removed,
// e.g, keeps 'sushiswap' but removes instances of 'sushiswap_v3' and 'sushiswap_b2'
const dexes = [...new Set(Object.keys(chartData[0]).map(x => x.split("_")[0]))].filter(x => {return (x !== "date")})


// displaying exchange rates between tokens without knowing what order the data comes in 
{(Number(item.decoded.params[3].value)/(Math.pow(10, 18))).toFixed(3) + " " + (item.decoded.params[1].value == '0x6b175474e89094c44da98b954eedeac495271d0f' ? 'DAI' : 'WETH') + " : " + (Number(item.decoded.params[4].value)/(Math.pow(10, 18))).toFixed(3) + " " + (item.decoded.params[2].value == '0x6b175474e89094c44da98b954eedeac495271d0f' ? 'DAI' : 'WETH') }
```
