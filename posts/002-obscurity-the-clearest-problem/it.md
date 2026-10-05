---
id: 002
titolo: "L'oscurità, il problema più chiaro di cui nessuno parla"
sottotitolo: "Il principio di progettazione che questa comunità sbaglia più spesso, e i manuali che lo dimostrano."
lingua: it
autore: Yuri da Silva Villas Boas
papers: [DS]
tempo_di_lettura: ~8 min
copertina: assets/cover-1200x675.webp
copertina_alt: "Due persone su un divano, una al portatile e una che legge, entrambe occupate, mentre un elefante enorme con una maschera di Guy Fawkes siede nella stanza alle loro spalle senza che nessuno lo nomini."
---

# L'oscurità, il problema più chiaro di cui nessuno parla

<p align="center"><img src="assets/cover-1200x675.webp" alt="Due persone su un divano, una al portatile e una che legge, entrambe occupate, mentre un elefante enorme con una maschera di Guy Fawkes siede nella stanza alle loro spalle senza che nessuno lo nomini." width="680"></p>

Chiunque abbia seguito un corso di progettazione di protocolli ha incontrato il
principio di Kerckhoffs più o meno alla seconda settimana. È quello che sanno
recitare tutti. E questa comunità, capace di discutere sei ore se il generatore
casuale di un wallet sia affidabile, consegna difese contro la coercizione fisica
costruite sulla sicurezza tramite oscurità, e falliscono alla prima pagina del
manuale.

Niente di sottile. Lo dicono i manuali stessi, e questo pezzo è quasi soltanto
citarli.

## Cosa dice davvero Kerckhoffs

Lascia perdere il gergo. Un sistema deve restare sicuro quando l'attaccante sa
esattamente come funziona. Tutto tranne la chiave è pubblico: il progetto, il
software, la procedura, il fatto che la procedura esista. Un progetto si giudica
da come si comporta contro qualcuno che ha letto la stessa documentazione che hai
letto tu.

Non è pessimismo sugli attaccanti. È un'ammissione sulla pubblicazione. Nel
momento in cui una difesa arriva al pubblico, la sua descrizione sta in un
articolo di assistenza, nella lingua dell'attaccante, indicizzata, gratis.

### La sicurezza tramite oscurità ha un numero di catalogo

