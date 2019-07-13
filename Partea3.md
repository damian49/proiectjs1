## Exerciții de programare în JavaScript

### Un pic de pregătire...

Pentru a realiza rapid o pagină web elementară, SublimeText permite încărcare unei secvențe de cod predefite. De altfel facilitatea a fost deja folosită pentru încărcarea unui text aleator folosind scurtătura *lorem + Tab*.

Definirea unei astfel de secvențe se inițiază selectând în meniul aplicației *Tools / Developer / New Snippet...*:

![ST Snippet](/images/poza8.png)

Aplicația va afișa prototipul unui *snippet*. 

![ST Snippet](/images/poza9.png)

În prototipul afișat, secvența `Hello, ${1:this} is a ${2:snippet}.` va trebui înlocuită cu secvența de cod dorită. De asemenea  se va insera un marcaj *<tabTrigger>* pentru a impune comanda (scurtătura) care va declanșa inserarea codului (*web*):

![ST Snippet](/images/poza10.png)

În continuare se salvează snippet-ul definit folosind calea implicită accesată de SublimeText în momentul inițierii salvării (*Ctrl + S*). Extensia fișierului va fi obligatoriu *.sublime-snippet*, ca în imagine:

![ST Snippet](/images/poza11.png)

Se inserează apoi într-o fereastră secvența de cod predefinită. Pentru aceasta se va creea un nou fișier și se va tasta secvența de caractere defită prin marcajul *<tabTrigger>*, respectiv *web + Tab*. Apoi se salvează noul fișier. 
  
Rezultat:
  
![ST Snippet](/images/poza12.png)

Observație: Noul fișier va avea obligatoriu extensia *.html*!

## Ok, și acum JavaScript!

Să începem cu câteva lucruri simple:

1. Declarați două variabile, *a* și *b*, având valorile inițiale *10* și *17*. Afișați pe consolă cele două valori și apoi schimbați între ele conținuturile celor două variabile (adică *a* trebuie să fie *17* și *b 10*). Afișați apoi pe consolă noile valori. Verificați dacă totul a funcționat (afișați consola, *F12*!).

Secvența de cod ar putea fi următoarea:
```
<script>
   var a = 10, b = 17, aux;
   console.log("Inainte: a = ", a, ", b = ", b);
   aux = a; a = b; b = aux;
   console.log("Dupa: a = ", a, ", b = ", b);
</script>
```

După (re)încărcarea paginii ar trebui să vedeți în consolă valorile afișate:

![ST Snippet](/images/poza13.png)

Unde plasăm elementul *&lt;script>*? Eu l-aș pune la sfârșitul paginii, înainte de *&lt;/body>*. Nu prea are treabă cu restul paginii, deci se aplică regula.

2. Alt exemplu. Trebuie să transformăm gradele Fahrenheit în grade Celsius. Relația de calcul ar fi:

T(°C) = (T(°F) - 32) × 5/9

**Varianta 1:**
```
   var tf = 20, tc;
   tc = (tf - 32.) * 5. / 9.;
   console.out("Temperatura de " + tf + "grade Fahrenheit convetita in Celsius este: " + tc);
```

**Varianta 2:** Citiți valoarea de convertit (cu window.prompt()) și afișați rezultatul într-o fereastră alert. Spor!




