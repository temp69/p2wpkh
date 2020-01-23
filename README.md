# p2wpkh

This is a simple bitcoin paper wallet generator that utilizes Segregated Witness (SegWit) Pay To Witness Public Key Hash (P2WPKH) addresses and transactions. 
This repo uses those libraries:

*  BitcoinJS (5.1.7) : https://github.com/bitcoinjs/bitcoinjs-lib
*  html2pdf.js : https://github.com/eKoopmans/html2pdf.js
*  jQuery (3.1.4) : https://github.com/jquery/jquery
*  QR code generator : https://github.com/kazuhikoarase/qrcode-generator
*  secureRandom.js : https://github.com/pointbiz/bitaddress.org

## Information

### Features

 * Keypair generation utilizing BitcoinJS + secureRandom (bitaddress.org) for entrophy
 * View keypairs via QR codes
 * Print the generated QR codes
 
### External Support

 * Samourai Wallet can sweep funds from private keys and QR codes generated with segwitaddress.org 
 * Electrum can import private keys using the console and the `importprivkey()` command.
   Import as P2SH segwit:  
 	`importprivkey('p2wpkh-p2sh:L5eaxGKPZZMnanjxDzBd82VaxnHAE6MmBojiEFAVTM9mWZEhMMqG')`
   Import as native(bech32) segwit:  
 	`importprivkey('p2wpkh:L5eaxGKPZZMnanjxDzBd82VaxnHAE6MmBojiEFAVTM9mWZEhMMqG')`
  
### Contributing

 * Original forked from: https://github.com/coinables/segwitaddress
 * Please feel encouraged to contribute to this project. 
 * Anyone can create an issue if you find a bug or have a suggestion. 
 * If you are a developer feel free to submit a pull request or fork.
