# Chatbot Conversation

Questo progetto crea una conversazione interattiva tra tre modelli di intelligenza artificiale: **OpenAI GPT-4o-mini**, **Anthropic Claude**, e **Google Gemini**. Ogni modello ha una personalità unica e risponde ai messaggi in modo diverso, creando un dialogo interessante tra i chatbot. Il codice gestisce l'integrazione delle API di OpenAI, Anthropic e Google Gemini, e permette di simulare una conversazione tra di loro.

## Caratteristiche
- **Modelli di AI Coinvolti**:
  - **GPT-4o-mini (OpenAI)**: Un modello con una personalità sarcastica, che mette in discussione tutto e non è d'accordo con nulla.
  - **Claude (Anthropic)**: Un modello educato e cortese, sempre pronto a trovare un punto d'accordo, cercando di calmare i conflitti.
  - **Gemini (Google)**: Un assistente un po' confuso che mescola parole in italiano e inglese, creando risposte a volte comiche.
  
- **Funzionamento**: Ogni bot risponde ai messaggi degli altri, creando una conversazione dinamica. Ogni ciclo di messaggi coinvolge una risposta da ciascun modello, e la conversazione evolve in base a come i bot rispondono l'uno all'altro.

## Tecnologie
- **OpenAI GPT-4o-mini**: Utilizzato per generare risposte sarcastiche e argomentative.
- **Anthropic Claude**: Utilizzato per generare risposte educative e pacifiche.
- **Google Gemini**: Utilizzato per generare risposte confuse che mescolano due lingue.
- **Python 3**: Linguaggio di programmazione principale.
- **Dotenv**: Utilizzato per gestire variabili d'ambiente e chiavi API in modo sicuro.

## Installazione e Configurazione

### Prerequisiti
Prima di iniziare, assicurati di avere:
- **Python 3.x** installato sul tuo sistema.
- Un editor di testo come **Visual Studio Code** o **PyCharm**.
- Una connessione Internet per scaricare le dipendenze e interagire con le API.

### 1. Clona il Repository
Per ottenere il progetto sul tuo computer, esegui il comando di clonazione tramite Git:

```bash
git clone https://github.com/tuo-utente/chatbot-conversation.git

