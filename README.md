# Token requests for altrean

To request a new token to be added to altrean, please provide the following:

* Link to node.js library(s) for the token
* Provide code examples to sending, account generation, getting account balances, getting account's transactions, and getting transaction details for the token
* Provide details of a node that will be hosted for the communication


## Example

### NXT
Library: https://github.com/toenu23/nxtjs

```
var nxtjs = require('nxtjs');

// Create an account
var acc = nxtjs.secretPhraseToAccountId('secret');
// Send NXT

// Get Account Transactions
var txs = this.http.get(`${nodeUrl}/nxt?requestType=getBlockchainTransactions&account=${accountID}`)
// Get Account Balance
var bal = this.http.get(`${nodeUrl}/nxt?requestType=getBalance&account=${accountID}`);
// Get Transaction
var tx = this.http.get(`${nodeUrl}/nxt?requestType=getTransaction&id=${id}`)
```
