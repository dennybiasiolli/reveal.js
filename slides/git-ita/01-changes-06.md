### `git commit`

Crea una revisione con il contenuto dello staging

```sh
git commit [-a] -m "messaggio di commit"
```

`-a` permette di committare tutti i file modificati, ignorando l'area di staging

_Esercizio_
```md
- Lancia `git status`, dovresti avere `CONTRIBUTING.md`
  sia in staging che fuori dallo staging.
  In caso contrario fai delle modifiche nel file
- Esegui `git commit -m "Il mio primo commit"`
- Lancia nuovamente `git status`, cosa cambia?
- Prova ora `git commit -a -m "Modificato CONTRIBUTING.md"`
- Lancia nuovamente `git status`, cosa vedi ora?
```


<aside class="notes">
</aside>
