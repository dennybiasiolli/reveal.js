#### 🗄️ Provide initial data for tables

Export existing data to JSON fixtures

```sh
manage.py dumpdata my_app.feature > my_app/fixtures/feature.json
```

```json
// my_app/fixtures/feature.json
[
  {
    "model": "my_app.feature",
    "pk": 1,
    "fields": {
      "name": "Feature 1",
      "description": "First feature"
    }
  }
]
```


<aside class="notes">
</aside>
