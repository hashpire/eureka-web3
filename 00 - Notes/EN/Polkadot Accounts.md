---
version: "0.0.0"
published: true
---
uplinks::[Polkadot](./Polkadot.md)
tags:: #lang/en #type/term 
# Polkadot Accounts

- **Subkey and Polkadot-JS based wallets** use the[BIP39](./BIP39.md)dictionary for mnemonic generation, but **use the entropy byte array to generate the private key**, while **full BIP39 wallets (like Ledger) use 2048 rounds of PBKDF2 on the mnemonic**.The same mnemonic may generate different private keys on other wallets due to the various cryptographic algorithms used.



## References
1. https://wiki.polkadot.network/docs/learn-accounts
## See Also
