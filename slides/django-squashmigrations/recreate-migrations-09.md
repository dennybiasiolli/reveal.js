#### 🤯 Recreate migrations

9. back to post-squash tasks

<small>

- commit and release
- upgrade all systems with the new release
- remove old migration files, commit and do a second release
- update all migrations that depend on the deleted migrations
- remove the `replaces` attribute
- (optional) prune references to deleted migrations

</small>


<aside class="notes">
</aside>
