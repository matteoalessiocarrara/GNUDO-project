# Architettura di GNUDO

## Componenti


### Database

Dove sono conservati fisicamente i dati. Sarebbe meglio se non fosse un formato 
binario, perché così l'utente pùo accedervi (male) anche in assenza di programmi
particolari


### DBMS

Il dbms permette di lavorare sui dati senza conoscere la struttura fisica del db.


### GNUDO-backend

Si occupa di gestire il dbms/db, in modo che i front-end possano lavorare sui 
dati senza sapere niente di come sono salvati. Ci sono vari vantaggi:

 * Si evitano problemi di incoerenza, visto che un solo componente lavora sul db
 * Si semplifica la scrittura dei front-end, che non devono conoscere ne SQL ne 
   altro
 * Si rende possibile il cambiamento del db senza che debba essere riscritto il 
   front-end, visto che l'interfaccia di GNUDO-backend rimane uguale.


### GNUDO-fronted

Un front-end è l'interfaccia utente per la libreria GNUDO-backend. Può 
essere da terminale, con ncurses, in qt, in gtk ecc.


## Rappresentazione grafica dell'architettura


```
db(json)	<---> dbms <---> |               | <---> GNUDO-frontend-1  
db(sqlite)	<---> dbms <---> | GNUDO-backend | <---> GNUDO-frontend-2  
db(mysql)	<---> dbms <---> |               | <---> GNUDO-frontend-3  
...
```
