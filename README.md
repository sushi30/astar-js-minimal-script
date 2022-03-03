# astar-js-demo

1. clone
2. yarn
3. ts-node index.ts

## Expected error

```javascript
❯ ts-node index.ts
2022-03-03 11:58:20        API/INIT: RPC methods not decorated: eth_feeHistory
{ version: '336' }
2022-03-03 11:58:21        RPC-CORE: getStorage(key: StorageKey, at?: BlockHash): StorageData:: Unable to decode storage dappsStaking.contractEraStake:: createType(PalletDappsStakingEraStakingPoints):: decodeU8a: failed at 0xd38515e62f83f804861803773ae17af0… on stakers: BTreeMap<AccountId,Balance>:: Number can only safely store up to 53 bits
/home/imri/dev/astar-js-demo/node_modules/@polkadot/rpc-core/bundle.cjs:477
      throw new Error(`Unable to decode storage ${key.section || 'unknown'}.${key.method || 'unknown'}:${entryNum}: ${error.message}`);
            ^
Error: Unable to decode storage dappsStaking.contractEraStake:: createType(PalletDappsStakingEraStakingPoints):: decodeU8a: failed at 0xd38515e62f83f804861803773ae17af0… on stakers: BTreeMap<AccountId,Balance>:: Number can only safely store up to 53 bits
    at RpcCore._newType (/home/imri/dev/astar-js-demo/node_modules/@polkadot/rpc-core/bundle.cjs:477:13)
    at RpcCore._formatStorageData (/home/imri/dev/astar-js-demo/node_modules/@polkadot/rpc-core/bundle.cjs:422:17)
    at RpcCore._formatOutput (/home/imri/dev/astar-js-demo/node_modules/@polkadot/rpc-core/bundle.cjs:396:19)
    at RpcCore._formatResult (/home/imri/dev/astar-js-demo/node_modules/@polkadot/rpc-core/bundle.cjs:237:27)
    at callWithRegistry (/home/imri/dev/astar-js-demo/node_modules/@polkadot/rpc-core/bundle.cjs:261:19)
    at processTicksAndRejections (node:internal/process/task_queues:96:5
```
