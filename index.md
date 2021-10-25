<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<title>Jono Meko idilės</title>
<meta name="viewport" content="width = 1050" />
</head>
<style>
#canvas {
	background: #f6f9ed;
}
.container {
	background-color: #fff;
	border: 1px solid #e4e4e4;
	width: 75%;
	margin-left: auto;
	margin-right: auto;
	margin-top: auto;
	margin-bottom: auto;
	padding: 15px;
}
.container p{
	text-shadow: 0 1px 0 #fff;
	padding: 0% 10%;
	font-family: 'Nunito', Verdana, Arial, Helvetica, sans-serif;
	text-align: center;
}
.container p:not(:nth-child(1)) {
	text-indent: 70px;
	text-align: left;
}
.container p.undertext {
	font-size: 10px;
	text-align: center;
	text-indent: 0px;
}
.container p.static {
	font-size: 12px;
}
.container p.smalltext {
	font-size: 14px;
}


.imgLOGO {
	display: block;
	width: 125px;
	opacity: .5;
	margin-left: auto;
	margin-right: auto;
	transition: 1s;
}
.imgLOGO:hover {
	transform: scale(1.25);
	opacity: .9;
}
</style>
<body id="canvas">

<div class="container">
	<p><b>Kviečiame klausytis Jono Meko <i>„Semeniškių idilių“</i></b></p>
	<p>Panašu, kad buvimas namuose bus pratęstas, o kad laikas neprailgtų, biblioteka siūlys jums nuo kovo 20 d. kasdien pasiklausyti po Jono Meko idilę iš audioknygos <i>„Semeniškių idilės“.</i></br>

	<p>Audioknyga išleista 2019 m. gruodį. Ji pristatyta Biržuose sausį J. Meko mirties metinių proga ir tarptautinėje Vilniaus knygų mugėje šių metų vasarį.</p>

	<p>Idiles J. Meko pageidavimu įskaitė biržietis Leonidas Čiudaras, garso takelį sukūrė Giedrius Žilinskas.</br>

	Audioknygą sudaro 26 idilės ir prologas. Ir visa tai - apie gimtuosius J. Meko Semeniškius, lietuvišką kaimą.</br>

	Kasdien čia, <i><a href='https://www.birzai.rvb.lt/'>bibliotekos tinklalapyje</a></i>, ir <i><a href='https://www.facebook.com/Bir%C5%BE%C5%B3-Vie%C5%A1oji-Biblioteka-1700931990118643/'>feisbuke</a></i> skelbsime po vieną idilę - ir nebūtinai eilės tvarka. Viena idilė kiekvieną dieną keis kitą, jas tam tikrai dienai parinksime pagal tos dienos realijas.</br>

	</p>
	<p class='undertext smalltext'><i>Visą audioknygą galima įsigyti mūsų bibliotekoje - tik teks palaukti karantino pabaigos.</i>
	</p>
	<p class='undertext static'>Iki kitos idilės liko:</p>
	<b><p id="CountdownTime" class='undertext static'></p></b>

<iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/788213323%3Fsecret_token%3Ds-lCDYvGCrQkt&color=%23a4bc8c&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true"></iframe>

	<p class="undertext"><i>Jono ir Adolfo Mekų palikimo studijų centras</br>

	Biržų r. savivaldybės Jurgio Bielinio viešoji biblioteka</i></p>
	
	<a href='https://www.birzai.rvb.lt/'><img class="imgLOGO" src="pics/LOGO.png"/></a>
</div>

<script>
// Set the date we're counting down to
var countDownDate = new Date("Apr 12, 2020 24:00:00").getTime();
var noncountdate = new Date("Apr 12, 2020 23:00:00");
var mani_link = "file:///C:/Users/Gr9Ag/Desktop/Idiles/index";

currentDate = new Date();
CurentTime = (currentDate.getMonth()+1).toString() + currentDate.getDate().toString();
TargetTime = (noncountdate.getMonth()+1).toString() + noncountdate.getDate().toString();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();

  // Find the distance between now and the count down date
  var distance = countDownDate - now;

  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);

  // Display the result in the element with id="demo"
  document.getElementById("CountdownTime").innerHTML = days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";

  // If the count down is finished, write some text
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("CountdownTime").innerHTML = "EXPIRED";
  }
}, 1000);
</script>

</body>
</html>