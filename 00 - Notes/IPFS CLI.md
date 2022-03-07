---
version: "0.0.0"
published: true
---
uplinks:: [[IPFS]]
tags:: #lang/en #type/cli
# IPFS CLI
## Start
```bash
ipfs daemon
```

## Peers
```bash
ipfs swarm peers # list all connected peers
ipfs swarm addrs # list known addresses
```

## Networking

```bash
ipfs stats bw # show bandwidth usage
```

## Storage

### Show pinned files
```bash
ipfs pin ls [<ipfs-path>] # List objects pinned to local storage.
ipfs pin ls # list all pinned files
```
Indirect pins are those that are pinned as a result of being child blocks of recursive pins.

### Show all stored files
```bash
ipfs refs local
```

### Perform Garbage Collection
Remove files that have not been pinned
```bash
ipfs repo gc              
```


