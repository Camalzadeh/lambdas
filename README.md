# Lambdas and Functional Interfaces

A small book catalogue searched through a custom functional interface, so the filter
itself is the thing being passed around. Java Lessons, task 6.

## What it covers

- Writing a `@FunctionalInterface` (`Filter`) and implementing it with a lambda
  rather than a named class.
- Passing behaviour into a method - `Search` takes a filter and applies it to the
  catalogue, and knows nothing about what the filter tests.
- Filtering by genre, author and title, including combined conditions.

## Running it

```bash
javac -d out src/*.java
java -cp out Main
```

## Layout

- `src/Filter.java` - the functional interface.
- `src/Search.java` - applies a filter to the catalogue.
- `src/Book.java`, `src/Genres.java` - the model.
- `src/Main.java` - the lambdas being handed in.
