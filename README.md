BIP39 Mnemonics for bitcore-divi
=======

[![NPM Package](https://img.shields.io/npm/v/bitcore-mnemonic-divi.svg?style=flat-square)](https://www.npmjs.org/package/bitcore-mnemonic-divi)
[![Build Status](https://img.shields.io/travis/divicoin/bitcore-mnemonic-divi.svg?branch=master&style=flat-square)](https://travis-ci.org/divicoin/bitcore-mnemonic-divi)
[![Coverage Status](https://img.shields.io/coveralls/divicoin/bitcore-mnemonic-divi.svg?style=flat-square)](https://coveralls.io/r/divicoin/bitcore-mnemonic-divi)

A module for [bitcore-divi](https://github.com/divicoin/bitcore-divi) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install bitcore-mnemonic-divi
bower install bitcore-mnemonic-divi
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://bitcore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('bitcore-mnemonic-divi');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/divicoin/bitcore-divi/blob/master/CONTRIBUTING.md) on the main bitcore-divi repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/bitcore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
