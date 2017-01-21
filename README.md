# .NET scripting "dialects"

[![Gitter chat](https://badges.gitter.im/dotnet-scripting/general.png)](https://gitter.im/dotnet-scripting/general)

A draft proposal for .NET scripting "dialects".

A scripting "dialect" defines the following expectations by a given script:

- **Preprocessor directives:** E.g. `#r` and `#load`. For each directive:
  - Name
  - Syntax
  - Behaviour
- **Globals type:** The type which defines the global members available to the script. E.g. [`InteractiveScriptGlobals`](https://github.com/dotnet/roslyn/blob/b1fc93e4b6873e7a3e53f5e4a524941906a1ba0d/src/Scripting/Core/Hosting/InteractiveScriptGlobals.cs)
- **Implicit assembly references:** E.g. an implicit reference to `System.dll`.
- **Implicit namespace imports:** E.g. implicit C# `using` statements.
