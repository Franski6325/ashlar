# Batch F (26–31) — PROMPT TOP-TIER per Claude Fable 5.1 Max

> **A cosa serve questo file:** è il prompt pronto da incollare a Claude Fable 5.1 Max per generare
> **6 nuovi siti single-file** allo standard (e oltre) dei primi 5 della repo (`01-deckle`, `02-umbra`,
> `03-fieldform`, `04-halcyon`, `05-folio`).
>
> **Nota sul conteggio:** hai chiesto "5 altri siti" ma hai elencato **6 tipologie**.
> Questo prompt le copre **tutte e 6** (numerate 26–31). Se ne vuoi solo 5, elimina il brief che ti serve meno.
>
> **Come usarlo:**
> 1. Copia tutto il blocco tra `INIZIO PROMPT DA INCOLLARE` e `FINE PROMPT DA INCOLLARE` e incollalo a Claude Fable 5.1 Max.
> 2. Fagli generare **un sito alla volta** (ordine consigliato: 26 → 31), ognuno come singolo `index.html` completo.
> 3. Alla fine di ogni sito, fagli fare l'**autoverifica** con la checklist in fondo (§9) prima di passare al successivo.
> 4. Tutto ciò che genera deve essere **originale e fittizio**: nessun marchio reale, nessun testo copiato, nessuna immagine da web.

---

# ════════════════════════════════════════════════════════════════════
# INIZIO PROMPT DA INCOLLARE A CLAUDE FABLE 5.1 Max
# ════════════════════════════════════════════════════════════════════

## 0. RUOLO — chi sei quando esegui questo prompt

Sei contemporaneamente, a livello **Awwwards Site of the Day / Developer Award**:

- un **creative director** che inventa concept memorabili, mai banali, mai template;
- un **brand designer** che costruisce sistemi visivi coerenti (palette, type, griglie, texture, radius, cursori);
- un **copywriter italiano madrelingua** che scrive microcopy originale, concreto, senza fuffa da AI e senza lorem ipsum;
- un **creative developer** che padroneggia **GSAP 3.12.5 core + ScrollTrigger + Lenis** in vanilla JS dentro un singolo file HTML;
- un **motion designer** che coreografa scroll come regia cinematografica: ogni sezione ha un'idea di movimento propria, mai la stessa del sito precedente;
- un **legal-safe designer**: tutto ciò che produci è **originale al 100%**, fittizio, senza marchi reali, senza testi copiati, senza immagini altrui.

Il tuo gusto: **editoriale, audace, preciso**. Odi i template SaaS viola, gli hero "Lorem + bottone",
i counter 0–100 con barra, i fade-up generici, i marquee decorativi messi a caso.
Ogni sito che consegni deve poter stare in un portfolio Awwwards senza sfigurare.

---

## 1. CONTESTO — cosa esiste già e cosa devi superare

Stai estendendo **Ashlar Lab**, portfolio di landing page fittizie single-file.

**I primi 5 siti (Batch A) hanno già fissato questa asticella — tu devi superarla, non ripeterla:**

| # | Nome | Concept | Palette già presa (NON riusare) | Type già usato |
|---|------|---------|----------------------------------|----------------|
| 01 | Deckle | Atelier carta, Bruges | carta `#f2ede3` + oro `#b07d2a` + sigillo `#8d3b2b` | Newsreader + DM Sans + IBM Plex Mono |
| 02 | Umbra | Console perimetrale dark | nero `#0a0a0a` + viola `#7C4DFF` | Archivo variable + JetBrains Mono |
| 03 | Fieldform | Pattern studio procedurale | bianco + lime `#c8f03c` + spettrali | Outfit + Instrument Serif + JetBrains Mono |
| 04 | Halcyon | Research lab AI | crema `#F5F1E9` + mesh iridescente pastello | Fraunces + Inter + JetBrains Mono |
| 05 | Folio Press | Magazine indipendente | carta `#f4f1ea` + blu elettrico `#1b3cff` | Newsreader + Archivo + JetBrains Mono |

**Stack condiviso (obbligatorio, identico per tutti i nuovi siti):**

- Un solo file `index.html` per sito: CSS e JS inline. Niente build, niente framework, niente file esterni oltre i CDN sotto.
- `GSAP 3.12.5 + ScrollTrigger` via CDN (licenza Standard gratuita, solo core + ScrollTrigger — **niente plugin Club a pagamento**, niente SplitText del Club: lo split testuale lo implementi a mano in JS).
- `Lenis 1.1.18` via CDN (MIT) per lo smooth scroll, sincronizzato con `ScrollTrigger.update`.
- `Google Fonts` via CDN (solo licenze OFL/Apache). Massimo 3 famiglie per sito.
- **Zero immagini raster esterne.** Niente `.jpg/.png` da web, niente Unsplash/Pexels/hotlink. Tutta la grafica è **CSS + SVG inline + data-URI**. Favicon via SVG data-URI.
- Responsive mobile-first: `360 / 768 / 1280 / 1600px`. Accessibilità: HTML semantico, skip-link, focus visibile, contrasto AA, `prefers-reduced-motion` rispettato.

**La tua missione:** creare i siti **26–31** (cartelle `sites/26-alveo/`, `sites/27-ardere/`, `sites/28-calandra/`, `sites/29-rotta/`, `sites/30-altrove/`, `sites/31-voltabit/`, ognuna con il suo `index.html`).
Ognuno deve avere **concept, palette, tipografia, layout, cursore, strumento interattivo e coreografia GSAP completamente diversi** sia dal Batch A sia dagli altri 5 nuovi siti.

---

## 2. VINCOLI LEGALI — non negoziabili, verificali su ogni sito

Leggi con attenzione: **tutto deve essere lecito, originale e senza alcuna violazione di copyright, marchi o diritti altrui.**

