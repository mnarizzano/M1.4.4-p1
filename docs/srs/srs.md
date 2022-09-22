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
    3. [](#p2.3)
    4. [](#p2.4)
    5. [](#p2.5)
    6. [](#p2.6)
    7. [](#p2.7)
    8. [](#p2.8)
    9. [](#p2.9)
    10. [](#p2.10)
    11. [](#p2.11)
    12. [](#p2.12)
    13. [](#p2.13)
    14. [](#p2.14)
    15. [](#p2.15)
    16. [](#p2.16)
    17. [](#p2.17)
    18. [](#p2.18)
    19. [](#p2.19)
    
    
	
  

<a name="p1"></a>

## 1. Usecases


<a name="sp1.1"></a>

### 1.1 Diagramma


<a name="sp1.2"></a>

### 1.2 Attori


<a name="sp1.3"></a>

### 1.3 Lista Funzionalità




 

<a name="p2"></a>

## 2. Scenari

<a name="sp2.1"></a>

### 2.1

Caso d’uso			Visualizza Lista Corsi Iscritto

Tipo				Primario

Precondizioni			Essere registrato nel sistema

Scenario Principale		1 Lo studente scrive matricola corretta

				2 Lo studente scrive password corretta

				3 Lo studente seleziona la propria pagina Profilo

				4 Lo studente seleziona “Visualizza Lista Corsi Iscritto”

				5 Sistema apre una schermata con la lista

Scenario Alternativo		1 Lo studente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Post condizioni			Sistema mostra schermata con lista

<a name="sp2.2"></a>

### 2.2

Caso d’uso			Visualizza Lista Corsi Superati

Tipo				Primario

Precondizioni			Essere registrato nel sistema, aver superato almeno un esame

Scenario Principale		1 Lo studente scrive matricola corretta

				2 Lo studente scrive password corretta

				3 Lo studente seleziona la propria pagina Profilo

				4 Lo studente seleziona “Visualizza Lista Voti”

				5 Sistema apre una schermata con la lista

Scenario Alternativo		1 Lo studente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		1 Lo studente non ha ancora ricevuto un voto d’esame

				2 Sistema segnala l’impossibilità, ritorna al punto 3 dello scenario principale

Post condizioni			Sistema mostra schermata con lista

<a name="sp2.3"></a>

### 2.3

Caso d’uso			Visualizza Lista dei Corsi accessibili

Tipo				Primario

Precondizioni			Essere registrato nel sistema, essere in regola coi pagamenti

Scenario Principale		1 Lo studente scrive matricola corretta

				2 Lo studente scrive password corretta

				3 Lo studente seleziona la propria pagina Profilo

				4 Lo studente seleziona “Visualizza Lista Corsi accessibili”

				5 Sistema apre una schermata con la lista

Scenario Alternativo		1 Lo studente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		1 Lo studente ha già superato tutti gli esami

				2 Sistema segnala l’impossibilità, ritorna al punto 3 dello scenario principale

Scenario Alternativo		1 Lo studente non è in regola con il pagamento delle tasse

				2 Sistema segnala l’inadempienza, ritorna al punto 3 dello scenario principale

Post condizioni			Sistema mostra schermata con lista 

<a name="sp2.4"></a>

### 2.4

Caso d’uso			Visualizza lista corsi in cui insegna

Tipo				Primario

Precondizioni			Essere registrato nel sistema, avere almeno un corso

Scenario Principale		1 Docente scrive matricola corretta

				2 Docente scrive password corretta

				3 Docente seleziona la propria pagina Profilo

				4 Docente seleziona “Visualizza Lista Corsi Docente”

				5 Sistema apre una schermata con la lista

Scenario Alternativo		1 Docente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		1 Docente non ha nessuna docenza

				2 Sistema segnala la mancanza, ritorna al punto 3 dello scenario principale

Post condizioni			Sistema mostra schermata con lista

<a name="sp2.5"></a>

### 2.5

Caso d’uso			Indire un esame per corso in cui insegna

Tipo				Primario

Precondizioni			Essere registrato nel sistema, avere almeno un corso

Scenario Principale		1 Docente scrive matricola corretta

				2 Docente scrive password corretta

				3 Docente seleziona la propria pagina Profilo

				4 Docente seleziona “Inserisci Nuova data esame”

				5 Sistema apre una schermata con la lista delle materie insegnate 

				6 Docente seleziona un corso

				7 Sistema apre un calendario con le possibili date selezionabili

				8 Docente seleziona una data

Scenario Alternativo		1 Docente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		1 Docente non ha nessuna docenza

				2 Sistema segnala la mancanza, ritorna al punto 3 dello scenario principale

Post condizioni			Sistema mostra schermata con lista 

<a name="sp2.6"></a>

### 2.6

Caso d’uso			Registrare un voto

Tipo				Primario

Precondizioni			Essere registrato nel sistema, avere almeno un corso

Scenario Principale		1 Docente scrive matricola corretta

				2 Docente scrive password corretta

				3 Docente seleziona la propria pagina Profilo

				4 Docente seleziona “Inserisci Voto esame”

				5 Sistema apre una schermata con la lista delle materie insegnate 

				6 Docente seleziona un corso

				7 Sistema apre una schermata con la lista degli studenti iscritti

				8 Docente seleziona uno studente

				9 Sistema apre un menù a tendina con un elenco di voti da 1 a 30

Scenario Alternativo		1 Docente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		1 Docente non ha nessuna docenza

				2 Sistema segnala la mancanza, ritorna al punto 3 dello scenario principale

Scenario Alternativo		1 Nessun studente ha ancora dato l’esame

				2 Sistema segnala la mancanza, ritorna al punto 6 dello scenario principale

Post condizioni			Sistema mostra schermata con lista

<a name="sp2.7"></a>

### 2.7

Caso d’uso			Visualizza lista iscritti ad un esame

Tipo				Primario

Precondizioni			Essere registrato nel sistema, avere almeno un corso

Scenario Principale		1 Docente scrive matricola corretta

				2 Docente scrive password corretta

				3 Docente seleziona la propria pagina Profilo

				4 Docente seleziona “Visualizza Lista esame”

				5 Sistema apre una schermata con la lista degli esami già fissati

				6 Docente seleziona un esame/data

				7 Sistema visualizza una schermata con gli studenti iscritti all’appello

Scenario Alternativo		1 Docente inserisce una combinazione matricola/password errata

				2 Sistema segnala l’errore, ritorna al punto 1 dello scenario principale

Scenario Alternativo		1 Docente non ha nessuna docenza

				2 Sistema segnala la mancanza, ritorna al punto 3 dello scenario principale

Post condizioni			SW mostra schermata con lista 

<a name="sp2.8"></a>

### 2.8

<a name="sp2.9"></a>

### 2.9

<a name="sp2.10"></a>

### 2.10

<a name="sp2.11"></a>

### 2.11

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

<a name="sp2.18"></a>

### 2.18

<a name="sp2.19"></a>

### 2.19
