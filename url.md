# cara baca pautan

## apa yang kita faham tentang url
localhost merujuk kepada server dalam pc/laptop sendiri

kebiasaanya url akan ditulis seperti ini => localhost/index.php?query=param

jika kita guna .htaccess, url akan jadi seperti ini => localhost/query=param

kalau url kita ubah seperti ini => localhost/index.php?/class/method/param/param

guna .htaccess akan jadi seperti ini => localhost/class/method/param/param

ini lebih mudah untuk enjin carian index website kita dan beri user senang faham macam mana website kita berfungsi

## macam mana framework php baca url

dalam pembolehubah global $_SERVER ada beberapa benda yang berkaitan dengan url

* $_SERVER['PHP_SELF'] => index.php <= contoh nilai 
* $_SERVER['SCRIPT_NAME'] = index.php <= contoh nilai 
* $_SERVER['REQUEST_URI'] = index?/class/method/param/param  <= contoh nilai 
* $_SERVER['QUERY_STRING'] = /class/method/param/param  <= contoh nilai 
* $_SERVER['REQUEST_SCHEME'] => http atau https
* $_SERVER['SERVER_PORT'] => 80 atau 443

kebiasaanya kita akan guna 3 pembolehubah iaitu 
* REQUEST_URI
* PHP_SELF
* QUERY_STRING

kita jarang guna SCRIPT_NAME sebab panjang sangat berbanding dengan PHP_SELF

## jika guna parsel_url
```php
$svrReqSch = $_SERVER['REQUEST_SCHEME'];
$svrName = $_SERVER['SERVER_NAME'];
$svrReqUri = $_SERVER['REQUEST_URI'];
$p = $svrReqSch . '://' .  $svrName . $svrReqUri;
$paparURL = parse_url($p,-1);
echo '<pre>$svrReqUri = '; print_r($paparURL['query']); echo '</pre>';
/* contoh output 
$svrReqUri = /class/method/param/param
*/
```
kita cuba juga kononnya hack dengan guna url seperti => localhost/?"><script>alert(111);</script>

dalam REQUEST_URI tanpa filter, akan jadi seperti ini => 
```php
$svrReqUri = %3Cscript%3Ealert(111);%3C/script%3E
```

