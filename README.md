# Hinotech Software — il sito della casa madre

Avvio: 17/11/2026. Pagine di progetto (si aprono nel browser, con internet: 3D e caratteri vengono dalla rete):

- [`design/home.html`](design/home.html): **la home di adesso** (18/11). Si apre con un tunnel: la frase al centro, attorno i cinque principi, ognuno con il suo simbolo moldavo o giapponese; alla fine la frase diventa una maschera sulla pagina chiara, in stile linear.app. La grafica sta sulla tela Claude Design «Hinotech · deschiderea» (https://claude.ai/artifact/95NipTVRzS7wjLaswWmKFp, privata); il ritmo compatto del 19/11 sta sull'altra tela con lo stesso nome (https://claude.ai/artifact/7VHuB1hZBpUND2eoWt5W32, tavola «Tunelul · ritm compact (19/11)»).
- [`design/apertura.html`](design/apertura.html), [`design/home-otel.html`](design/home-otel.html), [`design/home-fereastra.html`](design/home-fereastra.html): le prove del 18/11 da cui è nata la home.
- [`design/sat.html`](design/sat.html): il villaggio di notte (17–18/11), messo da parte il 18/11.
- [`design/proposte.html`](design/proposte.html): le tre proposte da cui è stata scelta (A villaggio, B cantiere di hinoki, C corte coreana).
- [`design/tempio.html`](design/tempio.html) e [`design/direzioni.html`](design/direzioni.html): il primo tentativo (il tempio), messo da parte il 17/11.

Repository git proprio, privato su GitHub (`CristiPerciun/Hinotech_Software_sito`, ramo `main`), escluso da
Brainstorming con `.git/info/exclude`.

## Che cosa è

Il sito della casa madre del Dossier Strategico §2.6: chi siamo, principi, portafoglio (PrivacyBox
come primo prodotto, «un prodotto di Hinotech Software»), sicurezza e conformità, lavora con noi,
contatti istituzionali. **Nessun prezzo di prodotto**: i prezzi stanno sui siti di prodotto.
Chi lo legge: ODA, banche, partner istituzionali, futuri collaboratori, investitori.

## Vincoli

- **Il nome va online solo dopo il deposito del marchio all'AGEPI** (§2.6: il marchio si deposita
  prima di annunciare il nome). Fino ad allora il sito resta su questo PC.
- Domini: `hinotech.md` e `hinotechsoftware.com` (`hinotech.com` è preso). Si scrive sempre
  «Hinotech Software», in due parole.
- È la casa madre di un prodotto di privacy, quindi il sito dà l'esempio: nessun tracker, nessun
  cookie non necessario (quindi nessun banner), font e librerie serviti dal nostro dominio (niente
  Google Fonts né CDN in produzione), CSP e intestazioni di sicurezza severe.
- Lo scroll resta quello del browser: niente scroll dirottato. La morbidezza la mettiamo negli
  oggetti (seguono lo scroll con un piccolo ritardo), non nella pagina.
- Con `prefers-reduced-motion` ogni scena si ferma sul suo stato finale; il testo si legge anche
  senza nessuna animazione.
- Caratteri con i segni del romeno (ș, ț con la virgola sotto, ă, â, î) e il cirillico per il russo.

## Un'opera, con pochi elementi

Il founder, 17/11: il sito dev'essere un'opera d'arte, con le regole del design professionale, il
fuoco sulle cose importanti, pochi elementi grafici ma fondamentali. Nel tempio gli elementi sono
sei, e non se ne aggiungono altri:

