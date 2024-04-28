#  Specifica Dei Requisiti Webapp Gestione Finanziaria

## 1. Requisiti di Autenticazione
### 1.1 Login
- Gli utenti registrati possono effettuare il login inserendo le loro credenziali.
- Include: Inserimento delle credenziali di accesso.
- Extend: Recupero della password.
### 1.2 Gestione dell'Accesso
- Modifica il sistema di autenticazione per supportare l'autenticazione multitenant. Ogni volta che un utente tenta di accedere, è necessario verificare le credenziali rispetto ai dati del tenant corrispondente.
- Implementa la gestione delle sessioni in modo che ciascun tenant abbia la propria sessione e che le informazioni di sessione siano isolate tra i tenant.
### 1.3 Recupero Password
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
- Extend: Modifica della fonte di reddito.
- Extend: Eliminazione della finte di reddito.

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
### 6.2 Configurabilità
- Aggiungi un'interfaccia utente per consentire agli amministratori del sistema di gestire le impostazioni specifiche del tenant, come limiti di spesa personalizzati, categorie personalizzate e preferenze di visualizzazione.
- Assicurati che le modifiche alle impostazioni di configurazione siano applicate solo al tenant specifico e non influiscano sugli altri tenant.
  
## 7. Gestione degli Utenti (Amministratore del Sistema)
### 7.1 Creazione di Utenti
- L'amministratore del sistema può creare nuovi utenti e assegnare privilegi.
- Extend: Disabilitazione o Eliminazione di Utenti.                
- Extend: Modifica dei Privilegi degli Utenti.

### 7.2 Assistenza agli Utenti
- L'amministratore del sistema può fornire assistenza agli utenti e risolvere i loro problemi.
  
## 8. Aggiornamento del Software (Amministratore del Sistema)
- L'amministratore del sistema può installare gli aggiornamenti del software per garantire le prestazioni e la sicurezza ottimali dell'applicazione.

## 9. Gestione degli Errori e Monitoraggio
- Aggiungi un sistema di logging e monitoraggio che consenta di tracciare e monitorare le attività specifiche del tenant, inclusi gli errori e le eccezioni che si verificano durante l'utilizzo dell'applicazione.
- Assicurati che gli amministratori del sistema possano accedere ai log e ai dati di monitoraggio specifici del tenant per risolvere eventuali problemi.
### 9.1 Reporting e Analisi Multitenant
- Modifica i moduli di reporting e analisi per supportare l'aggregazione dei dati tra tutti i tenant. Ciò potrebbe richiedere la creazione di query SQL complesse o l'utilizzo di strumenti di reporting che supportano il multitenancy.
- Assicurati che i report generati siano specifici del tenant e mostrino solo i dati relativi al tenant corrente.

# DIAGRAMMA UML
<img src="https://yuml.me/diagram/usecase/[Utente%20Registrato]-(Login%20In),%20(Login%20In)%3E(Inserimento%20credenziali%20di%20accesso),%20(Login%20In)%3C(Recupero%20della%20password),%20(Login%20In)%3C(Modifica%20Profilo),%20[Utente%20Registrato]-(Registrazione%20delle%20entrate),%20(Registrazione%20delle%20entrate)%3E(Aggiunta%20fonte%20di%20reddito),%20(Registrazione%20delle%20entrate)%3E(Visualizzazione%20del%20riepilogo%20delle%20entrate),%20(Aggiunta%20fonte%20di%20reddito)%3C(Modifica%20o%20Eliminazione%20della%20fonte%20di%20reddito),%20[Utente%20Registrato]-(Gestione%20delle%20spese),%20(Gestione%20delle%20spese)-(Aggiunta%20di%20una%20spesa),%20(Aggiunta%20di%20una%20spesa)%3C(Modifica%20o%20eliminazione%20di%20una%20spesa),%20[Utente%20Registrato]-(Pianificazione%20del%20budget),%20(Pianificazione%20del%20budget)-(Creazione%20di%20un%20budget%20mensile),%20(Creazione%20di%20un%20budget%20mensile)%3E(Aggiornamento%20del%20budget),%20[Utente%20Registrato]-(Visualizzazione%20delle%20Analisi%20Finanziarie),%20(Visualizzazione%20delle%20Analisi%20Finanziarie)%3E(Visualizzazione%20di%20grafici),%20(Visualizzazione%20di%20grafici)%3C(Gestione%20delle%20Notifiche),%20(Gestione%20delle%20Notifiche)%3E(Notifica%20superamento%20dei%20limiti%20di%20spesa),%20[Amministratore%20del%20sistema]-(Gestione%20degli%20Utenti),%20(Gestione%20degli%20Utenti)%3C(Disabilitazione%20o%20Eliminazione%20utenti),%20[Amministratore%20del%20sistema]-(Aggiornamento%20del%20software),%20(Gestione%20degli%20Utenti)%3E(Assistenza%20agli%20Utenti),">

