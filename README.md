# 🏫 Gestionale Classe 2^B - Web App

> Dall'inefficienza dei fogli di calcolo a una Web App progressiva realizzata con l'aiuto dell'IA.

## 📖 Storia e Genesi del Progetto
Questo progetto nasce da un'esigenza reale e operativa. Inizialmente, la gestione della classe (2^B) era affidata a un sistema frammentato basato su fogli di calcolo:

1. **Foglio Privato (Admin):** Gestione interna per me e la Vice-Rappresentante.
2. **Foglio Pubblico (Studenti):** Consultazione orari e avvisi.

La difficoltà nel mantenere sincronizzati i dati e la gestione macchinosa ("sclerare tra un foglio e l'altro") hanno fatto scattare la scintilla: **automatizzare tutto tramite una Web App.**

L'obiettivo era creare un unico hub centralizzato che mostrasse dati diversi in base all'utente (Studenti vs Rappresentanti), eliminando il doppio lavoro.

## ⚙️ Metodologia di Sviluppo: "Human-in-the-loop"
Il progetto è un esempio pratico di collaborazione tra sviluppatore umano e Intelligenza Artificiale Generativa (Gemini). Il workflow seguito è stato:

1. **Ideazione & Prompt Engineering:** Ho definito la struttura e le richieste specifiche fornendo a Gemini il contesto e i framework desiderati.
2. **Generazione della Base:** L'IA ha fornito lo scheletro del codice e la logica JavaScript complessa (interazione con Firebase).
3. **Refining Manuale (Il tocco umano):**
    * Intervento diretto sul codice per correzioni di UI/UX.
    * Aggiustamento fine del CSS (padding, spaziature, layout) per garantire la leggibilità che l'IA non riusciva a perfezionare.
4. **Beta Testing & QA:** Collaborazione con la Vice-Rappresentante che ha testato le funzionalità in tempo reale, permettendo di identificare bug e migliorare il flusso utente.

## ✨ Funzionalità del Sito

### 🔒 Area Riservata (Rappresentanti)
*Sostituisce il vecchio "Foglio Privato".*
* **Login differenziato:** Accesso sicuro (Admin/Vice).
* **Gestione centralizzata:** Modifica rapida di orari e comunicazioni.
* **Pannello di controllo:** Strumenti per monitorare quote e segnalazioni.

### 🌍 Area Pubblica (Classe)
*Sostituisce il vecchio "Foglio Pubblico".*
* **Mobile First:** Interfaccia ottimizzata stile iOS.
* **Orario dinamico:** Sempre aggiornato in tempo reale.
* **Bacheca:** Avvisi urgenti e countdown per le verifiche.

## 🛠️ Stack Tecnologico
* **Core:** HTML5, JavaScript (Vanilla/ES6).
* **Design:** Tailwind CSS (con configurazione custom per effetto Glassmorphism).
* **Backend:** Google Firebase (Firestore & Auth).

---
*Progetto sviluppato da Ibrakovic Andrea con il supporto di Gemini AI - Classe 2^B*
