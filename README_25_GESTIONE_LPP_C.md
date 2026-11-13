# PROGETTO OLD GESTIONE LLPP_C
## NOTE
		Il vecchio progetto di gestione dei lavori pubblici è stato ricostruito utilizzando i dati salvati a casa
		con tutte le path originali.
		Gli archivi con le path originali sono state salvate in questa cartella :
			START "APRI LE PATH ORIGINALI TOLTA LA ZZ_CASA_MARINO" "c:\Gestioni\GESTIONE_LLPP\25_GESTIONE_LLPP\ZZ_CASA_MARINO\"
		Al suo interno c'è la cartella 25_GESTIONE_LLPP con i salvataggi fino a marzo 2025.

		tutte le altre cartelle della directory casa sono state ricostruite in questa path e l'albero delle
		sottocartelle è il seguente: 

		c:\Gestioni\GESTIONE_LLPP\
			|
			|--01_POSTA_BOZZE
			|--02_SCANNER
			|--03_FATTURE_SCARICATE
			|--03_PLUS
			|--04_ANAC_ATTESTAZIONI
			|--07_EMAIL
			|--08_MODELLI
			|--10_LEGGI
			|--11_OUTLOOK
			|--12_BILANCIO
			|--14_FINANZIAMENTI_RL
			|--17_PEG_E_BILANCIO
			|--25_GESTIONE_LLPP                = archivi e gestionale .mdb
			|--26_RESIDUI
			|--27_APPALTI
			|--71_TRASPARENZA
			|--98_DESKTOP
			|--99_GESTIONI_SERVIZI

	todo: continuare allineamento tra c ed Y.


	

# PROGETTO 25_GESTIONE_LLPP_C
## Note
		questo è il progetto di gestione dei lavori pubblici su C ossia la parte di gestione con i collegamenti; la 
		path di salvataggio è : 
			c:\GESTIONE_LLPP\25_GESTIONE_LLPP\
				c:\GESTIONI\GESTIONE_LLPP\25_GESTIONE_LLPP\ARCHIVI_ACCESS_LLPP_C\C_LLPP_GESTIONE\

## PATH_PROGETTI_APRI
			Note
				il progetto di archiviazione si trova su Y con tutti gli archivi di access, ma la gestione avviene su 
				C: nel futuro si potra anche prevedere di salvare gli archivi su C invia provvisoria ma si deve studiare.

		PROGETTO_C
			Se vuoi apri il progetto nella gestione utente, C: occorre aprire questa path:
				start "APRI PROGETTO 25_GESTIONE_LPP SU C" "c:\GESTIONE_LLPP\25_GESTIONE_LLPP\"
		PROGETTO_Y	
			Se devi aprire i salvataggi del progetto SU Y occorre fare riferimento a questa path:

			 	START "APRI PROGETTO SU Y:" "y:\LAVORI_PUBBLICI_FINO_AL_30_09_2019\Valter\OPERE_PUBBLICHE\96_ARCHIVI_LLPP_MDB\25_GESTIONE_LLPP_Y\"

## DIAGRAMMA


# STRUTTURA DEL SISTEMA MULTIPROGETTO

## C_LLPP_GESTIONE — CARTELLA MASTER

> **Scopo:** rappresentazione generale della struttura del sistema Access multiprogetto per la gestione degli atti dei Lavori Pubblici.
	deve essere aggiornata ad ogni modifica.

## 1. DIAGRAMMA GENERALE

TODO: da fare

---

## 2. ALBERO DELLA CARTELLA MASTER

