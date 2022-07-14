#### management commands

##### deleterevisions

<small>

With no arguments, this command will delete your entire revision history!

</small>

```sh
manage.py deleterevisions

# keep any changes from last 30 days
manage.py deleterevisions your_app.YourModel --days=30

# keep 30 most recent changes for each item
manage.py deleterevisions your_app.YourModel --keep=30

# Keep last 30 days and at least 3 from older changes
manage.py deleterevisions your_app.YourModel \
    --keep=3 --days=30
```

<aside class="notes">
</aside>
