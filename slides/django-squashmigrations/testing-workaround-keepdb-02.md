`--keepdb` pros and cons

- 🎉 Saves ~20s for each test run after the first one

- 😥 Not easy to configure in CI/CD

    - cache/artifacts in GitHub workflows
    - external test DB
    - <a href="https://github.com/businho/django-migrations-ci">django-migrations-ci</a>
        (thanks <a href="https://twitter.com/rmistaken">@rmistaken</a>)


<aside class="notes">
</aside>
