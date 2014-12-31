rubycoin-php
============

PHP library for developing Rubycoin applications.

```
require('Rubycoin.php');

$rubycoin = new RubycoinClient("http", "rubycoinrpc", "password", "localhost");
$can_connect = $rubycoin->can_connect();

if($can_connect>0) {
      $difficulty = $rubycoin->getdifficulty();
      $rubycoin_address = $rubycoin->getnewaddress();
}
```
