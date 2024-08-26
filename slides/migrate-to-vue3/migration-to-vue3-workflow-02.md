2. update vue in `package.json`

```diff
"dependencies": {
-  "vue": "~2.7",
+  "vue": "^3.4.38",
+  "@vue/compat": "^3.4.38"
   ...
},
"devDependencies": {
-  "vue-template-compiler": "~2.7"
}
```

```bash
npm i -S vue@^3.4 @vue/compat@^3.4 --force
npm uninstall vue-template-compiler --force
```


<aside class="notes">
</aside>
