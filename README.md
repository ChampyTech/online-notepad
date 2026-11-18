# Modern Browser Notepad

Modern Browser Notepad e un editor di testo plain-text completo, eseguito interamente nel browser. Il progetto e composto da un unico file `index.html`, utilizza Tailwind CSS tramite CDN, Lucide Icons e JavaScript senza framework.

## Funzionalita principali

### Gestione dei documenti

- Creazione di nuovi documenti.
- Apertura di file locali tramite il pulsante Open, `Ctrl+O` o trascinamento nell'area dell'editor.
- Formati apribili: TXT, Markdown, JSON, JavaScript, HTML, CSS, CSV, XML e LOG.
- Rinomina del nome del documento direttamente dalla barra superiore o con `F2`.
- Salvataggio come download tramite `Ctrl+S`.
- Salvataggio con nome personalizzato tramite `Ctrl+Shift+S`.
- Avviso per modifiche non salvate quando si crea o apre un documento.
- Indicatore `*` accanto al nome del file e nel titolo della pagina quando ci sono modifiche.
- Inserimento automatico dell'estensione `.txt` se manca il nome del file.
- Supporto per undo e redo fino a 100 stati.

### Editor di testo

- Editor a tutta altezza con area di testo centrale.
- A capo automatico con attivazione/disattivazione tramite il pulsante o `Alt+Z`.
- Selezione del font tra JetBrains Mono, Fira Code, Consolas, Courier New, Inter, Arial e Georgia.
- Dimensione del testo da 11 a 28 pixel.
- Zoom da 50% a 200%.
- Interlinea regolabile da 1.2 a 2.4.
- Inserimento della data e dell'ora corrente con `F5`.
- Pulizia degli spazi doppi e degli spazi finali.
- Divisore testuale.
- Statistiche per riga, colonna, caratteri, parole e testo selezionato.
- Barra di stato con posizione del cursore, totale caratteri/parole, zoom, formato Windows CRLF e codifica UTF-8.
- Barra di stato attivabile/disattivabile dal menu View.

### Ricerca e sostituzione

- Popup trascinabile con ricerca e sostituzione.
- Ricerca successiva e precedente con `F3` o `Shift+F3`.
- Evidenziazione simultanea di tutte le corrispondenze nel documento.
- Evidenziazione differente per la corrispondenza corrente.
- Sostituzione della corrispondenza corrente.
- Sostituzione di tutte le corrispondenze.
- Opzioni Maiuscole/minuscole.
- Opzione Parola intera.
- Opzione Wrap Around.
- Accesso rapido con `Ctrl+F`, `Ctrl+H` e `F3`.
- Apertura in sola ricerca o con il campo sostituisci tramite i rispettivi comandi.

### Trasformazioni del testo

- Maiuscolo.
- Minuscolo.
- Capitalizzazione delle parole.
- Elenco puntato.
- Elenco numerato.
- Blockquote.
- Aumento e riduzione indentazione.
- Tab per indentare e Shift+Tab per rimuovere indentazione.
- Le trasformazioni applicate selezionano il blocco modificato solo quando necessario; il cursore resta dopo i prefissi inseriti.

### Menu e toolbar

- Menu File, Edit, Format, View e Help.
- Azioni rapide per nuovo documento, apri, rinomina, salva e stampa.
- Azioni rapide per undo, redo, taglia, copia e incolla.
- Azioni rapide per testo, elenchi e inserimento data/ora.
- Dropdown delle famiglie di font e delle dimensioni in stile moderno.
- Animazioni leggere per menu, popup e modali.
- Supporto per apertura dei menu da tastiera con freccia giu, Invio o spazio.
- Rispetto di `prefers-reduced-motion`.

### Menu contestuale

- Menu personalizzato con clic destro dentro l'editor.
- Taglia.
- Copia.
- Incolla.
- Conversione Maiuscolo.
- Conversione Minuscolo.
- Conversione Capitalizza.
- Posizionamento automatico del menu entro i bordi della finestra.

### Trascinamento dei file

- I file compatibili possono essere trascinati direttamente nell'area dell'editor.
- Sovrapposizione visiva durante il trascinamento.
- Apertura del contenuto tramite FileReader.
- Aggiornamento del nome del documento, dello stato editor, della cronologia e delle statistiche.

### Esportazione

