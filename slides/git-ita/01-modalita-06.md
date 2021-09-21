### Distribuito

- repository su server e "cloni" locali
- ogni "clone" contiene l'intero repository
- funzionamento anche senza collegamento al server
- strumenti per sincronizzazione con il server
- collaborazione con metodologie avanzate

<aside class="notes">
Qui entrano in gioco i Sistemi di Controllo di Versione Distribuiti.
I client non solo controllano lo snapshot più recente dei file, ma piuttosto fanno una copia identica dell’archivio (repository),
completa di tutta la propria storia.
In questo modo se un server smettesse di funzionare e se i sistemi interagissero tramite questo server,
il repository di un qualsiasi client potrebbe essere copiato sul server per ripristinarlo.
Ogni clone è proprio un backup completo di tutti i dati.

Inoltre, molti di questi sistemi trattano bene l’avere più repository remoti su cui poter lavorare,
così puoi collaborare con gruppi differenti di persone in modi differenti, simultaneamente sullo stesso progetto.
Questo ti permette di impostare diversi tipi di flussi di lavoro che non sono possibili in sistemi centralizzati,
come i modelli gerarchici.
</aside>
