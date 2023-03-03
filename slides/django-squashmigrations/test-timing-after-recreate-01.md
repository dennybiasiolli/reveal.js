#### Test performances after recreating

```text
$ time manage.py test

Ran 152 tests in 0.988s
python manage.py test  5.12s user 0.21s system 82% cpu 6.485 total
```

<small>

| | Creating test DB | Running tests |
|-|-|-|
| Before | ~20s | ~0.9s |
| ~~After squashing~~ | ~20s 😑 | ~0.9s |
| After recreating | ~5s 🥳 | ~0.9s |

</small>


<aside class="notes">
</aside>
