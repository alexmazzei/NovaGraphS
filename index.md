# Sinossi del progetto
 
Principal Investigator: Alessandro Mazzei, Dipartimento di Informatica, Università degli Studi di Torino

---

## Sinossi del progetto 

Il progetto NoVAGraphS (Non-Visual Access to Graphical Structures)
intende affrontare il problema dell'accesso all'informazione scientifica
contenuta nelle strutture grafiche da parte di persone con disabilità
visive. Le tecnologie attuali hanno messo a disposizione diversi
strumenti per aiutare le persone non vedenti o ipovedenti, ma spesso
queste tecnologie hanno delle forti limitazioni in contesti non
prettamente testuali. I libri scientifici, per l'appunto, contengono
molto spesso delle informazioni grafiche "strutturate", che possono
prendere, ad esempio, la forma di tabelle o più in generale di
diagrammi. L'idea del progetto NoVAGraphS e di fornire degli standard,
sia in forma di buone pratiche che di software funzionanti, per
permettere la comprensione di tali informazioni grafiche strutturate. Il
punto di partenza del progetto è l'idea di rendere tali strutture
*navigabili* da parte di una persona con disabilità visiva.

# Motivazioni: quali bisogni vuole soddisfare l'iniziativa

Gli studenti non vedenti e ipovedenti incontrano numerose difficoltà
nell'accesso agli studi universitari
[@supalo2013historical; @beck2008advancing; @cryer2013teaching]. In
particolare, la fruizione di rappresentazioni grafiche strutturate, come
tabelle, diagrammi, circuiti, ecc., risulta molto difficile per almeno
tre ragioni. In primo luogo, tali immagini sono pensate per essere
fruite mediante il canale visivo [@heller2002tactile]. In secondo luogo,
le più comuni rappresentazioni non visive delle immagini, ad esempio le
riproduzioni tattili
[@gupta2017tactile; @panotopoulou2020tactile; @thevin2019creating],
presentano numerosi limiti. Ad esempio, rappresentazioni con molti
dettagli non sono facilmente percepibili al tatto
[@kalia2011tactile; @watanabe2018effectiveness] e alcuni strumenti, come
ad esempio i dispositivi aptici, sono molto costosi e poco diffusi
[@ramloll2000constructing; @yu2003evaluation; @van2005auditory; @bernareggi2019mugraph; @moll2013haptic; @besse2017understanding].
In terzo luogo, per realizzare rappresentazioni non visive delle
immagini strutturate, è necessaria una conoscenza approfondita del
dominio e dell'esplorazione non visiva
[@gorlewicz; @prescher2014production; @moon2012accommodating]. C'è
quindi un bisogno urgente di strumenti per trasformare le
rappresentazioni grafiche strutturate in rappresentazioni fruibili da
persone con disabilità visiva, bisogno percepito sia da parte degli
studenti disabili nel loro percorso di studio, sia da parte delle figure
che si occupano di adattare il materiale didattico (tutor, trascrittori,
ecc.)
[@chockthanyawat2017towards; @sorge2015end; @engel2019svgplott; @sorge2019scientific].

#### Il progetto sul territorio Piemontese

Il Laboratorio Polin[^1] dal 2013 svolge ricerca e sviluppo,
sperimentazione e disseminazione di tecnologie per l'accesso agli studi
universitari di persone con disabilità. Perciò, i bisogni delle persone
con disabilità visive, dei tutor e dei trascrittori sono stati
individuati nel corso delle attività ordinarie del Laboratorio. In
particolare, i bisogni sono emersi dalle numerose attività di confronto
e sperimentazione con le associazioni sul territorio (Unione Italiana
Ciechi e Ipovedenti, Associazione Pro Retinopatici ed Ipovedenti), con
le scuole e con gruppi di studenti con disabilità; dalle esperienze
dirette di trascrizione di testi scientifici in formati digitali
accessibili a persone con disabilità visive messi a disposizione agli
studenti attraverso la biblioteca digitale del Laboratorio; dalla
partecipazione ogni anno a numerosi convegni nazionali e internazionali
sul tema dell'accessibilità alle tecnologie digitali e dalla
collaborazione con esperti di tecnologie assistive non vedenti e
ipovedenti mediante assegni di ricerca e borse di studio.

