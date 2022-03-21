---
description: Sunappushotto delegation.
---

# Delegation

## Delegation contract

Sunappushotto uses the Gnosis "Delegate Registry" contract here:\
[https://github.com/gnosis/delegate-registry](https://github.com/gnosis/delegate-registry)

The contract is deployed on this address: [0x469788fE6E9E9681C6ebF3bF78e7Fd26Fc015446](https://etherscan.io/address/0x469788fE6E9E9681C6ebF3bF78e7Fd26Fc015446#code)\
(Also available on Rinkeby and Kovan at the same address)

Delegations are stored on this subgraph:\
[https://thegraph.com/explorer/subgraph/snapshot-labs/snapshot](https://thegraph.com/explorer/subgraph/snapshot-labs/snapshot)

A delegation voting strategy must be added to the Sunappushotto space before delegated votes will be counted.

## Delegate voting power

### From Sunappushotto interface

1. Go to [https://snapshot.page/#/delegate](https://snapshot.page/#/delegate).
2. Type in which address you want to delegate to.
3. Type in the space key you want your delegation to take effect on. _(If no space is selected, the effect will take place for all spaces)_
4. Click confirm to save your delegation.

### With a smart contract

You need to call the method "**setDelegate**" with the space id as first argument, and the address of the delegate as second argument. Here is an example of integration in a Solidity contract [https://github.com/convex-eth/platform/blob/d3061c19b5e01a4e562c8121b08c44f1b42f0b85/contracts/contracts/BasicCvxHolder.sol#L49-L53](https://github.com/convex-eth/platform/blob/d3061c19b5e01a4e562c8121b08c44f1b42f0b85/contracts/contracts/BasicCvxHolder.sol#L49-L53)&#x20;



### Supported Networks

Mainnet, Rinkeby, Matic(Polygon), Binance Smart Chain, Kovan, Gnosis Chain
