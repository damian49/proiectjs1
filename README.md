# proiectjs1
A project designed to learn some basic HTML, CSS and JavaScript concepts.

# Crearea proiectului 
Se crează pe discul *D:* un director denumit *proiect1*. În acest director se crează subdirectoarele *css* și *js*.
Rezultat:
![Img. 1](https://github.com/damian49/proiectjs1/blob/master/images/poza1.jpg)

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
Paginile web sunt afișate folosind o aplicație destinată navigării în Internet. Pentru cei care folosesc calculatoare pe care este instalat Windows, cele mai folosite sunt Google Chrome, Mozilla Firefox sau Microsoft Edge.
Paginile web sunt primite (servite) apelând o aplicație specializată denumită *server de web*. Procesul de transfer în fereastra browser-ului a unei pagini din Internet este inițiat prin tastarea în caseta de adrese a browser-ului a adresei paginii web dorite. Adresa unei pagini web este introdusă automat în caseta de adrese dacă se selectează cu mausul o adresă (eng. link) dintr-o pagină deschisă. De exemplu, pentru a învăța cum se navighează pe discul calculatorului Dv. în fereastra *Command prompt* (important!) folosind comanda *cd* accesați pagina [](https://www.youtube.com/watch?v=sjaCgavMO18).
Pentru a porni pe calculatorul Dv. un server de web capabil să vă servească pagina creată anterior (*index.html*) deschideți o fereastră *Command prompt* și navigați în directorul proiectului *proiectjs1* (în cazul meu calea este *D:\Proiecte2019\proiect1*).
Tastați apoi în fereasta *Command prompt* comanda:
```
browser-sync start --server --files "*.html, css/*.css, js/*.js"
```
Această comandă pornește aplicația *browser-sync* și un server de web (opțiunea *--server*). De asemenea instituie supravegherea fișierelor *html*, *css* și *JavaScript* din cadrul proiectului Dv. (opțiunea *--files* ...).
Dacă totul decurge perfect, browser-ul implicit de pe calculetorul Dv. va fi lansat în execuție automat și în fereastra acestuia veți vedea efectul încărcării paginii *index.html*.

