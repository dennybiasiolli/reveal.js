#### Don't panic!

1. Commit o stash del lavoro in corso su `develop`
2. Spostati su `master` e crea un branch di `hotfix` temporaneo
3. Fai modifiche e commit necessari
4. Spostati su `master` e fai merge del branch `hotfix`
5. Rilascia le modifiche
6. Torna su `develop` e fai merge del branch `master`,
  per incorporare le modifiche in produzione anche su master,
  che era andato avanti separatamente

<aside class="notes">
</aside>
