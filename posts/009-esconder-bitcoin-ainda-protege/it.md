---
id: 009
titolo: "Nascondere i tuoi bitcoin ti protegge ancora?"
sottotitolo: "Il Brasile ha la peggiore statistica al mondo per il tipo di attacco in cui nascondersi non serve, e il mercato continua a vendere nascondigli."
lingua: it
autore: Yuri da Silva Villas Boas
papers: [DS, DR]
tempo_di_lettura: ~7 min
traduzione_di: pt-BR.md
copertina: assets/capa-1200x675.webp
copertina_alt: "Un uomo alza un setaccio per coprire il sole, e la luce passa attraverso la rete. È il modo di dire brasiliano per nascondere ciò che è già sotto gli occhi di tutti."
---

# Nascondere i tuoi bitcoin ti protegge ancora?

<p align="center"><img src="assets/capa-1200x675.webp" alt="Un uomo alza un setaccio per coprire il sole, e la luce passa attraverso la rete. È il modo di dire brasiliano per nascondere ciò che è già sotto gli occhi di tutti." width="680"></p>

**Il consiglio standard, per chi teme di essere rapito a causa dei suoi bitcoin,
arriva in tre parti: non dirlo a nessuno, nega se te lo chiedono, e tieni un
*decoy* da consegnare.**

**Tutte e tre sono scommesse su quello che il criminale *crederà*. E nessuna è
mai stata valutata per quello che è: un meccanismo di sicurezza la cui forza
dipende interamente dall'ignoranza dell'avversario.**

Questo testo sostiene che nascondere bitcoin non è soltanto inefficace. È
**autodistruttivo su scala**, e il conto arriva a persone che quel consiglio non
l'hanno mai seguito.

---

## Nascondere bitcoin ha un nome, un numero e dei precedenti

Prima il vocabolario.

Un *decoy*, o portafoglio-esca. In Brasile lo chiamiamo «i soldi del rapinatore»,
e lo conosciamo bene: una somma più piccola, messa da parte apposta per essere
consegnata durante una rapina.

