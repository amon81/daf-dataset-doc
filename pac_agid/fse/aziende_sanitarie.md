# AGID FSE: Aziende sanitarie

## Descrizione del dataset


**Tipo di dataset:** ordinary

**Tipo di flusso:** batch

**Tipo di file:** JSON

**Scheda:** 

**Modalità di ingestion su DAF:** scarico su SFTP


## Elementi
| Nome | Tipo   | Descrizione                     |
|------|--------|---------------------------------|
| id | long | id del record |
| denominazione | string | denominazione dell'azienda sanitaria |
| paid | int | identificativo interno della Regione di appartenza |
| pa | string | denominazione della Regione di appartenenza |
| indirizzo | string | |
| cap | string | |
| comune | string | |
| provincia | string | |
| telefono | string | |
| sitoweb | string | |
| codice_azienda | string | |
| regione | string | codice regione fornito dal fornitore dei dati delle aziende sanitarie |
| codice_asl | string | |
| data_istituzione | date | |
| data_fine | date | data cessazione fornita dal fornitore dei dati delle aziende sanitarie |
| denominazione_struttura | string | |
| codice_tipo_struttura | string | |
| tipo | int | Tipo di azienda sanitaria: <br> 0 = ASL <br> 1 = Aziende Ospedaliere <br> 2 = Istituti di ricovero e cura a carattere scientifico <br> 3 = Fondazioni pubbliche |
| descrizione_tipo_struttura | string | |
| anno | int | |
| codice_struttura | string | |
| subcodice | string | |
| denominazione_stabilimento | string | |
| comune_stabilimento | string | |
| cap_stabilimento | string | |


## Esempio del flusso

```
[
  {
    "id": 1214,
    "paid": 12,
    "denominazione": "TO3",
    "cap": null,
    "indirizzo": null,
    "provincia": null,
    "comune": null,
    "regione": "010",
    "telefono": null,
    "sitoweb": null,
    "codice_asl": null,
    "tipo": 0,
    "codice_azienda": null,
    "denominazione_struttura": null,
    "codice_tipo_struttura": null,
    "descrizione_tipo_struttura": null,
    "anno": "2016",
    "codice_struttura": "010203",
    "subcodice": null,
    "denominazione_stabilimento": null,
    "cap_stabilimento": null,
    "comune_stabilimento": null,
    "data_fine": null,
    "data_istituzione": null,
    "pa": "Regione Piemonte"
  },
  ...
]
```

