# Cursed C#

This is a repo containing small samples of "cursed" C# code, i.e. code that is intentionally confusing, obscure, counter-intuitive, comically impractical, and/or otherwise bizarre.

The main purpose of this code is to demonstrate quirks of C# syntax and semantics.

## A note on execution

There are two ways to run C#: regular and script mode. Regular mode is what is enabled when running a C# project using `dotnet run` from the command-line, and script mode is what REPLs like [CSharpRepl](https://github.com/waf/CSharpRepl) and [MODiX](https://github.com/discord-csharp/MODiX) or interactive environments such as [.NET Interactive](https://github.com/dotnet/interactive) run using. There are couple differences in script mode as compared to regular mode, most notably for the purposes of cursed code:

- A `Main` method is not required.
- Simlarly to top-level statements, scripts can contain both top-level type declarations and statements.
- Unlike top-level statements, type declarations can precede statements.
- The last expression of a script is treated as the result of the script.

Files in this repo are distinguished between regular and script mode by their file extensions. `.cs` files are regular files which will compile using `dotnet build`, while `.csx` files are scripts which can run inside interactive environments.

## Language versions

Code in this repo mainly uses the latest preview/development language version. [Sharplab](https://sharplab.io) is a fantastic resource for exploring language features currently in development.

## Other fun quirks

Some quirks which are good to know for the purposes of reading code in this repo:

- `var` is a valid identifier, and if a type called `var` is declared then it effectively overrides the `var` keyword.
    - This is also the case with other [contextual keywords](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/#contextual-keywords) such as `async`.
- `_` is a valid identifier despite also acting as a wildcard and discard depending on context.
- `@` can be used to eliminate whitespace before and after identifiers.
