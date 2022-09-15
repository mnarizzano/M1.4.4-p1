**VERSION : 1.0**

**Autori**  
Dana Luta
Matteo Bonino
Sara Urdangaray

**REVISIONE N.**


| Version    | Date        | Authors      | Notes        |
| ----------- | ----------- | ----------- | ----------- |
| 0.5 | 15/09/22 | Matteo | Studente |
| 0.5 | 15/09/22 | Sara | Corso, Esame, Voto |
| 0.5 | 15/09/22 | Dana | Docente |
# Tabella dei contenuti

1. [Introduzione](#p1)
	1. [Obbiettivi del documento](#sp1.1)
	2. [Definizioni e Acronimi](#sp1.2) 
	3. [Riferimenti](#sp1.3)
2. [Descrizione del Sistema](#p2)
	1. [Contenuti e Motivazioni](#sp2.1)
	2. [Obbiettivi del Progetto](#sp2.2)
3. [Richieste](#p3)
 	1. [Soggetti](#sp3.1)
 	2. [Richieste Funzionali](#sp3.2)
 	3. [Richieste non Funzionali](#sp3.3)
  
  

<a name="p1"></a>

## 1. Introduzione

<a name="sp1.1"></a>
Su richiesta dell'Università degli Studi di Genova con lo scopo  di  sostituire il
sistema cartaceo, il presente Software permetterà di effettuare le operazioni in base alla 
tipologia di utente, tramite l'utilizzo di un PC o smartphone,garantendo al tempo stesso accuratezza e sicurezza.

### 1.1 Obbiettivi del Documento
Lo scopo  di questo documento è quello di illustrare ogni aspetto del Software, presentare 
le sue features, nonché essere anche una guida introduttiva sul suo funzionamento.

<a name="sp1.2"></a>

### 1.2 Definizione e Acronimi

| Acronym				| Definition | 
| ------------------------------------- | ----------- | 
| SW                                    | Software |
| GUI					| Graphical User Interface |
| Login					| Autenticazione Accesso |

<a name="sp1.3"></a>

### 1.3 Riferimenti 

<a name="p2"></a>

## 2. Descrizione Del Sistema 
<a name="sp2.15"></a>
Il SW può essere essenzialmente definito come un Gestionale: esso permette a studenti e 
docenti di visualizzare e agire sugli esami universitari - in maniera appropriata in base 
al tipo di utente. Attraverso una GUI, l'utente potrà effettuare diverse operazioni 
online senza la necessità di presentarsi personalmente all'Università.

### 2.1 Contenuti e Motivazioni
Il contesto di utilizzo previsto è nell'ambito dell'istruzione: per come il SW è progettato
può essere applicabile ad altre tipologie di istituti scolastici.
Il SW ha lo scopo di ridurre le tempistiche e i costi dovuti all'attuale sistema in uso 
presso l'Università di Genova, che prevede la compilazione di moduli cartacei, richiedendo
quindi la presenza di personale ad hoc per la compilazione e la successiva comunicazione 
tra studente e docente.
Permettere la fruizione dei servizi anche a distanza, in particolare per venire incontro
a studenti fuori sede, con disabilità motorie, e per ridurre i contatti fisici in seguito 
alla pandemia CoVid 19.

<a name="sp2.2"></a>

### 2.2 Obbiettivi del Progetto 
Realizzare un SW che sia in grado di funzionare sulla maggior parte delle piattaforme in 
uso: PC Windows, PC MacOS, smartphone iOS e Android. 
Realizzazione di un'ambiente di sistema che permetta di non avere ridondanza di dati e 
che abbia requisiti hardware minimi molto accessibili.

<a name="p3"></a>

## 3. Richieste

| Priorità | Significato | 
| --------------- | ----------- | 
| M | **Mandatorio:**   |
| D | **Desiderabile:** |
| O | **Opzionale:**    |
| E | **Futura Espansione:** |

<a name="sp3.1"></a>
### 3.1 Soggetti
Client: Università degli Studi di Genova, Città Metropolitana di Genova, Assessore 
della Cultura
Regulators: un team dedicato alla verifica del rispetto dei regolamenti universitari 
vigenti al fine di garantire massima trasparenza e regolarità delle procedure
Users: studenti e docenti sono in primis coloro che agiranno sul SW; avranno altresì 
accesso anche il personale universitario, amministrativo e direttivo

<a name="sp3.2"></a>
### 3.2 Richieste Funzionali

| ID | Descrizione | Priorità |
| --------------- | ----------- | ---------- | 
| 1.0 |  Docente potrà visualizzare i corsi di cui è docente  |M|
| 1.1 |  Docente potrà indire un esame per ogni corso |M|
| 1.2 |  Docente potrà visualizzare la lista degli iscritti all'esame |M|
| 1.3 |  Docente potrà registrare un voto per ogni studente iscritto |M|
| 2.0 |  Studente potrà visualizzare la lista dei corsi a cui è iscritto |M|
| 2.1 |	 Studente potrà visualizzare la lista dei corsi superati con il voto |M|
| 2.2 |  Studente potrà visualizzare la lista degli esami a cui iscriversi |M|
| 2.3 |  Studente potrà iscriversi nuovamente ad un esame se non superato |M|
| 3.0 |  Studente e Docente dovrebbero avere la possibilità di segnalare eventuali errori |D|
| 3.1 |  Il SW dovrebbe permettere di estrarre dei files PDF delle liste |D|
| 4.0 |  Il SW dovrebbe permettere di visualizzare lo stato delle operazioni |O|

<a name="sp3.3"></a>
### 3.2 Richieste non funzionali 
 
| ID | Descrizione | Priorità |
| --------------- | ----------- | ---------- | 
| 1.0 | Il SW deve poter gestire un numero di almeno 2000000 utenti in contemporanea |M|
| 1.1 | Il SW deve essere compatibile con PC Windows e PC MacOS |M|
| 2.1 | Il SW dovrebbe poter essere compatibile con smartphone iOS e Android |D|
| 3.1 | Il SW dovrebbe essere accessibile a persone ipovedenti |O|
| 3.2 | Il SW dovrebbe essere disponibile in inglese, francese, tedesco, spagnolo |O|