1. **La carta** (`n-000`, con la sua grana): il fondo di tutto.
2. **L'inchiostro** al 30 %: il disegno di ciò che è progetto.
3. **Il legno di hinoki**, fotografato dal vero: ciò che esiste.
4. **Un solo accento**, il colore della corteccia di hinoki (`rust` #9C4A38): il tetto del primo
   piano e il sigillo 檜.
5. **Due caratteri**: Cormorant Garamond per le frasi, IBM Plex Sans per il resto (con Plex Mono per
   le etichette e Plex Sans JP per i segni giapponesi).
6. **Una frase per schermata**, con un'etichetta e una riga di spiegazione: tre livelli, mai di più.

## Il concept: hinoki 檜

Il nome viene dalle proposte del 7/11 («cultura giapponese, semplicità, bellezza minimale,
affidabilità»): **hinoki**, il cipresso dei templi, il legno chiaro che non marcisce. Il sito racconta
il software come lavoro di falegnameria: pezzi precisi che si incastrano senza chiodi, fatti per
durare e per essere mantenuti.

| Principio | Giapponese | Coreano | Sul sito |
|---|---|---|---|
| Lo spazio vuoto | 余白 *yohaku* | 여백 *yeobaek* | un'idea per schermata, molto margine |
| La semplicità | 簡素 *kanso* | | si toglie finché resta l'essenziale |
| Il mestiere | 匠 *takumi* | | il dettaglio curato anche dove nessuno guarda |
| La durata | 檜 *hinoki* | | si costruisce per decenni, si mantiene come un tempio |

## Il tempio: la pagoda a cinque piani (五重塔)

La direzione A, scelta il 17/11, diventa una **pagoda a cinque piani in hinoki** con il suo
pilastro centrale (心柱, *shinbashira*). La struttura della pagoda è la struttura della SRL: **un
motore, molti prodotti** (Dossier §2.4). All'apertura il tempio è tutto disegnato a inchiostro: è il
progetto. Mentre scorri si costruisce in legno ciò che esiste già; ciò che verrà resta disegno.

| Parte del tempio | Che cosa è per Hinotech | Stato nella scena | Fonte |
|---|---|---|---|
| 基壇 la base di pietra | la semplicità: per ogni problema la soluzione più semplice che funziona, spiegata con chiarezza | pietra vera | il founder, 17/11 («tecnologia e semplicità, chiarezza») |
| 心柱 il pilastro centrale | il motore comune: clienti, ruoli, versioni, registri, termini, giornale | legno, attraversa tutti i piani | Dossier §2.3, principio 5; §2.4 |
| 初重 il primo piano | PrivacyBox, il primo prodotto, online dal 3/10/2026 | legno, con il tetto di corteccia | dosar ODA §1 e §6 |
| 柔構造 i piani che oscillano | costruiti per cambiare: leggi nuove, clienti nuovi, dispositivi nuovi, dallo stesso codice | scossa: i piani ondeggiano, il pilastro resta fermo | dosar §3, «Pe orice dispozitiv, din același cod» |
| 二重 il secondo piano | il prossimo prodotto | legno, senza tetto: in costruzione | Dossier §2.4 (oggi: la sicurezza sul lavoro, con i corsi; sul sito senza nome) |
| 三重–五重 i piani alti | i prodotti che verranno | inchiostro: progetto | Dossier §2.4 (candidati: antiriciclaggio, personale, e-Factura; sul sito senza nome) |
| 木組み l'incastro senza chiodi | la prova prima della promessa: test a ogni rilascio, dati di ogni cliente isolati, risultati verificabili da chiunque | primo piano ravvicinato sulle mensole | Dossier §2.3, principio 3; dosar §3 |
| 相輪 la guglia | pezzo per pezzo: ciò che esiste è di legno, ciò che verrà è disegno | inchiostro, si disegna per ultima | la scena stessa; Dossier §2.4, la regola di ammissione |

## Il paesaggio: i Codri, a inchiostro

Il founder, 17/11: un paesaggio moldavo famoso, ma molto minimale, come le sue tre immagini di
riferimento (un campo unico di texture, un solo elemento rosso). La scelta sono **i Codri**:
le colline di bosco del centro della Moldova, il paesaggio più noto del paese insieme a Orheiul
Vechi. Orheiul Vechi è scartato: è un monastero ortodosso, e una pagoda lì sarebbe fuori luogo.
I Codri tengono insieme il legno del tempio e il bosco moldavo; «Codru» era anche una delle idee
di nome del Dossier §2.6, perché contiene «cod».

Come è fatto, con pochi elementi:
- **il colle**: un prato verde salvia, pallido, con la radura del tempio;
- **cinque creste di bosco** dipinte a inchiostro diluito, sempre più chiare con la distanza, che
  sfumano nella carta come in un paravento giapponese (non alberi in 3D: un primo tentativo con
  migliaia di chiome sembrava un videogioco);
- **la nebbia** nelle valli, che scorre appena con lo scroll;
- **un solo rosso**: il tetto di corteccia del primo piano, come la barca e l'albero delle immagini
  di riferimento.

**La camera** (il founder, 17/11: «non ingrandirei e allontanerei 3 volte, al massimo una volta,
zoom molto più lento e meno aggressivo»): un solo avvicinamento, dal paesaggio intero al tempio,
sui primi due terzi dello scroll, con la distanza che cala in modo uniforme all'occhio; poi solo
un giro leggero intorno al tempio. Nessun primo piano.

## Le parole del sito

**La regola**: ogni frase del sito viene da un fatto o da una decisione scritta nei documenti, o da
una parola del founder, e qui accanto c'è la fonte. Se una frase non ha una fonte, non si scrive.

**Il founder, 17/11**: Hinotech Software è un'azienda che fa soluzioni software; le frasi di un
prodotto (il «dosar viu» di PrivacyBox) non stanno nella prima pagina della SRL. Le frasi del tempio
parlano dell'azienda; PrivacyBox compare solo come primo piano.

| # | Etichetta | Frase | Riga | Che cosa vuol dire |
|---|---|---|---|---|
| 0 | | Soluții software simple, clare, făcute să dureze. | O firmă tehnologică din Republica Moldova, cu produse în română și în rusă. | Chi siamo, con le parole del founder (soluzioni software, semplicità, chiarezza) e l'hinoki (durata); bilingui per costituzione (Dossier §2.3, principio 4) |
| 1 | 基壇 · Temelia | Simplitatea ține totul. | Pentru fiecare problemă căutăm cea mai simplă soluție care funcționează și o explicăm clar. | La semplicità come fondamenta (il founder, 17/11; 簡素 *kanso*) |
| 2 | 心柱 · Stâlpul central | Un singur stâlp trece prin toate etajele. | Un motor comun ține clienții, rolurile, versiunile, registrele, termenele și jurnalul. Îl scriem o dată; fiecare produs nou îl folosește. | Un motore, molti prodotti (Dossier §2.3, principio 5; §2.4) |
| 3 | 初重 · Primul etaj | PrivacyBox. | Primul nostru produs: protecția datelor pentru firme, după Legea nr. 195/2024. Online din 3 octombrie 2026. | Ciò che abbiamo costruito (dosar §1, §6) |
| 4 | 柔構造 · Structura flexibilă | Când lumea se mișcă, clădirea rămâne în picioare. | Legi care se schimbă, clienți noi, dispozitive noi: totul din același cod, cu versiuni, verificat la fiecare livrare. | Costruiti per cambiare (dosar §3; Dossier §5.2, punto 7) |
| 5 | 二重 — 五重 · Etajele de sus | Etajele de sus se ridică pe rând. | Fiecare produs nou se ridică pe același motor, numai când cel de dedesubt se susține singur. | Ciò che vogliamo fare, con la regola: il prodotto nuovo arriva quando il precedente si paga da solo (Dossier §2.4) |
| 6 | 木組み · Îmbinarea | Dovada, înaintea promisiunii. | Ca într-o îmbinare fără cuie, fiecare piesă se verifică: teste la fiecare livrare, datele fiecărui client izolate, rezultate pe care le poate verifica oricine. | «Prova prima della promessa» (Dossier §2.3, principio 3; dosar §3) |
| 7 | 相輪 · Vârful | Piesă cu piesă. | Ce există se vede în lemn; ce urmează, în desen. | Come leggere il tempio, e come lavoriamo: nessun prodotto mostrato prima che esista |

Firma in fondo: il sigillo 檜, «Hinotech Software», «Coteala, raionul Briceni · Republica Moldova»
(la sede decisa il 27/10).

**Che cosa non scriviamo**, anche se è vero:
- le frasi di un prodotto (il «dosar viu», le clausole «De revizuit», il controllo): stanno sul sito
  del prodotto;
- i nomi e le date dei prodotti futuri: i piani alti restano disegno;
- numeri che invecchiano (documenti, registri) e numeri interni (righe di codice, settimane di lavoro);
- la paura delle multe, il grant, ODA, i bandi;
- l'etimologia «albero del fuoco» (火の木) di hinoki: è popolare e contestata (Wiktionary, 檜).

**Fatti verificati il 17/11**, per quando il sito spiegherà il tempio:
- il pilastro centrale delle pagode (心柱) attraversa i piani al centro e ne smorza le oscillazioni; il
  sistema antisismico della Tokyo Skytree, un nucleo centrale collegato con smorzatori, porta lo
  stesso nome ([Shinbashira](https://en.wikipedia.org/wiki/Shinbashira),
  [Pagoda in the Sky](https://web-japan.org/trends/09_sci-tech/sci100722.html)). Il suo ruolo esatto
  è ancora discusso: anche le gronde larghe contano. Sul sito diciamo solo ciò che fa nella scena;
- il pilastro della pagoda del Hōryū-ji è di hinoki, abbattuto nel 594 secondo la datazione degli
  anelli del 2001 ([Web Japan](https://web-japan.org/trends00/honbun/tj010330.html));
- Kengo Kuma usa incastri di hinoki senza chiodi: *cidori* al GC Prostho Museum, *jigoku-gumi* a
  SunnyHills.

## Il tunnel: cinque principi, cinque simboli (18/11)

Il founder, 18/11: il tunnel ha **una frase centrale** («Soluții software simple, clare, făcute să
dureze.»); attorno compaiono, uno alla volta, i **cinque principi di Hinotech** e subito dopo ognuno il suo
**simbolo tradizionale**, giapponese o moldavo; alla fine la frase centrale si rivela una **maschera** che
mostra il contenuto sotto. Ordine e frequenza li ha lasciati a noi. Poi, la sera stessa: niente
descrizioni (né la didascalia del simbolo né la frase che spiega il principio), **solo il nome del
principio e il suo simbolo**; disposizione equilibrata e coerente per tutta l'animazione; via le linee
dei quadranti; ogni modifica passa prima dalla tela Claude Design.

| # | Principio (il founder) | Sul sito: il nome | Simbolo | Perché quel simbolo (nota nostra, non sul sito) | Fonte |
|---|---|---|---|---|---|
| 1 | Tecnologia al servizio dell'uomo | Tehnologie în serviciul omului | **Cârligul ciobanului**, Moldova, punto croce | rappresenta lo strumento del pastore: uno strumento che lavora per chi lo usa | [moldovenii.md, «Motive și simboluri în arta populară a moldovenilor»](https://www.moldovenii.md/md/section/691) |
| 2 | Unificazione della frammentazione | Unificare, nu fragmentare | **Shippō**, Giappone, medaglione | cerchi uguali che si sovrappongono e si legano ai vicini: un disegno solo | [JAANUS, «shippōmon»](https://projects.mcah.columbia.edu/jaanus/node/1215) |
| 3 | Trasparenza e usabilità | Transparență și ușurință | **Șănătăul**, Moldova, punto croce | la linea ondulata dei tappeti simboleggia l'acqua e le sue onde: chiaro come l'acqua | moldovenii.md, come sopra |
| 4 | Sicurezza dei dati | Securitatea datelor | **Kikkō**, Giappone, medaglione | il guscio di tartaruga: lunga vita, buona sorte, protezione; ogni cella chiusa | [NGV, «Monyō: exploring traditional kimono patterns»](https://www.ngv.vic.gov.au/essay/monyo-exploring-traditional-kimono-patterns/) |
| 5 | Sicurezza legale | Siguranță juridică | **Dinții de lup**, Moldova, punto croce | motivi usati come cornice sul bordo dei tappeti antichi: tutto dentro il quadro della legge | moldovenii.md, come sopra |

**La disposizione** (tela Claude Design, tavole «Tunelul · principiul 1 și simbolul lui», «Ordinea și
frecvența» e «Pagina deschisă · fraza se întunecă»). Il founder, 18/11 sera: il simbolo non deve stare sulla
stessa riga del nome; disposizione più studiata e dinamica, con posizioni distinte; e nessuna linea durante il
tunnel (né le pareti né un filo tra nome e simbolo). Una prova con i simboli sopra i nomi, in cerchio, era
stata scartata. Ora ogni principio è una composizione sua, grande quanto lo schermo: il nome in un angolo, il
simbolo nell'angolo opposto. Le diagonali cambiano: 1 il nome in alto a sinistra e il simbolo in basso a
destra, 2 in alto a destra → in basso a sinistra, 3 in basso a destra → in alto a sinistra, 4 in basso a
sinistra → in alto a destra, 5 in alto al centro → in basso al centro. L'equilibrio passa sempre per il
centro. Posizioni in frazioni dello schermo nel codice (`COMP`), uguali a quelle della tela; sul telefono le
stesse diagonali in verticale.

**Come si muove** (ritmo compatto, 19/11). Il founder, 19/11: si scorreva troppo e non invogliava a leggere;
le scritte e i simboli devono partire più dal centro; non uno, poi il vuoto, poi il successivo, ma uno dopo
l'altro, più compatti («quando si avvia la terza scritta far sparire completamente la prima»); il nome grande
circa il doppio. Ora la frase si stringe al centro e resta lì. Un principio ogni **mezzo schermo di scroll**:
la composizione parte vicino al centro (al 30 % della sua distanza; prima compariva già al 55–70 %), arriva
nel suo angolo, si ferma, poi passa accanto a chi guarda. Il successivo parte mentre il precedente è ancora
fermo; quando parte il terzo, il primo è già sparito. Il nome è il doppio di prima (68 px sul computer,
adattato allo schermo come prima; 44 px sul telefono invece di 24) e si accende parola per parola mentre
arriva; il simbolo si cuce punto per punto (moldavi) o si disegna (giapponesi). Questa parte va a tempo, poco
più di un secondo, così si completa anche se ci si ferma; con lo scroll veloce non resta indietro, perché
quando la composizione si ferma nel suo angolo il disegno è già finito. Alla fine i cinque simboli tornano
piccoli attorno alla frase, ognuno dalla parte in cui si era cucito, ed entrano in lei; la frase diventa una
maschera (tre strati fissi: nero con le lettere bianche in moltiplica, il colore del tunnel in schiarisci, il
bordo delle lettere). Dentro le lettere sale la pagina chiara e si entra dalla «l» di «clare»; lo zoom
finisce quando la pagina arriva in alto: **4,75 schermi** (il tunnel è 575vh; prima 960vh, 8,6 schermi). Con
«riduci movimento» i cinque stanno fermi, in griglia.

**Il lampo bianco** (il founder: «si nota molto quando lo scroll è veloce»). La maschera segue lo scroll con
il piccolo ritardo di tutto il tunnel; la pagina chiara invece segue lo scroll vero. Con una spinta forte la
pagina arrivava sullo schermo prima della maschera: un fotogramma bianco, poi di nuovo scuro. Ora la pagina
chiara resta nascosta finché la maschera non la copre, la maschera si accende un istante prima che sotto ci
sia la carta, e verso la fine la camera insegue lo scroll più da vicino. Provato registrando ogni fotogramma
con spinte forti in giù, in su e sul telefono (`tools/flash.mjs`): la luce sale una volta sola, dallo scuro
alla pagina, senza tornare indietro; sulla versione precedente lo stesso test mostrava il lampo.

**La pagina sotto la maschera**: la sezione 1.0 parte più in basso (34vh), così quando la maschera si apre
del tutto la frase «Regulile care decid ce construim…» sta a metà schermo. Le sue parole partono
chiarissime e si scuriscono una dopo l'altra mentre si scorre, da quando la pagina è quasi tutta visibile
(4,5 schermi) fino a 5,05: la prima frase diventa inchiostro, il resto quasi nero.

**Il menu** (il founder, 18/11): il menu in alto con il logo sparisce appena si comincia a scorrere e
ricompare solo scorrendo all'insù, in cima alla pagina o arrivandoci con la tastiera.

**Che cosa non diciamo dei simboli**: la stessa fonte moldava avverte che i significati dei motivi sono
studiati poco e che circolano invenzioni. Le note restano qui e sulla tela; sul sito solo nome e simbolo.

## I colori: quelli della console, letti alla giapponese

Gli stessi esadecimali della console («Nordic Roots», `cos_palette.dart` e il blocco 1 di
`apps/site/assets/site.css`). Cambia la lettura, non i valori.

| Token della console | Esadecimale | Qui si chiama | Uso sul sito |
|---|---|---|---|
| `n-000` | `#FBFAF8` | 和紙 *washi* / 한지 *hanji*, la carta | il fondo |
| `n-050` … `n-200` | `#F1EEE9` … `#C8C1B4` | la carta in ombra | fasce, filetti, piani |
| `n-500` … `n-700` | `#7A756D` … `#463F38` | l'inchiostro diluito | testo secondario |
| `n-900` | `#141311` | 墨 *sumi* / 먹 *meok*, l'inchiostro | il testo, il disegno del tempio |
| `rust` | `#9C4A38` | 檜皮色 *hiwada-iro*, la corteccia di hinoki | **un solo accento**: il tetto del primo piano e il sigillo |
| `ochre` | `#A67C44` | il legno di hinoki | solo negli oggetti e nelle immagini |
| `moss` | `#5A6B54` | 苔 *koke*, il muschio | solo negli oggetti e nelle immagini |
| `fjord` | `#4A6472` | 藍鼠 *ai-nezumi*, il grigio indaco | solo negli oggetti e nelle immagini |

Il ruggine della console è quasi lo stesso colore di 檜皮色, la corteccia di hinoki con cui si
coprono i tetti dei templi (`#965036` nelle tavole dei colori tradizionali più diffuse: non è un
valore ufficiale). I nomi di muschio e indaco sono nomi d'uso, non i valori delle tavole.
Versione notte: come la console, la rampa si rovescia e il ruggine si schiarisce a `#C06B54`.

## Tecnologia (proposta da decidere)

| | Proposta: **Astro 6** | Next.js + React Three Fiber | HTML a mano, come `apps/site` |
|---|---|---|---|
| Pagine | statiche, HTML puro, JS solo dove serve | React su ogni pagina | statiche |
| Tre lingue | routing i18n integrato | integrato | a mano, pagina per pagina |
| Font e sicurezza | Fonts API (font dal nostro dominio), CSP API | da configurare | a mano |
| 3D | il tempio come «isola» Three.js, solo nella home | ecosistema R3F/drei, il più ricco | Three.js da modulo |
| Hosting | Cloudflare (Astro è di Cloudflare dal 16/01/2026), gratuito, stesso account di PrivacyBox | Vercel/Cloudflare | Cloudflare |
| Peso | il più leggero | il più pesante | leggero |

Con Astro: **Three.js** per il tempio (già scritto così in `tempio.html`), **GSAP 3** se servono
scene più complesse (gratuito con tutti i plugin dal 2025), le **CSS scroll-driven animations** (in
tutti i browser da ottobre 2026) per i movimenti semplici: il testo del tempio entra già così.
Astro 6 vuole Node 22 o più recente: su questo PC c'è Node 25.

### Da dove viene il realismo

Il founder, 17/11: il tempio è bello ma non abbastanza realistico, vuole la vivacità; si possono avere
pezzi di legno veri? Tre livelli:

1. **Materiali fotografati dal vero, in tempo reale** (fatto il 17/11). Legno, corteccia e pietra
   sono fotografie vere, CC0, di Poly Haven: `hinoki_planks` (hinoki, con nodi e venature),
   `japanese_cedar_bark` (corteccia di cedro giapponese, posata a corsi come nei tetti 檜皮葺) e
   `japanese_stone_wall`, con le mappe di rilievo e di ruvidità. Ogni pezzo prende una tavola diversa
   in un punto diverso; gli spigoli sono smussati e prendono la luce; l'occlusione d'ambiente (GTAO)
   scurisce i giunti, sullo schermo largo. Nel prototipo le texture arrivano dalla rete di Poly Haven;
   nel sito vanno scaricate nel nostro dominio e compresse (KTX2), con il tuo sì al download.
2. **Render di Blender** (blender-mcp), con la luce calcolata come in fotografia, sfogliati con lo
   scroll come le pagine prodotto di Apple: il massimo del realismo digitale, non interattivo.
   Blender non è installato su questo PC.
3. **Legno vero, fotografato.** Esiste il kit in legno della pagoda a cinque piani del Hōryū-ji,
   Woody Joe 1/150 (uscito il 24/04/2025, 9.900 yen, legno di cipresso secondo il venditore): montato
   pezzo per pezzo e fotografato a ogni passo sulla stessa carta, diventa la sequenza che lo scroll
   sfoglia. Pezzi veri, montati davvero: «Piesă cu piesă» diventa letterale.
4. **Foto** (Canva, piano gratuito) per persone e luoghi.

## Strumenti per Claude su GitHub

Non esiste un repository che «crea» da solo un sito così: esistono skill che alzano il livello di
Claude su design e motion, e ponti verso gli strumenti 3D.

| Strumento | Che cosa fa | Quando |
|---|---|---|
| [anthropics/skills → frontend-design](https://github.com/anthropics/skills) | skill ufficiale di Anthropic: scelte tipografiche e cromatiche decise, niente aspetto «generato» | da subito |
| [greensock/gsap-skills](https://github.com/greensock/gsap-skills) | skill ufficiali di GSAP: timeline, ScrollTrigger, prestazioni | da subito |
| [cloudai-x/threejs-skills](https://github.com/cloudai-x/threejs-skills) | Three.js per Claude: luci, shader, texture, post-processing | da subito |
| [ahujasid/blender-mcp](https://github.com/ahujasid/blender-mcp) | Claude guida Blender: modelli, materiali, asset Poly Haven, render (MIT) | se scegliamo il realismo 2 |
| [sparkjsdev/spark](https://github.com/sparkjsdev/spark) | Gaussian splat in Three.js (World Labs, MIT) | se scegliamo il realismo 3 |
| [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | catalogo di stili, palette e font (MIT) | non serve: palette e concept li abbiamo |
| Claude Design (claude.ai/design) | impaginare e provare con te, poi «Handoff to Claude Code» | per le pagine interne |

Le skill si installano nel progetto (`hinotech-site/.claude/skills/`), non in tutto il PC.

## Decisioni

| # | Decisione | Proposta | Stato |
|---|---|---|---|
| D1 | Direzione grafica | la home `design/home.html`: tunnel con la frase centrale e i cinque principi con i loro simboli, poi la pagina chiara in stile linear.app; il villaggio (`design/sat.html`) e il tempio sono messi da parte | **in corso** (18/11) |
| D2 | Tecnologia | Astro 6 + Three.js (+ GSAP se serve), su Cloudflare | da decidere |
| D3 | Realismo del tempio | materiali fotografati in tempo reale (fatto); poi il kit vero o i render | da decidere |
| D4 | Caratteri | T2, editoriale (Cormorant Garamond + IBM Plex): è quello del tempio | da decidere |
| D5 | Lingue | romeno, russo, inglese | da decidere |
| D6 | Skill da installare | frontend-design, gsap-skills, threejs-skills | da decidere |