# Il progetto NoVAGraph rispetto allo stato dell'arte

Numerose soluzioni sono state proposte per permettere alle persone con
disabilità visive di fruire di particolari tipologie di immagini. Si
possono individuare quattro principali tecniche per la rappresentazione
non visiva di immagini: le descrizioni testuali, le rappresentazioni
tattili e audiotattili, le rappresentazioni aptiche e la sonificazione.

::: description
*Le descrizioni testuali di immagini* sono state studiate in particolare
per la rappresentazione di immagini generiche [@wu2017automatic], di
formule chimiche [@sorge2015end], di circuiti elettronici
[@zapirain2010learning], di grafici di funzione
[@chockthanyawat2017towards] e diagrammi di statistica
[@ault2002evaluation]. Gli studi svolti evidenziano due limiti
principali di tali soluzioni: è necessaria un'approfondita conoscenza
del dominio e delle caratteristiche della percezione non visiva da parte
di chi realizza la descrizione testuale, inoltre il carico cognitivo per
comprendere la descrizione testuale di un'immagine complessa è molto
elevato poichè l'esplorazione è sequenziale.

*Le rappresentazioni tattili e audiotattili* sono state studiate in
particolare per rappresentare immagini artistiche
[@cavazos2021accessible; @krivec2014adapting], grafici di funzione
[@watanabe2006practical; @bornschein2014svgplott], forme geometriche
[@panotopoulou2020tactile; @thevin2019creating; @kalia2011tactile] e
varie tipologie di diagramma (istogramma, diagramma a barre, circolare,
ecc.)
[@engel2020touchpen; @engel2019svgplott; @gupta2017tactile; @watanabe2018effectiveness].

*Le rappresentazioni aptiche* sono state proposte in sistemi multimodali
in particolare per comunicare informazioni grafiche in movimento
[@besse2017understanding], per l'esplorazione di grafi
[@bernareggi2008multimodal], di formule chimiche
[@bernareggi2019mugraph], di grafici di funzione
[@ramloll2000constructing; @van2005auditory], di forme geometriche
[@theurel2012haptic; @moll2013haptic; @manshad2011micoo] e di varie
tipologie di diagrammi [@yu2003evaluation].

*La sonificazione* è stata studiata per esplorare immagini generiche
[@sarkar2012], grafici di funzione
[@taibbi2014audiofunctions; @ahmetovic2019audiofunctions; @walker2010universal],
forme geometriche elementari
[@yoshida2011edgesonic; @gerino2015eyes; @mascetti2017evaluation; @banf2013sonification],
mappe [@delogu2010non; @su2010timbremap] e varie tipologie di diagrammi
[@godfrey2018accessible; @sorge2019scientific].
:::

Il progetto NoVAGraphS intende adottare la tecnica della descrizione
testuale con l'introduzione di un'importante novità, ovvero rendere la
descrizione testuale della struttura interattiva così da poter
permettere la *navigabilità* della struttura stessa. Le moderne tecniche
di elaborazione del linguaggio umano permettono infatti di creare dei
nuovi scenari di interazione testuale e vocale tra uomo e macchina.
Grazie agli sviluppi della linguistica computazionale, se limitiamo una
conversazione ad uno specifico dominio applicativo, i computer oggi sono
in grado sia di comprendere il linguaggio umano [@porporato2019mume],
sia di esprimersi con naturalezza [@mazzei2019using]. L'idea innovativa
del progetto sta nell'applicare queste moderne tecniche per l'analisi e
la generazione automatica del linguaggio umano per permettere alle
persone con disabilità visiva di interagire con un sistema interattivo
che descriva testualmente la struttura grafica.

# Azioni concrete previste nel progetto NoVAGraph

Il progetto NoVAGraphS intende rispondere ai bisogni individuati
perseguendo tre obiettivi principali:

-   **realizzare un software trasformatore** di immagini strutturate
    (primariamente tabelle, diagrammi entità-relazione, diagrammi UML,
    alberi, grafi, circuiti) verso un formato accessibile, adatto
    all'esplorazione non visiva;

