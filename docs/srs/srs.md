**Versione : 1.0**

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
	1. [diagramma](#sp1.1)
	2. [attori](#sp1.2) 
	3. [lista funzionalità](#sp1.3)
2. [Scenari](#p2)
    1. [lista dei corsi a cui l'utente è iscritto](#p2.1)
    2. [lista dei corsi superati](#p2.2)
    3. [lista dei corsi a cui può iscriversi](#p2.3)
    4. [lista dei corsi di cui il docente è insegnante](#p2.4)
    5. [per ogni corso indire un esame](#p2.5)
    6. [per ogni studente registrare un voto](#p2.6)
    7. [visualizzare la lista degli studenti iscritti ad un esame](#p2.7)
    8. [aggiungere un corso](#p2.8)
    9. [inserire un nuovo percorso di studi che può accedere a un corso](#p2.9)
    10. [elimina corso](#p2.10)
    11. [aggiungere uno studente](#p2.11)
    12. [aggiungere un docente](#p2.12)
    13. [associa ad ogni corso un docente](#p2.13)
    14. [elimina studente](#p2.14)
    15. [elimina docente](#p2.15)
    16. [visualizzazione delle segnalazioni](#p2.16)
    17. [segnalazione degli errori](#p2.17)
    18. [login](#p2.18)
    
    
	
  

<a name="p1"></a>

## 1. Usecases


<a name="sp1.1"></a>

### 1.1 Diagramma
![Gestionale_Scuola](https://user-images.githubusercontent.com/113334515/191721870-867f580e-7b92-4557-95eb-cc2fbff3964e.png)


<a name="sp1.2"></a>

### 1.2 Attori
Gli attori sono: Utente, Docente, Segreteria

<a name="sp1.3"></a>

### 1.3 Lista Funzionalità




 

<a name="p2"></a>

## 2. Scenari

<a name="sp2.1"></a>

### 2.1

Caso d’uso			Visualizza Lista Corsi Iscritto

Tipo				Primario

Precondizioni			Essere registrato nel sistema

Scenario Principale		
				
				1 Lo studente scrive matricola corretta

				2 Lo studente scrive password corretta

				3 Lo studente seleziona la propria pagina Profilo

				4 Lo studente seleziona “Visualizza Lista Corsi Iscritto”

				5 Sistema apre una schermata con la lista

Scenario Alternativo		

				1 Lo studente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Post condizioni			Sistema mostra schermata con lista

<a name="sp2.2"></a>

### 2.2

Caso d’uso			Visualizza Lista Corsi Superati

Tipo				Primario

Precondizioni			Essere registrato nel sistema, aver superato almeno un esame

Scenario Principale		

				1 Lo studente scrive matricola corretta

				2 Lo studente scrive password corretta

				3 Lo studente seleziona la propria pagina Profilo

				4 Lo studente seleziona “Visualizza Lista Voti”

				5 Sistema apre una schermata con la lista

Scenario Alternativo		

				1 Lo studente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		

				1 Lo studente non ha ancora ricevuto un voto d’esame

				2 Sistema segnala l’impossibilità, ritorna al punto 3 dello scenario principale

Post condizioni			Sistema mostra schermata con lista

<a name="sp2.3"></a>

### 2.3

Caso d’uso			Visualizza Lista dei Corsi accessibili

Tipo				Primario

Precondizioni			Essere registrato nel sistema, essere in regola coi pagamenti

Scenario Principale		

				1 Lo studente scrive matricola corretta

				2 Lo studente scrive password corretta

				3 Lo studente seleziona la propria pagina Profilo

				4 Lo studente seleziona “Visualizza Lista Corsi accessibili”

				5 Sistema apre una schermata con la lista

Scenario Alternativo		

				1 Lo studente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		

				1 Lo studente ha già superato tutti gli esami

				2 Sistema segnala l’impossibilità, ritorna al punto 3 dello scenario principale

Scenario Alternativo		

				1 Lo studente non è in regola con il pagamento delle tasse

				2 Sistema segnala l’inadempienza, ritorna al punto 3 dello scenario principale

Post condizioni			Sistema mostra schermata con lista 

<a name="sp2.4"></a>

### 2.4

Caso d’uso			Visualizza lista corsi in cui insegna

Tipo				Primario

Precondizioni			Essere registrato nel sistema, avere almeno un corso

Scenario Principale		

				1 Docente scrive matricola corretta

				2 Docente scrive password corretta

				3 Docente seleziona la propria pagina Profilo

				4 Docente seleziona “Visualizza Lista Corsi Docente”

				5 Sistema apre una schermata con la lista

Scenario Alternativo		

				1 Docente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		

				1 Docente non ha nessuna docenza

				2 Sistema segnala la mancanza, ritorna al punto 3 dello scenario principale

Post condizioni			Sistema mostra schermata con lista

<a name="sp2.5"></a>

### 2.5

Caso d’uso			Indire un esame per corso in cui insegna

Tipo				Primario

Precondizioni			Essere registrato nel sistema, avere almeno un corso

Scenario Principale		

				1 Docente scrive matricola corretta

				2 Docente scrive password corretta

				3 Docente seleziona la propria pagina Profilo

				4 Docente seleziona “Inserisci Nuova data esame”

				5 Sistema apre una schermata con la lista delle materie insegnate 

				6 Docente seleziona un corso

				7 Sistema apre un calendario con le possibili date selezionabili

				8 Docente seleziona una data

Scenario Alternativo		

				1 Docente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		

				1 Docente non ha nessuna docenza

				2 Sistema segnala la mancanza, ritorna al punto 3 dello scenario principale

Post condizioni			Sistema mostra schermata con lista 

<a name="sp2.6"></a>

### 2.6

Caso d’uso			Registrare un voto

Tipo				Primario

Precondizioni			Essere registrato nel sistema, avere almeno un corso

Scenario Principale		

				1 Docente scrive matricola corretta

				2 Docente scrive password corretta

				3 Docente seleziona la propria pagina Profilo

				4 Docente seleziona “Inserisci Voto esame”

				5 Sistema apre una schermata con la lista delle materie insegnate 

				6 Docente seleziona un corso

				7 Sistema apre una schermata con la lista degli studenti iscritti

				8 Docente seleziona uno studente

				9 Sistema apre un menù a tendina con un elenco di voti da 1 a 30

Scenario Alternativo		

				1 Docente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		

				1 Docente non ha nessuna docenza

				2 Sistema segnala la mancanza, ritorna al punto 3 dello scenario principale

Scenario Alternativo		

				1 Nessun studente ha ancora dato l’esame

				2 Sistema segnala la mancanza, ritorna al punto 6 dello scenario principale

Post condizioni			Sistema mostra schermata con lista

<a name="sp2.7"></a>

### 2.7

Caso d’uso			Visualizza lista iscritti ad un esame

Tipo				Primario

Precondizioni			Essere registrato nel sistema, avere almeno un corso

Scenario Principale		

				1 Docente scrive matricola corretta

				2 Docente scrive password corretta

				3 Docente seleziona la propria pagina Profilo

				4 Docente seleziona “Visualizza Lista esame”

				5 Sistema apre una schermata con la lista degli esami già fissati

				6 Docente seleziona un esame/data

				7 Sistema visualizza una schermata con gli studenti iscritti all’appello

Scenario Alternativo		

				1 Docente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		

				1 Docente non ha nessuna docenza

				2 Sistema segnala la mancanza, ritorna al punto 3 dello scenario principale

Post condizioni			SW mostra schermata con lista 

<a name="sp2.8"></a>

### 2.8


Caso d’uso: aggiungere nuovo corso

Tipo: secondario

Precondizioni: avere info corso

Scenario principale: 

				1- effettuare l’accesso alla piattaforma

				2- tra le operazioni che può effettuare la segreteria scegliere aggiungere un nuovo corso

				3- compilare i campi con le informazioni sul corso e selezionare quali corsi di studio 
				possono accedere a questo corso       


Scenario alternativo: nel caso di problemi di accesso alla piattaforma 

				1- cliccare su recupero password

				2- inviare un'email con un link per resettare la password

				3- cliccare sul link e resettare la password

				4- ritentare l’accesso con la nuova password

Post condizioni: 


<a name="sp2.9"></a>

### 2.9






Caso d’uso: inserire un nuovo percorso di studi che può accedere a un corso


Tipo: secondario

Precondizioni: avere info docente, del corso

Scenario principale: 

				1- effettuare l’accesso alla piattaforma

				2- tra le operazioni che può effettuare la segreteria scegliere aggiungere corso al percorso di studio

				3- compilare i campi con il corso di studio, obiettivi e CFU



Scenario alternativo: nel caso di problemi di accesso alla piattaforma 

				1- cliccare su recupero password

				2- inviare un'email con un link per resettare la password

				3- cliccare sul link e resettare la password

				4- ritentare l’accesso con la nuova password



Post condizioni: tutti gli studenti del corso di studio aggiunto ora potranno accedere al corso


<a name="sp2.10"></a>

### 2.10


Caso d’uso: elimina corso

Tipo: secondario

Precondizioni:	avere il codice corso e il nome del corso

Scenario principale: 

				1- effettuare l’accesso alla piattaforma

				2- tra le operazioni che può effettuare la segreteria scegliere rimuovere corso

				3- inserire il codice del corso ed effettuare la ricerca di tale corso

				4- se il codice del corso corrisponde al corso che si desidera eliminare cliccare sul corso e poi su elimina


Scenario alternativo: se il codice non corrisponde

				1- cancellare dalla barra di ricerca il codice e provare ad inserire il nome del corso

				2- se il nome del corso corrisponde al corso che si desidera eliminare cliccare sul corso e poi su elimina

Post condizioni: se il corso è in corso allora tenere una coda con i corsi attivi e fino alla scadenza dei corsi attivi mantenere il corso e poi eliminarlo



<a name="sp2.11"></a>

### 2.11

Caso d’uso: aggiungere studente

Tipo: secondario

Precondizioni: avere info studente

Scenario principale:

				1- effettuare l’accesso alla piattaforma

				2- tra le operazioni che può effettuare la segreteria scegliere aggiungere studente

				3- compilare i campi con i dati dello studente compreso il percorso di studi da lui scelto

				4- cliccare su aggiungi studente

				5- inviare una mail di benvenuto allo studente comprese le credenziali per accedere alla piattaforma

Scenario alternativo:

Post condizioni: lo studente può accedere ai corsi e agli esami



<a name="sp2.12"></a>

### 2.12

<a name="sp2.13"></a>

### 2.13

<a name="sp2.14"></a>

### 2.14

<a name="sp2.15"></a>

### 2.15

<a name="sp2.16"></a>

### 2.16

<a name="sp2.17"></a>

### 2.17
Caso d’uso: visualizzazione segnalazioni

Tipo: secondario

Precondizioni: ricevere notifiche

Scenario principale:

				1- effettuare l’accesso alla piattaforma

				2- tra le operazioni che può effettuare la segreteria scegliere visualizza segnalazioni

				3- legge le segnalazioni inviate dai docenti e dagli studenti

Scenario alternativo:

Post condizioni:


<a name="sp2.18"></a>

### 2.18