```text
C_LLPP_GESTIONE
│
├── 📁 AA_SALVATAGGI_CARTELLE_ELENCO
│   │
│   ├── 📁 2026_08_12_BACKUP_C_MDB
│   ├── 📁 2026_08_19_BACKUP_C_MDB
│   └── 📁 2026_08_26_BACKUP_C_MDB
│
├── 📁 C_MDB
│   │
│   ├── 📁 C_LLPP_ATTI_PROJECT
│   │
│   ├── 📁 C_LLPP_ATTI_Tb01_GESTIONE
│   │   └── 📁 MDB
│   │
│   ├── 📁 C_LLPP_ATTI_Tb02_ALLEGATI
│   │   ├── 📁 MDB
│   │   │   └── 📁 Logs
│   │   └── 📁 OBJECT
│   │       ├── 📁 MODULO_ALLEGATI_AGGIORNA_Y_C
│   │       ├── 📁 QUERY_ALLEGATI_INSERT
│   │       ├── 📁 QUERY_ALLEGATI_SELECT
│   │       ├── 📁 QUERY_ALLEGATI_UNION
│   │       └── 📁 QUERY_ALLEGATI_UPDATE
│   │
│   ├── 📁 C_LLPP_ATTI_TB03_IMPEGNI
│   │   ├── 📁 Logs
│   │   ├── 📁 MDB
│   │   │   └── 📁 Logs
│   │   └── 📁 OBJECT
│   │       ├── 📁 QUERY
│   │       │   ├── 📁 QUERY_GROUP_TB03
│   │       │   ├── 📁 QUERY_SELECT
│   │       │   └── 📁 QUERY_UPDATE
│   │       └── 📁 TABLE
│   │
│   ├── 📁 C_LLPP_ATTI_TB04_VISTO_CONTABILE
│   │   └── 📁 MDB
│   │       └── 📁 Logs
│   │
│   ├── 📁 C_LLPP_ATTI_TB05_PER_ISTRUTTORE
│   │   ├── 📁 MDB
│   │   │   └── 📁 Logs
│   │   │
│   │   └── 📁 OBJECT
│   │       ├── 📁 CHATGBT
│   │       ├── 📁 FORMS
│   │       │   ├── 📁 FORMS_DETERMINE
│   │       │   ├── 📁 FORMS_GROUP
│   │       │   ├── 📁 FORMS_NOTE
│   │       │   ├── 📁 FORMS_XLS
│   │       │   └── 📁 FORM_ISTRUTTORE
│   │       │
│   │       ├── 📁 HELP
│   │       │   └── 📁 HELP_FORM_LLPP_ATTI_Tb05_Frm99_ISTRUTTORE_SERVIZI
│   │       │
│   │       ├── 📁 MODULES
│   │       ├── 📁 QUERY
│   │       │   ├── 📁 QUERY_EXPORT_SELECT
│   │       │   ├── 📁 QUERY_EXPORT_UPDATE
│   │       │   ├── 📁 QUERY_LLPP_ATTI_TB05_01_SELECT
│   │       │   ├── 📁 QUERY_LLPP_ATTI_TB05_06_NOTE
│   │       │   ├── 📁 QUERY_LLPP_ATTI_TB05_11_GROUP
│   │       │   ├── 📁 QUERY_LLPP_ATTI_TB05_13_DELETE
│   │       │   ├── 📁 QUERY_LLPP_ATTI_TB05_60_UPDATE
│   │       │   ├── 📁 QUERY_LLPP_ATTI_TB05_70_INSERT_(ACCODA)
│   │       │   ├── 📁 QUERY_LLPP_ATTI_TB05_DELIBERE
│   │       │   ├── 📁 QUERY_LLPP_ATTI_TB05_DETERMINE
│   │       │   ├── 📁 QUERY_XLS
│   │       │   ├── 📁 QUERY_XWORK_INSERT_70
│   │       │   ├── 📁 QUERY_XWORK_SELECT
│   │       │   └── 📁 QUERY_XWORK_UPDATE
│   │       │
│   │       ├── 📁 TABLES
│   │       └── 📁 XLS
│   │
│   ├── 📁 C_LLPP_DF13_CONTEGGI_UNION
│   │
│   └── 📁 C_LLPP_DF99_LINK
│       ├── 📁 LOGS
│       ├── 📁 MDB
│       │   └── 📁 LOGS
│       └── 📁 OBJECT
│           ├── 📁 FORM
│           ├── 📁 MODULI
│           └── 📁 QUERY
│
├── 📁 C_OBJECT
│   │
│   ├── 📁 FORMS-(SISTEMARE)
│   │
│   ├── 📁 QUERY_(SISTEMARE)
│   │
│   ├── 📁 Tb01_GESTIONE
│   │   ├── 📁 Tb01_QUERY_INSERT
│   │   └── 📁 Tb01_QUERY_SELECT
│   │       └── 📁 INSERT_ATTI
│   │
│   └── 📁 Tb02_ALLEGATI
│
├── 📁 LOGS
│
├── 📄 DOS_FOR_N05_SALVA_CARTELLE_ARCHIVI_ACCESS_LLPP.bat
├── 📦 DOS_FOR_N05_SALVA_CARTELLE_ARCHIVI_ACCESS_LLPP.zip
│
├── 📄 Project_C_LLPP_GESTIONE.sublime-project
├── 📄 Project_C_LLPP_GESTIONE.sublime-workspace
├── 📄 Project_C________________________________________________________________.txt
├── 📄 README_C_LLPP_GESTIONE.MD
├── 📄 AA________________________________________________________________________AA.txt
├── 📄 ZZ________________________________________________________________________ZZ.txt
└── 📄 a.txt
```

---

## 3. MAPPA FUNZIONALE DEL SISTEMA

```text
                         ┌──────────────────────────────┐
                         │      C_LLPP_GESTIONE         │
                         │       CARTELLA MASTER        │
                         └──────────────┬───────────────┘
                                        │
              ┌─────────────────────────┼─────────────────────────┐
              │                         │                         │
              ▼                         ▼                         ▼
       ┌──────────────┐          ┌──────────────┐          ┌──────────────┐
       │    C_MDB     │          │  C_OBJECT    │          │   BACKUP     │
       │  DATABASE    │          │   OGGETTI    │          │ SALVATAGGI   │
       └──────┬───────┘          └──────────────┘          └──────────────┘
              │
      ┌───────┼───────────────────────────────────────┐
      │       │       │       │       │       │       │
      ▼       ▼       ▼       ▼       ▼       ▼       ▼
     TB01    TB02    TB03    TB04    TB05    DF13    DF99
   GESTIONE ALLEGATI IMPEGNI VISTO  ISTRUTT. CONTEGGI LINK
                              CONTABILE
      │       │       │       │       │
      │       │       │       │       └──────────────┐
      │       │       │       │                      │
      ▼       ▼       ▼       ▼                      ▼
     MDB     MDB     MDB     MDB                   MDB
             │       │                           OBJECT
             │       │
             ▼       ▼
          OBJECT   OBJECT
                    │
          ┌─────────┴─────────┐
          ▼                   ▼
        QUERY                TABLE
```

