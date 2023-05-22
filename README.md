# Cursed C#

This is a repo containing a collection of personal snippets of "cursed" C# code, i.e. code that is intentionally confusing, obscure, counter-intuitive, comically impractical, and/or otherwise bizarre.

The main purpose of this code is to demonstrate quirks of C# syntax and semantics.

## Stuff

| File | Output | Description |
| --- | --- | --- |
| [ListPattern.csx](./src/ListPattern.csx) | `true` | Uses a [list pattern](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/patterns#list-patterns) to match an array of structs. |
| [Var.cs](./src/Var.cs) | Compiles | Uses three different naming scopes with the identifier `var`. |
| [Delegate.csx](./src/Delegate.csx) | Throws `NullReferenceException` | Confusingly named delegate invoked with a null instance of itself as an argument. |
| [StackOverflow.csx](./src/StackOverflow.csx) | Stack overflow | Abuses a recursive property in script mode. |

<!-- uwu -->