1. **Marchi 100% fittizi.** I nomi nei brief (§8) sono proposte originali inventate per l'occasione. Non usare mai nomi di aziende, prodotti, ristoranti, hotel, SaaS, font commerciali o loghi reali. Non evocare marchi famosi nemmeno con giochi di parole ("Notion-like", "Airbnb di…", "il Uber di…"). Se un nome ti ricorda un marchio reale, cambialo.
2. **Copy 100% originale.** Scrivi tu ogni headline, paragrafo, testimonianza, voce di menu, prezzo, metrica. Niente testi copiati da siti reali, niente citazioni attribuite a persone reali, niente recensioni vere. Testimonianze e clienti sono **personaggi fittizi con nome + cognome inventati** (mai nomi di celebrità).
3. **Niente asset altrui.** Solo CSS/SVG/data-URI creati da te. Niente foto, icone, illustrazioni o texture scaricate o hotlinkate. Le icone sono SVG disegnati da te (stroke geometrici, non repliche di set famosi).
4. **Solo librerie con licenze compatibili:** Google Fonts (OFL/Apache) via CDN, GSAP core + ScrollTrigger (Standard gratuita), Lenis (MIT). Niente plugin GSAP Club a pagamento, niente font pirata, niente snippet copiati da CodePen/temi senza licenza: **scrivi il codice da zero**.
5. **Dati fittizi dichiarati.** P.IVA, telefoni, indirizzi, email, metriche ("+312%") sono inventati e plausibili-ma-finti: usa formati palesemente demo (`P.IVA 00000000000`, `02 0000 0000`, `via Esempio 0, Milano`, `ciao@nomefittizio.it`). Mai dati personali reali.
6. **Footer con disclaimer su ogni sito**, adattato al concept (traducilo nel tono del sito ma mantieni il senso):
   > "Demo di design — marchio, dati, prezzi e persone fittizi a scopo dimostrativo. Nessuna affiliazione con aziende reali. I moduli non inviano dati né processano pagamenti."
7. **Niente dark pattern, niente claim ingannevoli** ("migliore al mondo", certificazioni inventate, "approvato da…"). Niente finta urgenza, niente countdown falsi, niente badge di pagamento/enti reali.
8. Il codice che consegni è destinato a una repo **MIT**: deve essere tuo e originale, con commento di testa che attribuisce i CDN ai rispettivi titolari.

Se durante la generazione ti accorgi che un nome, un testo o un visual assomiglia a qualcosa di esistente, **cambialo proattivamente** e segnalalo nel riepilogo.

---

## 3. VINCOLI TECNICI — non negoziabili

### 3.1 Struttura file

- Un `index.html` autonomo per sito. Ordine: `<head>` (meta, title/description/OG fittizi-ma-coerenti, preconnect fonts, CSS) → body (skip-link, cursore, progress/nav, `<main>` con sezioni, footer, overlay) → `<script>` CDN (GSAP, ScrollTrigger, Lenis, con `defer` dove sensato) → script inline.
- Design tokens in `:root`: `--bg`, `--bg-2`, `--ink`, `--muted`, `--line`, accenti, `--radius-*`, `--font-display/body/mono`, `--ease-*`, fluid type con `clamp()`.
- Griglia dichiarata (12 colonne su desktop, 4–6 su mobile). Spaziature su scala (es. `8/16/24/40/64/96/128`).
- CDN esatti (non cambiarli, non aggiungerne altri senza motivo):
  - GSAP `https://cdn.jsdelivr.net/npm/gsap@3.12.5/dist/gsap.min.js`
  - ScrollTrigger `https://cdn.jsdelivr.net/npm/gsap@3.12.5/dist/ScrollTrigger.min.js`
  - Lenis `https://cdn.jsdelivr.net/npm/lenis@1.1.18/dist/lenis.min.js`
- Niente Tailwind/Bootstrap/jQuery/React. Vanilla JS pulito, commentato il giusto, niente `console.log` in produzione.

### 3.2 Qualità ingegneristica

- **Lenis + ScrollTrigger sincronizzati**: `lenis.on('scroll', ScrollTrigger.update)`, `gsap.ticker.add(t => lenis.raf(t * 1000))`, `gsap.ticker.lagSmoothing(0)`.
- `gsap.registerPlugin(ScrollTrigger)` una sola volta.
- **ScrollTrigger solo su tween/timeline top-level**, mai su tween annidati in una timeline; mai `scrub` + `toggleActions` insieme (scegli uno dei due); `markers: false` in produzione.
- `gsap.matchMedia()` per breakpoint (mobile vs `min-width: 900px`) e per `prefers-reduced-motion: reduce` (durata `0` o animazione saltata, contenuto sempre leggibile senza JS-motion).
- **Solo `transform` + `opacity`/`autoAlpha`** per le animazioni (x/y/xPercent/yPercent/scale/rotation/skew). Mai `width/height/top/left/margin` animati. `will-change` solo sugli elementi che animano davvero, rimosso a fine animazione dove possibile.
- `gsap.quickTo()` per follower/cursori e per tutto ciò che si aggiorna a ogni mousemove.
- Timeline con `defaults`, `position parameter` (`"<"`, `"<0.2"`, `"-=0.3"`), `addLabel()` leggibili. Mai sequenze costruite con catene di `delay`.
- `ScrollTrigger.refresh()` dopo font/layout/contenuto dinamico; `refreshPriority` in ordine top-to-bottom se crei trigger fuori ordine; `invalidateOnRefresh: true` per valori funzionali (`x: () => ...`).
- `immediateRender: false` sui `from()/fromTo()` successivi che condividono target+proprietà; `clearProps` dove il CSS deve riprendere il controllo; `overwrite: "auto"` sui tween che possono scontrarsi (hover vs scroll).
- Performance: stagger invece di centinaia di tween; batch reads poi writes; canvas/particle throttled con `gsap.ticker`, DPR clampato a 2, pausa quando offscreen (`ScrollTrigger onToggle` o IntersectionObserver); kill dei trigger offscreen non più necessari.
- Accessibilità: sezioni `<section aria-labelledby>`, heading gerarchici, `alt`/ `aria-label` sugli SVG informativi (`aria-hidden="true"` su quelli decorativi), contrasto testo/sfondo ≥ 4.5:1 (≥ 3:1 per display grandi), target touch ≥ 44px, form con `<label>` reali, focus `:focus-visible` disegnato, navigazione tastiera completa di menu/overlay/tab/accordion (Esc chiude, focus trap leggero).
- Form e checkout sono **demo**: `submit` intercettato in JS con stato di successo animato inline, nessun invio reale, testo "Demo — nessun dato inviato".

---

## 4. BARRA DESIGN — cosa significa "livello Awwwards" qui

### 4.1 Direzione artistica (vale per tutti, declinata per sito)

