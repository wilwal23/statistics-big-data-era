# statistics-big-data-era

Repository containing the small and big project related to the course of Statistics in the Big Data Era, developed and maintained by R. Giussani.

## Covid

This section includes datasets, code and report of a study aimed at finding relations between Covid-19 cases, lockdowns and drugs' sale during and/or after the Covid-19 pandemic in Italy.

### Datasets 
The data considered are the following:
- **Covid cases monitoring** (cases, ICU, hospitalization, ...)(20200224-20230219)<br />
Source: [Dipartimento della Protezione Civile](https://emergenze.protezionecivile.gov.it/en/health/coronavirus)<br />
Repository: [github repository](https://github.com/pcm-dpc/COVID-19)
- **Regional lockdown history** (region-by-region lockdown status during the pandemic)(20201106-20220328)<br />
Source: [OnData association](https://www.ondata.it/)<br />
Repository: [github repository](https://github.com/ondata/covid19italia/blob/master/webservices/COVID-19Aree/processing/areeStorico.csv)<br />
NOTE: actual data retrieved from [Gazzetta Ufficiale](https://www.gazzettaufficiale.it/) and [Ministero della Salute](https://www.trovanorme.salute.gov.it/) 
- **Drugs sale data by drug type** (region-by-region, month-by-month)(20160101-20211231)<br />
Source: [Agenzia Italiana del Farmaco (AIFA)](https://www.aifa.gov.it/web/guest)<br />
Repository: [official website](https://www.aifa.gov.it/web/guest/spesa-e-consumo-relativi-al-flusso-della-farmaceutica-convenzionata-e-degli-acquisti-diretti)

#### Datasets example
- **Covid cases monitoring**

|data|stato|codice_regione|denominazione_regione|lat|long|ricoverati_con_sintomi|terapia_intensiva|totale_ospedalizzati|isolamento_domiciliare|totale_positivi|variazione_totale_positivi|nuovi_positivi|dimessi_guariti|deceduti|casi_da_sospetto_diagnostico|casi_da_screening|totale_casi|tamponi|casi_testati|note|ingressi_terapia_intensiva|note_test|note_casi|totale_positivi_test_molecolare|totale_positivi_test_antigenico_rapido|tamponi_test_molecolare|tamponi_test_antigenico_rapido|codice_nuts_1|codice_nuts_2|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|2023-01-01T17:00:00|ITA|13|Abruzzo|42.35122196|13.39843823|241|11|252|15874|16126|379|536|617497|3831|637454||7283064|1354465|||0|||241385|396069|2559894|4723170|ITF|ITF1|

- **Regional lockdown history**

|anno|mese|codreg|regione|classe|atc1|descrizione_atc1|atc2|descrizione_atc2|atc3|descrizione_atc3|atc4|descrizione_atc4|numero_confezioni_traccia|spesa_flusso_tracciabilita|numero_confezioni_convenzionata|spesa_convenzionata|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|2016|01|010|PIEMONTE|C|A|Apparato gastrointestinale e metabolismo|A01|Stomatologici|A01A|Stomatologici|A01AA|Sostanze impiegate per la profilassi della carie|2|13.42|

- **Drugs sale data by drug type**

|NUTS_code|datasetIniISO|versionID|nomeTesto|FID|datasetIni|datasetFin|designIniz|designFine|nomeAutCom|legNomeBre|legData|legLink|legSpecRif|legLivello|legGU_Link|zona|datasetFinISO|NUTS_level|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|ITF6|2020-11-06|1|Calabria|0|06/11/2020|20/11/2020|1604620800000|20/11/2020|Ministero della Salute|Ordinanza 04/11/2020|1604448000000|https://www.trovanorme.salute.gov.it/norme/dettaglioAtto?id=77054|art.3|regionale|https://www.gazzettaufficiale.it/eli/id/2020/11/05/20A06144/sg|rossa|2020-11-20|2|

#### Doubts 
Data are taken from different time periods, only a subset of the datasets is suitable to define a relation between variables, correct? Will it be enough?

![alt text](https://github.com/wilwal23/statistics-big-data-era/blob/main/datasets-timespan.png?raw=true)