La famiglia di tattiche che infrange questa regola ha un nome e un numero di
fascicolo. *Reliance on Security Through Obscurity*, catalogata come
[CWE-656](https://cwe.mitre.org/data/definitions/656.html). In qualunque altro
ambito del software quella voce è un difetto da correggere. Nella custodia di
bitcoin è la raccomandazione condivisa.

E questo paradigma, che la progettazione di protocolli chiama **oscurità**, è
intrinsecamente condiscendente. Presuppone che il ladro non sia mentalmente in
grado di leggere gli stessi manuali, guardare gli stessi tutorial e seguire gli
stessi corsi delle sue vittime. Se una procedura si impara su internet, la impara
anche un ladro, e saprà di sicuro che la procedura esiste.

Punta all'assunto, non a chi lo sostiene. Le persone che consegnano queste
funzioni sono ingegneri scrupolosi che hanno sbagliato una premessa. Si dà il
caso che sia quella che regge tutto il resto.

## Tre scommesse su cosa crederà un attaccante

Il consiglio corrente arriva in tre parti: tieni in silenzio, nega se te lo
chiedono, tieni qualcosa di piccolo da consegnare. Riscrivile senza il tono
rassicurante e sono tre scommesse sullo stato mentale di un avversario. Non tre
controlli. Tre congetture su cosa penserà qualcun altro, fatte da chi ha meno
modo di verificarlo.

Un controllo funziona quando l'attaccante ne è al corrente. La distinzione è
tutta lì, e ogni meccanismo qui sotto fallisce da quel lato.

## La classe, nelle parole dei produttori stessi

Citerò la documentazione invece di caratterizzarla, perché la classificazione fa
il lavoro da sola e caratterizzarla invita una discussione sulle intenzioni di
cui nessuno ha bisogno.

### Il PIN che cancella, e il backup che dà per scontato

Il Jade di Blockstream ha un PIN alternativo che, nelle parole del centro
assistenza, "automatically delete[s] the encrypted wallet information from Jade
if entered". Viene presentato come "especially useful in the event of a physical
threat, as you can provide this PIN to an attacker". Lo digiti e il dispositivo
riporta solo "Internal Error", così la cancellazione si legge come un guasto e
non come una decisione.

Va dato atto: la cancellazione in sé è reale, istantanea e non interrompibile.
Non c'è nessuna corsa da vincere.

Ora leggi l'avvertenza successiva sulla stessa pagina. Dopo "there is no way to
regain access to your funds except by restoring using your recovery phrase",
quindi il detentore deve "make sure you have a backup before proceeding".

La funzione presuppone un backup. Chi segue la documentazione ce l'ha; chi non la
segue ha distrutto i propri risparmi sotto pressione. Quindi quello che la
cancellazione rimuove non è il segreto. Rimuove il percorso *del dispositivo*
verso il segreto, e lascia in piedi quello che passa per il ricordo che la
persona ha di dove si trova il backup.

La cancellazione elimina la strada che non obbligava a fare male a nessuno, e
tiene quella che ci obbliga.

### Coldcard documenta la regressione

Non devi dedurre tu il passo successivo. L'ha pubblicato un produttore.

Coldcard offre PIN trabocchetto, fra cui un wallet di coercizione descritto come
"a personal safety feature… If you must reveal a PIN under duress, give the
duress PIN instead of your Main PIN". Logica dell'esca, normalissima. La
documentazione del firmware poi considera cosa succede quando l'esca non viene
creduta, e il consiglio è di alzare il tiro: "you may be asked what the actual
duress PIN is, while under duress. We suggest providing the 'brickme' PIN in that
case."

È un produttore che contempla un attaccante consapevole che le esche esistono, e
raccomanda una cancellazione irreversibile eseguita con la vittima ancora nella
stanza, ancora viva, ancora a disposizione per farsi chiedere dov'è il backup.

Altre due ammissioni sulla stessa pagina meritano la citazione perché i
produttori le fanno di rado. La prima concede che l'esca è distinguibile: "if you
are somehow facing an attacker who is willing to verify he has the real main PIN,
it's possible that careful analysis of system responses will imply he's working
with the duress PIN." Il rimedio offerto non è una riparazione. È una richiesta:
"if you discover any sequences that reveal this easily, please tell us and we'll
see if we can cover them up better."

Sicurezza tramite oscurità enunciata come programma di manutenzione. Quello che si sta difendendo
non è che l'esca sia indistinguibile, ma che nessuno abbia ancora pubblicato come
distinguerla. Uno schema la cui sicurezza è lo stato attuale della coda delle
divulgazioni è uno schema che non puoi invocare nella stanza, perché non hai idea
di cosa abbia letto l'uomo che ti sta davanti.

La seconda ammissione è la smentita stessa, proposta dove mattonare il
dispositivo risulta indigesto: "alternatively, you can say you set the duress PIN
once, but have since forgotten it."

Non puoi dimostrare di aver dimenticato. È tutto il paper gemello in cinque
parole, ed eccolo come indicazione pubblicata. Il produttore ha enumerato i rami
e ha trovato un bluff su ciascuno.

### Cosa afferma davvero ciascun produttore

Questo conta, ed è il punto in cui sbaglia gran parte delle critiche di questo
tipo. Le tre aziende non fanno le stesse affermazioni, e un produttore che
consegna un meccanismo senza sostenere che sconfigge la coercizione non ha
commesso l'errore di cui parla questo pezzo.

Blockstream vende la cancellazione per la minaccia fisica, e non afferma nulla di
simile per i suoi wallet con passphrase. L'inquadramento anti-coercizione delle
esche per passphrase è un'invenzione della comunità, non del produttore. Coldcard
vende entrambe le metà. Trezor è l'immagine speculare di Blockstream: i suoi
wallet con passphrase sono venduti sulla negabilità, mentre il wipe code, che il
produttore stesso chiama PIN di "self-destruct" e che cancella il seme di
recupero, è documentato senza alcun accenno a coercizione, costrizione o minaccia
fisica.

Trezor è anche quella a cui è stato chiesto, nel gennaio 2022, di rendere la
cancellazione *dissimulabile*: un messaggio definito dall'utente all'inserimento,
così che una cancellazione potesse passare per un guasto hardware. La richiesta è
stata chiusa come **not planned**. Il dispositivo annuncia ancora la
cancellazione apertamente.

Quel rifiuto è il documento più interessante di tutta la classe. Mostra che il
travestimento da "Internal Error" non è intrinseco alla cancellazione. È una
scelta di presentazione: un produttore l'ha costruita, a un altro è stata chiesta
direttamente e ha detto di no.

### Un'ignoranza, o due

C'è un modo pulito di ordinarli, e non è per quanto è probabile che l'attaccante
sia ignorante. È per quante cose distinte deve ignorare.

Un'esca ne richiede una. Non deve sapere che le esche esistono. Concediglielo e
l'esca funziona davvero: se ne va con un saldo plausibile e una storia che
chiude.

Un'autodistruzione ne richiede due, e sono indipendenti. Non deve sapere che la
funzione esiste, così il fallimento si legge come guasto. E non deve arrivare per
ragionamento al backup, che il manuale ha detto al detentore di conservare. La
seconda non discende dalla prima. «Questo dispositivo è rotto» non ha mai
implicato «questa persona non ha bitcoin». Implica che lo strumento è rotto, e la
domanda naturale successiva è dove tieni il backup, rivolta a qualcuno che è
ancora lì in piedi.

Quindi contro un attaccante informato l'autodistruzione fallisce per l'ordinaria
ragione kerckhoffsiana, e contro uno ignorante fallisce lo stesso, perché la
convinzione che fabbrica non chiude l'incontro. È l'unico schema oscuro che non
ha alcun ramo in cui vince.

<p align="center"><img src="assets/m1-one-ignorance-or-two.png" alt="Un'esca richiede che l'attaccante ignori una cosa. Un'autodistruzione richiede che ne ignori due, in modo indipendente, e non ha alcun ramo in cui vince." width="680"></p>

C'è una versione più silenziosa dello stesso fallimento. La FAQ di Sparrow
documenta un'opzione per tenere i dati del wallet su supporti rimovibili, notando
che "allows you to store all Sparrow data on removable media making for more
plausible deniability". La pagina di buone pratiche di Sparrow, dal canto suo,
tiene le parole del seme salvate a parte, "ideally in a different location".
Quindi l'attaccante estorce il backup del seme, lo carica nel proprio wallet, e
non tocca mai il supporto nascosto. Un'esca almeno si mette fra lui e le monete.
Questa non ci si avvicina nemmeno, e quello che aggiunge è la sicurezza per
sostenere una smentita.

## Ottantotto persone, dodici casi

La classe presuppone un avversario che gli atti dicono non esistere.

La procura francese ha incriminato 88 persone in una dozzina di casi di sequestro
ed estorsione legati alle cripto, che è un conteggio a un dato istante di una
serie di procedimenti in corso e non un totale chiuso. Il conteggio di CertiK per
il primo semestre 2026 porta le invasioni domiciliari da 1 a 20 su 52 episodi
anno su anno, che è il campione semestrale di un'azienda e non il registro
pubblico, quindi leggi la direzione e non il decimale.

Dovunque si assestino le cifre esatte, descrivono squadre organizzate con
ricognizione e selezione delle vittime basate su banche dati trafugate. Non
opportunisti incapaci di leggere una pagina di assistenza nella lingua in cui è
stata scritta.

## L'effetto boomerang

La sicurezza tramite oscurità non è soltanto inefficace. Venduta su scala si sconfigge da sola, e
chi ne esce peggio non ha comprato niente.

L'esca non è solo una pratica tollerata. È un prodotto ed è un programma
didattico. Una consulenza di autocustodia in lingua spagnola elenca fra i suoi
livelli a pagamento "*Passphrase (tu bóveda señuelo)* — Billetera señuelo +
billetera real. Protección ante coacción/coerción": un wallet esca
commercializzato, a lettere chiare, come protezione contro la coercizione. Ci
sono guide pubblicate che addestrano la recita. Una dice al detentore di tenere
un saldo piccolo sul seme nudo come ciò che consegneresti sotto coercizione
fisica, aggiungendo che «perché funzioni, il saldo esca deve essere *credibile*:
abbastanza da sembrare un wallet vero, non abbastanza da devastarti se lo
perdi».

Leggilo come obiettivo formativo e il problema salta fuori. Un'esca deve essere
credibile solo davanti a un attaccante che potrebbe non crederci, e il consiglio
tace su cosa succede quando non ci crede, che è tutta la domanda. La sicurezza
tramite oscurità qui viene venduta come se fosse un controllo, con un prezzo e un
corso.

### La smentita è un bene comune, e lo stiamo prosciugando

L'addestramento pubblicizzato alza la probabilità a priori che una smentita
fluida sia stata provata. Una volta che l'attaccante sa che la credibilità si
insegna e si vende, la scioltezza smette di essere prova di verità e diventa
prova di coaching. Il rimedio degrada la cosa che vende.

E la degrada per tutti. Chi non si è mai addestrato, chi sta dicendo la verità
nuda, adesso nega davanti a un attaccante che sconta le smentite fluide in
generale. Lo stesso vale per chi non ha alcun bitcoin. Lo sviluppo completo sta
in *The Denial Spiral*, ed è il motivo per cui questa serie tratta l'oscurità
come un problema di salute pubblica e non come un problema personale.

Nascondersi ha bisogno di un posto in cui nascondersi. Ciò dentro cui sparisce un
detentore discreto è l'enorme folla di persone che visibilmente non hanno
bitcoin, e funziona solo finché la folla è in prevalenza genuina. Addestra
abbastanza gente a presentarsi come ordinaria e l'ordinario smette di portare
informazione, perché l'attaccante non sta più separando chi detiene da chi no. Se
sono tutti aghi, non c'è pagliaio.

<p align="center"><img src="assets/m2-no-hay.webp" alt="Un mucchio di aghi da cucito su fondo bianco, e nient'altro che aghi nel mucchio." width="612"></p>

<p align="center"><em>Strutturale, non misurato. Nessuno ha contato quanti
detentori pratichino la discrezione, e per il meccanismo 1 nessuno può farlo:
l'oscurità non si annuncia. L'affermazione riguarda cosa succede alla folla man
mano che l'addestramento si diffonde, non dove sia la folla oggi.</em></p>

## Un progetto pubblico rende più credibile una smentita ordinaria

Un'ultima inversione, ed è la parte che trovo davvero sorprendente.

Una difesa oscura chiede all'attaccante di credere a un'affermazione, contro il
suo interesse a non crederci e senza alcun modo, per nessuno dei due, di
dirimere la questione. Un progetto specificato pubblicamente cambia quanto costa
fare quell'affermazione. Un attaccante che dà credito alla circolazione di
meccanismi efficaci sta dando credito al fatto che mentire non sia l'unico
strumento a disposizione della vittima, e un detentore con alternative vere ha
meno motivi per ricorrere a una bugia.

Così un progetto pulito secondo Kerckhoffs migliora la posizione proprio di
quelle smentite oscure che era stato costruito per rendere inutili. La sicurezza
tramite oscurità resta infondata come difesa primaria. Non è indifferente a quale
progetto accompagni.

---

*La classificazione, la documentazione dei produttori e l'argomento del bene
comune sono sviluppati in*
[***The Denial Spiral***](https://zenodo.org/doi/10.5281/zenodo.22778480)*, accesso
aperto, senza registrazione. Il suo gemello,*
[***The Deadly Race***](https://zenodo.org/doi/10.5281/zenodo.22018891)*, riguarda cosa
succede una volta che l'attaccante è già nella stanza: un sequestro che lascia un
percorso praticabile ma incompiuto trasforma una rapina in una corsa, e mette un
prezzo sulla tua eliminazione.*

*Ogni citazione di produttore qui sopra viene da documentazione pubblica,
collegata nel paper. Se ho letto male una funzione, o se una pagina è cambiata,
dimmelo e correggo in pubblico.*

---

**Se è valso il tuo tempo.** Mandalo a qualcuno che consegna un PIN di
coercizione. Una ⭐ su [Great Wall](https://github.com/Yuri-SVB/Great-Wallet),
sulla [ricerca](https://github.com/Yuri-SVB/great-wall-docs) o su
[questi testi](https://github.com/Yuri-SVB/great-wall-posts) non ti costa nulla e
rende il lavoro trovabile. E se vuoi finanziarlo,
[support](https://github.com/Yuri-SVB/support) accetta ⚡ Lightning e on-chain,
senza registrazione, senza livelli e senza nulla in cambio.