- **Un'idea forte per sito, non sei template.** Ogni sito deve essere descrivibile in una frase memorabile ("il SaaS come sala di controllo navale", "il ristorante come rituale del fuoco", "la S.R.L. come disegno tecnico vivente"…). Se due siti sembrano cugini, hai fallito: ricomincia dal concept.
- **Tipografia da protagonista.** Display con carattere estremo (variable axes, italic taglienti, condensed industriali, serif ardenti), gerarchia netta display/body/kicker/mono, almeno un momento tipografico memorabile per sito (parola gigante che reagisce allo scroll, manifesto con scrub parola-per-parola, orizzontale tipografica…).
- **Palette con disciplina.** 2 neutri + 1–2 accenti + muti/linee. Ogni colore ha un ruolo (sfondo, inchiostro, segnale, evidenziazione). Niente arcobaleni, niente gradienti viola-blu generici. Ogni brief (§8) ti dà gli esadecimali esatti: usali, non improvvisare altri accenti.
- **Materiali e texture originali.** Niente stock: costruisci profondità con sistemi generativi tuoi — reticoli tecnici, halftone calibrati, grane SVG leggere, pattern CSS, mesh dedicate al concept. Ma: il Batch A usa già `feTurbulence` + halftone + scanlines ovunque — per il Batch F inventa **almeno un materiale mai visto nel Batch A per ogni sito** (es. brace viva, blueprint, bussola, phosphor CRT, timbro S.R.L., collage studio).
- **Radius come dichiarazione.** Ogni brief dichiara la sua filosofia di raggio (tagliente / industriale / morbido / misto): rispettala con coerenza maniacale, inclusi bottoni, card, chip, input, cursori.
- **Micro-dettagli che vincono premi:** stati hover/active/focus disegnati, numeri con tabular-nums, unità e label mono calibrate, bordi da 1px con opacità studiate, ombre usate come luce (non come sporco), transizioni `150–300ms` con ease coerenti, selezione testo `::selection` nel colore del brand, scrollbar sobria, orologi/fusi reali via JS dove previsti dal brief.
- **Densità editoriale.** Ogni sito: nav + hero + 6–9 sezioni + 1 strumento interattivo sostanzioso (vedi §6) + form/demo + footer ricco. Niente pagine vuote, niente sezioni "placeholder".

### 4.2 Copywriting (italiano, originale, concreto)

- Italiano curato e specifico del settore; micro-inglese solo dove naturale (SaaS: *timeline, sprint*; studio: *case study*; IT: *benchmark*). Mai lorem, mai "Lorem ipsum", mai frasi da generatore ("Soluzioni innovative per un mondo in continua evoluzione").
- Headline che dicono qualcosa di vero sul concept fittizio ("La brace non ha fretta. Noi nemmeno."). Sottotitoli che spiegano il meccanismo, non aggettivi vuoti.
- Numeri e prezzi fittizi-ma-plausibili, con unità e footnote ("Prezzi demo. Listino reale su richiesta.").
- Tone of voice diverso per sito (vedi brief): il SaaS è asciutto-operativo, il ristorante è sensoriale-lento, la S.R.L. è solida-tecnica, lo studio è colto-ironico, i viaggi sono contemplativi, l'informatica è schietta-da-laboratorio.

---

## 5. BARRA MOTION GSAP — il top del top, non le solite

### 5.1 VIETATO come "numero principale" (sono già il kit standard del Batch A)

Questi pattern esistono già in tutti/c quasi i primi 5 siti. Puoi usarli **solo come tappezzeria secondaria**, mai come idea di movimento portante di un sito Batch F:

- ❌ Preloader con counter `0–100` + barra + uscita slide-up come unica intro.
- ❌ Reveal generico `[data-reveal]` fade-up identico ovunque come unica reveal.
- ❌ Marquee infinito `xPercent: -50` a velocità costante come unico movimento.
- ❌ Counter `[data-count]` semplice come unico momento "dati".
- ❌ Bottone magnetico base come unica interazione.
- ❌ `feTurbulence` + grana + scanlines come unica texture in movimento.

Se il tuo sito si riduce a "preloader + hero split + ticker + fade-up + counter + magnetic", **ricomincia da capo**.

### 5.2 RICHIESTO — cassetta degli attrezzi avanzata (almeno 3 tecniche signature per sito)

Scegli e combina — usando **solo core + ScrollTrigger + JS vanilla** (niente plugin Club) — tra queste famiglie. Ogni brief (§8) ti dice già quali sono le sue signature obbligatorie; qui trovi come eseguirle da professionista:

1. **Timeline pinned multi-stage con scrub e label.**
   Pinned `end: "+=2500/3500"` su desktop (`matchMedia`), timeline con label (`addLabel("atto1")…`), scrub `0.8–1.2`, fasi che si susseguono (diagramma → evidenziazione → morph → risoluzione). Mai animare l'elemento pinnato: anima i figli. `pinSpacing: true` salvo layout dedicato.
2. **Capitoli orizzontali veri (fake-horizontal con `containerAnimation`).**
   Sezione viewport pinnata, tween interno `x/xPercent` con **`ease: "none"` obbligatorio**, ScrollTrigger con `pin + scrub`, trigger innestati via `containerAnimation` con `start: "left center"`. Niente pin/snap sui trigger innestati. Calcola `x` con funzione + `invalidateOnRefresh`.
3. **Coreografia SVG scrubbed.**
   `strokeDashoffset` per disegno tecnico/rotte/sparkline, `fill-opacity`/`stroke` in sequenza, `svgOrigin` per rotazioni attorno a un punto comune, `motionPath`-like manuale (se vuoi traiettorie, implementale con `gsap.to` su `x/y` lungo keyframes o con `MotionPathPlugin` gratuito via CDN solo se sai dichiararne la licenza — altrimenti keyframes manuali). Rotazioni direzionali (`"_short"`, `"_cw"`, `"_ccw"`) per bussole/orbite.
4. **Wipe e maschere con `clip-path` / `scaleY` scrubbed.**
   Reveal editoriali: `clipPath: inset(0 0 100% 0 → 0)` scrubbed, tendine, sipari, transizioni tra capitoli. Preferisci `clip-path` + `transform` a `height`.
5. **Tipografia cinetica avanzata (split manuale, niente SplitText Club).**
   Split in JS (parole→`<span class="w">`, caratteri→`<span class="ch">` con `overflow:hidden` sui wrapper), poi: assemble da scattered (`stagger: {from:"random", amount:0.8}` + `rotation`/`yPercent`), scrub parola-per-parola (`color`/`opacity` stagger scrubbed su manifesto pinnato), headline che scala/trasla in parallax (`yPercent` scrub), skew da velocità (`skewX` mappato da `self.getVelocity()` con `clamp` e ritorno elastico).
6. **Velocity-driven motion.**
   `onUpdate: self => self.getVelocity()` per mappare velocità di scroll su `timeScale` (ticker che accelera), `skewX`, intensità particellare, spessore stroke. Usa `gsap.utils.clamp()` e `mapRange()`, con decadimento dolce (`gsap.to` verso 0 allo stop).
