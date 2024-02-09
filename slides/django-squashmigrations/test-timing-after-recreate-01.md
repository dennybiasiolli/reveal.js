#### Test performances after recreating

```text
$ time manage.py test

Ran 152 tests in 0.988s
python manage.py test  5.12s user 0.21s system 82% cpu 6.485 total
```

<small>

| | Creating test DB | Running tests |
|-|-|-|
| Before | ~20s | ~1s |
| `MIGRATE = False` | ~25s 😑 | ~1s |
| `--keepdb` (local) | ~0s 🥳 | ~1s |
| Seed DB + `--keepdb` (GitHub actions) | ~2s 🥳 | ~1s |
| After squashing | ~19s 😑 | ~1s |
| After recreating | ~5s 🥳 | ~1s |

</small>


<aside class="notes">
</aside>
