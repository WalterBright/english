# Imports and modules

To write a simple hello world program in D you need
`import`s. The `import` statement makes all public functions
and types from the given **module** available.

The standard library, called [Phobos](https://dlang.org/phobos/),
is located under the **package** `std`
and those modules are referenced through `import std.MODULE`.

The `import` statement can also be used to selectively
import certain symbols of a module:

    import std.stdio: writeln, writefln;

Selective imports can be used to improve the readability by making
it obvious where a symbol comes from and also as a way to
prevent clashing of symbols with the same name from different modules.

An `import` statement does not need to appear at the top a source file.
It can also be used locally within functions or any other scope.

## {SourceCode}

```d
void main()
{
    import std.stdio;
    // or import std.stdio: writeln;
    writeln("Hello World!");
}
```
