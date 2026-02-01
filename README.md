# accessing-a-relational-database

Introduces the basics of accessing a database using the Go standard library.

## Overview

This project demonstrates how to connect to and interact with relational databases using Go's standard library, covering:

- Database connection setup (MySQL, PostgreSQL, SQLite)
- Basic CRUD operations (Create, Read, Update, Delete)
- Prepared statements for security
- Transaction handling
- Error handling

## Quick Start

```bash
# Clone the repository
git clone https://github.com/GallifreyGoTutoural/accessing-a-relational-database.git
cd accessing-a-relational-database

# Run the example
go run main.go
```

## Database Configuration

Edit the database connection string in `main.go`:

```go
dsn := "user:password@tcp(localhost:3306)/database?parseTime=true"
```

### Supported Databases

- MySQL
- PostgreSQL
- SQLite

## Example Operations

| Operation | Method | Description |
|-----------|--------|-------------|
| Create | `InsertUser()` | Add new records |
| Read | `GetUser()` | Query single record |
| Read | `ListUsers()` | Query multiple records |
| Update | `UpdateUser()` | Update existing records |
| Delete | `DeleteUser()` | Remove records |

## Project Structure

```
accessing-a-relational-database/
├── main.go           # Entry point
├── db/               # Database operations
├── models/           # Data models
└── README.md
```

## Dependencies

- Go 1.19+
- Database driver (mysql, postgres, or sqlite3)

## License

MIT
