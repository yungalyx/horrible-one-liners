# horrible-one-liners
javascript but pythonic

```javascript
// creates a clean array with 'similar' duplicates removed,
// e.g, keeps 'sushiswap' but removes instances of 'sushiswap_v3' and 'sushiswap_b2'
const dexes = [...new Set(Object.keys(chartData[0]).map(x => x.split("_")[0]))].filter(x => {return (x !== "date")})
```
