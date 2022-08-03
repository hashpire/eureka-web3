---
version: "0.0.0"
published: true
---
uplinks::[multiformats](./multiformats.md)
tags:: #lang/en #type/term #note/develop 
# multiaddr
A standard which aims to make network addreses future-proof, composable, and efficient

## Specification
### Human-readable multiaddr
```text
(/<protoName string>/<value string>)+
```
Example
```text
/ip4/127.0.0.1/udp/1234
```
### Machine-readable multiaddr
```text
(<protoCode uvarint><value []byte>)+
```
Example
```text
0x4 0x7f 0x0 0x0 0x1 0x91 0x2 0x4 0xd2
```
## References
1. https://github.com/multiformats/multiaddr
