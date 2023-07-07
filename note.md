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