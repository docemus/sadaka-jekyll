# SADAKA Charity Site

Questo repository contiene il [SADAKA Charity Site](https://docemus.github.io/webtest/), un template responsive per enti benefici e non-profit realizzato con Jekyll e GitHub Pages. Il sito è basato su Bootstrap, Font Awesome e Owl Carousel ed è stato strutturato in maniera modulare per facilitare la manutenzione e l'aggiornamento dei contenuti.

--------------------------------------------------
## Struttura del Progetto

Il repository è organizzato in modo da separare il layout, i componenti e gli assets:

my-jekyll-site/  
├── _config.yml          # Configurazione principale di Jekyll  
├── Gemfile              # Definizione delle dipendenze (incluso github-pages)  
├── _layouts/  
     └── default.html     # Layout principale usato da tutte le pagine  
├── _includes/           # Include modulari per facilitare la manutenzione  
     ├── head.html                # Meta tag, CSS, fonts e script in head  
     ├── header.html              # Header e navbar del sito  
     ├── carousel.html            # Carousel per la homepage  
     ├── about_us.html            # Sezione "About Us"  
     ├── home_reasons.html        # Sezione "Home Reasons" (con variabili esternalizzate)  
     ├── our_causes.html          # Sezione "Our Causes" (con progress bar ed info)  
     ├── our_sponsors.html        # Sezione "Our Sponsors" (lista di loghi in carousel)  
     ├── donate_modal.html        # Modal per la donazione  
     ├── footer-top.html          # Parte superiore del footer (placeholder)  
     ├── footer-main.html         # Parte centrale del footer (About, Tweets, Contact)  
     ├── footer-bottom.html       # Parte inferiore del footer (credits e link)  
     └── footer.html              # Include principale del footer che riunisce le tre parti  
├── index.md               # Pagina principale in formato Markdown con front matter per i contenuti testuali  
└── assets/  
    ├── css/               # File CSS (Bootstrap, Font Awesome, Owl Carousel, style.css)  
    ├── js/                # Script JavaScript (jQuery, Bootstrap, Owl Carousel, main.js)  
    └── images/            # Immagini ed icone usate dal sito (icons, slider, causes, sponsors, ecc.)

--------------------------------------------------
## Come è Stato Realizzato

- **Jekyll:** Usato per generare il sito statico. Il file di configurazione (_config.yml_) consente di parametrizzare il sito (ad esempio, url e baseurl).
  
- **Layout e Include:** Il layout principale (in _layouts/default.html_) include file modulari (nella cartella _includes_) per header, carousel, sezioni di contenuto, footer e modali.
  
- **Contenuti Esternalizzati:** I testi della homepage sono gestiti tramite il front matter di index.md. Ciò permette di modificare i contenuti testuali senza alterare la struttura HTML: negli include si utilizzano le variabili (es. {{ page.carousel_slide1_title }}) con un eventuale fallback tramite il filtro default.
  
- **Design Responsive:** Grazie a Bootstrap il template è responsive e si adatta sia a dispositivi mobili sia a desktop.
  
- **Interattività:** Owl Carousel viene usato per il carosello della homepage e per la sezione sponsor, mentre il modal di donazione sfrutta il JavaScript di Bootstrap.

--------------------------------------------------
## Configurazione per GitHub Pages

Il sito è pubblicato all'indirizzo:  
https://docemus.github.io/webtest/

Pertanto, il file _config.yml_ è configurato come segue:

title: "SADAKA Charity Site"  
description: "Charity / Non-profit responsive Bootstrap Jekyll template."  
baseurl: "/webtest"       # La sottocartella in cui è ospitato il sito  
url: "https://docemus.github.io"      # Il dominio base

--------------------------------------------------
## Come Testare il Sito in Locale

1. **Prerequisiti:**  
   Assicurati di avere Ruby e Bundler installati.

2. **Installa le dipendenze:**  
   Esegui "bundle install" nella cartella del progetto.

3. **Avvia il server Jekyll:**  
   Esegui "bundle exec jekyll serve".

4. **Visualizza il sito:**  
   Apri il browser ed accedi a http://localhost:4000.

--------------------------------------------------
## Come Effettuare il Push su GitHub

1. **Inizializza la repository (se non già fatto):**  
   Esegui "git init", poi "git add ." e "git commit -m 'Initial commit'".

2. **Aggiungi il remote (sostituisci con l'URL del tuo repository):**  
   Esegui "git remote add origin https://github.com/docemus/webtest.git".

3. **Fai il push sul branch principale:**  
   Esegui "git branch -M main" e "git push -u origin main".

Nota: GitHub non permette più l'uso della password in chiaro per le operazioni Git tramite HTTPS. Utilizza un Personal Access Token (PAT) oppure configura l'autenticazione SSH se ti viene richiesta la password.

--------------------------------------------------
## Contributi

Se desideri contribuire al progetto:
- Forka il repository.
- Crea un branch per la tua feature (ad esempio "git checkout -b my-feature").
- Esegui i commit con le tue modifiche.
- Esegui il push sul branch e apri una pull request.

--------------------------------------------------
## Licenza

Questo progetto è distribuito sotto la Licenza MIT.

--------------------------------------------------
## Contenuti Esternalizzati nel Front Matter (index.md)

Il file index.md contiene il front matter per esternalizzare i testi di tutte le sezioni (Carousel, About Us, Home Reasons, Our Causes, Our Sponsors). Ad esempio, il front matter include variabili come:

layout: default  
title: "Home"  

-- Carousel --  
carousel_slide1_title: "Because they need your help"  
carousel_slide1_subtitle: "Do not let them down"  
carousel_slide2_title: "Together we can improve their lives"  
carousel_slide2_subtitle: "So let's do it!"  
carousel_slide3_title: "A penny is a lot of money, if you have not got a penny."  
carousel_slide3_subtitle: "You can make the difference!"

-- About Us --  
about_us_our_mission_text: "Lorem ipsum dolor sit amet, consectetur adipisscin elit..."  
about_us_make_donations_text: "Lorem ipsum dolor sit amet..."  
about_us_help_support_text: "Lorem ipsum dolor sit amet..."  
about_us_our_programs_text: "Lorem ipsum dolor sit amet..."

-- Home Reasons --  
home_reasons_reason1_title: "We fight together"  
home_reasons_reason1_subtitle: "We are humans"  
home_reasons_reason1_paragraphs: "Contenuto per la ragione 1..."  
home_reasons_reason2_title: "We care about others"  
home_reasons_reason2_subtitle: "We are humans"  
home_reasons_reason2_paragraphs: "Contenuto per la ragione 2..."

-- Our Causes --  
our_causes_title: "Our Causes"  
our_causes_cause1_title: "HUNGER AND POVERTY"  
our_causes_cause1_progress: "10$ / 500$"  
our_causes_cause1_details: "Dettagli per Hunger and Poverty..."  
our_causes_cause2_title: "EDUCATION AND TRAINING"  
our_causes_cause2_progress: "400$ / 700$"  
our_causes_cause2_details: "Dettagli per Education and Training..."  
our_causes_cause3_title: "HUMAN RIGHTS"  
our_causes_cause3_progress: "400$ / 1000$"  
our_causes_cause3_details: "Dettagli per Human Rights..."  
our_causes_cause4_title: "ARTS AND CULTURE"  
our_causes_cause4_progress: "400$ / 700$"  
our_causes_cause4_details: "Dettagli per Arts and Culture..."

-- Our Sponsors --  
our_sponsors_title: "Our Sponsors"

Nel corpo del file index.md, sono inclusi i seguenti include:

{% include carousel.html %}  
{% include about_us.html %}  
{% include home_reasons.html %}  
{% include our_causes.html %}  
{% include our_sponsors.html %}

--------------------------------------------------
Questo README fornisce una panoramica completa sul contenuto e sulla configurazione del repository, illustrando come è stato realizzato il sito, come testarlo, come effettuare il push su GitHub e come contribuire al progetto.
--------------------------------------------------

Puoi personalizzare ulteriormente questo file in base alle tue esigenze.
