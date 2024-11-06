# Solid Cache features

* デフォルトで生成される設定ファイルは下記の通り

```yml
default: &default
  store_options:
    # Cap age of oldest cache entry to fulfill retention policies
    # max_age: <%= 60.days.to_i %>
    max_size: <%= 256.megabytes %>
    namespace: <%= Rails.env %>

development:
  <<: *default

test:
  <<: *default

production:
  database: cache
  <<: *default
```

* その他オプション等については[README](https://github.com/rails/solid_cache/blob/main/README.md)参照