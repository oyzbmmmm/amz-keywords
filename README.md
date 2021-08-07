# Amazon Keyword Scraper
From 1 keyword you can scrape up to hundreds and even thousands **Unique and Relevant Keywords** with a **Number of Active Products** per each keyword.


## Features
*   Scrape Keywords with the number of active products from Amazon Store
*   Save result to a csv file or use as plugin in your app

## Module
```javascript
import { GrabKeywords } from './src';

const options = {
    keyword: "iphone",
    limit: 100,
};
let amazon = new GrabKeywords(options)._initScraper();

amazon.on('keywords', key => {
    console.log(key);
});

```
**Options**
```javascipt
let options = {
    // Keyword: {string default: ''}
    keyword: `iphone`,
    
    // Number of keywords to collect: {int default: 50}
    limit: 50,
    
    // Save result to a CSV file: {boolean default: false}
    save: false,

    // How many post should be downloaded asynchronously. Only if {download:true}: {int default: 5}
    asyncDownload: 5,
    
    // File path where all files will be saved: {string default: 'CURRENT_DIR'}
    filepath: `CURRENT_DIR`,
};
```


----
License
----

**MIT**

**Free Software**