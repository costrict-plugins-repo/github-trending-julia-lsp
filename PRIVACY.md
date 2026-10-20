# Privacy Policy

`julia-lsp` is a Claude Code plugin that configures a local Julia language server (LanguageServer.jl) for code intelligence.

## Data Collection

This plugin does **not** collect, store, or transmit any user data. It runs entirely on your local machine.

## How It Works

The plugin starts a local instance of LanguageServer.jl that communicates with Claude Code over stdio. All code analysis happens locally on your machine. No data is sent to any external server by this plugin.

## Third-Party Services

This plugin relies on:

- **LanguageServer.jl** — runs locally; see its [repository](https://github.com/julia-vscode/LanguageServer.jl) for details
- **SymbolServer.jl** — a dependency of LanguageServer.jl that may download package symbol caches from GitHub on first run

## Contact

For questions, open an issue at https://github.com/alecloudenback/ClaudeCodeJuliaLSP/issues
