# julia-lsp

Julia language server plugin for [Claude Code](https://claude.ai/code), powered by [LanguageServer.jl](https://github.com/julia-vscode/LanguageServer.jl).

Gives Claude Code real-time code intelligence for Julia projects: diagnostics, go-to-definition, find references, hover info, and more.

## Prerequisites

Install [LanguageServer.jl](https://github.com/julia-vscode/LanguageServer.jl) in your Julia environment. It's recommended to install this in your global Julia environment (e.g. `@v1.12`).

```julia
using Pkg; Pkg.add("LanguageServer")
```

## Usage

```bash
claude --plugin-dir /path/to/this/repo
```

The first LSP request in a session may take 30-60 seconds while Julia JIT-compiles LanguageServer.jl. Subsequent requests are fast.

## Configuration

The plugin is configured in `.claude-plugin/plugin.json`. The `startupTimeout` is set to 120 seconds to accommodate Julia's JIT compilation. You can adjust this if needed.

## License

MIT