# VALUE PROPOSITION
## FinanziaLife 
### Migliora la tua gestione finanziaria con FinanziaLife 
-FinanziaLife è la tua soluzione completa per la gestione finanziaria personale. Con un'interfaccia intuitiva e potenti funzionalità, ti offriamo il controllo totale sulle tue entrate, spese e budget. Grazie a strumenti avanzati di analisi finanziaria e notifiche personalizzate, raggiungi i tuoi obiettivi finanziari.

### Lista dei benefici 
-Controllo Totale delle Finanze:
Gestisci le tue entrate e spese in un'unica piattaforma intuitiva.
Crea e aggiorna facilmente il tuo budget mensile.

-Analisi Dettagliata:
Visualizza grafici e report dettagliati sulle tue finanze.
Ricevi consigli personalizzati basati sulle tue abitudini di spesa.

-Notifiche Intelligenti:
Ricevi avvisi immediati quando superi i limiti di spesa.
Resta sempre informato sullo stato del tuo budget.

-Gestione Utenti Semplificata:
Per gli amministratori del sistema, crea, modifica o disabilita utenti con facilità.
Fornisci assistenza rapida agli utenti in caso di problemi.

-Aggiornamenti Continui:
L'amministratore del sistema può garantire prestazioni e sicurezza ottimali con gli aggiornamenti regolari del software.

-Recupero Sicuro delle Credenziali:
Recupera la password in modo sicuro tramite email o numero di telefono.

-Personalizzazione del Profilo:
Modifica facilmente le informazioni del tuo profilo utente.

-Pianificazione Finanziaria Efficiente:
Crea, aggiorna e visualizza il tuo budget corrente con facilità.



# User Stories e Stima delle Ore

## Sprint 1

### 1. Utente Autenticato
1. Come utente autenticato, essere in grado di effettuare il login inserendo le mie credenziali per accedere alla piattaforma.

**Stima delle Ore:** 4 ore

### 2. Recupero Password
2. Come utente, poter richiedere il recupero della password tramite email o numero di telefono per ripristinare l'accesso al mio account.

**Stima delle Ore:** 6 ore

### 3. Modifica Profilo
3. Come utente autenticato, avere la possibilità di modificare le informazioni del mio profilo per tenerle aggiornate.

**Stima delle Ore:** 3 ore

### 4. Registrazione
4. Come nuovo utente, poter effettuare la registrazione fornendo le informazioni di base richieste.

**Stima delle Ore:** 5 ore

### 5. Aggiunta Fonte di Reddito
5. Come utente autenticato, poter aggiungere nuove fonti di reddito alla mia lista.

**Stima delle Ore:** 4 ore

## Sprint 2

### 6. Visualizzazione Riepilogo Entrate
6. Come utente autenticato, poter visualizzare un riepilogo delle entrate registrate nella piattaforma.

**Stima delle Ore:** 5 ore

### 7. Aggiunta Spesa
7. Come utente autenticato, poter registrare le mie spese in varie categorie.

**Stima delle Ore:** 6 ore

### 8. Visualizzazione Riepilogo Spese
8. Come utente autenticato, visualizzare un riepilogo delle spese registrate nella piattaforma.

**Stima delle Ore:** 5 ore

### 9. Creazione Budget Mensile
9. Come utente autenticato, creare un budget mensile basato sulle mie entrate e categorie di spesa.

**Stima delle Ore:** 8 ore

### 10. Aggiornamento Budget
10. Come utente autenticato, poter aggiornare il mio budget in base alle entrate effettive e alle spese.

**Stima delle Ore:** 6 ore

## Sprint 3

### 11. Visualizzazione Budget Corrente
11. Come utente autenticato, poter visualizzare il mio budget corrente e le differenze tra budget pianificato ed effettivo.

**Stima delle Ore:** 5 ore

### 12. Visualizzazione Grafici e Report Finanziari
12. Come utente autenticato, poter visualizzare grafici e report dettagliati sulle mie entrate e spese.

**Stima delle Ore:** 7 ore

### 13. Ricezione Consigli Finanziari
13. Come utente autenticato, ricevere consigli finanziari personalizzati basati sulle mie abitudini di spesa.

**Stima delle Ore:** 6 ore

### 14. Notifica Superamento Limiti di Spesa
14. Come utente autenticato, ricevere notifiche quando supero i limiti di spesa predefiniti.

**Stima delle Ore:** 4 ore

## Sprint 4

### 15. Creazione Utenti (Amministratore)
15. Come amministratore del sistema, poter creare nuovi utenti e assegnare privilegi.

**Stima delle Ore:** 6 ore

### 16. Assistenza agli Utenti (Amministratore)
16. Come amministratore del sistema, poter fornire assistenza agli utenti e risolvere i loro problemi.

**Stima delle Ore:** 7 ore

### 17. Disabilitazione o Eliminazione Utenti (Amministratore)
17. Come amministratore del sistema, poter disabilitare o eliminare utenti se necessario.

**Stima delle Ore:** 5 ore

### 18. Aggiornamento Software (Amministratore)
18. Come amministratore del sistema, poter installare gli aggiornamenti del software per garantire le prestazioni e la sicurezza ottimali.

**Stima delle Ore:** 6 ore

### Sequenza di Fibonacci per le Stime:
1, 2, 3, 5, 8, 13
