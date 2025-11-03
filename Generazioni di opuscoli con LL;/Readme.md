# 🤖 Generatore di Opuscoli Aziendali con LLM

Questo progetto è un'applicazione web costruita con Python e Gradio che genera opuscoli informativi per aziende, analizzando il contenuto della loro pagina web. L'utente può scegliere tra diversi modelli linguistici di grandi dimensioni (LLM) come GPT-4o, Claude 3 Haiku e Gemini 1.5 Flash per creare la brochure.

*(Esempio di come appare l'interfaccia)*

***

## ✨ Funzionalità Principali

-   **Analisi Web Semplificata**: Inserisci l'URL di un'azienda e il sistema estrae automaticamente il contenuto testuale rilevante.
-   **Supporto Multi-Modello**: Genera contenuti utilizzando i modelli più recenti di OpenAI (GPT), Anthropic (Claude) e Google (Gemini).
-   **Interfaccia Intuitiva**: Un'applicazione web semplice e pulita creata con Gradio, che non richiede competenze tecniche per essere utilizzata.
-   **Output in Streaming**: Le risposte vengono generate e mostrate in tempo reale, migliorando l'esperienza utente.
-   **Risposte in Formato Markdown**: Gli opuscoli sono formattati professionalmente utilizzando Markdown per una facile leggibilità e integrazione.

***

## 🛠️ Tecnologie Utilizzate

-   **Backend**: Python
-   **Web Framework**: Gradio
-   **Web Scraping**: `requests` & `BeautifulSoup4`
-   **Modelli LLM**:
    -   OpenAI API (`gpt-4o-mini`)
    -   Anthropic API (`claude-3-haiku-20240307`)
    -   Google Gemini API (`gemini-1.5-flash`)

***

## 🚀 Come Iniziare

Segui questi passaggi per eseguire il progetto sul tuo computer locale.

### 1. Prerequisiti

-   Python 3.8 o superiore installato.
-   Un editor di codice (es. Visual Studio Code).
-   Le chiavi API per OpenAI, Anthropic e/o Google Gemini.

### 2. Installazione

**a. Clona il repository:**
Apri un terminale e clona questo repository GitHub.

```bash
git clone https://github.com/TUO_NOME_UTENTE/NOME_DEL_PROGETTO.git
cd NOME_DEL_PROGETTO

