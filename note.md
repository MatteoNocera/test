# Appunti

## prima settimana
siti utili

1. [GitHub 104](https://github.com/fabiopacifici/104_html)


2. [Validator](https://validator.w3.org/) 
Da tatuare in petto! è un sito per vedere se è valido il codice

3. [special characters](https://www.whatsmyip.org/html-characters/) 
sito per vedere i caratteri speciali

4. Code the hidden language of computer hardware and software
libro su amazon

5. [tag semantici](https://www.w3schools.com/html/html5_semantic_elements.asp)
Tag Semantici

6. [appunti](https://www.markdownguide.org/basic-syntax/)
appunti

# Ricorda sempre di committare e pushare
- ol : ordered list
- ul : unordered list
- li : list item
- em : corsivo
- br : a capo
- hr : linea
- button : bottone
- a hreaf : link
- table : tabella (thead, tbody, tfoot, tr(riga di celle), th(intestazione), td(cella))
- target : attributo per link, apre una nuova scheda se "blanck"

i titoli possono arrivare fino ad h6 e ci deve essere solo un h1. In section deve esserci sempre il titolo

dentro ul/ol puoi annidare solo li come primi figli

`#` nel ref mi crea un link interno alla pagina

dividi sempre la pagina in macroaree (header, main, section, nav, footer)

Puoi mettere il testo dell'esercizio come commento in modo da avere sempre tutto sotto mano

Il sito [penpot](https://penpot.app/) mi rileva il layout

# CSS
## Regola di reset
## * {border: 0; margin: 0; box-sixing: border-box;}<br><br>

E' un file con regole di stile a cascata, vale l'ultimo scritto. Può essere scritto su un file.css a parte oppure usando dentro l'indez il tag style.<br><br>
Utilizzo # per selezionare id, utilizzo il . per selezionare la classe, utilizzo il tag per selezionarlo per intero ( body, div, section, ecc..). L'ordine di potenza è dal più forte al più debole.<br><br>
I Font di Google vanno inseriti prima di tutto, subito dopo il title del documento html e poi vanno indicati in css, sempre con un secondo Font più "sicuro". <br>
.element '>' h3 - seleziona tutti gli h3 figli di element

h1,h2 - seleziona entrambi gli elementi<br><br>
Cerca di inserire meno regole e dividere bene le sezioni per riutilizzare le regole CSS <br><br>
puoi inserire su main una max-width e il margin auto per avere i testi più centrati senza avvicinarsi troppo ai margini.<br><br>
Si può usare le righe di comando per inserire una cartella in una nuova repo su GitHub.<br><br>
## Con :root {} possiamo annidare tutti i colori e riprenderli con var() <br><br>
#region e #endregion per collassare le regole CSS<br><br>
Nelle classi usa il _ invece del - per poter selezionare in un click l'intera classe.<br><br>
Il box model sono gli spazi del tag<br><br>
Per il border con 4 valori si parte dall'alto e si gira in senso orario, con due valori sono sopra e sotto, destra e sinistra.<br><br>
## Display specifica la visualizzazione dell'elemento. Puoi cambiare i connotati degli elementi.
None, block, inline ed inline-block sono i maggiormente usati.<br><br>
 ![Alt text](image.png)<br>
 Grarda il [Riferimento](https://www.w3schools.com/cssref/pr_class_display.php)<br>
 ## Text Align
<br><br>
 ## box shadow 
 assex assey px ombreggiatura colore <br><br>

## Usa sempre rem e non pixel perchè quando cambi schermo si adatta meglio ai font<br><br>

# link [GitHub Fabio Pacifici](https://github.com/fabiopacifici)<br><br>

# Selettori Avanzati<br><br>
![Alt text](image-1.png)<br>
vedi il lin ai [selettori Avanzati](https://www.w3schools.com/cssref/css_selectors.php)

![Alt text](image-2.png)<br>
[Gioco Selettori](https://flukeout.github.io/)<br><br>

# Clearfix non mi fa collassare quando uso float
Può avere valori none,  left, right, both<br>

## La soluzione migliore è<br><br>
# ::after { content:''; display: table; clear: both;}<br><br>

# .clearfix::after {

    content:'';
    display: table;
    clear: both;
}

Puoi utilizzare una classe di debug per visualizzare a schermo se tutto funziona.

# Per fare repo da terminale 
# git init - git status - git add . - git commit -m"add html" - copia e incolla i comandi creati su GitHub creando una nuova repo
Il punto dopo add aggiunge tutto, se voglio solo un file devo togliere il punto e selezionare il file da aggiungere. <br><br>

# FLEXBOX

![Alt text](image-4.png)

![Alt text](image-5.png)

![Alt text](image-6.png)

## - <mark> justify-content (container rule) agisce su main axis<br>
## - <mark> align-items agisce (container rule) su cross axis<br>
## - <mark> flex-wrap (container rule) specifica se gli oggetti rimangono su una riga o no e quindi si comprimino oppure vadano su un'altra linea per non rompere il layout. Se imposto su wrap non si schiacciano, di base invece è impostato su no-wrap.<br>
## - <mark> flex-basis (item rule) imposta la dimensione legata al Main Axis<br>
## - <mark> flex-grow (item rule) fattore di crescita impostato su 0, se è 1 può crescere. Agisce come le percentuali.<br>
## - <mark> flex-shrink (item rule) fattore di riduzione agisce al contrario di grow.<br>
## - <mark> flex-order (item rule) ordino gli elementi disposti sulla pagina quando si restringe lo schermo in modo differente, dò una numerazione volontaria. Accetta il -1 che verrà all'inizio della fila<br>

## Consiglio per la lettura
[CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)<br><br>
# Struttura tabella tipo con display flex

![Struttura Tipo](image-7.png)

![Alt text](image-10.png)

# Per copiare icone di FONTAWESOME entra nella libreria, copia il link style ed incollalo nell'head di HTML. Poi entra sul sito awesome e copia il codice HTML dell'icona scelta ( trova quelle free ).

# Position
Lo uso per posizionare i singoli elementi nella pagina.
![Position](image-11.png)

## - relative : elemento posizionato relativamente alla posizione naturale e rimane nel flusso del documento.
## - absolute : si sposta in modo assoluto in base al primo elemento genitore che ha position diversa da static e lascia lo spazio nel documento lasciandolo libero.
## - fixed : analogo ad absolute ma il "contenitore" è sempre di riferimento al Viewport, quindi scrollando rimane visibile e ce lo portiamo dietro. <br><br>

# z-index
![z-indez](image-12.png)
Non può avere valore static per essere utilizzata.
Il numero più alto appare sovrapposto.
Posso usare un numero molto elevato se l'elemento deve essere per forza davanti.

# vw vh 
![Alt text](image-13.png)
E' la parte visibile dall'utente di una pagina web.
![Alt text](image-14.png)
![Alt text](image-15.png)
![Alt text](image-16.png)

# Effetti e transizioni
Servono per abbellire le animazioni in pagina <br>

## transition 
![transition](image-17.png)

## animation
![animation](image-18.png)
![Alt text](image-19.png)
## filters
![filters](image-20.png)

![Alt text](image-21.png)

## Riepilogo filtri [CSS Filter](https://css-tricks.com/almanac/properties/f/filter/)

# CSS Media Query

Regole CSS Dinamiche

![Alt text](image-22.png)

Gli ordini di visualizzazione sono sempre dall'alto al basso. <br>

Inseriamo sempre meta nell'head. <br>

Di base viene preferito usare il Mobile First per facilità e per avere il CSS più senllo.

![Alt text](image-23.png)

Fai attenzione alle selezioni, se le selezioni sono meno forti la media queri non funziona

# Le Griglie
Esprimiamo i contenuti dividendo lo spazio interno sempre in dodicesimi. <br>
![Alt text](image-24.png)
![Alt text](image-25.png)
![Alt text](breakpoint.png)<br>

# Bootstrap
Tramite cdn immettiamo un framework tramite link, compreso codice js. Non servirà più la regola di reset. Utilizza il Mobile first. Scatti 576, 768, 992, 1200, 1400. Pensati per multipli di 12. Tutto ciò che fa Boostrap è per essere ben visualizzato su dispositivi di varie misure. Non serve mai mettere un .container dentro un altro .container. Serve sempre utilizzare riga che incarta la colonna in modo da avere una responsività corretta.<br>
## I GUTTER servono per dare spazio.<br>
Per annidare puoi inserire direttamente una .row dentro una .col.<br>
## Se aggiungi delle classi usa il trattino basso o un prefisso in modo da distinguerle dalle regole di Bootstrap.
## Il tag script va in fondo, prima della chiusura del body ed il link va subito dopo il title.
# [GetBootStrap](https://getbootstrap.com/docs/5.3/examples/cheatsheet/)


# JAVASCRIPT
Prima di iniziare a programmare scriviti i vari passaggi in modo da avere sotto gli occhi le procedure da portare avanti step-by-step con uno pseudo-codice per poi ampliare il codice in ordine. <br>
AND richiede che si verifichino entrambe le condizioni.<br>
OR richiede che si verifichi almeno una condizione.<br>
Javascript è un linguaggio usato principalmente per il front-end.<br>
Il codice inline si utilizza usando il tag script e quando si usa sempre il tag script con l'attributo src.<br>

![Alt text](image-26.png)

## Si può scrivere nell'html con writeln

## Si può scrivere con alert facendo uscire una allerta
## Si può modificare un pezzo dell'html con la dom manipulation con innerHTML

Le variabili sono contenitori che contengono dati ed informazioni richiamabili in un secondo momento.

![Alt text](image-27.png)

![Alt text](image-28.png)

Le condizioni devono rispondere sempre con true o false.

![Alt text](image-29.png)

![Alt text](image-30.png)

![Alt text](image-31.png)

![Alt text](image-32.png)

Con queryselector seleziono il primo elemento e posso richiamarlo con il suo nome (es .btn chiamo la classe btn). Usando .classList mi restituisce la lista delle classi di un elemento e posso andare a modificare le proprietà (esempio .add oppure .remove).<br>
Con += aggiungo a ciò che già è presente (esempio .innerHTML += 'luca' aggiunge luca a ciò che era già scritto).<br>

## Breve intro alle funzioni

function name(params) {}

Per esempio alert è una funzione

![Alt text](image-33.png)
![Alt text](image-34.png)

addEventListener () dentro le parentesi vuole obbligatoriamente almeno due cose, la seconda della quale è la funzione che avviene all'evento.<br>

# Loops ( o Cicli)
ovvero basta copia e incolla

![Alt text](image-35.png)

## 1 - Ciclo for
![Alt text](image-36.png)

![Alt text](image-37.png)

![Alt text](image-39.png)

![Alt text](image-40.png)

![Alt text](image-41.png)

![Alt text](image-42.png)

![Alt text](image-43.png)

# [Switch Case](https://www.w3schools.com/js/js_switch.asp)

# Function
Possiamo richiamare del codice già utilizzato per non ripetere.
E' buona norma riutilizzare in modo da non ripetersi. Il codice risulta più pulito. Sono pezzi di codice da richiamare più volte in pagina. 

![Alt text](image-44.png)

Posso poi invocare la funzione ogni volta richiamandola. Nelle parentesi tonde possono esserci dei parametri.

![Alt text](image-45.png)

Diamo un nome espressivo alla funzione in modo che si capisca a cosa si riferisce.

## I parametri da soli servono da 'segnaposto' nel senso che non hanno valore finchè non lo inseriamo noi attraverso l'invocazione della funzione.

Parametro è dentro la funzione, l'argomento è quando definisco il parametro.

## La parola chiave return fa terminare la funzione

![Alt text](image-46.png)

![Alt text](image-47.png)

## Possiamo riusare la logica della funzione su un addEventListener

![Alt text](image-48.png)

![Alt text](image-50.png)

![Alt text](image-51.png)

## This è una parola chiave per recuperare l'elemento della DOM selezionato in precedenza

## function declaration = function my_function_name(params) {}
## my_function_name()

oppure

## const my_second_function = function() {}

# [IIFE](https://developer.mozilla.org/en-US/docs/Glossary/IIFE) (immediatly invoked function expression) 

## (function({ })) ();

# C'è poi un metodo per scrivere le funzioni più snelle --> Arrow Functions

Il this è riferito diversamente a seconda del suo posizionamento.

![Alt text](image-52.png)

# Timing Function

Funzioni non sincrone, posso lasciarle in attesa finchè non tolgo io la "pausa".
Evito di bloccare il programma se ci sono delle tecniche che richiedono attese di risposta.

![Alt text](image-53.png)

## setTimeout Eseguo il codice dopo un tot di tempo

![Alt text](image-54.png)

## setInterval Eseguo il codice ogni tot tempo

![Alt text](image-55.png)

## Per bloccare l'esecuzione

![Alt text](image-56.png)

# Objects

![Alt text](image-57.png)

![Alt text](image-58.png)

![Alt text](image-59.png)

![Alt text](image-60.png)

# For Each

Per ciclare in un array

## Map crea un nuovo array con return obbligatorio
Creo una nuova mappatura
## Filter se verifica il suo elemento crea un array e infila il nuovo elemento
Inserisce solo i valori true, obbligatorio il return

# Local storage mi permette di salvare i dati all'interno del pc dell'user.

# VUE JS Framework javascript

Tutto il codice è caricato su un'unica pagina in modo da essere più veloce. 

![Alt text](image-61.png)

![Alt text](image-62.png)

![Alt text](image-63.png)

![Alt text](image-64.png)

![Alt text](image-66.png)

![Alt text](image-67.png)

![Alt text](image-68.png)

![Alt text](image-69.png)

![Alt text](image-70.png)

![Alt text](image-71.png)

![Alt text](image-72.png)

![Alt text](image-73.png)