-   **realizzare un software esploratore** per navigare, ed
    eventualmente modificare, queste tipologie di immagini accessibili
    interagendo mediante voce e suono;

-   **validare il trasformatore e l'esploratore** con una
    sperimentazione somministrata in diversi contesti didattici
    (Università o scuole secondarie superiori), ad esempio: studenti e
    docenti in classi inclusive, studenti con ipovisione/cecità nelle
    attività didattiche individuali o di gruppo, ecc.

Il trasformatore assume che in ingresso venga data una rappresentazione
semantica della struttura dell'immagine (ad esempio LaTeX o PPT), per
poterla convertire in una rappresentazione SVG (Standard Vector
Graphics, uno standard W3C). Quest'ultima sarà arricchita con i metadati
necessari all'esplorazione non visiva. Inoltre, poiché non sempre la
rappresentazione semantica in LaTeX o PPT è disponibile (si pensi ad
esempio ad immagini bitmap presenti nei libri di testo), il progetto
**svilupperà anche delle linee guida contenenti delle buone pratiche**
di conversione manuale verso l'SVG, per aiutare i trascrittori in questo
compito. L'esploratore consisterà in un'estensione di un browser
(Firefox o Chrome) per permettere la lettura e la navigazione
dell'immagine vettoriale mediante dei comandi da tastiera, touchscreen,
vocali, o mediante l'uso della display Braille. L'esploratore permetterà
anche di adattare i parametri di visualizzazione ad alto contrasto, il
tipo di carattere e l'ingrandimento in modo da facilitare le persone con
ipovisione lieve/media. Infine, gli strumenti sviluppati saranno
valutati sia mediante studi supervisionati sia mediante studi
longitudinali in specifici percorsi didattici.

# Comunicazione dei Risultati del progetto NoVAGraphS

La comunicazione verso i destinatari del progetto seguirà due canali
paralleli. Da un lato, seguendo la metodologia di Adoption-Centered
Design consolidata nei progetti di trasferimento tecnologico, tutti gli
stake holders (associazioni, servizi per studenti con disabilità nelle
università, scuole, ecc.) saranno coinvolti fin dalle prime fasi del
progetto in modo da condurre una sperimentazione su vasta scala e
realizzare strumenti che possano realmente essere adottati dai
destinatari. Dall'altro, il Laboratorio condurrà una campagna di
informazione sui risultati ottenuti in cinque direzioni principali: sui
canali web e social del Laboratorio, attraverso articoli su giornali e
riviste con cui il Laboratorio ha collaborato in passato (PC
Professionale, Corriere della sera, ecc.), partecipando a liste e gruppi
di discussione sul tema delle tecnologie assistive e della didattica
inclusiva, organizzando webinar tematici e partecipando a convegni
nazionali e internazionali sia a carattere scientifico (ACM ASSETS e
HCI, Springer ICCHP, ecc.) sia divulgativo (Accessibility days,
Didamatica, Handimatica, ecc.).

#### Azioni previste per valutare il successo di NoVAGraphS

Per la valutazione del successo del progetto verranno realizzati due
step di raccolta e analisi dei dati:

-   il primo step prevede l'analisi dei dati con metriche qualitative e
    quantitative ottenuti da sperimentatori con diversi tipi di
    disabilità visiva.

-   il secondo step prevede un'analisi qualitativa sui dati raccolti
    durante le esperienze didattiche (case study/ies), compresi i casi
    di didattica inclusiva, e mediante quadri teorici specifici della
    ricerca in Didattica della Matematica.

#### Principi di focalizzazione dell'attività

L'iniziativa risponde al bisogno di promuovere lo sviluppo economico e
sociale del territorio, ma anche il welfare di comunità in un'ottica di
inclusione e di partecipazione delle persone con difficoltà. Attualmente
le barriere che le persone con disabilità visive incontrano nelle
discipline scientifiche disincentivano l'accesso a molti Corsi di Laurea
e di conseguenza l'inclusione socio-lavorativa risulta raggiungibile
solo con enormi sforzi. Le ricadute a livello occupazionale sono ampie
perché questa mancanza impedisce l'accesso a impieghi ad alta
qualificazione alle persone con disabilità. Infine, la necessità di
erogare didattica a distanza, per i motivi legati all'attuale situazione
pandemica e post-pandemica, ha ulteriormente evidenziato e reso palese
l'urgente necessità degli studenti con difficoltà di disporre di
materiale didattico digitale scientifico accessibile.

