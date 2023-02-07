# cara baca pautan

## apa yang kita faham tentang url
kebiasaanya url akan ditulis seperti ini => http:80//localhost/index.php?query=param#cangkuk

jika kita guna .htaccess, url akan jadi seperti ini => http://localhost/query=param#cangkuk

kalau url kita ubah seperti ini => http:80//localhost/index.php?/class/method/param/param

guna .htaccess akan jadi seperti ini => http://localhost/class/method/param/param

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
