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
