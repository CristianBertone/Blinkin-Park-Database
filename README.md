# Blinkin' Park 
**Autori:** Cristian Bertone, Manuel Cerise  
**Anno Accademico:** 2025/2026  

## Il Progetto
Blinkin' Park è un database relazionale pensato per gestire l'infrastruttura di un'azienda di parcheggi a Torino. L'obiettivo del sistema è tracciare in modo efficiente veicoli, utenti e personale. Nello specifico, il database gestisce:
* **Le infrastrutture:** Parcheggi coperti (garage con orari di apertura) e all'aperto, suddivisi in zone cittadine.
* **Tariffe e Soste:** Ingressi e uscite dei veicoli, ticket a tariffa oraria (in base alla zona) e aggiornamento in tempo reale dei posti liberi.
* **Utenti:** Clienti occasionali, registrati, abbonamenti annuali nominali e gestione degli sconti promozionali.
* **Personale:** Turni di lavoro dei controllori, assegnazione degli operatori ai garage e registrazione delle multe per soste non autorizzate.

## Struttura della Repository
* `assets/`: Immagini e schemi concettuali/logici (Schema E-R).
* `docs/`: Documentazione del progetto.
* `sql/`: Script SQL per la creazione e il popolamento del database.
  * `ddl.sql`: Creazione delle tabelle e dei vincoli di integrità.
  * `dml.sql`: Popolamento iniziale con dati di test.
  * `query.sql`: Query di verifica, statistiche e test sui vincoli.

## Documentazione Completa
Questo README è solo una panoramica rapida. Tutta l'analisi tecnica e le scelte progettuali sono documentate nel dettaglio all'interno del report ufficiale in `docs/Bertone_Cristian_Cerise_Manuel.pdf`. Nel documento PDF sono presenti:
* Glossario e Business Rules (come i vincoli di contemporaneità per gli abbonati e le regole sulle multe).
* Tavola dei volumi e delle operazioni.
* Analisi dei costi e gestione delle ridondanze (ad esempio, il calcolo che ci ha portato a mantenere l'attributo dei posti disponibili per risparmiare sulle letture).
* Risoluzione delle gerarchie e schema logico definitivo.
