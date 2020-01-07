# Javascript

### New Features in 2020

#### Dynamic Import
```javascript
async function loadLib(){
  const lib = await import('some lib');
}
```

#### Optional Chainning
```javascript
let item = data?.prop?.['something'] // no error when data is undefined
```

#### Nullish Coalescing
```javascript
...
const number = value ?? 400 // assign 400 to number if value is null or undefined
...
```

#### Big Int
```javascript
const largeNum = BigInt(some big number);
const superLarge = largeNumber ** 23n
```

# CSS

### Ticks

#### Fake Scrollspy: [Code](https://gist.run?id=d1a286b919e764342bda7dc391ea4a42)

# HTML

#### Lazy loading
```html
<img loading="lazy" />
```
