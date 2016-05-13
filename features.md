# Funzionamento logico del software


Questo software gestisce una lista di cose da fare. Segue una descrizione dei 
vari componenti logici e funzioni.


## Obbiettivi

L'oggetto principale. Il software di base è una lista di obbiettivi, senza 
nient'altro.


## Categorie

Quando leggo la lista delle cose da fare, lo faccio perché mi chiedo:
 
 - Sono in questa situazione, cosa dovevo fare?
 - Ho voglia di fare questo, cosa avevo da fare a riguardo?
 
Per es:

 - Sono al supermercato, cosa dovevo comprare?
 - Ho voglia di programmare, quali programmi volevo scrivere?
 

Gli obbiettivi quindi secondo me dovrebero essere raggruppati per situazioni e 
interessi.

Una situazione può essere "sono in questo posto", oppure "sono con questa persona",
o ancora "sto facendo questa cosa". Le situazioni potrebbero essere anche (in parte) 
rilevate automaticamente, quindi ci potrebbe essere un menù simile a questo:

`
Cosa dovrei fare?
> Adesso (situazione autorilevata)  
> Vicino a te (situazioni autorilevate)  
> Quando? (specifica manualmente)  
---> (sottomenù con varie situazioni)  
`

Gli interessi sono invece tipo "programmazione", "film", "libri" ecc. Quando si ha
voglia di fare qualcosa, basta selezionare l'interesse corrispondente per vedere 
cosa si potrebbe fare.


## Priorità

Questo sistema di raggruppamento da solo non è sufficiente: ho un po' di tempo per 
programmare, con cosa inizio? Con qualcosa a caso?  No, inizio risolvendo i bug 
gravissimi nel software x, poi posso implementare nuove funzioni nel software y.

Le cose da fare oltre che raggruppate devono anche essere ordinate per importanza. 
Ci sono le cose da fare il prima possibile, le cose importanti, le cose da 
fare quando si ha tempo e le cose da fare prima o poi.

