### Controllo di versione locale

- alternativa a file e cartelle rinominati
- singolo repository locale
- archiviazione e consultazione modifiche effettuate
- operazioni di ripristino semplificate

Lati negativi

- utente singolo
- dati in una sola postazione
- strumenti limitati per lo sviluppo collaborativo

<aside class="notes">
Molte persone gestiscono le diverse versioni copiando i file in un’altra directory (magari una directory denominata con la data).
Questo approccio è molto comune perché è molto semplice, ma è anche incredibilmente soggetto ad errori.
É facile dimenticare in quale directory sei e modificare il file sbagliato o copiare dei file che non intendevi copiare.

Il controllo di versione locale è la forma più essenziale e primitiva di versioning; si immagini uno sviluppatore che crea un'applicazione, effettua la presentazione o la messa in produzione di quest'ultima e poi, magari su suggerimento del committente, effettua delle modifiche introducendo aggiornamenti e correzioni. In questo caso le diverse versioni del progetto potrebbero essere salvate in differenti cartelle rinominate, ad esempio associando la data dell'ultima modifica effettuata al nome del progetto.

Almeno in teoria tale approccio non necessita di un software per la gestione delle diverse release, ma cosa potrebbe accadere nel caso di progetti articolati coinvolti da numerose modifiche? Tenere traccia degli interventi effettuati diventerebbe complesso con il rischio di perdere molte informazioni con il passare del tempo e l'accumularsi degli interventi eseguiti.

Le soluzioni per il versiong funzionano grazie ad un database destinato a registrare le modifiche apportate ai file e tramite delle patch che memorizzano le differenze tra le revisioni in modo da semplificare le operazioni di ripristino.

Il controllo di versione locale offre strumenti limitati per lo sviluppo in ambito collaborativo.
</aside>
