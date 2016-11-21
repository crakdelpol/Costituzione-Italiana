# Costituzione Italiana

Esercizio di versionamento della costituzione italiana, basato 
sul fantastico lavoro di rappresentazione delle diverse versioni del 
testo costituzionale in formato `Markdown` 
realizzato da [Lorenzo Breda](https://github.com/LBreda/costituzione)
con l'integrazione versione della proposta costituzionale creata da
[Stefano Zacchiroli](http://zacchiro.github.io/costituzione/diff/2012-04-20/2016-01-20).

A differenza del lavoro originale, in questo repositorio si sono usati
i nomi dei Presidenti del Consiglio in carica negli anni delle riforme.

Ove possibile (a partire dal 1970), si sono alterate pure le date
di `commit` delle modifiche per farle corrispondere a quelle reali.

# Motivi

[Git](https://it.wikipedia.org/wiki/Git_(software)) è un potente strumento informatico ideato per gestire le versioni dei codici
sorgenti di software. 

Nella pratica può essere utilizzato per gestire le versioni di qualsiasi
file in formato di [testo puro](https://it.wikipedia.org/wiki/Testo_puro),
come il formato [Markdown](https://it.wikipedia.org/wiki/Markdown) 
usato in questo caso.

L'idea è di introdurre l'uso di Git per gestire le modifiche alla 
costituzione italiana, facilitando sia la consulta storica e statistica,
ma anche la valutazione di proposte di riforma.

Un esempio di uso è quello di visualizzare la differenza tra
la costituzione attuale e una nuova proposta del 2016:
 

# Tecniche

## Commit

Per alterare la data e l'autore di ogni commit, 
si è usato un comando come il seguente:

```
GIT_AUTHOR_DATE='2012-04-20T00:00:00' \
GIT_COMMITTER_DATE='2012-04-20T00:00:00' \
git commit -a --author="Mario Monti <MarioMonti@derecho.it>"
L. cost. 20 aprile 2012, n. 1

Introduzione del principio del pareggio di bilancio nella Carta costituzionale

http://www.gazzettaufficiale.it/gunewsletter/dettaglio.jsp?service=1&datagu=2012-04-23&task=dettaglio&numgu=95&redaz=012G0064&tmstp=1335261341150
https://it.wikipedia.org/wiki/Mario_Monti
```


## Autori

Come autori vengono indicati i presidenti del consiglio in carica.

Git, per l'operazione di `commit`, richiede l'associazione 
di un indirizzo email al nome dell'autore. 
Questi indirizzi email associati sono fittizzi per tutti gli ex-presidenti,
mentre nel caso del presidente attuale si è usato l'indirizzo ufficiale.


# Fonti

Questo esercizio è stato realizzato nel giro di un paio d'ore, 
appoggiandomi al grande lavoro di rappresentazione del testo costituzionale
in formato [Markdown](https://it.wikipedia.org/wiki/Markdown), 
fatto da [Lorenzo Breda](https://github.com/LBreda/costituzione).

Per l'integrazione della nuova proposta di legge costituzionale,
la sorgente è stato il lavoro di [Stefano Zacchiroli](http://zacchiro.github.io/costituzione/diff/2012-04-20/2016-01-20).

L'associazione con i presidenti del consiglio in carica è stata fatta
basandomi sui dati presenti ai seguenti link:

 * https://it.wikipedia.org/wiki/Costituzione_della_Repubblica_Italiana#Cronologia_delle_leggi_costituzionali
 * https://it.wikipedia.org/wiki/Presidenti_del_Consiglio_dei_ministri_della_Repubblica_Italiana
 * http://www.gazzettaufficiale.it/
