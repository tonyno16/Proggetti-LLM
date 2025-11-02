# Chatbot Conversation

Questo progetto crea una conversazione interattiva tra tre modelli di intelligenza artificiale: **OpenAI GPT-4o-mini**, **Anthropic Claude**, e **Google Gemini**. Ogni modello ha una personalità unica e risponde ai messaggi in modo diverso, creando un dialogo interessante tra i chatbot. Il codice gestisce l'integrazione delle API di OpenAI, Anthropic e Google Gemini, e permette di simulare una conversazione tra di loro.

## Caratteristiche

### Modelli di AI Coinvolti:

* **GPT-4o-mini (OpenAI)**: Un modello con una personalità sarcastica, che mette in discussione tutto e non è d'accordo con nulla.
* **Claude (Anthropic)**: Un modello educato e cortese, sempre pronto a trovare un punto d'accordo, cercando di calmare i conflitti.
* **Gemini (Google)**: Un assistente un po' confuso che mescola parole in italiano e inglese, creando risposte a volte comiche.

### Funzionamento:

Ogni bot risponde ai messaggi degli altri, creando una conversazione dinamica. Ogni ciclo di messaggi coinvolge una risposta da ciascun modello, e la conversazione evolve in base a come i bot rispondono l'uno all'altro.

## Tecnologie

* **OpenAI GPT-4o-mini**: Utilizzato per generare risposte sarcastiche e argomentative.
* **Anthropic Claude**: Utilizzato per generare risposte educative e pacifiche.
* **Google Gemini**: Utilizzato per generare risposte confuse che mescolano due lingue.
* **Python 3**: Linguaggio di programmazione principale.
* **Dotenv**: Utilizzato per gestire variabili d'ambiente e chiavi API in modo sicuro.

## Installazione e Configurazione

### Prerequisiti

Prima di iniziare, assicurati di avere:

* Python 3.x installato sul tuo sistema.
* Un editor di testo come Visual Studio Code o PyCharm.
* Una connessione Internet per scaricare le dipendenze e interagire con le API.

### 1. Clona il Repository

Per ottenere il progetto sul tuo computer, esegui il comando di clonazione tramite Git:

```bash
git clone https://github.com/tonyno16/chatbot-conversation.git
```

### 2. Installa le Dipendenze

Naviga nella cartella del progetto e installa tutte le dipendenze necessarie utilizzando pip:

```bash
cd chatbot-conversation
pip install -r requirements.txt
```

Se non hai il file `requirements.txt`, puoi installare manualmente le dipendenze necessarie:

```bash
pip install openai anthropic google-generativeai python-dotenv
```

### 3. Configura le API Keys

Per far funzionare correttamente il progetto, dovrai configurare le tue chiavi API per OpenAI, Anthropic e Google Gemini.

Crea un file `.env` nella cartella principale del progetto (nella stessa cartella del file `README.md`).

Aggiungi le tue chiavi API come segue (assicurati di ottenere le chiavi da ciascun servizio):

```env
OPENAI_API_KEY=la-tua-chiave-openai
ANTHROPIC_API_KEY=la-tua-chiave-anthropic
GOOGLE_API_KEY=la-tua-chiave-google
```

Se non hai ancora le chiavi, puoi registrarti sui seguenti siti per ottenerle:

* [OpenAI API](https://beta.openai.com/signup/)
* [Anthropic API](https://www.anthropic.com/)
* [Google Gemini API](https://developers.google.com/gemini)

### 4. Aggiungi il File `.env` a `.gitignore`

Assicurati di non caricare mai il file `.env` su GitHub, in quanto contiene informazioni sensibili. Crea un file `.gitignore` e aggiungi `.env` al suo interno:

```bash
echo ".env" >> .gitignore
```

### 5. Esegui il Codice

Ora puoi eseguire il codice Python che simula la conversazione tra i bot. Basta eseguire il seguente comando:

```bash
python chatbot_conversation.py
```

Il codice inizierà una simulazione di conversazione tra i chatbot, dove ognuno risponde agli altri creando un dialogo continuo.

## Funzionamento del Codice

Il codice crea una conversazione tra tre modelli, ciascuno con una propria personalità. Ogni bot risponde ai messaggi degli altri in modo ciclico, con l'interazione che continua per un numero definito di iterazioni.

### Dettagli sulla Personalità dei Bot

* **GPT-4o-mini (OpenAI)**: Questo modello è progettato per essere sarcastico, rispondendo in modo provocatorio a tutto ciò che gli viene detto. Mette in discussione ogni affermazione e non è mai d'accordo con nessuno.
* **Claude (Anthropic)**: Un bot molto educato, che cerca sempre di trovare un terreno comune e di calmare eventuali conflitti. È cortese e pacifico.
* **Gemini (Google)**: Questo bot è un po' confuso con la lingua italiana e mescola spesso parole italiane con l'inglese, creando risposte divertenti e talvolta esilaranti.

### Ciclo della Conversazione

Ogni ciclo di conversazione consiste in tre messaggi:

1. Un messaggio da **GPT-4o-mini**.
2. Un messaggio da **Claude**.
3. Un messaggio da **Gemini**.

Ogni modello risponde ai messaggi degli altri, creando una conversazione che si evolve di ciclo in ciclo.

## Problemi Comuni

### Problema 1: API Key non configurata

Se il codice segnala un errore relativo alle chiavi API, assicurati di aver configurato correttamente il file `.env` con le chiavi ottenute dai rispettivi servizi.

### Problema 2: Errore di connessione con le API

Se riscontri problemi di connessione, verifica la tua connessione Internet. Assicurati anche che le tue chiavi API siano valide e non siano scadute.

### Problema 3: Errore durante l'installazione delle dipendenze

Se ricevi errori durante l'installazione delle dipendenze, prova ad aggiornare pip:

```bash
pip install --upgrade pip
```

Poi riprova a installare le dipendenze.

## Contribuire

Contribuire a questo progetto è semplice! Se desideri migliorare il codice o aggiungere funzionalità, segui questi passaggi:

1. Fai un **fork** del repository.
2. Crea un nuovo **branch** per le tue modifiche.
3. Aggiungi le tue modifiche e fai un **commit**.
4. Invia una **pull request** per la revisione.
