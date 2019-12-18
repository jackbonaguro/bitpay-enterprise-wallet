# bitpay-enterprise-wallet

### Install

`npm i`

### Steps to create an XRP wallet

From the root directory:

1. Enter the scripts directory: `cd scripts`

2. Create an XRP wallet: `./wallet-create --name <name> --chain XRP --network mainnet --baseUrl <bitcore url>`
	* **This will output the wallet's mnemonic *to the terminal* on creation - save it securely in order to recover the wallet**
	* You can recover your wallet with: `./wallet-create --name <name> --chain XRP --network mainnet --baseUrl <bitcore url> --phrase <mnemonic>`
3. Derive one address for the wallet - this will be the XRP acceptance address: `./wallet-derive —-name <name> —-gap 1`
	* This will output the address - copy that and send it to John.
	* To see the last derived address, run: `./wallet-check —-name <name>`

### Other Commands
See [bitcore-client documentation](https://github.com/bitpay/bitcore/tree/master/packages/bitcore-client#commands)
