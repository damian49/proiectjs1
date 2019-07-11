# proiectjs1
# ==========


A project designed to learn some basic HTML, CSS and JavaScript concepts.

# Crearea proiectului 
Se crează pe discul *D:* un director denumit *proiect1*. În acest director se crează subdirectoarele *css* și *js*.
Rezultat:
![Img. 1](/images/poza1.jpg)

# Instalări 
## a.	SublimeText
Accesați: [site-ul aplicației](https://www.sublimetext.com/) 

## b.	Browsersync
*Browsersync* este o aplicație care permite instituirea supravegherii unui număr de fișiere dintr-un director.  Ori de câte ori unul dintre fișierele supravegheate se modifică, *Browsersync* va reîncărca pagina web sau aplicația web căreia fișierul modificat îi aparține.

Procesul de instalare este următorul:
1.	Se accesează [](https://nodejs.org/en/) și se instalează *Node.js*.  
2.	Se instalează *Browsersync*. Pentru aceasta se tastează într-o fereastră *command prompt* comanda:
```
npm install -g browser-sync
```

## Prototipul unei pagini web create folosind *HTML5*
Porniți aplicația *Sublime Text* și tastați următorul cod HTML:
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>
  </body>
</html>
```
Salvați conținutul tastat în fișierul denumit *index.html* din directorul proiectului *proiectjs1*.

## Afișarea paginilor web
Paginile web sunt afișate folosind o aplicație destinată navigării în Internet (eng. *browser*). Pentru cei care folosesc calculatoare pe care este instalat Windows, cele mai folosite sunt Google Chrome, Mozilla Firefox sau Microsoft Edge.

Paginile web sunt primite (*servite*) apelând o aplicație specializată denumită *server de web*. Procesul de transfer în fereastra browser-ului a unei pagini din Internet este inițiat prin tastarea în caseta de adrese a browser-ului a adresei paginii web dorite. Adresa unei pagini web este introdusă automat în caseta de adrese dacă se selectează cu mausul o adresă (eng. link) dintr-o pagină deschisă. De exemplu, pentru a învăța cum se navighează pe discul calculatorului Dv. în fereastra *Command prompt* (important!) folosind comanda *cd* accesați pagina [youtube.com](https://www.youtube.com/watch?v=sjaCgavMO18).

Pentru a porni pe calculatorul Dv. un server de web capabil să vă servească pagina creată anterior (*index.html*) deschideți o fereastră *Command prompt* și navigați în directorul proiectului *proiectjs1* (în cazul meu calea este *D:\Proiecte2019\proiect1*).
Tastați apoi în fereasta *Command prompt* comanda:
```
browser-sync start --server --files "*.html, css/*.css, js/*.js"
```
Această comandă pornește aplicația *browser-sync* și un server de web (opțiunea *--server*). De asemenea instituie supravegherea fișierelor *html*, *css* și *JavaScript* din cadrul proiectului Dv. (opțiunea *--files* ...).

Dacă totul decurge perfect, browser-ul implicit de pe calculatorul Dv. va fi lansat în execuție automat și în fereastra acestuia veți vedea efectul încărcării paginii *index.html*.

![Img. 2](/images/poza2.jpg)

Observație: *index.html* este denumirea implicită a paginii principale a unui site web. Din acest motiv în caseta de adrese a browser-ului nu apare denumirea paginii încărcate ci numai adresa din internet de unde a fost preluată. Adresa localhost se referă la propriul calculator. La pornirea serverului de web, în fereastra Command prompt aveți pentru site-ului accesat două adrese, localhost și o adresă în care se folosesc 4 numere (*192.168.56.1*), ca în imaginea următoare:

![Img. 3](/images/poza3.jpg)

A doua adresă ar putea fi folosită pentru a accesa pagina creată (*index.html*) de pe telefonul Dv. 

## Elemente HTML5
- Paragraf: `<p>...</p>`
- Titlu: `<h1>...</h1>, <h2>...</h2> ( ... <h6>...</h6>)`
- Sfârșit de linie (break): `<br> (sau <br />)`
- Listă neordonată (cu marcatori): `<ul>...</ul>, <li>...</li>`
- Listă ordonată: `<ol>...</ol>, <li>...</li>`
- Division (section): `<div>...</div>`

## CSS – *Cascading Style Sheets*
Exemplu fundamental:
```
<style>
body {
   background-color: #3d7cb2;
}

h1 {
   color: #dfe3e6;
   text-align: center;
}

p {
   font-family: verdana;
   font-size: 20px;
}
</style>
```
Elementul *<style>* se plasează în secțiunea *<head>* a paginii *index.html*.
  
Exemplu de rezultat posibil:
```
<!DOCTYPE html>
<html lang="en">
<head>
	<!-- poveste ... -->
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
	<title>Proiect 1</title>
	<style>
body {
   background-color: #3d7cb2;
}

h1, h2 {
   color: #dfe3e6;
   text-align: center;
}

p, li {
   font-family: verdana;
   font-size: 16px;
}
</style>

</head>
<body>
	<div>
	<h2>Primul proiect</h2>
	<p>Acest proiect ne acomodează cu principiile HTML.<br>Este vorba despre un proiect simplu, de vară.</p>
	<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 
    
Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.<br><a href="https://www.w3schools.com">This is a link</a></p>
	<ol>
		<li>Primul element</li>
		<li>Al doilea element...</li>
	</ol>
</div>
</body>
</html>
```

Continuarea (pentru curioși :)) la adresa [w3schools.com](https://www.w3schools.com/css/css_intro.asp) ...





