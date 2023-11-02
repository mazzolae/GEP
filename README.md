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

<img src="https://yuml.me/diagram/usecase/[Utente Registrato]-(Login In),(Login In)>(Inserire dati di accesso),(Login In)<(Recupero della password),(Login In)<(Modifica Profilo),[Utente Registrato]- (Registrazione delle entrate),(Registrazione delle entrate)>(Aggiunta fonte di reddito),(Registrazione delle entrate)>(Visualizzazione del riepilogo delle entrate),(Aggiunta fonte di reddito)<(Modifica o Eliminazione della fonte di reddito),[Utente Registrato]- (Gestione delle spese),
(Gestione delle spese)>(Aggiunta di una spesa),(Aggiunta di una spesa)< (Modifica o eliminazione di una spesa),[Utente Registrato]- (Pianificazione del budget),(Pianificazione del budget)>(Creazione di un budget mensile),(Creazione di un budget mensile)>(Aggiornamento del budget),[Utente Registrato]- (Visualizzazione delle Analisi Finanziarie),(Visualizzazione delle Analisi Finanziarie)>(Visualizzazione di grafici),[Utente Registrato]< (Gestione delle Notifiche),
(Gestione delle Notifiche)>(Notifica superamento dei limiti di spesa)[Amministratore del sistema]-(Gestione degli Utenti),(Gestione degli Utenti)<(Disabilitazione o Eliminazione utenti),[Amministratore del sistema]-(Aggiornamento del software),(Gestione degli Utenti)>(Assistenza agli Utenti),[Utente Non Registrato] - (Sign Up),">
