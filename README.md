¨SUPSI 2026  
Corso d’interaction design, CV429.01  
Docenti: A. Gysin, G. Profeta  

Progetto 1: La conquista dello spazio

# Titolo progetto
Autore: Riccardo Vosti \
[Titolo progetto](https://riccardovosti.github.io/TESTGRAVITY/)


## Introduzione e tema
Questo progetto è un'avventura web interattiva in pixel-art dedicata al Programma Artemis della NASA. È un omaggio all'esplorazione spaziale che mette l'utente al centro dell'azione, trasformandolo in una recluta pronta per il ritorno dell'umanità sulla Luna.
Il gioco è un vero e proprio simulatore di addestramento astronautico. Sotto la guida del Dr. Aris, il giocatore deve affrontare e superare un percorso in sei fasi basato sui reali test della NASA.


## Riferimenti progettuali
Dolor sit amet consectetur adipiscing elit duis tristique. Sociis natoque penatibus et magnis dis parturient montes nascetur. Est sit amet facilisis magna. Tellus rutrum tellus pellentesque eu. Dictum sit amet justo donec enim. Aliquam malesuada bibendum arcu vitae elementum curabitur vitae. Sed faucibus turpis in eu mi bibendum neque egestas congue. Tellus in metus vulputate eu scelerisque felis imperdiet proin. Dolor magna eget est lorem ipsum dolor. Sit amet mattis vulputate enim nulla. Elit pellentesque habitant morbi tristique senectus et. Vestibulum mattis ullamcorper velit sed ullamcorper morbi tincidunt ornare massa.


## Design dell’interfaccia e modalità di interazione
Il design dell'**Artemis Training Simulator** nasce dall'incrocio tra *gamification* e divulgazione scientifica, con l'obiettivo primario di abbassare la barriera d'ingresso a contenuti aerospaziali complessi.

Le scelte progettuali si basano su:

- 🕹️ **Task-based Gameplay (es. *Among Us*, *Google Doodles*):** Ho strutturato l'interazione per micro-task. Dividere l'esperienza in minigiochi brevi abbassa il carico cognitivo dell'utente e mantiene alto l'engagement, trasformando subito la teoria in un'azione pratica (*learning by doing*).

- 👾 **Pixel-Art Funzionale:** L'estetica guarda ai platform indie e ai retro-game anni '90. Oltre all'effetto nostalgia, è una precisa scelta di *usabilità*: semplifica visivamente ambienti enormi (come la centrifuga o la piscina N.B.L.), chiarisce l'*affordance* degli elementi interattivi e garantisce ottime performance di caricamento sul browser.

- 🖥️ **Sci-Fi Minimal UI:** Per l'interfaccia utente mi sono ispirato ai veri terminali di controllo delle stazioni spaziali. Colori ad alto contrasto (bianco su nero), font squadrati e finestre modali grezze. Questo garantisce accessibilità e coerenza visiva, favorendo l'immersione dell'utente senza distrarlo dal core loop del gioco.

- 🏛️ **Reward System e Museo Virtuale:** Il flusso utente è pensato come un *funnel*. Il videogioco fa da "esca" per catturare l'attenzione; una volta completata la sfida, l'utente riceve come *reward* l'accesso a un archivio interattivo in stile museo virtuale, sbloccando i veri filmati storici della NASA corrispondenti alle prove appena superate.



## Tecnologia usata
Il progetto è stato sviluppato interamente come applicazione web client-side, senza l'uso di framework complessi per la UI (come React o Vue), per mantenere il codice leggero e incentrato sulle performance di gioco.

Le tecnologie principali includono:

- 🎮 **Phaser 3 (Arcade Physics):** Il vero motore del progetto. Ho utilizzato questa potente libreria JavaScript per gestire il *core loop* del gioco, la fisica 2D (gravità, collisioni, bounding box), il rendering degli sprite in pixel-art, le animazioni e la gestione della camera dinamica.
- 🌐 **HTML5 & CSS3:** Utilizzati per strutturare e stilizzare tutta l'interfaccia utente (HUD), i menu di navigazione, i popup modali e le finestre di dialogo. Le transizioni fluide e le cinematiche (come il testo a scorrimento e il decollo dell'astronave) sono realizzate interamente tramite animazioni CSS (keyframes).
- 🟨 **Vanilla JavaScript (ES6):** Sfruttato per manipolare il DOM in tempo reale, gestire la logica dei quiz e coordinare il passaggio di stato tra i vari livelli. 
- 💾 **Web Storage API (localStorage e la sessionStorage):** Fondamentali per la *data persistence*. Permettono di salvare il nome dell'utente, calcolare il timer globale tra le diverse pagine HTML e gestire la continuità della colonna sonora (evitando che la musica riparta da zero ad ogni cambio livello).
- 🎨 **HTML5 Canvas API:** Utilizzata nativamente (al di fuori di Phaser) nelle schermate di transizione per generare sistemi particellari leggeri e performanti (come lo sfondo stellato e le fiamme dei motori).
- 🔊 **HTML Audio API:** Per la gestione dinamica degli effetti sonori spaziali e della musica di background, con logiche anti-blocco per le policy di autoplay dei browser moderni.


## Target e contesto d’uso
**Target: Studenti delle Scuole Medie (11-14 anni)**
Ho scelto questa fascia d'età perché concetti complessi come la microgravità o l'attrito aerodinamico risultano spesso troppo astratti se affrontati solo sui libri. Trattandosi di nativi digitali, la *gamification* è il linguaggio più diretto per mantenere alta la loro attenzione e tradurre la teoria in pratica (*learning by doing*).

**Contesto d'Uso: Edutainment**
L'app è *browser-based* (nessuna installazione richiesta) e si presta a diversi scenari:
- **In classe:** Come supporto interattivo per i docenti durante le lezioni di scienze.
- **A casa:** Per trasformare lo studio autonomo in una sfida gratificante.
- **Eventi STEM:** Come *exhibit* digitale per incuriosire i ragazzi durante open-day o fiere scientifiche.

**Approccio Didattico**
Il design usa il videogioco come "cavallo di Troia" per l'apprendimento. L'errore non è mai punitivo, ma diventa un *feedback* visivo che spiega le leggi della fisica (es. sbagliare il minigioco della centrifuga fa svenire il personaggio, spiegando cos'è la forza G). Questo prepara i ragazzi cognitivamente, rendendoli curiosi e pronti ad assimilare i veri filmati storici della NASA sbloccati alla fine dell'esperienza.

