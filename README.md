# tree-sitter-elixir

[![Test](https://github.com/elixir-lang/tree-sitter-elixir/actions/workflows/test.yml/badge.svg)](https://github.com/elixir-lang/tree-sitter-elixir/actions/workflows/test.yml)

Elixir grammar for [tree-sitter](https://github.com/tree-sitter/tree-sitter).

Modified to bail out of external scanner when in error recovery.

Snippet for trying it out in Emacs
```emacs-lisp
    (setq treesit-language-source-alist
      (append treesit-language-source-alist '((elixir . ("https://github.com/Jacob-Nielsen/tree-sitter-elixir.git" "bail-when-in-error-receovery")))))
    (treesit-install-language-grammar 'elixir)
```
Ready for production. Currently used by GitHub itself for source code highlighting and code navigation.

## Development

See [the docs](./docs/index.md) for more details.
