# Solid Cache

* Rails 8.0で新規にアプリケーションを作成した場合、デフォルトでSolid Cacheが使われるようになっている
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
