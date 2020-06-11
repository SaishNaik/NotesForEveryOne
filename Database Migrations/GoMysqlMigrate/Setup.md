# Golang Mysql migration using golang-migrate for MySQL

[golang-migrate](https://github.com/golang-migrate/migrate) allows you to run migrations either through cli or through code.

## CLI Commands

Create Migration

```
migrate create -ext sql -dir migrations/mysql -seq initializeDB
```

Force Migration
``` 
  migrate -database "mysql://root:root@tcp(localhost)/db_name" -path yourMigrationScriptPath force V
``` 
where V is the version you want to force it to.

## Migration through code

```
migrate.New("file://migrations/mysql", "mysql://root:root@tcp(localhost)/db_name")
```
Where ```migrations/mysql``` is the location of your migration scripts and ```mysql://root:root@tcp(localhost)/db_name``` is
the database url needed for [ go-sql-driver/mysql](https://github.com/go-sql-driver/mysql).


