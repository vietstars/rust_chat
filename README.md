# Rust React Chat App

# Make migration file
```cmd
diesel migration generate create_users
```

down.sql
up.sql

```sql
CREATE TABLE users (
  id TEXT PRIMARY KEY NOT NULL,
  username VARCHAR NOT NULL,
  phone VARCHAR NOT NULL,
  created_at TEXT NOT NULL,
  unique(phone)
)
```

# Make dump data
```cmd
diesel migration generate dummy_data
```

# Build migration
```cmd
diesel database setup
```

# Run migration - dump data
```cmd
diesel migration run
```

cargo b

cargo r

https://dev.to/roxie/how-to-add-google-s-two-factor-authentication-to-a-laravel-8-application-4jjp

cargo add actix actix-files actix-web actix-web-actors actix-cors

cargo add rand uuid chrono

cargo install diesel_cli --no-default-features --features sqlite

# postgress
https://blog.ediri.io/building-a-restful-api-with-actix-web-and-diesel-for-persistent-data-storage

# JWT
https://codevoweb.com/rust-actix-web-jwt-access-and-refresh-tokens

# RPC
https://github.com/dirien/rust-grpc
