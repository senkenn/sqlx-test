# sqlx-test

This is a copy of the [SQLx TODOs Example](https://github.com/launchbadge/sqlx/tree/main/examples/postgres/todos)

## Pre Setup

```bash
# Install sqlx-cli
cargo install sqlx-cli

# Run postgres
docker compose up -d
```

---

# TODOs Example

## Setup

1. Declare the database URL

   ```
   export DATABASE_URL="postgres://postgres:password@localhost:5432/todos"
   ```

2. Create the database.

   ```
   $ sqlx db create
   ```

3. Run sql migrations

   ```
   $ sqlx migrate run
   ```

## Usage

Add a todo

```
cargo run -- add "todo description"
```

Complete a todo.

```
cargo run -- done <todo id>
```

List all todos

```
cargo run
```
