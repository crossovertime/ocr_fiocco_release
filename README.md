# OCR Fiocco

**OCR Fiocco** è il modulo di Cross Over Time per l'estrazione dei dati dai PDF delle DCR
(modelli A, B, C e fatture), con esportazione in **Excel** e, dove disponibile, nel
**Software DCR** (database Microsoft Access).

Questo repository contiene **solo le versioni distribuite** del programma, pronte da installare.
Le trovi nella sezione **[Releases](../../releases)**.

---

## Requisiti

- Windows 10 o 11 a **64 bit**
- Per l'**Export su Software DCR** (facoltativo): driver *Microsoft Access Database Engine 2016* **a 64 bit**.
  Senza il driver il programma funziona normalmente: i pulsanti dell'export DCR risultano disattivati,
  con il motivo indicato, e l'export in Excel resta disponibile.

## Installazione

1. Apri l'ultima versione in **[Releases](../../releases)** e scarica `OCR_Fiocco_installazione_<data>.zip`.
2. Estrai **il contenuto** dell'archivio in una cartella, ad esempio `C:\dcrfarma\ocr_fiocco`.
3. Avvia `ocr_fiocco.exe`.

Al primo avvio il programma crea da solo i file di configurazione nella propria cartella.

## Aggiornamento

1. Chiudi OCR Fiocco.
2. Scarica la nuova versione da **[Releases](../../releases)**.
3. Estrai il contenuto **sopra la cartella esistente**, confermando la sostituzione dei file.

La configurazione (`config.ini`), le licenze e i dati già presenti **non vengono toccati**:
l'archivio di aggiornamento non li contiene.

## Verifica del file scaricato

Ogni Release riporta l'impronta **SHA-256** dell'archivio e di `ocr_fiocco.exe`.
Per controllare che il file scaricato sia integro e autentico, in PowerShell:

```powershell
Get-FileHash .\OCR_Fiocco_installazione_<data>.zip -Algorithm SHA256
```

Il valore ottenuto deve coincidere con quello indicato nella Release.

## Licenza e modalità dimostrativa

Senza un'autorizzazione rilasciata da Cross Over Time il programma funziona in **modalità dimostrativa**:

- utilizza un database Access di prova (`msaccess_demo\demo_pdf_import.accdb`, creato al primo avvio
  nella radice del disco su cui è installato il programma);
- la finestra di controllo all'avvio e la *Dichiarazione di Autorizzazione* (pulsante "Stampa Info")
  riportano lo stato del servizio.

Per l'attivazione del servizio applicativo presso il proprio Ente, contattare Cross Over Time.

## Contatti

**Cross Over Time**
- Email: [info@crossovertime.it]
- PEC: [crossovertime@pec.it]
