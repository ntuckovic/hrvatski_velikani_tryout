hrvatski_velikani_tryout
========================

Are you a frontend dev?

<h3>Zadatak</h3>

0. Instaliraj git, napravi github account ako nemaš i javi se vlasniku ovog repozitorija.<br>
HELP:<br>
http://git-scm.com/downloads <br>
https://help.github.com/articles/set-up-git/

1. Kloniraj ovaj repozitorij kod sebe lokalno i napravi inicijalni commit i push<br>
HELP:<br>
<b>git pull origin master</b><br>
<b>git commit -a -m 'initial commit'</b><br>
<b>git push origin master</b>

2. Skini neki frontend framework, postavi iskoristivu <b>index.html</b> stranicu. Postavi za title <b>Hrvatski Velikani</b> i za prvi h1 title na vrhu stranice isti naslov.<br>
HELP:<br>
http://getbootstrap.com<br>
http://foundation.zurb.com

3. napravi dva ajax poziva na json datoteke u folderu <b>src</b>, te dobiveno(<i>data</i>) na <b>success</b> ili <b>done</b> funkciju prvo ispiši u konzolu browsera.<br>
HELP:<br>
http://api.jquery.com/jquery.ajax/ ili http://www.w3schools.com/jquery/ajax_getjson.asp <br>
http://stackoverflow.com/questions/4539253/what-is-console-log

4. Učitaj ispravno c3.js library na stranici, te za prvi ajax poziv "velikani_chart.json" u <b>success</b> ili <b>done</b> funkciji loadaj c3 graf sa dobivenom <i>data</i> iz ajax poziva, postavi da se graf iscrta kao <b>Bar chart</b>.<br>
HELP:<br>
<b>c3.js</b> ovisi o <b>d3.js</b> libraryu, ne zaboraviti učitati <b>d3.js</b> prije kako je opisano: http://c3js.org/gettingstarted.html<br>
Bar chart primjer: http://c3js.org/samples/axes_x_tick_rotate.html

5. Učitaj ispravno neki dostupan js slider plugin element na stranicu, te za drugi "velikani_gallery.json" u <b>success</b> ili <b>done</b> funkciji ajax poziva u slider <b>append</b>-aj ili na drugi način ubaci iteme iz loadanog json filea na način da u svakom slideu prikažeš sliku, ime osobe i organizaciju kojoj pripada. Sva tri itema su u json fileu navedeni za svaki objekt, pa dok se to učita ko npr. <i>data</i> u <b>success</b> ili <b>done</b> funkciju mogu biti dostupni na način:<br>
	```javascript
		$(data).each(function(i,obj){
			var ime = obj.full_name;
			var slika = obj.img;
			var organizacija = obj.organization;

			// ovo dolje je već appendanje
			$("#slider").append("<div class='item'>"+ <img src='img/"+ slika + "' />" + "<div>" + ime + "</div>" + "<div>" + organizacija + "</div>" + "</div>" );

		});
	```
	<br>
Hint: vidi navedeni json file i njegovu strukturu<br>
HELP:<br>
http://owlgraphic.com/owlcarousel/demos/json.html<br>
http://getbootstrap.com/javascript/#carousel

6. Inicijalizirati Git repozitorij na svom accountu i dignuti cijeli projekt gore. Link šibnut vlasniku ovog repozitorija.<br>
HELP:<br>
http://stackoverflow.com/a/5437611


Dodatne preporuke:<br>

1. Koristiti neki "quick-setup" dev server, tipa wamp, xamp, http-server:<br>
https://github.com/nodeapps/http-server<br>
http://www.wampserver.com/en/

2. Sve što nije jasno može se potražiti i saznati na: http://www.google.com

3. Sve što se nezna vezano za web development može se pitati, dobiti odogovor i naučiti na: http://stackoverflow.com (topla preporuka za registraciju) <br>
