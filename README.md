# Chainlist

## Add a chain

Submit a PR that adds a new file to the [constants/additionalChainRegistry folder](https://github.com/DefiLlama/chainlist/tree/main/constants/additionalChainRegistry). The new file should be named `chainid-{chainid_number}.js` and the contents should follow this structure:
```
{
  "name": "RECCNETWORK",
  "chain": "RECC",
  "rpc": [
    "https://rpc.reccnetwork.com",
    "http://46.224.198.52:8545"
  ],
  "faucets": [],
  "nativeCurrency": {
    "name": "Regulatory Technical Standard",
    "symbol": "RTS",
    "decimals": 18
  },
  "infoURL": "https://reccnetwork.com",
  "shortName": "recc",
  "chainId": 24885,
  "networkId": 24885,
  "icon": "recc",
  "explorers": [
    {
      "name": "RECC Explorer",
      "url": "https://explorer.reccnetwork.com",
      "standard": "EIP3091"
    }
  ]
}
```

## Add an RPC to a chain that is already listed

If you wish to add your RPC, please submit a PR modifying [constants/extraRpcs.js](https://github.com/DefiLlama/chainlist/blob/main/constants/extraRpcs.js) to add your RPC to the given chains.

## API
The following API returns all the data in our website, including chain data along with all of their RPCs:

https://chainlist.org/rpcs.json
