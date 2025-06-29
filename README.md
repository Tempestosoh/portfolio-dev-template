
# Portfolio Professionale - Template Moderno

Questo è un template di portfolio professionale moderno, progettato per essere facilmente personalizzabile e mostrare le tue competenze, progetti ed esperienze in modo accattivante.

## 🎯 A Chi è Rivolto Questo Template?

Questo template è ideale per:

* **Sviluppatori e Designer:** Presenta i tuoi progetti e le tue capacità tecniche o creative.
* **Freelance:** Mostra i tuoi servizi, le recensioni dei clienti e un chiaro invito all'azione per nuovi incarichi.
* **Professionisti di Varie Discipline:** Adatta le sezioni per esporre le tue esperienze, le pubblicazioni, i successi o qualsiasi altra informazione rilevante per la tua carriera.
* **Studenti e Neolaureati:** Un ottimo punto di partenza per creare la tua prima presenza online e presentare i tuoi progetti accademici o personali.

L'obiettivo è fornire una base solida e stilisticamente moderna che puoi adattare rapidamente al tuo brand personale.

## 🚀 Guida Rapida all'Avvio

### 1. Scaricare il Template da GitHub

Per iniziare a lavorare sul template, devi prima scaricarlo sul tuo computer. Hai due opzioni principali:

* **Clonare il Repository (consigliato per sviluppatori):**
    Se hai Git installato, puoi clonare il repository in locale tramite la riga di comando. Questo ti permetterà di tenere traccia delle modifiche e contribuire (se il repository è pubblico e lo permettesse).
    Apri il tuo terminale o prompt dei comandi e digita:
    ```bash
    git clone [https://github.com/](https://github.com/)[NomeUtente]/[NomeRepositoryDelTemplate].git
    # Esempio: git clone [https://github.com/tempestosoh/my-portfolio-template.git](https://github.com/tempestosoh/my-portfolio-template.git)
    ```
    Sostituisci `[NomeUtente]` e `[NomeRepositoryDelTemplate]` con i dati effettivi del repository da cui stai scaricando il template.

* **Scaricare come ZIP:**
    Vai alla pagina del repository su GitHub. Cerca il pulsante verde "Code" e clicca su "Download ZIP". Questo scaricherà una copia compressa dell'intero progetto che potrai estrarre sul tuo computer.

Dopo aver scaricato ed estratto i file, apri la cartella del template. Il file principale su cui lavorerai sarà `index.html` (o `esempio.html`, se lo hai rinominato).

## 🛠️ Come Modificare il Template

Per rendere questo template **tuo**, segui queste istruzioni passo-passo. Assicurati di aprire il file `index.html` (o `esempio.html`, a seconda di come hai nominato la pagina principale del tuo progetto) con un editor di testo (come VS Code, Sublime Text, o Notepad++).

### 1. Informazioni Base

* **Titolo della Pagina (Browser Tab):**
    Cerca il tag `<title>` nell' `<head>` del documento:
    ```html
    <title>Lorem Ipsum - Portfolio Esempio</title>
    ```
    Sostituisci `Lorem Ipsum - Portfolio Esempio` con il tuo nome e una breve descrizione, ad esempio `[Il Tuo Nome] - Portfolio Professionale`.

* **Favicon:**
    Cerca il tag `<link rel="icon">` nell' `<head>`:
    ```html
    <link href="assets/images/profile.jpg" rel="icon" type="image/png"/>
    ```
    Sostituisci `assets/images/profile.jpg` con il percorso alla tua immagine favicon (preferibilmente un file `.png` o `.ico`).

### 2. Contenuti Testuali

Tutti i testi di esempio (Lorem Ipsum) sono sparsi nel file HTML. Puoi trovarli e modificarli direttamente:

* **Logo (Navbar):**
    ```html
    <div class="logo">Lorem Ipsum</div>
    ```
    Cambia `Lorem Ipsum` con il tuo nome o il nome del tuo brand.

* **Sezione Hero (Home):**
    * **Titolo Principale:** Cerca il tag `<div>` con classe `title`.
        ```html
        <div class="title">Lorem ipsum dolor sit <span class="highlight">amet.</span></div>
        ```
        Modifica il testo `Lorem ipsum dolor sit amet.` e il testo evidenziato all'interno di `<span class="highlight">`.
    * **Sottotitolo Dattiloscritto (`typed.js`):**
        Il testo che appare con l'effetto macchina da scrivere è definito nello script alla fine del file HTML. Cerca la sezione `Typed.js`:
        ```javascript
        strings: ["Lorem Ipsum", "Dolor Sit Amet", "Consectetur Adipiscing", "Sed Do Eiusmod", "Tempor Incididunt"],
        ```
        Modifica gli array di stringhe con le tue competenze o ruoli (es. `"Web Developer"`, `"UI/UX Designer"`).
    * **Descrizione Hero:** Cerca il tag `<p>` con classe `description` subito sotto il sottotitolo.
        ```html
        <p class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
        ```
        Sostituisci il testo con una tua introduzione.

