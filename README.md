# Bismillah. Our-Mood
## ini adalah percubaan framework berasaskan emosi aka perasaan.

dalam php, jika kita petik satu nama class, ada satu fungsi dalaman php akan cari nama class tersebut dan kita boleh set automatik include / require

dalam php, ada $_SERVER['QUERY_STRING']

biasanya orang buat output => /class/method/param1/param2/param3

boleh juga nak buat output -> :get:tablename atau |post:ablename atau @put:tableame atau #del:tablename

nak semak satu persatu nilai $_SERVER['QUERY_STRING'] kita boleh guna if-else atau switch.

tak pasti ada kaedah lain yang kita boleh tambah kemudian hari tanpa kembangkan lagi if-else atau switch

jadi apakah konsep asas framework berasaskan emosi aka perasaan?

emosi ini berlawanan dengan logik.

umpana jirim dan anti-jirim.

antara dilema memilih awek melayu atau amoi, tiba-tiba pilih awek mata biru laut atau tak memilih langsung.

tidak pilih langsung ada nilai default dalam php if-else atau switch

tiba-tiba pilih awek mata biru laut itu tak jumpa konsep dalam php 7

___
> Bersambung...

###### mood cari ilham buat framework baru daa

# Php Version

```php
//phpinfo();
//echo PHPVERSION() . '<br>';
echo PHP_VERSION . '<br>';
echo PHP_MAJOR_VERSION . '.' . PHP_MINOR_VERSION . '.' . PHP_RELEASE_VERSION . '<br>';
echo '<pre>'; print_r($_SERVER); echo '</pre>';
```

```javascript
<script type="text/javascript">
function confirmdelete(id)
{
	var messege="Are you sure to DELETE the record(id:"+id+")?";
	var r=confirm(message);
	if(r==true)
	{
		//redirect if user press yes
		window.location.href = "delete.php?x="+id;
	}
}
</script>
```
___
# Sumber ilham kawan-kawan
* Stylesheet
  * [Bootstrap](http://getbootstrap.com)
  * [Bootstrap.Themes](http://bootstrap.themes.guide)
  * [AdminLTE](https://adminlte.io/themes/AdminLTE)
  * [animate.css](https://daneden.github.io/animate.css)
  * [Sweet Alert](http://t4t5.github.io/sweetalert)
  * [FontAwesome](http://fortawesome.github.io/Font-Awesome)
  * [Enjoy Css](https://enjoycss.com)
* Javascript
  * [jQuery](http://jquery.com)
  * [jQuery.Form](http://malsup.com/jquery/form)
  * [backstretch](http://srobbin.com/jquery-plugins/backstretch)
* Gambar Percuma
  * [7-themes](http://7-themes.com)
  * [Pexels](https://pexels.com)
  * [Pixabay](https://pixabay.com)
  * [Unslpash](https://unsplash.com)
* Lain-lain
  * [markdown-cheatsheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)
  * [how-to-match-data-in-excel](https://www.wallstreetmojo.com/how-to-match-data-in-excel)
  * [mvc-structure-in-php](https://www.techfry.com/php-tutorial/mvc-structure-in-php)
