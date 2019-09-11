# lisk-dex
Decentralized exchange module for the Lisk network.

## DEX protocol

These status codes and messages appear in transactions created by the DEX (as part of the transaction data field):

### Refunds:

- r1,${orderId}: Invalid order
- r2,${orderId}: Expired order
- r3,${orderId}: Canceled order
- r4,${orderId}: Unmatched market order part

### Trades:

- t1,${fromChain}: Matched some orders
- t2,${fromChain},${orderId}: Matched order

### Moved:

- m1,${walletAddress}: DEX has moved to a new address

### Stopped operating:

- d1: DEX has been disabled
