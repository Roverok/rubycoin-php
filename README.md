rubycoin-php
============

RPC bindings to create a service, website, or app that uses Rubycoin.

```
require('Rubycoin.php');

$rubycoin = new RubycoinClient("http", "rubycoinrpc", "password", "localhost");
$can_connect = $rubycoin->can_connect();

if($can_connect>0) {
      $difficulty = $rubycoin->getdifficulty();
      $rubycoin_address = $rubycoin->getnewaddress();
}
```