Nell'ingegneria della sicurezza l'intera famiglia di queste tattiche è
catalogata. Si chiama *Reliance on Security Through Obscurity*, registrata come
[CWE-656](https://cwe.mitre.org/data/definitions/656.html). In qualsiasi altro
ambito è un difetto di progettazione. Nella custodia di bitcoin è il consenso.

### Nascondere bitcoin è condiscendente per costruzione

Questo paradigma, che nella progettazione di protocolli si chiama **oscurità**, è
intrinsecamente condiscendente. Dà per scontato che il ladro non sia mentalmente
in grado di leggere gli stessi manuali, guardare gli stessi tutorial e seguire
gli stessi corsi delle sue vittime.

Se una procedura puoi impararla su internet, può impararla anche un ladro. E di
sicuro saprà che la procedura esiste.

---

## Il Brasile sta nel quadrante peggiore del registro

Jameson Lopp tiene da anni un [registro pubblico degli attacchi fisici ai
detentori di bitcoin](https://github.com/jlopp/physical-bitcoin-attacks), i
cosiddetti «attacchi con la chiave inglese». Ho codificato per modalità tutti i
351 incidenti del registro. La distribuzione per paese non è affatto
uniforme: varia di un ordine di grandezza.

| Giurisdizione | Incidenti | Sequestro | Rapina a mano armata | Rapporto S:R |
|---|---:|---:|---:|---:|
| **Brasile** *(n piccolo)* | 12 | 75,0 % | 8,3 % | **9,0** |
| Francia | 61 | 57,4 % | 8,2 % | 7,0 |
| *Tutti gli incidenti* | 351 | 35,0 % | 22,8 % | 1,5 |
| Stati Uniti | 59 | 20,3 % | 33,9 % | 0,6 |
| Russia *(n piccolo)* | 10 | 30,0 % | 50,0 % | 0,6 |

### Nove sequestri per ogni rapina

Guarda la colonna a destra. Negli Stati Uniti l'attacco tipico è una rapina:
arma puntata, trasferimento immediato, pochi minuti sul posto.

In Brasile la proporzione si ribalta. **Per ogni rapina a mano armata registrata,
nove sequestri.** L'attacco brasiliano non è un evento di minuti. È un evento di
ore o di giorni, con la vittima sotto il controllo del criminale per tutto il
tempo.

### L'avvertenza arriva insieme, ed è seria

Il registro è un campione di stampa, l'`n=12` del Brasile da solo non regge
nulla, e la codifica è per parola chiave nel titolo, non per durata misurata.
Prendi la riga del Brasile come indicativa.

Il confronto che pesa davvero è Francia contro Stati Uniti: due sottoinsiemi
della stessa dimensione (61 e 59) con composizioni invertite. La composizione
varia eccome con le condizioni locali, e quelle brasiliane le conosce chiunque
viva qui.

Tutto questo conta perché **l'intera promessa del nascondere bitcoin dipende dal fatto
che l'attacco sia breve**. Un decoy funziona se il criminale prende gli 8.000
real e se ne va. Non ha nessuna risposta alla domanda successiva, posta il terzo
giorno, in prigionia.

---

## Cosa succede quando tutti sono addestrati a negare

Ecco il meccanismo, ed è economico prima che crittografico.

### La credibilità di una smentita è una risorsa comune

È prodotta dall'insieme di tutti i detentori e consumata da ciascuno che nega.
Finché negare è raro, negare porta informazione: il criminale aggiorna la sua
convinzione e le tue probabilità di essere rilasciato salgono.

Quando negare diventa il copione atteso, quando ogni canale, ogni corso, ogni
gruppo Telegram insegna la stessa frase, **una smentita smette di portare
informazione**.

Un interrogatorio che si apre con «non ho niente» non dà al criminale nessun
aggiornamento a tuo favore. E la sua prosecuzione razionale, a quel punto, non è
rilasciarti. È insistere.

La risposta individualmente razionale a questo ambiente è nascondersi meglio e
provare di più. Il che **esaurisce ulteriormente la risorsa, per tutti**.

L'ho chiamata **Spirale della Smentita**, e il suo costo è una classica
esternalità: ricade su chi ha bisogno di essere creduto. Compreso chi usa un
assetto che non dipende dal mentire. Compreso chi, onestamente, **non ha bitcoin
affatto**, e nel registro casi così ci sono.

### Il mercato vende l'esaurimento come prodotto

Diverse consulenze, corsi e tutorial di autocustodia elencano, tra i servizi a
pagamento, la costruzione di decoy con addestramento alla credibilità.

Quindi: si paga per diventare fluenti in una smentita che il criminale già
sconta, proprio perché viene insegnata e venduta. Il rimedio degrada la cosa
stessa che vende, e non solo per il cliente.

---

## Il problema più grave: non puoi dimostrare di aver dimenticato

C'è un secondo cedimento, ed è peggiore, perché riguarda l'esito e non la durata.

Parti da un fatto semplice e inaggirabile: **nessuno può dimostrare di non sapere
qualcosa.** Sapere è dimostrabile; *non* sapere no. Non hai modo di dimostrare di
aver dimenticato la passphrase, né che non esista un backup da nessuna parte.

### La Corsa Mortale

Considera ora un qualsiasi schema che, dopo il sequestro del tuo dispositivo,
lasci al criminale un percorso **praticabile ma incompiuto** verso il denaro: un
timelock, un recupero in mano a un delegato, una cassaforte a ritardo, una chiave
ancora da forzare.

Ti rilasciano. E non puoi dimostrare di non aver conservato una copia usabile.

Quello che esiste da lì in avanti è una **corsa** tra te e lui per lo stesso
saldo. E una corsa contro un concorrente a portata di mano crea qualcosa che
nessun whitepaper di portafoglio menziona: **un incentivo materiale a
eliminarti.** Non per crudeltà. Per aritmetica. Togliere l'altro corridore dalla
pista è la mossa più economica disponibile.

L'ho chiamata **Corsa Mortale**. Nel registro, almeno il 4,6 % degli incidenti (16
su 351) riporta una vittima uccisa, e quella cifra è un **pavimento**, non una
stima: un omicidio tende a essere riportato come omicidio, non come «attacco a un
detentore di bitcoin». L'esito che l'argomento prevede è documentato nei fatti.

### Perché il decoy è una macchina da zona grigia

Il criterio di progettazione che ne esce è secco: **uno schema di custodia
resistente alla coercizione può ammettere solo due esiti. L'attacco riesce
chiaramente, o l'attacco fallisce chiaramente. Mai una corsa.**

La zona grigia è esattamente dove vive l'incentivo all'omicidio. L'ho chiamato
**Principio di Assenza di Zona Grigia**.

Guarda cosa fa questo al decoy. È, per costruzione, una macchina da zona grigia:
il criminale se ne va sospettando che ci sia dell'altro, senza alcun modo di
chiudere il sospetto. È il posto peggiore in cui stare.

---

## Un caso brasiliano che chiude l'argomento

Porto Velho, ottobre 2019. Una banda sequestra
[Arcilio Nogueira de Souza](https://archive.is/jyzcJ), lega la vittima a un
albero e la picchia per ore. I criminali **non hanno portato via nulla**: il
telefono non dava accesso ai fondi.

Quel caso è l'argomento intero in un paragrafo. L'inaccessibilità dei fondi *non
ha posto fine all'attacco*. Lo ha **prolungato**.

Lo schema ha «funzionato» nel senso in cui l'industria lo misura, i soldi non si
sono mossi, e la persona ha passato ore legata a un albero a prenderle, perché
fuori dalla sua testa non c'era niente che potesse chiudere il dubbio del
criminale.

È per questo che tengo separati i due meccanismi. La Corsa Mortale prezza
l'**esito**. La Spirale della Smentita prezza la **durata**. Un assetto può
essere innocente dell'uno e colpevole dell'altro, e la maggior parte di ciò che
si vende oggi è colpevole di entrambi.

---

## Cosa resta, se nascondere bitcoin non è una difesa

Restano tre strade oneste, e conviene sapere su quale ci si trova.

### 1. Fisica

Dispersione geografica, caveau, multisig con custodia lontana. Funziona, e riduce
la sicurezza del bitcoin a «quanto è buono il caveau». Il bitcoin diventa **oro
con passaggi in più**, a un costo che cresce con la difesa. Per la stragrande
maggioranza è fuori portata.

### 2. Delegata

Qualcuno fuori dalla portata del criminale tiene il pezzo mancante: un exchange,
una cocustodia, un recupero tramite terzi. Soddisfa il criterio, ma cambia la
premessa: la custodia smette di essere individuale. *Not your keys.* E la strada
si **chiude** se il delegato abita vicino a te.

### 3. Tacita

Il segreto non è mai stato sul dispositivo, e non può essere dettato nemmeno
sotto tortura, perché è riconoscimento percettivo e non una frase. Sequestrare
l'hardware non consegna niente di praticabile. **Fallimento chiaro**, nessun
corridore di troppo, custodia ancora individuale.

La terza strada è quella su cui lavoro, e il progetto si chiama **Great Wall**.
Ecco l'avvertenza che qualsiasi testo onesto in materia deve portare:
**l'implementazione è un prototipo. Non metterci ancora dietro i tuoi
risparmi.**

Quando cambierà sarà scritto, con la data, in
[`DELIVERED.md`](https://github.com/Yuri-SVB/support/blob/main/DELIVERED.md), un
file tenuto in git proprio perché «il lavoro sta procedendo» sia un'affermazione
verificabile e non una promessa.

### L'effetto collaterale controintuitivo

Questa strada ha un bell'effetto collaterale: **un progetto pubblico e non oscuro
migliora la posizione di chi nega.**

Un criminale che crede che sia in circolazione un meccanismo efficace sta
credendo che mentire non sia l'unico strumento a disposizione della vittima. E
una vittima con un'alternativa vera ha meno motivi per mentire.

Nascondersi resta pessimo come difesa primaria. Ma quale assetto accompagni non è
affatto indifferente.

---

## Cosa vendo, e cosa non vendo

**Non vendo software.** Great Wall, BTC-D20, BIP-450 e i paper sono MIT o
Apache-2.0, e questo non cambia: nessuna versione «pro», nessuna funzione
sbloccata a pagamento, nessuna corsia preferenziale per chi ha donato.

È scritto nel [repository di supporto](https://github.com/Yuri-SVB/support), ed è
scritto lì perché una promessa in un articolo non vale niente e una promessa in
git ha una data.

### Vendo invece consulenza di autocustodia

È un servizio, ed è questo: guardo l'assetto che hai già, portafoglio hardware,
passphrase, multisig, decoy, piano di successione, quel che c'è, e rispondo a
quattro domande in un rapporto riservato:

1. La tua sicurezza si regge su un **trucco segreto**? Dipende dal fatto che
   l'aggressore non sappia cosa fai, e come lo fai?
2. Una volta sequestrati i tuoi dispositivi e i tuoi segreti, l'aggressore
   potrebbe spendere **subito**, o solo **dopo un po'**? «Dopo un po'» vuol dire
   che sei ancora un corridore.
3. La tua custodia è **strettamente individuale**? Qualcun altro può fare
   qualcosa che ti impedisca di arrivare alle tue monete?
4. Dipende da **oggetti precisi in luoghi precisi**? E quei luoghi sono tuoi?

Non è vendita di un prodotto: nella maggior parte degli audit la raccomandazione
è sistemare quello che c'è già, e in alcuni il verdetto è che è ragionevole.
Quello che non farò è costruire un decoy con addestramento alla smentita, per
l'intero argomento qui sopra.

Contatto: **yuri@t3infosecurity.com**.

### E se non vuoi comprare niente

I paper sono gratuiti e non stanno dietro nessuna registrazione:
[*The Deadly Race*](https://zenodo.org/doi/10.5281/zenodo.22018891) (la corsa e il
criterio) e [*The Denial Spiral*](https://zenodo.org/doi/10.5281/zenodo.22778480) (la
spirale, la classificazione dei prodotti oscuri sul mercato, e il metodo di
codifica del registro).

I nuovi dati sugli incidenti vanno al [registro di
Lopp](https://github.com/jlopp/physical-bitcoin-attacks) e non in un database
mio, perché quell'informazione è un bene pubblico e appartiene a tutti, compreso
il prossimo bersaglio.

Se è servito, [il supporto sta qui](https://github.com/Yuri-SVB/support).
Lightning e on-chain, senza nulla in cambio e senza registrazione.

---

*Yuri da Silva Villas Boas è un crittografo applicato, autore della BIP-450
(Formosa) e del protocollo Great Wall. Le due affermazioni centrali di questo
articolo sono sviluppate formalmente nei paper citati, attualmente in valutazione
accademica.*
