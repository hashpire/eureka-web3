---
version: "0.0.0"
published: true
---
uplinks:: [[Bitcoin Improvement Proposals (BIP)]]
# BIP32
- The most commonly used large-scale key management technology is the layered deterministic wallet technology proposed in the BIP32 standard.
-  In addition to solving the issue of backing up a large number of private keys, the reason why this technology is widely used is because of its audit functionality and its hierarchical tree structure that can be used to express organizational structures.
- However, one of its disadvantages is that the above two features cannot be used at the same time. This is mainly due to the fact that BIP32 wallets cannot tolerate private key leakage. 
- Moreover, BIP32 wallets do not improve the actual storage space used by the wallet and are vulnerable to a special random number generator attack.
## References

## See Also
1. [[BIP32 and Ed25519]]