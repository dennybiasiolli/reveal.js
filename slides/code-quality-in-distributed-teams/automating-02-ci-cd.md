#### CI/CD Pipelines

Implement CI tools to automate tests, linting, and formatting checks before code is merged.

- Jenkins, CircleCI, GitHub Actions


```yaml
# .github/workflows/ci.yml
on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]
```

<aside class="notes">
</aside>
