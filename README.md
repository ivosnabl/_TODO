
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

modul Centra / kernel
is_tel2_obj  schazi v INSERT ?  

************************

pridat do functions:

do Mailwithmultiple…

  $mail->Body = $mail_text;

  if (IN_WIN === true and IS_PROD === false) {
    echo "<pre>$from|$to|$subj\n$mail_text</pre><hr />\n";
    return true;
  }

Hlavní
- přepočítání CEN eshopy !!!!   jak to má aalto, kontrola janoschik

TODO
mponline upgrade foundation + test implement offcanvas
mponline BO update



************************

vymazat z css
.box_projekty …
. box_events

… sladit s wysivyg

From: Ivo Snabl [mailto:snabl@iba.muni.cz]
Sent: Monday, March 23, 2015 4:48 PM
To: 'Ivo Snabl'
Subject: RE: bug bo

Vylepšit odesílání hesloraw  v local.php
$hesloraw = mb_substr($heslo, 0, 2) . str_repeat("*", mb_strlen($heslo)-4) . mb_substr($heslo, -2);


From: Ivo Snabl [mailto:snabl@iba.muni.cz]
Sent: Friday, March 20, 2015 4:30 PM
To: 'Ivo Snabl'
Subject: bug bo

cat_sort nahradit názvem sort anebo rozsirit ajax post:
echo "<tr class=\"datarow {id: ".$xxxxxxid.", sort: '".urlencode($cat_sort)."'


TODO
PNG ikonky pro akce a obarvené tr
