# php_socket_client

> 这个包的功能和[workerman](http://www.workerman.net/gatewaydoc/advanced/push.html) 的功能没有任何修改，只是把改功能做成了一个包。方便实用composer的项目使用

## 使用

### 引入文件

``` 
require "vendor/autoload.php";

use skylee\gateway;

Gateway::$registerAddress = '127.0.0.1:1236';
```

### 例子

``` 
Gateway::sendToAll('{"type":"broadcast","content":"hello all"}');

Gateway::sendToClient($client_id,'{"type":"say","content":"hello"}');

Gateway::isOnline($client_id);
```





