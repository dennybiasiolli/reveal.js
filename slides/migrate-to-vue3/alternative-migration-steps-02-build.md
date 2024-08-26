#### Step 2 - Build mode

```json
"scripts": {
    "build": "run-p type-check \"build-only {@}\" --",
    "build-only": "vite build",
```

```sh
npm run build -- -- --mode your_env
npm run build-only -- --mode your_env
# will use env variables stored in .env.your_env
```


<aside class="notes">
</aside>
