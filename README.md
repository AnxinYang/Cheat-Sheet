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
**Here's an example: https://gist.run?id=d1a286b919e764342bda7dc391ea4a42**

**index.html**

<!-- language: lang-html -->

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>GistRun</title>
      <link rel="stylesheet" href="styles.css">
    </head>
    <body>
    <div>
      <section id="one">Section One</section>
      <section id="two">Section Two</section>
      <section id="three">Section Three</section>
      <section id="four">Section Four</section>
      
      <nav>
        <a href="#one">One</a>
        <a href="#two">Two</a>
        <a href="#three">Three</a>
        <a href="#four">Four</a>
      </nav>
    </div>
    </body>
    </html>

**styles.css**

<!-- language: lang-css -->

    /* todo: add styles */
    *{
      scroll-behavior:smooth;
      font-family: Arial
    }
    nav{
      background: rgb(20,20,20);
      position:fixed;
      top:0;
      width:100%;
    }
    
    nav a{
      display:inline-block;
      padding: 8px;
      font-size:32px;
      text-decoration:none;
      color:  rgb(220,220,220);
      
    }
    section{
      height: 100vh;
      text-align:center;
      font-size: 64px;
      padding: calc(50vh - 32px) 0;
    }
    
    section:nth-child(odd){
      background-color:#eee;
    }
    nav a:hover,
    section#one:hover ~ nav a[href="#one"],
    section#two:hover ~ nav a[href="#two"],
    section#three:hover ~ nav a[href="#three"],
    section#four:hover ~ nav a[href="#four"]{
      font-weight:bold;
      background-color:white;
      color: rgb(20,20,20);
    }

# HTML

#### Lazy loading
```html
<img loading="lazy" />
```