7. **Z-stack / overlapping cards scrubbed.**
   Card sovrapposte che scalano (`scale 1→0.92`), ruotano di 1–2°, sfocano (`filter: blur` con parsimonia) e cedono il passo allo scroll. Profondità con `transformPerspective` e ombre coerenti.
8. **Parallasse multi-velocità calibrata.**
   `[data-speed]` diversi per layer (`yPercent` scrub con `scrub: true`), mai più di 4–5 layer, mai parallax su testo piccolo (leggibilità prima di tutto).
9. **Follower fisico con `quickTo`.**
   Peek-card che segue il puntatore con inerzia, card tilt `rotationX/Y` da mousemove normalizzato, spotlight che segue il mouse (CSS vars `--mx/--my` animate via `quickTo`). Un solo follower pesante per pagina.
10. **Morph di layout implementato a mano (stile-Flip senza plugin Club).**
    Misura `getBoundingClientRect()` prima/dopo un cambio stato (filtro, tab, reorder kanban), poi `fromTo` con `x/y/scaleX/scaleY` invertiti. Ottimo per: filtri portfolio, reorder colonne, espansione card→overlay.
11. **Canvas generativo leggero (solo dove il brief lo richiede).**
    Massimo ~150 particelle, `dpr ≤ 2`, loop su `gsap.ticker`, pausa offscreen, `prefers-reduced-motion` → canvas statico o nascosto. Braci, polvere di officina, stelle di rotta, pioggia di phosphor: una sola idea per sito, mai decorazione gratuita.
12. **Sequenze "macchina" (boot, odometro, diagnostica).**
    Timeline con label pertyping/boot checklist (testo battuto a macchina + voci che si spuntano), odometro a rulli (`yPercent` su colonne di cifre, non counter piatto), barre benchmark che reagiscono allo scroll. Ritmo teatrale: pause, accelerazioni, `ease: "steps()"` dove serve il sapore digitale.

### 5.3 Regole di regia

- **Un'apertura diversa per ogni sito.** Niente sei volte lo stesso preloader: sipario clip-path, boot checklist, tendina tecnica, lettere scattered, bussola che si orienta, tendina fiamma… L'intro dura max ~2.2s e rispetta `prefers-reduced-motion` (salto diretto al contenuto).
- **Un pinned al massimo per sito** (due solo se il brief lo autorizza esplicitamente), solo desktop, sempre con fallback mobile lineare.
- **Gerarchia del movimento:** 1 signature dominante + 2 supporting + tappezzeria sobria. Non tutto si muove: il bianco/nero fermo fa risaltare il momento cinetico.
- **Footer con momento finale** diverso per sito (parola gigante scrubbed, mappa che si completa, timbro che si imprime, terminale che saluta…), mai footer morto.
- **Cursore custom unico per sito** (solo `(pointer:fine)`, mai su touch; `cursor: none` solo dove il custom è pienamente funzionale; sempre fallback nativo su input/textarea/select; label contestuali via `data-cursor`).

---

## 6. STRUMENTO INTERATTIVO — il cuore di ogni sito

Ogni sito deve contenere **UNO strumento sostanzioso e coerente col concept** (non un soprammobile): configuratore, builder, ledger, diagnostica, composer. Requisiti:

