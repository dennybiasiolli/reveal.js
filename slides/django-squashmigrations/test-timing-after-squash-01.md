#### Test performances after squashing

```text
$ time manage.py test

Ran 152 tests in 0.948s
20.47s user 0.35s system 99% cpu 21.001 total
```

<small>

| | Creating test DB | Running tests |
|-|-|-|
| Before | ~20s | ~0.9s |
| After squashing | ~20s 😑 | ~0.9s |

</small>


<aside class="notes">
</aside>
