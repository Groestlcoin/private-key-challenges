## Helper Tools for Private Key Challenges!

### Installation
Requires [NodeJS](https://nodejs.org/en/)

First review the code in this repository. Never install code you haven't audited! Then open your terminal and enter the following:
```
git clone https://github.com/groestlcoin/private-key-challenges.git
cd private-key-challenges
npm i
```

### Find typo:

The `brute-force-find-typo.js` script will brute force check every character and try replacing it with
all the other valid Base-58 characters. Once it finds a valid WIF-encoded private key, it prints
out the answer.

Usage:

```
node brute-force-find-typo.js 5Jhacv9gEyp7yosCeq1zgRRQSitGZZ3Z2NbgKG9BFXHW16iYU4z
```

Once you find the valid WIF private key, you can import it into a wallet like Electrum-GRS

### Resources:
- [Base58Check Encoding](https://en.bitcoin.it/wiki/Base58Check_encoding)
- [Wallet Import Format (WIF)](https://en.bitcoin.it/wiki/Wallet_import_format)
- [GroestlcoinJS-Lib](https://github.com/Groestlcoin/groestlcoinjs-lib)
