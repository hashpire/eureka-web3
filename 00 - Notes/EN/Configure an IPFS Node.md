---
version: "0.0.0"
published: true
---
uplinks::[IPFS](./IPFS.md)
tags:: #lang/en #type/howto 
# Configure an IPFS Node
## Peer
- A peer address is represented in the[multiaddr](./multiaddr.md)format
	```text
	/ip4/49.0.49.123/tcp/4001/p2p/12D3KooWCZ5NPwfdc9zkcZ2ncHKmwuBht32zJfyit7ZrRx8Pzv2m
	```
- The peer address points to an IPFS node
## Bootstrap List
A list of ipfs nodes to connect to on launch
### Commands
```bash
ipfs bootstrap list # list all bootstrap nodes
ipfs bootstrap add [<peer>] # add peers to bootstrap list
ipfs bootstrap rm [<peer>] # remove peers from bootstrap list
ipfs bootstrap rm --all # remove all
ipfs bootstrap add --default # use default list
```
### Save and reload
```bash
ipfs bootstrap list > save1 # save to file
ipfs bootstrap rm --all
cat save2 | ipfs bootstrap add # reload
```



## Configuration File
### Swarm.AddrFilters
- An array of addresses (multiaddr netmasks) to not dial. 
- The configured IPPS node will not connect to these addresses.
- Use this to prevent certain peers from connecting

### Addresses.Swarm
- The configured node will listen on these addresses for p2p swarm connections
```json
[
  "/ip4/0.0.0.0/tcp/4001",
  "/ip6/::/tcp/4001",
  "/ip4/0.0.0.0/udp/4001/quic",
  "/ip6/::/udp/4001/quic"
]
```

### Addresses.Announce / Addresses.NoAnnounce
- Filter[#Addresses Swarm](./#Addresses Swarm.md)
- Peers will not see the unannounced swarm addresses, unless it is explicity added in the peer's bootstrap list
	- `ipfs swarm addrs`

## Profile
- Containts the default settings for an IPFS Node

---

To apply a profile
```bash
ipfs config profile apply <profile>
```

Available profiles
- `default-datastore`
	- flatfs
- `server`
	- Disables local host [Local Area Network (LAN)|LAN](./Local Area Network (LAN)|LAN.md) discovery — set `Swarm.AddrFilters`
	- Disable automatic[Network Address Translation (NAT)|NAT](./Network Address Translation (NAT)|NAT.md)port forwarding
	- Disable[MDNS](./MDNS.md)
	- Add LAN addresses to `Addresses.NoAnnounce`
- `local-discovery`
	- Allow discovery in local networks —  `Swarm.AddrFilters`
	- Enable automatic NAT port forwarding
	- Enable MDNS
	- Empty `Addresses.NoAnnounce`
- `randomports`
	- Use random port number for swarm
- `test`
- `default-networking`
	- Use default Bootstrap list
	- Inverse profile of the test profile
- `lowpower`
## References
1. https://docs.ipfs.io/how-to/configure-node/
