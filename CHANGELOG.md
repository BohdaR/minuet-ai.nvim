# Version 0.5.2 (2025-05-11)

## Features

- lsp: add option `adjust_indentation` for completion items.
- lualine: display provider and model name.
- chat input template can be a list of strings.

## Fixes

- Cursor Position: Put cursor at correct position when accepting single-line
  virtual text completion.

# Version 0.5.1 (2025-04-08)

## Features

- Added `transform` option for OpenAI-FIM-compatible providers.

  This feature enables support for non-OpenAI-FIM-compatible APIs with
  OpenAI-FIM-compatible provider, such as the DeepInfra FIM API. Example
  configurations are available in [recipes.md](./recipes.md).

# Version 0.5.0 (2025-03-28)

## Breaking Changes

- Modified the Gemini provider's default prompt strategy to use the new
  **Prefix First** structure.
- Other providers will continue to use their previous default prompt
  configurations.

## Features

- lsp: always `prepend_to_complete_word` without checking `TriggerCharacter`
- Add a new "Prefix-First" prompt structure for chat LLMs.

# Version 0.4.2 (2025-03-21)

## Breaking Change

- change multi-lines indicators to unicode character `⏎`.

## Features

- **lsp**: change multi lines indicators to unicode character `⏎`.
- Lualine integration: add spinner component.
- **lsp**: add detail field to show provider name.
- **Minuet Event**: add three user events during its request workflow.

## Fixes

- **lsp**: handle request where params.context is not provided (for mini.completion).

# Version 0.4.1 (2025-03-19)

## Breaking Change

- **lsp**: Don't explicitly disable auto trigger for filetypes not in `enabled_auto_trigger_ft`.

## Fixes

- **lsp**: Fix cursor column position when trying to get current line content.
- **lsp**: Early return on throttle.

# Version 0.4.0 (2025-03-18)

## Features

- Introduced in-process LSP support for built-in completion.
- For `blink-cmp`, the completion item's `kind_name` now reflects the LLM provider name.
- Improve error handling for both stream and non-stream JSON decoding, providing more informative messages.

# Version 0.3.3 (2025-02-18)

## Documentation

- Added recipes for llama.cpp
- Added recipes for integration with VectorCode

# Version 0.3.2 (2025-02-10)

- Add luarocks release

# Version 0.3.1 (2025-02-10)

## Features

- `Minuet change_model` now supports `vim.ui.select`

# Version 0.3 (2025-02-09)

## Breaking Changes

- Remove Hugging Face provider
- Remove deprecated commands (`MinuetToggle*`, `MinuetChange*`)

## Features

- Add option to show suggestion when completion menu is visible
- Support api_key as a function

# Version 0.2 (2025-02-05)

## Breaking Changes

- Update default gemini model to gemini-2.0-flash

## Features

- Add command `Minuet change_preset`
- Add option to show suggestion when completion menu is visible

## Documentation

- Add RAG experimental feature doc with vectorcode

# Version 0.1 (2025-02-02)

- Initial release
