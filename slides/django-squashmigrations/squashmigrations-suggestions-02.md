#### 👉 Recommended process

4. transition the squashed migration to a normal migration:

- delete all the migration files it replaces

- update all migrations that depend on the deleted migrations to depend on the squashed migration instead

- remove the `replaces` attribute in the squashed migration


<aside class="notes">
</aside>
