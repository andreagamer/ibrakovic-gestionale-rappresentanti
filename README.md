# 🏫 Gestionale Classe 2^B - Web App (AI-Assisted)

> **Un progetto "Human-in-the-loop":** Dalla frustrazione dei fogli di calcolo a una Web App progressiva, sviluppata collaborando con l'Intelligenza Artificiale.

---

## 📖 Genesi del Progetto: Una sfida personale

Tutto è nato durante un normale weekend, mentre cercavo di mettere ordine nel caos gestionale della classe. La situazione di partenza era inefficiente:

* ❌ **Foglio Privato (Admin):** Un file Excel per me e la Vice-Rappresentante per gestire quote e note.
* ❌ **Foglio Pubblico (Studenti):** Un altro file condiviso per gli orari, spesso non sincronizzato.

Mentre passavo da un file all'altro, ho deciso di sfidare me stesso e la tecnologia: *"Posso creare un sistema unificato facendomi aiutare dall'Intelligenza Artificiale (Gemini)?"*

### Il Rifiuto della "Strada Facile"
Alla mia prima richiesta, l'AI ha suggerito: *"Usa Google Sites e incorpora i fogli di calcolo."*
Sarebbe stato semplice, ma inutile per il mio apprendimento. Ho rifiutato la proposta e ho deciso di puntare in alto: **creare una Web App vera, scritta in codice, ospitata su server.**

---

## ⚙️ Il Percorso di Sviluppo (Devlog)

Lo sviluppo non è stato lineare. È stato un processo di *trial-and-error* che mi ha insegnato le basi dell'architettura web moderna.

### Fase 1: L'Errore del Principiante (LocalStorage)
La prima versione generata dall'AI salvava i dati nel `LocalStorage` del browser.
* **Risultato:** Funzionava perfettamente sul mio PC.
* **Problema:** Appena inviato il link a un compagno, lui vedeva una pagina vuota.
* 💡 **Lezione appresa:** Ho capito la differenza fondamentale tra **Client-side** (i dati restano nel dispositivo dell'utente) e **Cloud** (i dati sono condivisi).

### Fase 2: L'Integrazione del Cloud (Firebase)
Ho chiesto all'AI di riscrivere il "cervello" dell'app utilizzando **Google Firebase**.
* Abbiamo implementato **Firestore** (Database NoSQL) per salvare orari e avvisi in tempo reale.
* Abbiamo aggiunto **Firebase Auth** per proteggere l'area amministrativa.

### Fase 3: Il Tocco Umano & Beta Testing
L'AI è stata ottima per la logica, ma carente nel design fine e nell'esperienza utente (UX).
* **Intervento Manuale:** Sono intervenuto personalmente sul codice CSS (**Tailwind**) per correggere spaziature, padding e creare l'effetto "Glassmorphism" (stile iOS) che l'AI non riusciva a centrare.
* **Teamwork:** La mia Vice-Rappresentante ha agito da Beta Tester, provando l'app ad ogni mio singolo aggiornamento e segnalando bug funzionali che io e l'AI abbiamo poi risolto.

---

## ✨ Funzionalità del Sistema

L'applicazione è divisa in due interfacce che cambiano dinamicamente in base all'utente loggato.

### 👤 Lato Pubblico (Studenti)
* **Dashboard "Mobile First":** Design ottimizzato per smartphone.
* **Orario Interattivo:** Mostra le materie del giorno corrente con indicatori colorati.
* **Bacheca Digitale:** Avvisi, circolari e info urgenti in tempo reale.
* **Widget:** Countdown per verifiche ed eventi.

### 🛡️ Lato Amministrazione (Rappresentanti)
* **Login Sicuro:** Accesso riservato agli admin.
* **Gestione Orario:** Pannello per modificare le materie senza toccare il codice.
* **Sistema Segnalazioni:** Ticket system per raccogliere problemi della classe.
* **Tracker:** Monitoraggio digitale di quote, firme e scadenze.

---

## 🛠️ Stack Tecnologico

Il progetto è una Single Page Application (SPA) serverless.

| Tecnologia | Ruolo | Perché l'ho scelta |
| :--- | :--- | :--- |
| **HTML5 & JS (ES6)** | Core | Nessun framework pesante (React/Angular), solo velocità pura. |
| **Tailwind CSS** | Stile | Per un design rapido e moderno tramite classi di utilità. |
| **Google Firebase** | Backend | Database in tempo reale e autenticazione sicura gestita da Google. |
| **SweetAlert2** | UI | Per sostituire i brutti `alert()` nativi con popup eleganti. |

---

## 🚀 Deployment & Hosting: Perché Netlify?

Per rendere il sito accessibile H24 alla classe, ho dovuto scegliere dove ospitarlo. Ho scartato soluzioni vecchie (FTP) e ho scelto **Netlify**.

1.  **Integrazione Git:** Il sito è collegato a questa repository GitHub. Ogni volta che faccio un "commit" (salvo una modifica al codice), Netlify aggiorna automaticamente il sito pubblico.
2.  **CDN Globale:** Il sito viene caricato da server distribuiti, garantendo velocità.
3.  **HTTPS:** Sicurezza garantita dal protocollo SSL (il lucchetto verde), fondamentale per proteggere i login dei rappresentanti.

---

## 📦 Guida all'Uso del Template (Per Docenti/Studenti)

Ho reso il codice modulare affinché possa essere usato come base didattica per altre classi.

### 1. Prerequisiti
* Un account Google (per Firebase).
* Un editor di testo (VS Code).

### 2. Configurazione Database
1.  Creare un progetto su [Firebase Console](https://console.firebase.google.com/).
2.  Attivare **Firestore Database** e **Authentication** (Google o Email/Password).
3.  Copiare le chiavi di configurazione (`apiKey`, `projectId`, ecc.) dalle impostazioni del progetto.

### 3. Setup del Codice
Nel file `index.html`, cercare l'oggetto `firebaseConfig` e incollare le proprie chiavi:

```javascript
const firebaseConfig = {
    apiKey: "INCOLLA_QUI",
    authDomain: "...",
    projectId: "...",
    // ...
};