- Funziona davvero in JS (stato → render → output live: prezzo, spec, rotta, esito).
- Ha almeno 3 controlli (slider/tab/stepper/select/chip) + 1 output animato (GSAP: barre, morph numeri, draw SVG, transizione card).
- È tastierabile e annunciabile (`aria-live="polite"` sull'output, label reali).
- Su mobile resta usabile senza hover (niente interazioni solo-mouse).

Il brief di ogni sito (§8) ti dice quale strumento costruire e come deve comportarsi.

---

## 7. STRUTTURA OUTPUT — come consegni

Per ogni sito consegni **un `index.html` completo e funzionante**, più un riepilogo di 15 righe:

- Concept in una frase + palette usata (hex) + font usati (nomi + pesi).
- Sezioni in ordine con `id` (`#hero`, `#metodo`…).
- Le 3+ tecniche GSAP signature usate e dove.
- Lo strumento interattivo e come si usa.
- Autocertificazione legale: "marchi/copy/asset originali, dati fittizi, disclaimer presente, nessun plugin Club, nessun asset esterno oltre i 3 CDN + Google Fonts".
- Nota di accessibilità: cosa succede con `prefers-reduced-motion` e a 360px.

Ordine di consegna: **26 → 27 → 28 → 29 → 30 → 31**. Un sito per messaggio, completo, senza troncare codice. Ogni file deve funzionare aperto via server statico (`npx serve`) senza errori console.

---

## 8. I 6 BRIEF — 6 siti, 6 mondi diversi

> Regola d'oro: palette, font, radius, texture, cursore, strumento e signature motion di ogni brief sono **obbligatori e unici**.
> Se due siti finiscono per assomigliarsi, rifai il secondo da zero con un'idea più coraggiosa.

---

### 26 — ALVEO · SaaS operativo per progetti aziendali
**Cartella:** `sites/26-alveo/` · **Idea in una frase:** "il progetto aziendale come sala di regia navale: rotte, equipaggi, scadenze."

- **Brand fittizio:** Alveo — *il sistema operativo dei progetti*. Claim originale: "Ogni progetto ha una rotta. Alveo la tiene." Copy asciutta, operativa, con micro-inglese naturale (*timeline, sprint, handoff*). Prezzi demo a 3 tier fittizi.
- **Palette (esatta, non aggiungere accenti):**
  `--pine:#0E1B1A` (sfondo scuro) · `--paper:#F4EFE4` (sfondo chiaro) · `--ink:#101614` · `--signal:#FF5C38` (arancio segnale: solo CTA/stati critici) · `--mint:#7DD8C6` (conferme/successi) · `--line:rgba(16,22,20,.12)` su chiaro / `rgba(244,239,228,.14)` su scuro.
- **Tipografia:** display `Space Grotesk 500/700` (titoli, numeri grandi) · body `Instrument Sans 400/500/600` (testo/UI) · mono `Space Mono 400/700` (kicker, label, timeline). Google Fonts, 3 famiglie max.
- **Radius/materiali:** tagliente-tecnico `radius: 6px` card, `999px` solo su pill/stato. Materiali: reticolo di rotta (griglia + linee di rotta tratteggiate SVG), card "plancia" con header mono, timbro di stato (IN ROTTA / IN ATTESA / CRITICO). Niente mesh iridescente (già Halcyon), niente lime (già Fieldform).
- **Sezioni (`id` in ordine):** `#hero` (plancia live) → `#rotte` (capitoli prodotto) → `#timeline` (PINNED surf orchestrato, vedi motion) → `#metriche` → `#strumento` (simulatore di piano: vedi sotto) → `#piani` (pricing demo 3 tier) → `#sicurezza` (on-premise/permessi, senza claim certificativi reali) → `#faq` (accordion) → footer `#contatti` con disclaimer demo.
- **Strumento — "Simulatore di piano":** slider (persone 3–60, settimane 2–26, budget) + chip (metodo: Sprint / Kanban / Waterfall-fittizio "Cascata") → output live: data di approdo stimata (fittizia), carico equipaggio (barre animate), costo demo (odometro a rulli, non counter piatto), rotta SVG che si ridisegna (`strokeDashoffset`). `aria-live="polite"` sull'output.
- **Signature motion (obbligatorie, tutte e 3):**
  1. `#timeline` **pinned multi-stage scrub** (`end: "+=3200"`, desktop): 4 atti (Pianifica → Esegui → Controlla → Consegna) dove card kanban si spostano tra colonne con morph manuale stile-Flip + burndown SVG che si disegna + anello progressi che si chiude. Label timeline leggibili.
  2. Hero "plancia viva": righe attività che entrano con stagger, sparkline SVG draw-on, orologio di bordo reale via JS, parallasse sobria sui pannelli (max 3 layer).
  3. Tipografia skew-da-velocità sui titoli di sezione + ticker operativo che accelera con `getVelocity()` (mai marquee costante pigro).
- **Cursore custom:** mirino da carteggio (anello + croce + coordinate mono `X/Y` live). Solo `pointer:fine`.
- **Apertura:** tendina tecnica a pannelli con `clip-path` (non counter 0–100): i pannelli si aprono sulla plancia, le righe entrano in stagger.
- **Footer:** parola "ALVEO" gigante con scrub + tabella rotte/demo + disclaimer.

---

### 27 — ARDERE · Ristorante di brace
**Cartella:** `sites/27-ardere/` · **Idea in una frase:** "il ristorante come rituale del fuoco: lento, scuro, sensoriale."

- **Brand fittizio:** Ardere — *cucina di fuoco a Bologna (fittizio)*. Claim originale: "La brace non ha fretta. Noi nemmeno." Copy sensoriale-lenta, menu degustazione fittizio in 5 atti con prezzi demo, chef-personaggio fittizio (nome inventato, mai persona reale).
- **Palette (esatta):**
  `--char:#14100C` (sfondo scuro dominante) · `--cream:#F6EEDD` (carta calda) · `--ember:#E4572E` (brace: accento caldo, mai neon) · `--brass:#C9A227` (dettagli, filetto, numeri) · `--bark:#2E1F16` (superfici) · `--line:rgba(246,238,221,.14)`.
- **Tipografia:** display `Italiana 400` (titoli enormi, menu) · body `Manrope 400/500/600` (testo/UI) · mono `Space Mono 400` (kicker, orari, prezzi). Italiana è il gesto distintivo: usala grande, mai in all-caps stretto.
- **Radius/materiali:** morbido-cerimoniale `radius: 18px` card, `999px` pill, archi (`border-radius: 50% 50% 0 0 / 30%` su nicchie foto-disegnate). Materiali: brace viva (canvas leggero nel hero, vedi motion), carta bruciata ai bordi (gradienti radiali scuri), filetto ottone da 1px, timbro "dal martedì al sabato" (fittizio). Niente foto: i piatti sono **tavole SVG/CSS astratte** (composizioni circolari, fumi, braci) — dichiara in didascalia "illustrazione astratta, non fotografia del piatto".
- **Sezioni:** `#hero` (brace + nome gigante) → `#rito` (manifesto) → `#menu` (PINNED orizzontale 5 atti, vedi motion) → `#brace` (tecnica del fuoco: legni fittizi, temperature) → `#sala` (3 tavoli fittizi + turni) → `#strumento` (costruisci la serata: vedi sotto) → `#voci` (2–3 citazioni di ospiti fittizi) → `#prenota` (form demo turni, nessun invio) → footer con orari fittizi + disclaimer.
- **Strumento — "Costruisci la serata":** stepper (ospiti 1–8) + select (turno fittizio 19:30/21:45) + chip (percorso: 3/5/7 portate demo) + toggle (abbinamento fittizio sì/no) → output: durata stimata, prezzo demo a persona (odometro morbido), composizione atti (card che si accendono in sequenza), nota "Demo — la prenotazione vera è solo di persona."
- **Signature motion (obbligatorie):**
  1. `#menu` **capitoli orizzontali pinnati** con `containerAnimation` (`ease: "none"`): 5 atti scorrono in orizzontale, ogni atto ha numero ottone gigante + tavola astratta + piatti fittizi; trigger innestati per reveal interni.
  2. Hero **brace canvas generativa** (~120 particelle, deriva verso l'alto, intensità legata a scroll-velocity, pausa offscreen, statica con `reduced-motion`) + nome ARDERE in Italiana che emerge da `clip-path` sipario-fiamma (non preloader counter).
  3. Manifesto `#rito` con **scrub parola-per-parola** (colore da spento ad acceso) + parallax fumo (2 layer CSS, lentissimi).
- **Cursore custom:** alone brace (punto caldo + alone radiale che pulsa piano, label `SCORRI / APRI / PRENOTA`).
- **Footer:** brace che si spegne allo scroll (canvas che cala) + orari fittizi + disclaimer demo.

---

### 28 — OFFICINE CALANDRA S.R.L. · Carpenteria metallica e impianti (PMI fittizia)
**Cartella:** `sites/28-calandra/` · **Idea in una frase:** "la S.R.L. come disegno tecnico vivente: blueprint, quote, tolleranze."

- **Brand fittizio:** Officine Calandra S.R.L. — *carpenteria metallica e impianti dal 1978 (fittizio)*. Claim originale: "Ferro dritto, conti dritti." Copy solida-tecnica: reparti fittizi (taglio, piegatura, saldatura, montaggi), parco macchine fittizio, storia 1978→2026 inventata. Ragione sociale con "S.R.L." sempre per esteso nel footer + P.IVA demo `00000000000`.
- **Palette (esatta):**
  `--graphite:#131417` · `--concrete:#E8E6E0` (sfondo chiaro) · `--safety:#FFC400` (giallo sicurezza: solo segnali/CTA, mai sfondi interi) · `--steel:#5B5E63` (testi secondari, tratti) · `--ink:#0A0A0B` · `--blueprint:#1D4ED8` usato SOLO per tratti tecnici su scuro (sottile, non dominante).
- **Tipografia:** display `Oswald 500/600/700` in all-caps (titoli industriali, numeri commessa) · body `Inter Tight 400/500/600` · mono `IBM Plex Mono 400/500/600` (quote, tabelle, targhe). Mai serif.
- **Radius/materiali:** industriale `radius: 2px` quasi-tagliente (targhe, tabelle), `0` su nastri. Materiali: blueprint (griglia + quote + tratteggi SVG), nastro segnaletico (CSS repeating-linear-gradient, sobrio, solo dove serve), lamiera (gradienti lineari freddi), targhetta commessa (bordo 1px + angoli tacchettati). Niente cursori morbidi, niente mesh.
- **Sezioni:** `#hero` (targa + disegno tecnico animato) → `#reparti` (4 reparti fittizi) → `#linea` (PINNED: il pezzo percorre la linea, vedi motion) → `#numeri` (odometri, non counter) → `#strumento` (preventivatore demo: vedi sotto) → `#storia` (timeline 1978→2026 drag/scrub) → `#certificazioni` (solo voci fittizie generiche tipo "processo interno PQ-04" — MAI loghi/certificazioni reali) → `#contatti` (form demo + sede fittizia) → footer S.R.L. completo + disclaimer.
- **Strumento — "Preventivatore demo":** select (lavorazione: taglio/piegatura/saldatura/montaggio) + slider (pezzi 1–500, spessore 1–20mm) + chip (materiale fittizio: S235/S355/Inox demo) → output: fascia prezzo demo (odometro), lead-time fittizio (settimane), distinta base (righe che si aggiungono animate), nota "Stima demo a scopo illustrativo, non offerta commerciale."
- **Signature motion (obbligatorie):**
  1. `#linea` **pinned scrub**: un pezzo (SVG sagoma) percorre una traiettoria a keyframes attraverso 4 stazioni (taglio→piegatura→saldatura→controllo), ogni stazione si attiva (stroke→fill, quota che appare, timbro OK fittizio). Timeline con label, `end: "+=2800"` desktop.
  2. Hero **disegno-tecnico draw-on scrubbed**: blueprint SVG che si disegna (`strokeDashoffset`) con lo scroll + quote che compaiono + timbro commessa che si imprime (`scale` da 1.4→1 con `ease: "power4.in"` secco, una sola volta).
  3. `#storia` timeline 1978→2026 a **scrub orizzontale trascinabile** (bottoni prev/next + drag nativo su track, non solo hover) + `#numeri` con **odometri a rulli** (colonne cifre `yPercent`, feel meccanico).
- **Cursore custom:** crocino tecnico (croce + coordinate mm live in mono + angolo di snap a 45° su hover dei disegni).
- **Apertura:** tendina "serranda" (`clip-path` verticale secca + colpo di timbro), max 1.6s.
- **Footer:** targa S.R.L. completa (ragione sociale, REA fittizio `MI-0000000`, P.IVA demo, PEC fittizia) + disclaimer.

---

### 29 — STUDIO ROTTA · Web design indipendente
**Cartella:** `sites/29-rotta/` · **Idea in una frase:** "lo studio come sala collaudi editoriale: manifesti, prove, scarti."

- **Brand fittizio:** Studio Rotta — *web design editoriale, Milano (fittizio)*. Claim originale: "Siti che si leggono come riviste e convertono come negozi." Copy colta-ironica, prezzi demo a forfait fittizi, 6 case study **fittizi** (nomi inventati, mai clienti reali), sezione "scarti" (esperimenti buttati, divertente e originale).
- **Palette (esatta):**
  `--bone:#F2EFE9` (carta) · `--ink:#0F0F0E` · `--vermilion:#FF3D2E` (segnale: link, asterischi, stati) · `--lilac:#B8A9FF` (evidenziazioni, mai testo su chiaro) · `--line:rgba(15,15,14,.14)`.
- **Tipografia:** display `Syne 700/800` (titoli manifesto, numeri enormi) · body `Instrument Sans 400/500/600` · accento `Instrument Serif italic 400` (solo corsivi dentro i titoli Syne, contrasto colto) · mono `Space Mono 400` (kicker). Sì: 4 famiglie qui sono concesse perché il contrasto Syne/Serif è il gesto dello studio — tienile disciplinate.
- **Radius/materiali:** editoriale-misto: `0` sui manifesti, `14px` su card lavoro, `999px` su chip. Materiali: collage (strati sovrapposti, nastri, asterischi vermilion `*`, note a margine mono), griglia a vista (toggle "mostra griglia" divertente e utile), timbro "BOZZA/APPROVATO" fittizio. Niente lime, niente blueprint, niente brace.
- **Sezioni:** `#hero` (manifesto + indice) → `#lavori` (6 case fittizi + filtri con morph) → `#manifesto` (PINNED scrub parola-per-parola + cambio tinta sfondo) → `#metodo` (4 fasi sovrapposte z-stack) → `#strumento` (stimatore di progetto: vedi sotto) → `#scarti` (3 esperimenti buttati, hover divertenti) → `#prezzi` (3 forfait demo) → `#contatti` (form demo + calendario fittizio) → footer manifesto + disclaimer.
- **Strumento — "Stimatore di progetto":** chip (tipo: landing / sito / e-commerce demo) + slider (pagine 1–40, lingue 1–3) + toggle (copy, CMS fittizio, multilingua) → output: forfait demo (odometro), settimane fittizie, breakdown (barre animate per voce), CTA "Richiedi stima vera" (form demo).
- **Signature motion (obbligatorie):**
  1. `#manifesto` **pinned scrub**: parole che si accendono una per una + tinta di sfondo `--bone→--ink→--bone` guidata dallo scroll + asterisco vermilion che ruota (`rotation: "+=180_cw"`).
  2. `#lavori` con **filtro morph manuale stile-Flip** (misura rect → `fromTo` x/y/scale, non crossfade pigro) + peek-card che segue il cursore con `quickTo` e wipe `clip-path` all'hover (fallback tap su mobile).
  3. Hero **lettere scattered→assemble** (`stagger: {from:"random"}` + `rotation`/`yPercent` su split manuale) + titoli sezione con **skew-da-velocità** + marquee obliquo (`rotation: -2deg`) con `skewX` da `getVelocity()`.
- **Cursore custom:** asterisco `*` vermilion che ruota piano e diventa lente (`APRI / LEGGI / TRASCINA`) sui lavori.
- **Apertura:** lettere scattered che si assemblano + griglia che scatta in posizione (niente counter).
- **Footer:** indice-manifesto gigante con hover wipe + disclaimer.

---

### 30 — ALTROVE · Agenzia di viaggi lenti
**Cartella:** `sites/30-altrove/` · **Idea in una frase:** "l'agenzia come atlante contemplativo: una rotta alla volta, a passo d'uomo."

- **Brand fittizio:** Altrove — *viaggi lenti, 8–21 giorni (fittizio)*. Claim originale: "Meno tappe, più posti." Copy contemplativa, 5 destinazioni **fittizie-ma-plausibili** inventate con toponimi originali (NON luoghi reali spacciati per veri: inventa nomi tipo "Costa delle Nebbie" con nota "destinazione romanzata a scopo dimostrativo" — oppure usa macro-aree reali generiche come "Egeo" senza attribuire strutture/hotel reali). Niente hotel/volti/compagnie reali.
- **Palette (esatta):**
  `--lagoon:#0C2B2E` (profondo laguna, sfondo scuro) · `--sand:#F3EAD8` (sabbia, sfondo chiaro) · `--sun:#E9B44C` (sole: accento caldo) · `--teal:#2A9D8F` (acqua: secondario) · `--ink:#101B1C` · `--line:rgba(16,43,46,.14)` / su scuro `rgba(243,234,216,.16)`.
- **Tipografia:** display `Bricolage Grotesque 500/700/800` (titoli caldi, numeri) · body `Manrope 400/500/600` · mono `Space Mono 400` (coordinate fittizie, durate, kicker). Corsivi sobri, mai urlati.
- **Radius/materiali:** morbido-naturale `radius: 22px` card, `999px` pill, archi su testate destinazione. Materiali: strati di paesaggio (4–5 fasce CSS sovrapposte: cielo/sabbia/mare/profondità), tratteggio rotta (SVG dashed), timbro "partenza fittizia", cartolina (bordo + francobollo CSS disegnato da te). Niente foto: paesaggi astratti a fasce + sole/mare geometrici.
- **Sezioni:** `#hero` (orizzonte a strati + bussola) → `#filosofia` (manifesto lento) → `#rotte` (PINNED atlante: la rotta si disegna, vedi motion) → `#destinazioni` (5 schede romanzate, filtri per passo) → `#strumento` (componi il viaggio: vedi sotto) → `#diari` (3 estratti fittizi) → `#pratico` (accordion: bagagli/ritmi/demo) → `#contatti` (form demo + "chiamata di 20 minuti fittizia") → footer atlante + disclaimer.
- **Strumento — "Componi il viaggio":** slider (giorni 8–21, passo: lento/lentissimo chip) + select (stagione fittizia) + chip (mare/colline/borghi) → output: itinerario fittizio (tappe che si disegnano su mini-rotta SVG), prezzo demo (odometro morbido), impronta "lentezza" (arco che si riempie), nota "Itinerario dimostrativo, non prenotabile."
- **Signature motion (obbligatorie):**
  1. `#rotte` **atlante pinned scrub** (`end: "+=3000"` desktop): rotta SVG che si disegna (`strokeDashoffset`) attraverso 4 tappe, card tappa che si attivano in sequenza (label timeline), bussola che ruota verso ogni tappa (`rotation` direzionale), coordinate mono che scorrono.
  2. Hero **parallasse a strati** (5 fasce paesaggio con `[data-speed]` diversi, scrub dolce) + sole che sorge allo scroll (`yPercent` + `opacity` lenti).
  3. `#destinazioni` **capitoli orizzontali** (mobile: stack verticale; desktop: track orizzontale con `containerAnimation`, `ease: "none"`) + schede con wipe `clip-path` e sole che cambia tinta per destinazione (CSS var `--sun-tint` animata con GSAP).
- **Cursore custom:** bussola (anello + ago che punta verso il movimento del mouse via `quickTo rotation`, label `ESPLORA / APRI`).
- **Apertura:** bussola che si orienta (ago da spinning a nord) + orizzonte che sale da `clip-path` (niente counter).
- **Footer:** mini-atlante che si completa allo scroll + disclaimer "destinazioni romanzate".

---

### 31 — VOLTABIT · Laboratorio computer e reti
**Cartella:** `sites/31-voltabit/` · **Idea in una frase:** "l'informatica come banco da laboratorio: POST, teardown, benchmark."

- **Brand fittizio:** Voltabit — *laboratorio computer & reti per casa e PMI (fittizio)*. Claim originale: "Apriamo le macchine. Chiudiamo i problemi." Copy schietta-da-laboratorio: listini demo (assistenza/assemblaggio/reti), tempi fittizi ("diagnosi in 24h demo"), niente marchi hardware reali (usa sigle inventate: CPU "VX-8", GPU "FX-12", mai Intel/NVIDIA/Apple…).
- **Palette (esatta):**
  `--lab:#0B0E0C` (nero laboratorio) · `--phosphor-paper:#E8F0E8` (carta fosforescente, sfondo chiaro) · `--phosphor:#00E07A` (verde fosforo: accento su scuro) · `--amber:#FFB224` (ambra: warning/CTA) · `--moss:#3A4A40` (superfici) · `--line:rgba(232,240,232,.14)` su scuro.
- **Tipografia:** display `Unbounded 500/700` (titoli tecnici, numeri banco) · body `IBM Plex Sans 400/500/600` · mono `IBM Plex Mono 400/500/700` (PROTAGONISTA: terminale, tabelle, log, prezzi). Il mono qui è cittadino di prima classe, non accessorio.
- **Radius/materiali:** da-banco `radius: 8px` moduli, `4px` chip/log, `0` su nastri terminale. Materiali: CRT phosphor (testo fosforescente + glow sobrio + scanline leggerissima solo nel terminale, non globale), banco (griglia forata CSS), etichette cespiti (codici fittizi `VB-2026-0001`), cavi (SVG bezier colorati sobri). Dark-first: 70% scuro, 30% carta.
- **Sezioni:** `#hero` (terminale POST + banco) → `#servizi` (3 banchi: ripara/assembla/connetti) → `#teardown` (PINNED: esploso della macchina, vedi motion) → `#benchmark` (barre live + FPS meter) → `#strumento` (configuratore PC demo: vedi sotto) → `#listino` (tabella demo con filtri) → `#faq` (accordion tecnico) → `#contatti` (form demo + "porta la macchina" fittizio) → footer terminale + disclaimer.
- **Strumento — "Configuratore PC demo":** select fittizie (CPU VX-4/VX-8/VX-12, GPU FX-6/FX-12, RAM 16/32/64, SSD 1/2/4TB — sigle inventate) + toggle (assemblaggio/collaudo) → output: prezzo demo (odometro phosphor), watt stimati fittizi (barra + numero), livello (chip: UFFICIO/GIOCO DEMO/STUDIO), compatibilità fittizia (check list animata), nota "Sigle e prezzi dimostrativi, nessun hardware reale."
- **Signature motion (obbligatorie):**
  1. `#teardown` **esploso pinned scrub** (`end: "+=2800"` desktop, fallback mobile a stack): 5 strati CSS/SVG della macchina (scocca→dissipatore→scheda→alimentatore→cavi) che si separano in `y` + `rotationX` leggera con `transformPerspective`, etichette che si accendono in sequenza, vite che ruota (`rotation: "+=360"` scrubbed).
  2. Hero **sequenza POST/boot** (timeline con label, max 2s, skippabile, disabilitata con `reduced-motion`): log che si batte a macchina (`steps()`), voci OK fittizie che si spuntano, prompt che lampeggia, ingresso dei pannelli banco. Niente counter 0–100: è una checklist teatrale.
  3. `#benchmark` **barre reactive**: barre che crescono allo scroll + FPS-meter fittizio la cui lancetta trema con `getVelocity()` + log che aggiunge righe mentre scorri (throttled, max 12 righe, `aria-hidden` sul log decorativo + tabella dati vera per screen reader).
- **Cursore custom:** croce da banco + snap a griglia (punto che scatta di 8px, readout `μm` fittizio scherzoso-ma-tecnico, label `APR! / TEST / COMPILA`).
- **Footer:** terminale che "saluta" allo scroll (`> arrivederci_` battuto quando entra in vista) + disclaimer.
- **Nota licenze:** se vuoi traiettorie curve usa keyframes manuali; MotionPathPlugin gratuito solo se sai citarne correttamente CDN+licenza, altrimenti niente.

---

## 9. CHECKLIST DI ACCETTAZIONE — da eseguire self-review su OGNI sito prima di consegnarlo

Segna `[x]` solo ciò che è vero. Se una voce è `[ ]`, correggi prima di consegnare.

**Legale/originalità**
- [ ] Nome brand, copy, prezzi, metriche, testimonianze, toponimi: tutto inventato, nessun marchio/persona/luogo-struttura reale.
- [ ] Zero asset esterni oltre i 3 CDN + Google Fonts; zero hotlink; favicon SVG data-URI propria.
- [ ] Niente plugin GSAP Club; solo core + ScrollTrigger (+ Lenis MIT); licenze rispettate.
- [ ] Footer con disclaimer demo + (dove previsto) P.IVA/tel/indirizzi palesemente demo.
- [ ] Form demo: nessun invio reale, testo "Demo — nessun dato inviato", nessun countdown/badge falso.

**Design**
- [ ] Palette del brief rispettata alla lettera (controlla gli hex); nessun accento extra.
- [ ] Max 3 famiglie font (4 solo per lo Studio Rotta); pesi dichiarati; fallback di sistema.
- [ ] Radius-philosophy del brief coerente ovunque (bottoni/card/chip/input/cursore).
- [ ] Almeno 1 materiale/texture originale mai vista nel Batch A.
- [ ] Cursore custom unico del brief, solo `pointer:fine`, fallback nativo su campi/ touch.
- [ ] `::selection`, focus, hover/active, stati form, scrollbar, tabular-nums dove servono.

**Motion GSAP**
- [ ] Le 3 signature del brief sono implementate e visibili (elencale nel riepilogo con selettori/linee).
- [ ] NESSUNA signature è "preloader counter / fade-up generico / marquee costante / counter piatto / solo magnetic".
- [ ] `matchMedia` desktop/mobile + `prefers-reduced-motion` funzionanti (contenuto leggibile senza motion).
- [ ] Solo transform/opacity animati; `quickTo` per follower; timeline con label/defaults; niente `delay`-chains.
- [ ] ScrollTrigger top-level, `ease:"none"` su containerAnimation, `refresh()` dopo fonts, `markers:false`.

**Strumento interattivo**
- [ ] 3+ controlli + output live animato + `aria-live` + tastierabile + usabile a 360px senza hover.

**Responsive/a11y/perf**
- [ ] Layout integro a 360/768/1280/1600; niente overflow-x; tap-target ≥44px; pinned solo desktop con fallback.
- [ ] Semantica, heading, label, contrasto, focus-trap overlay, Esc chiude, skip-link.
- [ ] Zero errori console; canvas/DPR/pausa-offscreen ok; niente jank su scroll veloce.

**Consegna**
- [ ] Un `index.html` completo per sito, funzionante via server statico, + riepilogo 15 righe (§7).

---

## 10. DIVIETI FINALI — se li violi, rifai

1. Non copiare codice, testi o nomi dal Batch A o da siti reali: ogni riga è scritta da te per questo brief.
2. Non riusare palette/font/cursori/motion del Batch A come protagonisti (§1): sono presi.
3. Non consegnare siti che si assomigliano: 6 concept, 6 voci, 6 regie diverse.
4. Non usare immagini/foto/icone altrui, nemmeno "tanto è una demo".
5. Non inventare certificazioni, enti, premi, partnership reali o recensioni vere.
6. Non superare i CDN consentiti; non aggiungere framework, tracker, analytics, cookie.
7. Non troncare il codice: ogni `index.html` è completo, valido e funzionante.

**Inizia ora dal sito 26 — ALVEO.** Consegnalo completo (codice + riepilogo + checklist segnata), poi attendi il via per il 27.

# ════════════════════════════════════════════════════════════════════
# FINE PROMPT DA INCOLLARE A CLAUDE FABLE 5.1 Max
# ════════════════════════════════════════════════════════════════════

---

## Note per chi incolla (non parte del prompt)

- Il prompt è calibrato sul Batch A reale della repo (palette/font/motion esistenti) e sulle
  best practice GSAP ufficiali (matchMedia, quickTo, containerAnimation `ease:"none"`, transform-only).
- Se Claude propone nomi diversi da quelli fittizi suggeriti, va bene purché restino originali e verifichi che non collidano con marchi reali.
- Alloy (consiglio operativo): un sito alla volta, file interi, mai "continua dopo" a metà file.
- Licenze output: codice originale MIT come la repo; font/librerie restano dei rispettivi titolari via CDN.
