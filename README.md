# 🏫 Gestionale Classe 2^B - Web App

> Piattaforma web progressiva per la gestione delle attività scolastiche, orari e comunicazioni di classe. Sviluppata con tecnologie web moderne e il supporto dell'Intelligenza Artificiale.

## 📋 Descrizione del Progetto
Questo progetto nasce dall'esigenza di digitalizzare e semplificare l'organizzazione della classe 2^B. L'applicazione funge da hub centrale per studenti e rappresentanti, permettendo una gestione rapida e visuale delle informazioni scolastiche.

L'interfaccia è stata progettata con uno stile **"iOS Liquid Glass"**, offrendo un'esperienza utente moderna, fluida e responsive (ottimizzata sia per desktop che per mobile).

## ✨ Funzionalità Principali

### 👤 Per gli Studenti
* **Orario Interattivo:** Visualizzazione settimanale con indicatori per interrogazioni, verifiche ed eventi.
* **Bacheca Digitale:** Avvisi, circolari e comunicazioni filtrabili per categoria (Verifica, Avviso, Info).
* **Stato Rappresentanti:** Visualizzazione in tempo reale della disponibilità dei rappresentanti (Disponibile, In Studio, Offline, ecc.).
* **Countdown & Citazioni:** Widget motivazionali e conti alla rovescia per eventi importanti.
* **Archivio Documenti:** Accesso rapido a regolamenti e verbali.

### 🛡️ Pannello Amministrazione (Dashboard)
* **Gestione Ruoli:** Login differenziato per Rappresentante e Vice.
* **Editor Orario:** Modifica rapida delle materie e tipologie di lezione (es. Assemblea, Gita).
* **Gestione Segnalazioni:** Sistema di ticket per proposte e problemi della classe.
* **Tracker:** Monitoraggio quote, firme e scadenze.
* **Sistema di Votazione:** Modulo per sondaggi live durante le assemblee.

## 🛠️ Tecnologie Utilizzate
Il progetto è una *Single Page Application* (SPA) che non richiede compilazione, basata su:

* **Frontend:** HTML5, JavaScript (ES6 Modules).
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (configurato via CDN per Glassmorphism avanzato).
* **Backend & Database:** [Google Firebase](https://firebase.google.com/) (Firestore per i dati, Authentication per il login).
* **Librerie Ausiliarie:**
    * *SweetAlert2* per i popup e le modali.
    * *FontAwesome* per l'iconografia.

## 🤖 Ruolo dell'Intelligenza Artificiale
Questo progetto è stato realizzato con la collaborazione attiva dell'Intelligenza Artificiale. L'IA è stata utilizzata come *Pair Programmer* per:
1.  Generare la struttura boilerplate del codice HTML/JS.
2.  Ottimizzare le classi Tailwind per ottenere l'effetto "Glass" complesso.
3.  Debuggare le chiamate asincrone al database Firebase.
4.  Implementare la logica di rendering condizionale (vista Mobile vs Desktop).

## 🚀 Installazione e Uso
Poiché l'applicazione utilizza CDN e Firebase lato client, non è necessaria alcuna installazione locale (es. `npm install`).

1.  Clona la repository o scarica il file `index.html`.
2.  Apri il file `index.html` in un browser moderno.
3.  *Nota:* Per le funzionalità di amministrazione è necessario possedere le credenziali registrate nel database Firebase collegato.

---
*Progetto scolastico a scopo didattico - Classe 2^B Informatica - CFP Pio XI*
