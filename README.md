<div align="center">

🏫 Gestionale Classe 2^B - Web App

Powered by Human-AI Collaboration

Un progetto "Human-in-the-loop": Dalla frustrazione dei fogli di calcolo a una Web App progressiva, sviluppata collaborando con l'Intelligenza Artificiale.

Demo Live · Segnala Bug · Richiedi Feature

</div>

📑 Indice

Genesi del Progetto

Devlog: Il Percorso

Funzionalità

Stack Tecnologico

Deployment

Guida all'Uso

📖 Genesi del Progetto

Tutto è nato durante un normale weekend, nel tentativo di mettere ordine nel caos gestionale della classe. La situazione di partenza era frammentata e inefficiente:

🔴 Foglio Privato (Admin): Un file Excel per me e la Vice-Rappresentante per gestire quote e note.

🔴 Foglio Pubblico (Studenti): Un altro file condiviso per gli orari, spesso non sincronizzato.

Ho deciso di sfidare me stesso e la tecnologia: "Posso creare un sistema unificato facendomi aiutare dall'Intelligenza Artificiale (Gemini)?"

⛔ Il Rifiuto della "Strada Facile"

Alla mia prima richiesta, l'AI ha suggerito: "Usa Google Sites e incorpora i fogli di calcolo."
Sarebbe stato semplice, ma inutile per il mio apprendimento. Ho rifiutato la proposta e ho deciso di puntare in alto: creare una Web App vera, scritta in codice, ospitata su server.

⚙️ Il Percorso di Sviluppo (Devlog)

Lo sviluppo è stato un processo di trial-and-error che mi ha insegnato le basi dell'architettura web moderna.

1️⃣ Fase 1: L'Errore del Principiante (LocalStorage)

La prima versione generata dall'AI salvava i dati nel LocalStorage del browser.

Problema: I dati rimanevano nel dispositivo dell'utente. Se inviavo il link a un compagno, lui vedeva una pagina vuota.

Lezione: Ho compreso la differenza fondamentale tra Client-side (locale) e Cloud (condiviso).

2️⃣ Fase 2: L'Integrazione del Cloud (Firebase)

Ho chiesto all'AI di riscrivere il "cervello" dell'app utilizzando Google Firebase.

Firestore (NoSQL): Per salvare orari e avvisi in tempo reale.

Auth: Per proteggere l'area amministrativa.

3️⃣ Fase 3: Il Tocco Umano & Beta Testing

L'AI è stata ottima per la logica, ma carente nella UX/UI.

Intervento Manuale: Ho riscritto il CSS (Tailwind) per creare l'effetto "Glassmorphism" (stile iOS) e sistemare i padding.

Teamwork: La mia Vice-Rappresentante ha agito da Beta Tester, provando l'app a ogni aggiornamento.

✨ Funzionalità del Sistema

👤 Lato Pubblico (Studenti)

🛡️ Lato Amministrazione (Rappresentanti)

Mobile First: Design stile app nativa.

Login Sicuro: Accesso riservato.

Orario Live: Indicatori materie dinamici.

Editor Orario: Modifiche senza toccare codice.

Bacheca: Avvisi e Circolari.

Ticket System: Gestione segnalazioni classe.

Widget: Countdown verifiche.

Tracker: Monitoraggio quote e firme.

🛠️ Stack Tecnologico

Il progetto è una Single Page Application (SPA) serverless.

Frontend: HTML5, JavaScript (ES6 Modules)

Styling: Tailwind CSS (Configurazione Custom)

Backend: Google Firebase (Firestore, Auth)

UI Components: SweetAlert2, FontAwesome

🚀 Deployment & Hosting

Ho scelto Netlify per l'hosting per garantire accessibilità H24 e sicurezza.

CD (Continuous Deployment): Collegamento diretto a questa repository GitHub. Ogni git push aggiorna il sito live.

CDN Globale: Performance elevate ovunque.

HTTPS: Certificato SSL automatico.

📦 Guida all'Uso del Template

Vuoi usare questo progetto per la tua classe?

1. Configurazione Firebase

Crea un progetto su Firebase Console e copia le chiavi.

2. Setup Codice

Nel file index.html, sostituisci l'oggetto di configurazione:

const firebaseConfig = {
    apiKey: "LA_TUA_API_KEY",
    authDomain: "IL_TUO_PROGETTO.firebaseapp.com",
    projectId: "IL_TUO_PROJECT_ID",
    storageBucket: "IL_TUO_PROGETTO.appspot.com",
    messagingSenderId: "...",
    appId: "..."
};


3. Deploy

Carica il progetto su Netlify Drop o collega la repo.

<div align="center">

Progetto personale di Ibrakovic Andrea (2^B) 




Sviluppato per dimostrare l'uso etico e produttivo dell'IA nello sviluppo software

</div>
