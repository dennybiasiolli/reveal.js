#### SPOILER ALERT

```json
"vue": "^2.6.14"
```

means `2.x`

Starting from July 1, 2022<br>
it auto-updates to Vue 2.7<br>
<small>
if you don't use explicit `package-lock.json` or `yarn.lock` files
</small>

```diff
- "vue": "^2.6.14"
+ "vue": "~2.6.14"
```

to accept only patch releases 


<aside class="notes">
"~" is "tilde"
</aside>
