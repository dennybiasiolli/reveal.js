#### ⏱ Performances

<small>

| | Creating test DB | Running tests |
|-|-|-|
| Before | ~20s | ~1s |
| `MIGRATE = False` | ~25s 😑 | ~1s |
| `--keepdb` (local) | ~0s 🥳 | ~1s |
| Seed DB + `--keepdb` (GitHub actions) | ~2s 🥳 | ~1s |

</small>


<aside class="notes">
</aside>
