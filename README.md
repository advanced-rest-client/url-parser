[![Build Status](https://travis-ci.com/advanced-rest-client/url-parser.svg)](https://travis-ci.com/advanced-rest-client/url-parser)

A URL parsing library for Advanced REST Client.

It provides an interface similar to the URL class but it is more relax in terms of input validitiy. It means that it won't throw an error when the URL is invalid. This allows to use the library in request editors.

## Usage

### Installation
```
npm install --save @advanced-rest-client/url-parser
```

## Example

```javascript
import { UrlParser } from '@advanced-rest-client/url-parser';
const parser = new UrlParser('https:///path-with-missing-host?qury=value#string');
console.log(parser.protocol);
console.log(parser.host);
console.log(parser.path);
console.log(parser.searchParams);
console.log(parser.anchor);
```

## Development

```sh
git clone https://github.com/advanced-rest-client/url-parser
cd url-parser
npm install
```

### Running the tests
```sh
npm test
```
