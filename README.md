# Token requests for altrean

To request a new token to be added to altrean, please provide the following:

* Link to node.js library(s) for the token
* Provide code examples to sending, receiving, account generation, getting account balances, and getting transaction details for the token


## Example

### NXT
Library: https://github.com/toenu23/nxtjs

```
var nxtjs = require('nxtjs');

// Create an account
var acc = nxtjs.secretPhraseToAccountId('secret');
// Send NXT

// Receive NXT
Nothing special needed
// Get Account Balance
var bal = this.http.get(`${nodeUrl}/nxt?requestType=getBalance&account=${accountID}`);
// Get Transaction
var tx = this.http.get(`${nodeUrl}/nxt?requestType=getTransaction&id=${id}`)
```