* **Sezioni Generiche:**
    Ogni sezione (`<section>`) ha un titolo (`<h2>`) e spesso un paragrafo descrittivo (`<p class="description">`).
    Cerca gli `<h2>` e i `<p class="description">` all'inizio di ogni sezione per personalizzare i titoli e le introduzioni.

* **Contenuti Specifici delle Sezioni:**
    * **Chi Siamo (`#about`):** Modifica i valori numerici (`<div class="about-value">`) e le etichette (`<div class="about-label">`) nella griglia.
    * **Servizi (`#skills`):**
        Questa sezione è perfetta per elencare le tue competenze o i servizi che offri.
        Ogni singola skill è racchiusa in un blocco `<div class="skill-card">`.
        ```html
        <div class="skill-card">
            <i class="fas fa-laptop-code"></i> <h3>Sviluppo Web</h3> <p>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur...</p> </div>
        ```
        * Per **modificare** una skill: cambia il testo dell' `<h3>`, il paragrafo `<p>` e l'icona (`<i class="fas fa-..."></i>`). Puoi trovare una vasta gamma di icone su [Font Awesome Cheatsheet](https://fontawesome.com/v5/cheatsheet).
        * Per **aggiungere** una skill: copia l'intero blocco `<div class="skill-card">...</div>` e incollalo all'interno del `div` con classe `skills-grid`, poi personalizzalo.
        * Per **rimuovere** una skill: semplicemente elimina l'intero blocco `<div class="skill-card">...</div>` della skill che non ti interessa.
    * **Portfolio (`#projects`):** Per ogni `.project-item`, modifica il titolo (`<h3>`) e la descrizione (`<p>`) nell'overlay.
    * **Recensioni (`#testimonials`):** In ogni `.testimonial-card`, modifica la citazione (`<p class="testimonial-quote">`), il nome dell'autore (`<strong>`) e il suo ruolo/azienda (`<span>`).
    * **FAQ (`#faq`):** Modifica le domande (`<div class="faq-question">`) e le risposte (`<p>`) all'interno di ogni `.faq-item`.

### 3. Immagini

* **Immagine Profilo/Logo:**
    Cerca `src="assets/images/profile.jpg"` nella navbar e nel preloader. Sostituisci questo percorso con la tua immagine profilo.

* **Immagini Progetti:**
    Nella sezione portfolio (`#projects`), ogni `.project-item` ha un tag `<img>`:
    ```html
    <img src="assets/images/project1.jpg" alt="Progetto Esempio 1"/>
    ```
    Sostituisci `assets/images/project1.jpg` (e `project2.jpg`, `project3.jpg` ecc.) con i percorsi alle immagini dei tuoi progetti. Le immagini placeholder (`https://via.placeholder.com/...`) vanno anch'esse sostituite. Ricorda di aggiornare anche il testo `alt` per l'accessibilità.

* **Immagini Testimonial:**
    Nella sezione recensioni (`#testimonials`), ogni `.testimonial-author` ha un tag `<img>`:
    ```html
    <img src="[https://via.placeholder.com/60x60?text=C1](https://via.placeholder.com/60x60?text=C1)" alt="Testimonial 1"/>
    ```
    Sostituisci `https://via.placeholder.com/60x60?text=C1` con le immagini dei tuoi clienti.

### 4. Link e Riferimenti Esterni

* **Navbar Links:** I link della navbar (`<a class="nav-link-item" href="#sezione">`) puntano a sezioni interne alla pagina (es. `#about`, `#skills`). Non dovrebbero aver bisogno di modifiche a meno che tu non cambi gli ID delle sezioni.
* **CTA Buttons (Call To Action):**
    * Il pulsante "Scopri di Più" nella sezione Hero:
        ```html
        <a class="cta-button" href="#projects">Scopri di Più</a>
        ```
        Puoi cambiare `href="#projects"` per farlo puntare a un'altra sezione se preferisci.
    * I pulsanti "Vedi Progetto" nella sezione Portfolio:
        ```html
        <a class="view-project-btn" href="[https://www.example.com/project1](https://www.example.com/project1)" target="_blank">Vedi Progetto</a>
        ```
        Sostituisci `https://www.example.com/project1` con il link al tuo progetto reale. Mantieni `target="_blank"` per aprirlo in una nuova scheda.
    * Pulsanti di Contatto:
        ```html
        <a class="cta-button" href="mailto:info@example.com"><i class="fas fa-envelope"></i> Invia una Email</a>
        <a class="cta-button" href="[https://www.linkedin.com/company/lorem-ipsum-studio](https://www.linkedin.com/company/lorem-ipsum-studio)" target="_blank"><i class="fab fa-linkedin"></i> LinkedIn</a>
        <a class="cta-button" href="[https://github.com/lorem-ipsum-dev](https://github.com/lorem-ipsum-dev)" target="_blank"><i class="fab fa-github"></i> GitHub</a>
        ```
        Modifica l'indirizzo email in `mailto:` e gli URL per LinkedIn e GitHub (o altri social/siti) con i tuoi.

### 5. Stile e Colori (CSS)

I colori principali del template sono definiti tramite variabili CSS all'inizio del blocco `<style>` nell' `<head>`:

```css
        :root {
            --bg-dark: #0a0a0a; /* Nero profondo */
            --text-light: #F0F0F0; /* Grigio chiaro */
            --primary-accent: #00FF99; /* Verde neon */
            --secondary-accent: #00BFFF; /* Blu chiaro */
            --border-color: #222222; /* Grigio scuro per bordi */
            --shadow-color-primary: rgba(0, 255, 153, 0.4); /* Ombra per verde neon */
            --shadow-color-secondary: rgba(0, 191, 255, 0.4); /* Ombra per blu chiaro */
        }
````

Puoi facilmente modificare questi valori esadecimali (es. `#00FF99`) per cambiare lo schema di colori dell'intero sito. Per le ombre, assicurati di aggiornare anche i valori `rgba()`.

### 6\. Animazioni e JavaScript (Avanzato)

Il template utilizza diverse librerie JavaScript per le animazioni e le interazioni:

  * **`typed.js`:** Già menzionato per il sottotitolo della sezione Hero. Modifica le `strings` come spiegato sopra.
  * **`Three.js`:** Crea l'animazione di sfondo con le particelle. Se non desideri questa animazione, puoi rimuovere il tag `<canvas id="bg-canvas"></canvas>` dalla sezione `<header>` e i relativi script `initThreeJS()`, `animateThreeJS()`, `onWindowResizeThreeJS()` nel blocco `<script>` alla fine del file, e la linea `<script src="https://unpkg.com/three@0.152.2/build/three.min.js"></script>`.
  * **`GSAP` (GreenSock Animation Platform):** Utilizzato per le animazioni di entrata degli elementi allo scroll. Se desideri personalizzare o rimuovere queste animazioni, dovrai familiarizzare con la sintassi GSAP nello script. Per disattivare tutte le animazioni GSAP, puoi rimuovere i tag `<script>` relativi a GSAP e ScrollTrigger nell' `<head>` e nel `<body>`, e rimuovere la classe `gsap-active` dalle sezioni.
  * **Carosello Testimonial e FAQ Accordion:** La logica per queste funzionalità è scritta in JavaScript nativo alla fine del file. Se hai bisogno di modificare il loro comportamento (es. velocità dello scorrimento automatico, come si aprono le FAQ), puoi intervenire direttamente lì.

### 7\. Aggiungere Nuove Sezioni (es. "Curiosità")

Vuoi aggiungere una sezione personalizzata come "Curiosità"? Ecco come fare:

1.  **Scegli una sezione di base:** Puoi copiare l'intera struttura di una sezione esistente, come la sezione "About" o "Skills", per mantenere la coerenza stilistica.
2.  **Copia il codice HTML:** Trova un blocco `<section>` esistente e copialo. Ad esempio, copia l'intera sezione "About":
    ```html
    <section class="about-section gsap-active" id="about">
        </section>
    ```
3.  **Incolla e rinomina:** Incolla il codice copiato dove desideri che appaia la nuova sezione nel tuo `index.html`.
4.  **Assegna un ID univoco:** Cambia l'`id` della nuova sezione per renderlo unico (es. `id="curiosita"`). Questo ID sarà usato per il link nella navbar.
    ```html
    <section class="general-section gsap-active" id="curiosita">
        <h2>Le Mie <span class="highlight">Curiosità</span></h2>
        <p class="description">Qui puoi raccontare qualcosa di divertente o interessante su di te che non rientra nelle altre categorie.</p>
        </section>
    ```
5.  **Aggiorna il titolo e la descrizione:** Modifica l'`<h2>` e il `<p class="description">` con il testo desiderato per la tua nuova sezione.
6.  **Aggiungi il link nella Navbar:** Per rendere la nuova sezione accessibile, devi aggiungere un link nella tua barra di navigazione. Trova il `div` con classe `nav-links` e aggiungi un nuovo `<a>` tag con l'`href` che corrisponde all'ID della tua nuova sezione:
    ```html
    <div class="nav-links" id="nav-links">
        <a class="nav-link-item" href="#home">Home</a>
        <a class="nav-link-item" href="#curiosita">Curiosità</a>
        <a class="nav-link-item" href="#contact">Contatti</a>
    </div>
    ```

-----

## 🔒 Diritti e Attribuzione

Questo template è stato creato e fornito da **tempestosoh**.

Si prega di **non modificare** la riga relativa al copyright nel footer e di mantenere l'attribuzione a "tempestosoh" (o al nome utente/link fornito nel template originale) come segno di riconoscimento e rispetto per il lavoro svolto. La riga è la seguente:

```html
<footer>
    <p>© 2025 Lorem Ipsum Studio. Tutti i diritti riservati.</p>
    <p>Powered by <a href="[https://www.example.com](https://www.example.com)" target="_blank">Lorem Ipsum Developers</a></p>
</footer>
```

Nel tuo utilizzo, dovresti mantenere almeno la parte `Powered by <a href="[link_a_tempestosoh]" target="_blank">tempestosoh</a>` o una dicitura simile, anche se personalizzi il resto del footer.

-----

## 🚀 Utilizzare il Template con GitBook

Se desideri pubblicare questo portfolio utilizzando GitBook, ecco come puoi fare:

1.  **Crea un Nuovo Repository GitHub:**

      * Se non l'hai già fatto, crea un nuovo repository su GitHub (es. `my-portfolio`).

2.  **Inizializza il tuo Progetto GitBook:**

      * Assicurati di avere GitBook CLI installato (se stai lavorando localmente).
      * Crea una cartella per il tuo progetto GitBook.

3.  **Copia il Codice HTML del Template:**

      * La pagina di esempio Lorem Ipsum che ti ho fornito (e che hai modificato) si chiama `esempio.html` (o il nome con cui l'hai salvata).
      * **Apri il file `esempio.html` (o `index.html` del tuo template modificato) con un editor di testo.**
      * **Seleziona e copia l'intero contenuto del file** (tutto, dal `<!DOCTYPE html>` fino alla fine del tag `</html>`).

4.  **Incolla il Codice in `index.html` (o `README.md`) del tuo GitBook:**

      * All'interno della cartella del tuo progetto GitBook, devi avere un file HTML principale. Convenzionalmente, questo potrebbe essere `index.html`.
      * **Incolla l'intero codice HTML copiato direttamente nel file `index.html`** (crealo se non esiste) nella root del tuo progetto GitBook.
      * Se invece vuoi integrare solo alcune parti o se il tuo GitBook è principalmente basato su Markdown, dovrai estrarre sezioni specifiche e inserirle nei tuoi file `.md` o `SUMMARY.md`, ma per avere la pagina intera funzionante come un sito web, il modo più semplice è usare `index.html`.

5.  **Copia le Risorse (Immagini, Font, ecc.):**

      * Il template fa riferimento a una cartella `assets/images/`. Assicurati di copiare l'intera cartella `assets` (con tutte le sue sottocartelle e file) nella root del tuo progetto GitBook, allo stesso livello del tuo `index.html`.
      * Verifica che i percorsi delle immagini e degli altri asset nel tuo `index.html` siano corretti rispetto alla nuova struttura.

6.  **Configura GitBook (opzionale ma consigliato):**

      * Crea un file `book.json` nella root del tuo progetto GitBook per configurare plugin, temi, ecc. Per un portfolio a pagina singola, potresti non aver bisogno di molte configurazioni.

7.  **Pubblica il tuo GitBook:**

      * Se stai usando la GitBook CLI, esegui `gitbook build` per generare il sito statico, poi puoi caricarlo su un servizio di hosting come GitHub Pages.
      * Se stai usando la piattaforma GitBook, segui le loro istruzioni per collegare il tuo repository GitHub e pubblicare il tuo libro.

Seguendo questi passaggi, il tuo template di portfolio sarà online e pronto per essere mostrato\!

-----

Spero che questo tutorial esteso sia ora molto più utile per il tuo progetto e la gestione dei diritti\!

```
```