#### Continuità con progetti precedentemente finanziati dalla Fondazione CRT

In precedenza la fondazione CRT ha finanziato due progetti con tematiche
legate a quelle del presente progetto.

-   Il primo progetto, chiamato *Accessibilità di testi digitali con
    contenuti scientifici da parte di persone con disabilità
    visiva*[^2], riguardava l'accessibilità delle formule matematiche, e
    si è concluso con la realizzazione di un innovativo pacchetto LaTeX,
    chiamato axessibility[^3], che per la prima volta permette di
    generare documenti PDF contenenti formule matematiche fruibili dalle
    persone cieche mediante screen reader e display braille. Ciò
    attualmente permette una maggiore diffusione di materiale didattico
    accessibile di argomento matematico.

-   Il secondo progetto *Matematica a voce*[^4], ancora in svolgimento,
    riguarda il problema dell'accessibilità delle formule matematiche
    per le persone sorde, con disabilità motoria degli arti superiori e
    con disturbi specifici dell'apprendimento.

Il progetto NovaGraphSpotrà potrà sfruttare i risultati raggiunti in
questi due progetti. In particolare, i risultati di tutti questi
progetti saranno la base per realizzare una *Biblioteca Accessibile*[^5]
di documenti digitali fruibili da persone con disabilità visive e
sonore, che potrà costituire un punto di riferimento per il recupero di
materiale di studio da parte di studenti con diverse disabilità.

# Team del progetto

La natura multidisciplinare delle informazioni strutturate presenti nei
testi scientifici necessità di diverse competenze per potere verificare
l'efficacia dei risultati in un ampio spettro di applicazioni. A tal
fine, i Dipartimenti dell'Università di Torino che hanno aderito al
progetto sono cinque: Dipartimento di Informatica, Dipartimento di
Matematica, Dipartimento Filosofia e Scienze dell'Educazione,
Dipartimento di Fisica, Dipartimento di Economia e Statistica. Per ogni
Dipartimento è stato già individuato un responsabile, che avrà il
compito di coordinare il lavoro dei partecipanti strutturati, dei
borsisti e dell'assegnista di ricerca.

