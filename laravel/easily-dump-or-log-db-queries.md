# Easily dump or log DB queries

In order to dump SQL queries that will be executed during the request we can add `DB::listen(fn ($e) => dump($e->sql, $e->bindings));` to a controller and all of the queries and their bindings will be printed.

In a future Laravel version `DB::listen(fn ($e) => dump($e->toRawSql()));` could be used to get a query with bindings already in.

## Logging the queries

Instead of dumping the queries to the screen, we can log them with `DB::listen(fn ($e) => Log::debug($e->sql, $e->bindings));`.