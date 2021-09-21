### Centralizzato

- partecipazione di più utenti
- singolo repository su server
- configurazione privilegi di accesso differenti

Lati negativi

- storico modifiche in una sola postazione
- malfunzionamento di server / rete = utenti bloccati
- difficoltà di backup / ripristino

<aside class="notes">
Per far fronte a questo problema, vennero sviluppati sistemi di controllo di versione centralizzati.
Questi sistemi hanno un unico server che contiene tutte le versioni dei file e un numero di utenti che scaricano i file dal server centrale.
Questo è stato lo standard del controllo di versione per molti anni.

Questa impostazione offre molti vantaggi, specialmente rispetto ai VCS locali.
Per esempio, chiunque sa, con una certa approssimazione, cosa stia facendo un’altra persona del progetto.
Gli amministratori hanno un controllo preciso su chi può fare cosa, ed è molto più facile amministrare un CVCS che un database locale su ogni client.

Questa configurazione ha tuttavia alcune gravi controindicazioni.
La più ovvia è che il server centralizzato rappresenta il singolo punto di rottura del sistema.
Se questo va giù per un’ora, in quel periodo nessuno può collaborare o salvare una nuova versione di qualsiasi cosa su cui sta lavorando.
Se il disco rigido del database centrale si danneggia, e non ci sono i backup, perdi assolutamente tutto — tutta la storia del progetto ad eccezione dei singoli snapshot (istantanee) che le persone possono avere in locale sulle loro macchine.
Anche i sistemi locali di VCS soffrono di questo problema — ogni volta che tutta la storia del progetto è in un unico posto, si rischia di perdere tutto.
</aside>
