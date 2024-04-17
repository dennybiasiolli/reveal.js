#### Databases

Configure at least a URL for the database under databases.$name (in Rocket.toml), where $name is your choice of database name:

```toml
[default.databases.custom_name]
url = "database.sqlite"
# url = "postgresql://[user[:password]@][host][:port][/dbname][?param1=value1&...]"
```


<aside class="notes">
</aside>
