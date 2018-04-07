<img src="http://reddcore.io/css/images/module-mnemonic.png" alt="reddcore mnemonics" height="35">
BIP39 Mnemonics for reddcore
=======

[![NPM Package](https://img.shields.io/npm/v/reddcore-mnemonic.svg?style=flat-square)](https://www.npmjs.org/package/reddcore-mnemonic)
[![Build Status](https://img.shields.io/travis/reddcoin-project/reddcore-mnemonic.svg?branch=master&style=flat-square)](https://travis-ci.org/reddcoin-project/reddcore-mnemonic)
[![Coverage Status](https://img.shields.io/coveralls/reddcoin-project/reddcore-mnemonic.svg?style=flat-square)](https://coveralls.io/r/reddcoin-project/reddcore-mnemonic)

A module for [reddcore-lib](https://github.com/reddcoin-peoject/reddcore-lib) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install reddcore-mnemonic
bower install reddcore-mnemonic
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://reddcore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('reddcore-mnemonic');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/reddcoin-project/reddcore-lib/blob/master/CONTRIBUTING.md) on the main reddcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/reddcoin-project/reddcore-lib/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
