### Migrating global packages

`--reinstall-packages-from`

```sh
nvm install 'lts/*' --reinstall-packages-from=current
# or
nvm install node --reinstall-packages-from=node
```

<small>
This does not update the npm version.<br>
Use <code>`--latest-npm`</code> flag or
<code>`nvm install-latest-npm`</code>
</small>

```sh
nvm install 16 --reinstall-packages-from=16
# or use this command after migrating
nvm install-latest-npm
```

<small>
<a href="https://github.com/nvm-sh/nvm#migrating-global-packages-while-installing" target="_blank">
    github.com/nvm-sh/nvm#migrating-global-packages-while-installing
</a>
</small>

<aside class="notes">
</aside>
