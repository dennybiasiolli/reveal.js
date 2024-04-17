#### Databases

Rocket includes built-in, ORM-agnostic support for databases via rocket_db_pools.

The library simplifies accessing one or more databases via connection pools: data structures that maintain active database connections for use in the application.

```bash
cargo add rocket_db_pools --features "sqlx_sqlite"
# or
cargo add rocket_db_pools --features "sqlx_postgres"
# or
cargo add rocket_db_pools --features "diesel_postgres"
```

<small>

https://api.rocket.rs/v0.5/rocket_db_pools/#supported-drivers

</small>


<aside class="notes">
</aside>
