# database.yml for Solid Cache

* database.ymlはこんな感じ

```yml
# database.yml
production:
  primary:
    <<: *default
    database: storage/production.sqlite3
  cache:
    <<: *default
    database: storage/production_cache.sqlite3
    migrations_paths: db/cache_migrate
```
