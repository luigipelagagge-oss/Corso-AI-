# Navigare il Non-Determinismo - IA nella Didattica

> Una guida interattiva per docenti che trasforma il report metodologico sull'IA in un kit pratico di sopravvivenza per l'aula.

Questo sito web accompagna il corso di "Fondamenti di IA" con un approccio visuale e interattivo, pensato per spiegare perché l'IA non è un computer deterministico e come trasformare i suoi "errori" in opportunità didattiche.

## 🔍 Tecnologie Utilizzate

Il progetto è costruito con strumenti leggeri e moderni, tutti caricati via CDN (quindi **nessuna installazione locale** richiesta):

- **Tailwind CSS** – per lo stile utility-first e il layout responsive.
- **Chart.js** – per la visualizzazione dei dati (grafico a ciambella sui modelli di IA).
- **Vanilla JavaScript** – per il simulatore non-deterministico e le interazioni di scroll.
- **Google Fonts (Inter)** – per la tipografia pulita.

## 📁 Struttura del Progetto

Il repository è estremamente semplice perché il sito è interamente contenuto in un unico file:

/
├── index.html # L'intera applicazione (HTML, CSS, JS) + Hub dei Moduli
└── README.md # Questo file

Tutti gli assets (font, librerie) vengono risolti in remoto, quindi non ci sono cartelle `css` o `js` da gestire.

## 📚 Moduli disponibili

| Modulo | Titolo | Piattaforma | Link |
|--------|--------|-------------|------|
| 1 | Fondamenti di IA e Nuovi Paradigmi Didattici | Canva (esterno) | [Vai al modulo](https://luigi-pelagagge.my.canva.site/metodologie-didattiche-e-ia) |
| 2 | IA Generativa nella Scrittura Creativa | GitHub (in sviluppo) | - |
| 3 | Etica e Limiti dell'IA in Aula | GitHub (in sviluppo) | - |

## 🚀 Come Effettuare la Manutenzione

### Modificare i contenuti testuali
- Apri `index.html` con qualsiasi editor di testo (VS Code, Notepad++, Sublime).
- Cerca il paragrafo o la sezione che vuoi modificare (sono tutti commentati con `<!-- Sezione ... -->`).
- Salva e carica il file sul repository.

### Aggiornare i dati del grafico
- Nel blocco `<script>` in fondo alla pagina, trova `new Chart(ctx, {...})`.
- Modifica i valori nell'array `data: [45, 30, 25]` e le relative etichette per aggiornare le percentuali.

### Cambiare i colori (tema)
- I colori principali sono gestiti tramite le utility di Tailwind e variabili CSS nel `<style>`.
- Cerca `:root { ... }` per modificare i colori globali (es. `--accent-amber`, `--bg-warm`).

### Modificare le risposte del simulatore
- Cerca la funzione `simulateIA()` e all'interno dell'array `outputs`. Aggiungi o modifica le stringhe per cambiare gli esempi di output dell'IA.

### Aggiungere un nuovo modulo
1. Crea un nuovo file HTML (es. `modulo2.html`) copiando la struttura di `index.html`.
2. Modifica i contenuti per il nuovo argomento.
3. Nella sezione "Bacheca Moduli" di `index.html`, sostituisci la card "Prossimamente" con una card funzionante che punti al nuovo file.

## 🌐 Pubblicazione

Questo sito è progettato per essere ospitato su **GitHub Pages**:

1. Il file principale deve chiamarsi esattamente `index.html`.
2. Vai su *Settings → Pages* del repository.
3. Seleziona il branch `main` e la cartella root `/`.
4. Il sito sarà online all'indirizzo: `https://<tuo-username>.github.io/<repo-name>/`

## 📌 Note per i Docenti

- **Nessun back-end**: il sito è completamente statico. Funziona offline (dopo il primo caricamento delle risorse CDN) e non invia dati a nessun server.
- **Accessibilità**: il design è stato pensato per essere chiaro e leggibile, con contrasti adeguati e gerarchie visive nette.
- **Didattica**: usa il simulatore durante la lezione per mostrare dal vivo il concetto di "non-determinismo" e la sezione "Caso Studio" per il collegamento con la letteratura.

## 🛠️ Possibili Miglioramenti Futuri

- Aggiungere un dark mode toggle.
- Integrare più autori nella tabella del caso studio.
- Salvare lo storico delle simulazioni in una lista.
- Creare pagine HTML per i moduli 2 e 3.

---

*Progetto realizzato per il corso di aggiornamento docenti – 2024*
