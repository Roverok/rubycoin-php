rubycoin-php
============

Create a service, website, or app that uses Rubycoin.

```
require('Rubycoin.php');

$rubycoin = new RubycoinClient("http", "rubycoinrpc", "password", "localhost");
$can_connect = $rubycoin->can_connect();

if($can_connect>0) {
      $difficulty = $rubycoin->getdifficulty();
      $rubycoin_address = $rubycoin->getnewaddress();
      $unconfirmed_balance = $rubycoin->getbalance($rubycoin_address, 0);
      $confirmed_balance = $rubycoin->getbalance($rubycoin_address, 3);
}
```
