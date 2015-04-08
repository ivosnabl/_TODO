Hlavní
- přepočítání CEN eshopy !!!!   podle janoschik

- nutno skryt vypoctenou cenu v kosiku (problem s mnozstevni a klientskou cenou a s vypoctem - $_SESSION["cart_price"] se urcuje pri reccount z vychozi ceny / meny); 
- ověřit zda neni nutno potlačit načítání z cookie

reseni:
- na zacatku vsech indexu
- v BO v mene ve kt. bylo objednano (chybi ale celkove soucty z hlediska MO, tj. vc. DPH z ruznych zemi a dopravy)
- functions.php - Castka z demo

$config["curr_name"] = "&euro;";
//$config["curr_conv"] = 1/$config["global"]["eur_to_kc"];
$config["curr_conv"] = 1;
if (isset($_SESSION["auth_currency"]) && $_SESSION["auth_currency"] != "" && $_SESSION["auth_currency"] == "CZK") {
  $config["curr_name"] = "Kč";
  $config["curr_conv"] = $config["global"]["eur_to_kc"];
}




******************************************

TODO
mponline upgrade foundation + test implement offcanvas
mponline BO update
mponline - přidat z gigatel - slučování obj. ve FO, skupinové účty?  ochranu proti paral.prihl.

*******************************************

PNG ikonky pro akce a obarvené tr

*******************************************

<<<<<<< HEAD
=======
Obecný bug
modul Fullpage _check_link.php, projeví se při každém výskytu deadlink
- vymazat !!!! echo htmlspecialchars($file_contents);
>>>>>>> refs/remotes/origin/master

Obecný bug
modul Fullpage _check_link.php, projeví se při každém výskytu deadlink
- vymazat !!!! echo htmlspecialchars($file_contents);


*******************************************
oprava ckeditoru   do styleadm.css

.cke_source {
  white-space: pre-wrap !important; 
}


*******************************************

*******************************************
oprava ckeditoru   do styleadm.css

.cke_source {
  white-space: pre-wrap !important; 
}


*******************************************

centrum:
toptext-right   .. nesmyslny styl
form / parametr client_ dvojite uvozovky


Přidat podporu jazykově indiferentních bloků jako GA
a do indexu
<?php
if (!empty($block["GA"])) echo stripslashes($block["GA"]);
?>

učesat styly - seskupit styly pri eshop

projít functions.php pomocí parseru phpstormu !!!
 nejdriv skryt warnings
- správně $memoryLimit = $memoryLimitMB * $MB;
- init $return = "";
- nahradit $index


************************

pridat do functions:

do Mailwithmultiple…

  $mail->Body = $mail_text;

  if (IN_WIN === true and IS_PROD === false) {
    echo "<pre>$from|$to|$subj\n$mail_text</pre><hr />\n";
    return true;
  }


************************

vymazat z css
.box_projekty …
.box_events

… sladit s wysivyg

Vylepšit odesílání hesloraw  v local.php
$hesloraw = mb_substr($heslo, 0, 2) . str_repeat("*", mb_strlen($heslo)-4) . mb_substr($heslo, -2);


cat_sort nahradit názvem sort anebo rozsirit ajax post:
echo "<tr class=\"datarow {id: ".$xxxxxxid.", sort: '".urlencode($cat_sort)."'