Nella Tabella [1](#tab:team){reference-type="ref" reference="tab:team"}
abbiamo riportato la composizione completa del team di ricerca per il
personale appartenente all'Università degli Studi di Torino. A questi,
come già previsto nel budget, se il progetto verrà finanziato si
aggiungeranno cinque borsisti trimestrali, 1 borsista quadrimestrale e
un assegnista di ricerca annuale.

::: {#tab:team}
  **Nominativo**                                               **Dipartimento**            **Ruolo nel progetto**
  -------------------------------------------------- ------------------------------------- ------------------------------------
  Alessandro Mazzei                                               Informatica              Coordinatore
  Rossana Damiano                                                 Informatica              Validazione software e linee guida
  Daniele Radicioni                                               Informatica              Sviluppo software e validazione
  Anna Capietto                                                   Matematica               Referente Scientifico
  Ornella Robutti                                                 Matematica               Validazione software e linee guid
  Sandro Coriasco                                                 Matematica               Sviluppo software e validazione
  Tiziana Armano                                                  Matematica               Sviluppo software e validazione
  Carlotta Soldano                                                Matematica               Sviluppo software e validazione
  Davide Maietta                                                  Matematica               Sviluppo software e validazione
  Cristina Sabena                                     Filosofia e Scienze dell'educazione  Referente Scientifico
  Marisa PavoneFilosofia e Scienze dell'educazione    Validazione software e linee guida   
  Marina Serio                                                      Fisica                 Referente Scientifico
  Dalit Contini                                                                            Referente Scientifico
  Mari Laura Di Tommaso                                      Economia e Statistica         Validazione software e linee guida

  : Composizione del team di ricerca appartenente all'Università degli
  Studi di Torino
:::

[]{#tab:team label="tab:team"}

#### Partner del progetto

Un contributo importante allo svolgimento del progetto verrà dato
dall'associazione *Informatici senza Frontiere*[^6], che ha deciso di
contribuire con le proprie conoscenze e esperienze nel campo
dell'insegnamento e del supporto alla diffusione dell'informatica nei
soggetti diversamente abili. In coda a questo documento si può trovare
la lettera di intenti dell'associazione con l'intenzione di partecipare
al progetto.

# Fasi del progetto e GANTT

Il periodo di svolgimento del progetto è dal giorno 01/03/2022 alla data
del 31/08/2023. Il progetto si articola in tre fasi, per una durata
complessiva di 18 mesi.

Fase 1:

:   Studio e realizzazione del Trasformatore-Linee Guida.\
    Data inizio 01/03/2022, Data fine 30/09/2022

Fase 2:

:   Studio e realizzazione dell'Esploratore.\
    Data inizio 01/10/2022, Data fine 30/04/2023

Fase 3:

:   Validazione sperimentale dei software Trasformatore/Esploratore.\
    Data inizio 01/05/2023 Data fine 31/08/2023

Nella Figura [1](#fig:gantt){reference-type="ref" reference="fig:gantt"}
è proposto il diagramma di Gantt del progetto, per chiarire le scansioni
temporali delle varie fasi.

![Gantt del progetto](gantt-01.pdf){#fig:gantt width="0.9\\columnwidth"}

# Breve Curriculum Vitae del coordinatore

Alessandro Mazzei[^7] è ricercatore universitario confermato e
professore aggregato presso il Dipartimento di Informatica
dell'Università degli Studi di Torino. L'attività scientifica svolta da
Alessandro Mazzei si colloca nel campo dell'intelligenza artificiale e
più precisamente nell'area della linguistica computazionale. La sua
attività di ricerca si delinea essenzialmente lungo quattro filoni: la
sintassi computazionale, la semantica computazionale, le ontologie
informatiche, la generazione del linguaggio. Su queste tematiche ha
pubblicato oltre 100 lavori scientifici in *peer review*. Membro di
comitati di programma di diverse conferenze internazionali quali COLING,
LREC, AI\*IA, etc. È stato *program chair* e organizzatore della "Fifth
Italian Conference on Computational Linguistics", tenutasi a Torino nel
Dicembre 2018. È componente del laboratorio "S. Polin" dell'Università
degli Studi di Torino per la ricerca sulle Nuove Tecnologie Assistive
per le STEM. È stato componente del comitato scientifico del Master
universitario in Intelligenza Artificiale dell'Università di Torino. La
sua attività didattica riguarda la Linguistica Computazionale, la
programmazione JAVA, l'Informatica Generale, le Basi di dati. Alessandro
Mazzei ha partecipato a diversi progetti nazionali ed europei, ta cui
ATLAS, LIS4ALL, HPC4AI. Egli, inoltre, è stato proponente e coordinatore
del progetto MADiMan[^8] (Multimedia Applications for DIet MANagement
Innovation Hub for ICT, 2011-2014, 705 POR-FESR 07-13.)

[^1]: <http://www.integr-abile.unito.it>

[^2]: <https://www.dipmatematica.unito.it/do/progetti.pl/Show?_id=0se4>

[^3]: <https://ctan.org/pkg/axessibility>

[^4]: <https://www.dipmatematica.unito.it/do/progetti.pl/Show?_id=uwgr>

[^5]: <http://www.integr-abile.unito.it/knowledge-transfer/accessible-library-2/>

[^6]: <https://www.informaticisenzafrontiere.org/en/>

[^7]: <https://scholar.google.it/citations?user=QEWnKJwAAAAJ&hl=it>

[^8]: <https://di.unito.it/madiman>





# *NoVAGraphS*: Non-Visual Access to Graphical Structures

You can use the [editor on GitHub](https://github.com/alexmazzei/NovaGraphS/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block


## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/alexmazzei/NovaGraphS/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
