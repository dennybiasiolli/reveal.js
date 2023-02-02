#### Test performances after squashing

```text
$ time manage.py test

Ran 152 tests in 0.948s
20.47s user 0.35s system 99% cpu 21.001 total
```

<small>

| Command | Execution time (before) | Execution time (after) |
|-|-|-|
| Creating test database | ~20s | ~20s |
| Running tests | ~0.9s | ~0.9s |

</small>


<aside class="notes">
</aside>
