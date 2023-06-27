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