---

## 4. RUOLO DELLE PRINCIPALI CARTELLE

| Cartella                           | Funzione                                                        |
| ---------------------------------- | --------------------------------------------------------------- |
| `C_LLPP_GESTIONE`                  | **Master dell'intero sistema multiprogetto**                    |
| `C_MDB`                            | Contiene i **sottoprogetti Access** e relativi database         |
| `C_OBJECT`                         | Contiene gli **oggetti/documentazione esportati e condivisi**   |
| `AA_SALVATAGGI_CARTELLE_ELENCO`    | Contiene i **backup storici**                                   |
| `LOGS`                             | Log generali del sistema                                        |
| `C_LLPP_ATTI_PROJECT`              | Progetto/documentazione generale degli atti                     |
| `C_LLPP_ATTI_Tb01_GESTIONE`        | Gestione principale degli atti                                  |
| `C_LLPP_ATTI_Tb02_ALLEGATI`        | Gestione degli allegati                                         |
| `C_LLPP_ATTI_TB03_IMPEGNI`         | Gestione degli impegni                                          |
| `C_LLPP_ATTI_TB04_VISTO_CONTABILE` | Gestione del visto contabile                                    |
| `C_LLPP_ATTI_TB05_PER_ISTRUTTORE`  | Gestione per istruttore                                         |
| `C_LLPP_DF13_CONTEGGI_UNION`       | Area conteggi/UNION                                             |
| `C_LLPP_DF99_LINK`                 | Gestione dei collegamenti alle tabelle/database                 |
| `OBJECT`                           | Componenti Access esportati: form, query, moduli, tabelle, ecc. |
| `MDB`                              | Database Access fisici dei singoli sottoprogetti                |

---

## 5. PRINCIPIO ARCHITETTURALE

	La struttura attuale evidenzia una separazione in **tre livelli principali**:
	
	```text
	C_LLPP_GESTIONE
	│
	├── 01 - BACKUP
	│      └── AA_SALVATAGGI_CARTELLE_ELENCO
	│
	├── 02 - DATABASE / SOTTOPROGETTI
	│      └── C_MDB
	│           ├── TB01 - GESTIONE
	│           ├── TB02 - ALLEGATI
	│           ├── TB03 - IMPEGNI
	│           ├── TB04 - VISTO CONTABILE
	│           ├── TB05 - ISTRUTTORE
	│           ├── DF13 - CONTEGGI UNION
	│           └── DF99 - LINK
	│
	├── 03 - OGGETTI CONDIVISI
	│      └── C_OBJECT
	│
	└── 04 - CONTROLLO E DOCUMENTAZIONE
       	├── LOGS
       	├── README
       	├── PROJECT
       	├── WORKSPACE
       	└── SCRIPT / BAT
	```
	
	---

## 6. OSSERVAZIONE SULLA RIORGANIZZAZIONE

La struttura mostra già una distinzione importante:

C_MDB` = applicazioni/database operativi**

C_OBJECT` = archivio degli oggetti Access esportati o da riorganizzare**

AA_SALVATAGGI_CARTELLE_ELENCO` = storico dei backup**


Questa distinzione può diventare la **base architetturale della nuova organizzazione del multiprogetto**, mantenendo `C_LLPP_GESTIONE` come unico contenitore MASTER.

---

## 7. NOTA SULLA SITUAZIONE ATTUALE

LOGS = tracciamento delle operazioni, deve essere creato per ogni sottocartella di progetto

La struttura rilevata contiene anche cartelle esplicitamente indicate come:

OBJECT = ogni sottocartella di progetto deve avere la cartella object che rappresenta ogni 
oggetto del mini progetto.


---

## 8. RAPPRESENTAZIONE SINTETICA

```text
                         C_LLPP_GESTIONE
                         MASTER SYSTEM
                              │
        ┌─────────────────────┼─────────────────────┐
        │                     │                     │
        ▼                     ▼                     ▼
     C_MDB                da definire            BACKUP
        │                     │                     │
        │                     │                     └─ AA_SALVATAGGI...
        │                     │
        │                     ├─ 
        │                     ├─ 
        │                     ├─
        │                     └
        │
        ├─ TB01 GESTIONE
        ├   |____MDB
        ├   |____LOGS
        |   
        ├─ TB02 ALLEGATI
        ├─ TB03 IMPEGNI
        ├─ TB04 VISTO CONTABILE
        ├─ TB05 ISTRUTTORE
        ├─ DF13 CONTEGGI UNION
        └─ DF99 LINK

                         
```

**Questa è la struttura di riferimento del sistema `C_LLPP_GESTIONE` rilevata al 26/08/2026.**

