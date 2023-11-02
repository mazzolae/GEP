#  Specifica Dei Requisiti Webapp Gestione Finanziaria


## 1. Requisiti di Autenticazione
### 1.1 Login
- Gli utenti registrati possono effettuare il login inserendo le loro credenziali.
- Include: Inserire dati di accesso.
- Extend: Recupero della password.

### 1.2 Recupero Password
- Gli utenti possono richiedere il recupero della password tramite email o numero di telefono.
- Il sistema invierà un link di ripristino alla casella di posta dell'utente.
- Include: Recupero della password.

### 1.3 Modifica Profilo
- Gli utenti registrati possono modificare le informazioni del loro profilo.
- Include: Modifica del Profilo Utente.

### 1.4 Registrazione
- Gli utenti non registrati devono effettuare la registrazione fornendo informazioni di base.
- Include: Sign Up.

## 2. Gestione delle Entrate
### 2.1 Aggiunta Fonte di Reddito
- Gli utenti possono aggiungere fonti di reddito (stipendi, interessi, ecc.).
- Include: Aggiunta di una Fonte di Reddito.
- Extend: Modifica o Eliminazione della fonte di reddito.

### 2.2 Visualizzazione Riepilogo delle Entrate
- Gli utenti possono visualizzare un riepilogo delle entrate registrate.
- Include: Visualizzazione del riepilogo delle entrate.

## 3. Gestione delle Spese
### 3.1 Aggiunta di una Spesa
- Gli utenti possono registrare spese in varie categorie.
- Include: Aggiunta di una spesa.
- Extend: Modifica o Eliminazione di una spesa.

### 3.2 Visualizzazione Riepilogo delle Spese
- Gli utenti possono visualizzare un riepilogo delle spese registrate.
- Include: Visualizzazione del riepilogo delle spese.

## 4. Pianificazione del Budget
### 4.1 Creazione di un Budget Mensile
- Gli utenti possono creare un budget mensile basato sulle loro entrate e categorie di spesa.
- Include: Creazione di un budget mensile.
- Include: Aggiornamento del budget.

### 4.2 Aggiornamento del Budget
- Gli utenti possono aggiornare il budget in base alle entrate effettive e alle spese.
- Include: Aggiornamento del budget.

### 4.3 Visualizzazione del Budget Corrente
- Gli utenti possono visualizzare il budget corrente e le differenze tra budget pianificato ed effettivo.

## 5. Analisi Finanziaria
### 5.1 Visualizzazione dei Grafici
- Gli utenti possono visualizzare grafici e report dettagliati sulle loro entrate e spese.
- Include: Visualizzazione dei Grafici e dei Report Finanziari.

### 5.2 Ricezione di Consigli Finanziari
- Gli utenti riceveranno consigli finanziari basati sulle abitudini di spesa.
- Include: Ricezione di Consigli Finanziari.

## 6. Gestione delle Notifiche
### 6.1 Notifica Superamento dei Limiti di Spesa
- Gli utenti riceveranno notifiche quando superano i limiti di spesa predefiniti.
  
## 7. Gestione degli Utenti (Amministratore del Sistema)
### 7.1 Creazione di Utenti
- L'amministratore del sistema può creare nuovi utenti e assegnare privilegi.
- Extend: Disabilitazione o Eliminazione di Utenti.
- Extend: Modifica dei Privilegi degli Utenti.

### 7.2 Assistenza agli Utenti
- L'amministratore del sistema può fornire assistenza agli utenti e risolvere i loro problemi.
  
## 8. Aggiornamento del Software (Amministratore del Sistema)
- L'amministratore del sistema può installare gli aggiornamenti del software per garantire le prestazioni e la sicurezza ottimali dell'applicazione.

<img src=“https://yuml.me/diagram/usecase/[Utente%20Registrato]-(Login%20In),%20(Login%20In)>(Inserire%20dati%20di%20accesso),%20(Login%20In)<(Recupero%20della%20password),%20(Login%20In)<(Modifica%20Profilo),%20[Utente%20Registrato]-%20(Registrazione%20delle%20entrate),%20(Registrazione%20delle%20entrate)>(Aggiunta%20fonte%20di%20reddito),%20(Registrazione%20delle%20entrate)>(Visualizzazione%20del%20riepilogo%20delle%20entrate),%20(Aggiunta%20fonte%20di%20reddito)<(Modifica%20o%20Eliminazione%20della%20fonte%20di%20reddito),%20[Utente%20Registrato]-%20(Gestione%20delle%20spese),%20(Gestione%20delle%20spese)>(Aggiunta%20di%20una%20spesa),%20(Aggiunta%20di%20una%20spesa)<%20(Modifica%20o%20eliminazione%20di%20una%20spesa),%20[Utente%20Registrato]-%20(Pianificazione%20del%20budget),%20(Pianificazione%20del%20budget)>(Creazione%20di%20un%20budget%20mensile),%20(Creazione%20di%20un%20budget%20mensile)>(Aggiornamento%20del%20budget),%20[Utente%20Registrato]-%20(Visualizzazione%20delle%20Analisi%20Finanziarie),(Visualizzazione%20delle%20Analisi%20Finanziarie)>(Visualizzazione%20di%20grafici),[Utente%20Registrato]<%20(Gestione%20delle%20Notifiche),%20(Gestione%20delle%20Notifiche)>(Notifica%20superamento%20dei%20limiti%20di%20spesa),[Amministratore%20del%20sistema]-(Gestione%20degli%20Utenti),%20(Gestione%20degli%20Utenti)<(Disabilitazione%20o%20Eliminazione%20utenti),[Amministratore%20del%20sistema]-(Aggiornamento%20del%20software),%20(Gestione%20degli%20Utenti)>(Assistenza%20agli%20Utenti),%20[Utente%20Non%20Registrato]%20-%20(Sign%20Up),”>
