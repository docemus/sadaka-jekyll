# Sadaka 1.0 Jekyll Port

Il progetto **Sadaka 1.0 Jekyll Port** rappresenta un lavoro di porting del template HTML statico **Sadaka 1.0**, originariamente sviluppato per siti di beneficenza e organizzazioni no-profit, disponibile gratuitamente su [Free CSS](https://www.free-css.com/free-css-templates/page197/sadaka-1.0). L'obiettivo principale è stato quello di trasformare il template originale in una struttura compatibile con **Jekyll**, un generatore di siti statici ampiamente utilizzato per creare blog e siti web flessibili e moderni.

## Introduzione

Sadaka 1.0 è stato concepito come un template HTML statico con un design elegante e pulito, ma essendo statico, presentava limitazioni in termini di scalabilità, manutenzione e personalizzazione. Il lavoro di porting si è concentrato su:

1. **Adattamento strutturale**: Conversione degli elementi statici in layout, inclusioni e componenti riutilizzabili tipici di Jekyll, al fine di rendere il template modulare e facilmente gestibile.
2. **Organizzazione dei contenuti**: Creazione di cartelle standard di Jekyll come `_posts`, `_layouts`, `_includes` e `_data`, per semplificare l'aggiunta e la gestione di contenuti dinamici.
3. **Configurazione personalizzabile**: Implementazione di un file `_config.yml` che consente agli utenti di personalizzare parametri globali del sito, come titolo, descrizione, URL, social media e molto altro.
4. **Ottimizzazione**: Miglioramento della compatibilità con i moderni flussi di lavoro, come il deploy su piattaforme di hosting per siti statici (ad esempio, GitHub Pages).

Il risultato finale è un sito web flessibile, facilmente modificabile, pronto per essere esteso e adattato alle esigenze specifiche dell'utente o dell'organizzazione.

## Caratteristiche principali

- **Template modulare**: Gli elementi ripetuti (header, footer, sezioni comuni) sono stati suddivisi in file `_includes` per semplificare la gestione.
- **Supporto per post dinamici**: Grazie alla cartella `_posts`, è possibile gestire facilmente articoli e aggiornamenti tramite i file Markdown.
- **Personalizzazione intuitiva**: La maggior parte delle configurazioni può essere gestita centralmente attraverso `_config.yml`.
- **Compatibilità con hosting moderni**: Il sito è pronto per essere distribuito su piattaforme come GitHub Pages, Netlify o Vercel.

## Prerequisiti

Prima di iniziare, assicurati di avere installato:
- **Ruby** (versione 2.5 o superiore)
- **Bundler** (gestore di dipendenze per Ruby)
- **Jekyll** (puoi installarlo eseguendo `gem install jekyll`)

## Installazione

1. Clona il repository:
   ```bash
   git clone [<URL_DEL_TUO_REPOSITORY>] (https://github.com/docemus/sadaka-jekyll.git)
   cd sadaka-jekyll
   ```

2. Installa le dipendenze necessarie:
   ```bash
   bundle install
   ```

## Avvio del server in locale

1. Avvia il server Jekyll:
   ```bash
   bundle exec jekyll serve
   ```

2. Apri il tuo browser e visita:
   ```
   http://localhost:4000
   ```

## Struttura del progetto

Ecco una panoramica delle principali directory del progetto:
- `_includes`: Contiene componenti HTML riutilizzabili come header e footer.
- `_layouts`: Contiene i layout principali del sito, come `default` e `page`.
- `_posts`: Directory per la gestione di articoli e post dinamici.
- `_sass`: File di stile Sass per semplificare la gestione del CSS.
- `assets`: Contiene risorse statiche come immagini, file CSS e script JavaScript.

## Deploy

1. Compila il sito per la produzione:
   ```bash
   bundle exec jekyll build --destination _site
   ```

2. Carica i file generati nella cartella `_site` sul tuo hosting.

## Considerazioni finali

Questo porting rappresenta un esercizio di modernizzazione di un template statico, trasformandolo in uno strumento flessibile e scalabile grazie alle potenzialità di Jekyll. Il progetto è ideale per chi desidera un sito elegante e professionale con un focus su facilità di manutenzione e personalizzazione.

## Licenza

Il template originale **Sadaka 1.0** è fornito gratuitamente da [Free CSS](https://www.free-css.com) e il porting è stato realizzato esclusivamente a scopo educativo e non commerciale. Ricordati di rispettare le linee guida di utilizzo del template.
