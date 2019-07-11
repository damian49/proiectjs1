# proiectjs1


A project designed to learn some basic HTML, CSS and JavaScript concepts.

## Crearea proiectului 
Se crează pe discul *D:* un director denumit *proiect1*. În acest director se crează subdirectoarele *css* și *js*.
Rezultat:
![Img. 1](/images/poza1.jpg)

## Instalări 
### a.	SublimeText
Accesați: [site-ul aplicației](https://www.sublimetext.com/) 

### b.	Browsersync
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

## Și în sfârșit, JavaScript :anguished:!
Paginile Web pot conţine pe lângă ansamblul de elemente care formează informaţia afişată şi secvenţe de cod care contribuie la realizarea unor efecte deosebite. Sunt deja consacrate galeriile de imagini, meniurile derulante sau efectele declanşate cu ajutorul mouse-ului care amplifică senzaţia de interactivitate. Pentru toate acestea s-a creat JavaScript, un limbaj derivat din C.

### Inserarea secvenţelor de cod JavaScript
Codul JavaScript se rulează în cadrul unui *interpretor de comenzi* integrat în aplicaţia de navigare în Internet. Se spune că JavaScript este un limbaj interpretat (spre deosebire de C sau C++ care sunt limbaje compilate). Limbajele interpretate se mai numesc şi limbaje de scriptare (eng. *scripting languages*).

O aplicaţie Web este însă o aplicaţie în *arhitectură client-server*, componenta *client* fiind executată în aplicaţia de navigare. Din această perspectivă, JavaScript este limbajul destinat scrierii componentei client. Pentru *componenta server*, programarea se face frecvent în PHP, PYTHON sau chiar în Javascript (folosind [Node.js](https://www.tutorialsteacher.com/nodejs/create-nodejs-web-server)). 

Inserarea codului JavaScript într-un document hipertext se realizează folosind un element *<script>*. Acesta poate conține cod JavaScript sau o referință la un fişier *.js* care conţine codul necesar. Exemplu de utilizare a unui element *<script>*:

```
   <script>
      // Se inserează liniile de cod
   </script>
```

sau:

```
   <script src="js/program.js"></script>
```

Deşi un element *&lt;script>* poate fi plasat oriunde într-un fişier .html, există totuşi două locuri în care acesta este inserat cu precădere, respectiv la început, în *&lt;head>*, sau la sfârşit, înainte de *&lt;/body>*. Plasarea unui element *&lt;script>* la sfârşitul paginii are avantajul de a nu afecta sensibil viteza de afişare a acesteia, deoarece browser-ul tratează elementele conţinute în fişierul hipertext în ordine. Dacă elementul *&lt;script>* este plasat la început, pagina se va afişa doar după încărcarea codului pe care acesta îl conține.

O pagină poate avea mai multe elemente *&lt;script>*.

### Exemple fundamentale

**1. Afișarea unui mesaj dintr-un script JavaScript

```
<DOCTYPE! html>
<html>
<head>
	<meta charset="utf-8">
	<title>Java Script</title>
	<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
</head>
<body>
	<script>
		alert("Mesaj din script: Spor!");
	</script>
	<h1>Titlul paginii</h1>
	<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
	tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
	quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
	consequat.</p>
</body>
</html>
```

Încărcarea paginii va produce afișarea unei mici ferestre:

![Img. 4](/images/poza4.jpg)


**2. Declararea și utilizarea unor variabile

```
<!DOCTYPE html>
<html>
<head>
   <meta charset="UTF-8">
   <title>Programarea in JavaScript</title>
</head>
<body>
    <h1>O pagină HTML</h1>
    <p>Aceasta este o pagină HTML.</p>
    <p>Ea poate fi deschisă în diferite browsere:</p>
    <ul>
        <li>Internet Explorer</li>
        <li>Mozilla Firefox</li>
        <li>Google Chrome</li>
        <li>Opera, etc.</li>
    </ul>
    <script>
        var i = 100;
        console.log("i = ", i);
    </script>
</body>
</html>
```

Funcția apelată în finalul scriptului, *console.log()*, produce afișarea unei linii în *consola* browser-ului. Pentru a afișa consola, în funcție de browser-ul utilizat, se va apăsa o anumită combinație de taste.

* Google Chrome: F12 sau Ctrl+Shift+J;
* Safari: Ctrl+Alt+I;
* Firefox: Ctrl+Shift+K;

### Variabile
Ca în orice limbaj de programare, variabilele sunt containere folosite pentru a păstra valori. Pentru a declara o variabilă se foloseşte cuvântul rezervat var. Declararea unei variabile poate fi cumulată cu iniţializarea ei. Exemple:

```
   var nrLinii = 7;
   var sumaInt = 12 + 45;
   var coleg, prieteni;
   var anul=2014, luna=10, ziua=14;
```

În exemplele prezentate primele variabile (*nrLinii* şi *sumaInt*) sunt iniţializate în momentul declarării iar următoarele două (*coleg* şi *prieteni*) sunt doar declarate, urmând să fie iniţializate ulterior. Evident, o variabilă neiniţializată nu poate fi folosită decât după ce primeşte o valoare printr-o atribuire. Până la inițializare o variabilă are tipul *undefined* (nedefinit).

Denumirea unei variabile începe cu o literă şi poate conţine litere, cifre şi `'_'` (*underscore*). De obicei programatorii folosesc denumiri sugestive, formate prin alăturarea mai multor cuvinte. Pentru a face inteligibil numele astfel obţinut, cuvintele care îl compun sunt separate prin `'_'` sau încep cu o literă mare (variantă denumită sugestiv *camelCase*).

### Tipul unei variabile

Tipul unei variabile se stabileşte automat, în momentul iniţializării.

În JavaScript sunt definite următoarele tipuri:

* Number,
* String,
* Boolean,
* Object,
* null și
* undefined.
Observații: 
1. *null* diferă de *undefined* prin faptul că *undefined* este tipul unei variabile care încă nu a fost inițializată iar *null* este tipul unei variabile căreia i s-a dat valoarea *null* cu scopul de a impune lipsa unei valori.

2. O variabilă iniţializată poate primi ulterior altă valoare, de acelaşi tip sau având un tip diferit, caz în care îşi modifică automat tipul. Exemple:

```
   var varianta = 7;   //  varianta este de tip Number
   varianta = "Fructe de pădure";  //  varianta devine String
```

3. Şirurile de caractere pot fi delimitate atât prin ghilimele ("sir cu ghilimele") cât şi prin caractere apostrof ('sir cu apostrof').

### Şiruri de valori

Pe lângă tipurile simple, în JavaScript se pot declara şiruri de valori (eng. *arrays*) şi obiecte. Spre deosebire de limbajele puternic tipizate (C++, Java, C# etc.) în JavaScript şirurile de valori pot conţine elemente de diferite tipuri. Exemple:

```
   var intregi = [11, 21, 3, 45, 5];  //  sir de intregi, ca în C++
   var sir = ["Ambasador", 2300, "Functionar", 1800]; //  JavaScript!
   var nume = ["Ionescu", 1200, "Popa", 3400, "Alexandru", "Oltean"];
```

Un element al unui şir de valori poate fi accesat folosind indici, astfel:

```
   var unNume = nume[2];  //  Popa, pozitia a 3-a
```

Ca şi în C, numărarea elementelor începe de la 0.

Pentru a cunoaşte lungimea şirului se poate accesa proprietatea *length* scriind *nume.length* (va returna 6).

Şirurile din JavaScript pot conţine orice valori, inclusiv obiecte sau alte şiruri.

Tablourile bidimensionale se definesc asfel:

```
   var rude = [
      ["Ionescu", "Popa", "Alexandru"],
      ["23", "12", "34"]
   ];
```

Pentru a accesa elemente dintr-un astfel de tablou se vor folosi doi indici, ca înlimbajul C:

```
   nume = rude[0][0]; // Ionescu
   varsta = rude[1][0]; // 23
   nr = rude[1][2];     // 34
```

Observaţie: Ca şi în C, `rude[0]` reprezintă şirul `["Ionescu", "Popa", "Alexandru"]` iar `rude[1]` şirul `["23", "12", "34"]`.

Pentru a adăuga un element la sfârşitul unui şir se foloseşte funcţia *push()*. Exemplu:

```
   nume.push("Alexandra");
   console.log("Lungimea sirului: " + nume.length);  //  Afiseaza: Lungimea sirului: 7
```

### Aplicație

Se propune realizarea unei mici aplicații web care să afișeze tabla înmulțirii cu 7 si apoi, după generalizeare, să afișeze tabla înmulțirii cu orice număr.

**Varianta 1**

```
<DOCTYPE! html>
<html>
<head>
	<meta charset="utf-8">
	<title>Java Script</title>
</head>
<body>
	<h1>Tabla înmulțirii cu 7</h1>
	<p>7 x 1 = <script>document.write(7*1);</script><br>
		7 x 2 = <script>document.write(7*2);</script><br>
		7 x 3 = <script>document.write(7*3);</script><br>
	</p>
</body>
</html>
```
Funcția document.write() permite scrierea în pagină a unui șir de caractere. Este oarecum asemănătoare funcției console.log().

![Img. 5](/images/poza5.jpg)

Comentariu: Soluția prezentată este rudimentară deoarececare utilizează nejustificat de multe elemente `<script>`.


**Varianta 2**

```
<DOCTYPE! html>
<html>
<head>
	<meta charset="utf-8">
	<title>Java Script</title>
</head>
<body>
	<h1>Tabla înmulțirii cu 7</h1>
	<p>
	<script>
	document.write("7 x 1 = " + 7*1 + "<br>");
	document.write("7 x 2 = " + 7*2 + "<br>");
	document.write("7 x 3 = " + 7*3 + "<br>");
        </script>
	</p>
</body>
</html>
```
Comentariu: Evident, tot o soluție rudimentară deoarece pentru fiecare linie de pe ecran se apelează *document.write()*, deși se poate observa că s-ar putea automatiza generarea liniilor scriind un ciclu *for*.

**Varianta 3**

```
<DOCTYPE! html>
<html>
<head>
	<meta charset="utf-8">
	<title>Java Script</title>
</head>
<body>
	<h1>Tabla înmulțirii cu 7</h1>
	<p>
	<script>
	   var n = 7, i;
	   for(i=1; i <= 10; i++) {
	      document.write(n + " x " + i + " = " + n*i + "<br>");
	   }
	</script>
	</p>
</body>
</html>
```
Comentariu: O soluție corectă.

**Generalizare**

Pentru a genera table înmulțirii cu orice număr, valoarea variabilei n poate fi citită folosind window.prompt(). Această funcție afișează o fereastră conținând un mesaj și o casetă de text în care se poate tasta o valoare.

![Img. 6](/images/poza6.jpg)

```
<DOCTYPE! html>
<html>
<head>
	<meta charset="utf-8">
	<title>Java Script</title>
	<script>
    	var n = prompt("Tabla înmulțirii cu n. Introduceți n: ");
    </script>
</head>
<body>
	<h1>Tabla înmulțirii cu <script>document.write(n);</script></h1> 
	<p>
	<script>
	var i;
	for(i=1; i<=10; i++) {
		document.write(n + " x " + i + " = " + n*i + "<br>");
	}
	</script>
	</p>
</body>
</html>
```
Rezultat:

![Img. 7](/images/poza7.jpg)

Se poate rescrie aplicația astfel încât codul JavaScript să fie înregistrat într-un fișier denumit *tabla.js*, astfel:


```
<DOCTYPE! html>
<html>
<head>
	<meta charset="utf-8">
	<title>Java Script</title>
</head>
<body>
	<h1 id="titlu"></h1>
	<p id="tabla"></p>
	<script src="js/tabla.js"></script>
</body>
</html>
```

Scriptul javascript *tabla.js* este următorul:

```
var n = 9;
var tit = document.querySelector("h1");
var parag = document.querySelector('p');

tit.innerHTML = "Tabla inmultirii cu " + n;
var sir= "", i;
for(i=1; i<=10; i++) {
	sir = sir + n + " x " + i + " = " + n * i + "<br>";
}
console.log("sir: " + sir);
parag.innerHTML = sir;
```

**Observație:**
Cele două elemente care intervin în cod, &lt;h1> si &lt;p> au atribute *id* (*titlu* respectiv *tabla*). Valorile atributelor *id* sunt prin definiție unice în cadrul unei pagini web. În astfel de cazuri memorarea lor în variabile ale scriptului se realizează folosind valorile atributelor *id*, astfel:

```
var tit = document.querySelector("#titlu");
var parag = document.querySelector('#tabla');
```


