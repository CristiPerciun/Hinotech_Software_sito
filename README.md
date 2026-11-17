# Hinotech Software — il sito della casa madre

Avvio: 17/11/2026. Ancora nessun codice: questa cartella tiene il brief e la tavola delle direzioni
([`design/direzioni.html`](design/direzioni.html), si apre con un doppio clic) su cui decidiamo
tecnologia e grafica. Repository git proprio, privato su GitHub (`CristiPerciun/Hinotech_Software_sito`,
ramo `main`), escluso da Brainstorming con `.git/info/exclude`.

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

## Il concept: hinoki 檜

Il nome viene dalle proposte del 7/11 («cultura giapponese, semplicità, bellezza minimale,
affidabilità»): **hinoki**, il cipresso dei templi, il legno chiaro che non marcisce. Il Hōryū-ji,
in hinoki, è tra gli edifici di legno più antichi al mondo; i santuari di Ise si ricostruiscono
identici ogni vent'anni. Il sito racconta il software come lavoro di falegnameria: pezzi precisi
che si incastrano senza chiodi (*kigumi* 木組み), fatti per durare e per essere mantenuti.

| Principio | Giapponese | Coreano | Sul sito |
|---|---|---|---|
| Lo spazio vuoto | 余白 *yohaku* | 여백 *yeobaek* | un'idea per schermata, molto margine |
| La semplicità | 簡素 *kanso* | | si toglie finché resta l'essenziale |
| Il mestiere | 匠 *takumi* | | il dettaglio curato anche dove nessuno guarda |
| La durata | 檜 *hinoki* | | si costruisce per decenni, si mantiene come un tempio |

## I colori: quelli della console, letti alla giapponese

Gli stessi esadecimali della console («Nordic Roots», `cos_palette.dart` e il blocco 1 di
`apps/site/assets/site.css`). Cambia la lettura, non i valori.

| Token della console | Esadecimale | Qui si chiama | Uso sul sito |
|---|---|---|---|
| `n-000` | `#FBFAF8` | 和紙 *washi* / 한지 *hanji*, la carta | il fondo |
| `n-050` … `n-200` | `#F1EEE9` … `#C8C1B4` | la carta in ombra | fasce, filetti, piani |
| `n-500` … `n-700` | `#7A756D` … `#463F38` | l'inchiostro diluito | testo secondario, le stecche dello shōji |
| `n-900` | `#141311` | 墨 *sumi* / 먹 *meok*, l'inchiostro | il testo; il fondo della versione notte |
| `rust` | `#9C4A38` | 檜皮色 *hiwada-iro*, la corteccia di hinoki | **un solo accento per pagina**: il sigillo |
| `ochre` | `#A67C44` | il legno di hinoki | solo negli oggetti e nelle immagini |
| `moss` | `#5A6B54` | 苔 *koke*, il muschio | solo negli oggetti e nelle immagini |
| `fjord` | `#4A6472` | 藍鼠 *ai-nezumi*, il grigio indaco | solo negli oggetti e nelle immagini |

Il ruggine della console è quasi lo stesso colore di 檜皮色, la corteccia di hinoki con cui si
coprono i tetti dei templi (`#965036` nelle tavole dei colori tradizionali più diffuse: non è un
valore ufficiale). I nomi di muschio e indaco sono nomi d'uso, non i valori delle tavole.
Versione notte: come la console, la rampa si rovescia e il ruggine si schiarisce a `#C06B54`.

## Le tre direzioni (vive nella tavola)

- **A — Kigumi 木組み** (proposta). Un reticolo di bastoncini di hinoki, come gli incastri *cidori*
  e *jigoku-gumi* di Kengo Kuma (GC Prostho Museum, SunnyHills), sospeso sulla carta: i pezzi
  scorrono lungo il proprio asse e si incastrano mentre scorri, la luce del sole si scalda.
  Oggetto 3D realistico in tempo reale.
- **B — Komorebi 木漏れ日**. Niente oggetti: lo schermo è la carta di uno shōji (o di un *ttisal*
  coreano, 띠살) illuminata da dietro. L'ombra dei rami di hinoki scorre e la luce si scalda dal
  mattino alla sera mentre scorri.
- **C — Sumi e sigillo 墨と印**. Un *ensō* a pennello che si traccia con lo scroll e il sigillo
  color corteccia che chiude la pagina. Più grafica che realistica.

A e B si sommano bene (l'oggetto di A sotto la luce di B); il sigillo di C può firmare tutte e tre.

## Tecnologia (proposta da decidere)

| | Proposta: **Astro 6** | Next.js + React Three Fiber | HTML a mano, come `apps/site` |
|---|---|---|---|
| Pagine | statiche, HTML puro, JS solo dove serve | React su ogni pagina | statiche |
| Tre lingue | routing i18n integrato | integrato | a mano, pagina per pagina |
| Font e sicurezza | Fonts API (font dal nostro dominio), CSP API | da configurare | a mano |
| 3D | un'«isola» Three.js solo nell'hero | ecosistema R3F/drei, il più ricco | Three.js da modulo |
| Hosting | Cloudflare (Astro è di Cloudflare dal 16/01/2026), gratuito, stesso account di PrivacyBox | Vercel/Cloudflare | Cloudflare |
| Peso | il più leggero | il più pesante | leggero |

Con Astro: **Three.js** per gli oggetti, **GSAP 3** (ScrollTrigger, SplitText: gratuiti con tutti i
plugin dal 2025) per le scene legate allo scroll, le **CSS scroll-driven animations** (in tutti i
browser da ottobre 2026, con Firefox 159) per i movimenti semplici. Astro 6 vuole Node 22 o più
recente: su questo PC c'è Node 25.

### Da dove viene il realismo

1. **Tempo reale** (proposta per l'hero): geometria in codice, materiali PBR con texture CC0
   (Poly Haven, ambientCG), luce d'ambiente. Leggero e interattivo. Nella tavola le venature sono
   generate in codice.
2. **Render di Blender guidato da Claude** (blender-mcp), sfogliati con lo scroll come le pagine
   prodotto di Apple: fotorealistico, più pesante, non interattivo. Blender non è installato su
   questo PC.
3. **Scansione di un oggetto vero** (un *kumiki* di hinoki, il rompicapo a incastro) in Gaussian
   splat, mostrata con Spark: il più vero e il più nuovo, ma va comprato e scansionato l'oggetto.
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
| D1 | Direzione grafica | A, con la luce di B; il sigillo di C come firma | da decidere |
| D2 | Tecnologia | Astro 6 + Three.js + GSAP, su Cloudflare | da decidere |
| D3 | Realismo dell'hero | 1, tempo reale; 2 o 3 più avanti se serve | da decidere |
| D4 | Caratteri | T1 o T2 (nella tavola) | da decidere |
| D5 | Lingue | romeno, russo, inglese | da decidere |
| D6 | Skill da installare | frontend-design, gsap-skills, threejs-skills | da decidere |
