cheerio-cli
===========
[![NPM Version][npm-image]][npm-url]

cheerio in command line

installation
-----------
    $ npm install cheerio-cli -g
    
Example 
-----------
  
  $ curl -s https://www.bonprix.com.tr/kategori/indirim-erkek-giyim/ | \
    cheerio each : .product-list-item,url : .product-link*href, \ 
    title: .product-title, brand: .product-brand, discount-price: .price-tag, \ 
    price: .former, image: .product-image noscript img*src | jq

  
 
[npm-image]: https://img.shields.io/npm/v/cheerio-cli.svg?style=flat
[npm-url]: https://npmjs.org/package/cheerio-cli
