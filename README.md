# Chai Things
Chai Things adds support to [Chai](http://chaijs.com/) for assertions on array elements.

## Example
```javascript
// Although they are equal, two different { a: 1 } objects are not the same
[{ a: 1 }, { b: 2 }].should.not.include({ a: 1 })
// However, Chai Things allows us to test what we want
[{ a: 1 }, { b: 2 }].should.include.something.that.deep.equals({ b: 2 })
```

## Installation and usage
```bash
$ npm install chai-things
```

```javascript
var chai = require("chai");
chai.should();
chai.use(require('chai-things'));
```