- Salvataggio come TXT.
- Esportazione come Markdown con estensione `.md`.
- Esportazione come HTML completo con contenuto racchiuso in `<pre>`.
- Esportazione PDF tramite finestra di stampa del browser, dopo la quale e possibile scegliere Salva come PDF.
- Stampa pulita tramite un'area dedicata priva delle interfacce di notepad.

### Tema e stile

- Tema chiaro e scuro.
- Cambio tema dalla barra superiore e dal menu View.
- Palette Slate con accenti indaco.
- Componenti arrotondati, bordi, ombre leggere e sfondi translucidi.
- Dropdown, selettori, slider, modali e menu coerenti con la palette del sito.
- Slider dell'interlinea leggibile in entrambi i temi.
- Icone Lucide.
- Stile responsive per tablet e smartphone.

### Accessibilita

- Link Skip to editor per raggiungere rapidamente l'editor.
- Etichetta ARIA sull'editor e descrizione delle scorciatoie principali.
- Etichette associate ai campi delle modali.
- Trigger dei menu con `aria-haspopup`, `aria-expanded` e `aria-controls`.
- Menu contestuale con ruolo `menu` e elementi `menuitem`.
- Popup di ricerca e sostituzione con ruolo dialog.
- Chiusura popup e modali con Esc.
- Contenimento del focus nelle finestre modali e nel popup di ricerca con Tab e Shift+Tab.
- Messaggi e valori di stato leggibili tramite elementi e attributi semantici.
- Animazioni disattivate automaticamente per utenti con riduzione del movimento.

### Layout mobile

- Barra dei menu con scorrimento orizzontale.
- Dropdown dei menu fissati sotto l'intestazione su schermi piccoli.
- Toolbar rapida con scorrimento orizzontale.
- Popup di ricerca adattato alla larghezza dello schermo.
- Modali con larghezza massima contenuta al viewport.
- Barra di stato ridotta per preservare lo spazio.
- Controlli ottimizzati per il tocco.

## Scorciatoie da tastiera

| Comando | Scorciatoia |
| --- | --- |
| Nuovo documento | `Ctrl+N` |
| Apri file | `Ctrl+O` |
| Rinomina file | `F2` |
| Salva | `Ctrl+S` |
| Salva con nome | `Ctrl+Shift+S` |
| Stampa / PDF | `Ctrl+P` |
| Cerca | `Ctrl+F` |
| Cerca e sostituisci | `Ctrl+H` |
| Risultato precedente | `F3` / `Shift+F3` |
| Vai alla riga | `Ctrl+G` |
| Inserisci data e ora | `F5` |
| Undo | `Ctrl+Z` |
| Redo | `Ctrl+Y` |
| Taglia | `Ctrl+X` |
| Copia | `Ctrl+C` |
| Incolla | `Ctrl+V` |
| Seleziona tutto | `Ctrl+A` |
| Word wrap | `Alt+Z` |
| Maiuscolo | `Ctrl+Shift+U` |
| Minuscolo | `Ctrl+Shift+L` |
| Capitalizza | `Ctrl+Shift+T` |
| Elenco puntato | `Ctrl+Shift+B` |
| Elenco numerato | `Ctrl+Shift+M` |
| Blockquote | `Ctrl+Shift+Q` |
| Inserisci divisore | `Ctrl+Shift+D` |
| Pulisci spazi | `Ctrl+Shift+K` |
| Zoom avanti | `Ctrl++` |
| Zoom indietro | `Ctrl+-` |
| Zoom predefinito | `Ctrl+0` |
| Indenta | `Tab` |
| Deindenta | `Shift+Tab` |
| Chiudi popup/menu | `Esc` |
| Elenco scorciatoie | `F1` |

## Avvio locale

1. Aprire `index.html` direttamente nel browser.
2. In alternativa, avviare un server locale nella cartella del progetto:

```bash
python -m http.server 4173
```

3. Visitare `http://localhost:4173`.

## Limitazioni

- Il salvataggio utilizza il download del browser; non scrive automaticamente sul file locale.
- La gestione della clipboard puo richiedere permessi o un'origine sicura come localhost o HTTPS.
- Il PDF reale dipende dalla finestra di stampa e dalle opzioni del browser.
- Le impostazioni non vengono salvate automaticamente tra due sessioni.
- Trascinare file nel browser legge il contenuto locale senza caricarlo su un server.
