# My NeoVim Configuration

This repository contains my Neovim configuration files, organized for ease of use and modularity. The setup leverages Lua for configuring Neovim and includes a variety of plugins managed by LazyVim.

## Table of Contents

- [Installation](#installation)
- [File Structure](#file-structure)
- [Core Configuration](#core-configuration)
- [Plugins](#plugins)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. **Clone the repository:**

   ```sh
   git clone https://github.com/robbylew/nvim-config.git ~/.config/nvim
   ```

2. **Install dependencies:**
   - Ensure you have Neovim (>= 0.5.0) installed.
   - Install [lazy.nvim](https://github.com/folke/lazy.nvim) for plugin management.

3. **Start Neovim and install plugins:**

   ```sh
   nvim
   ```

   Inside Neovim, run:

   ```vim
   :Lazy sync
   ```

## File Structure

```sh
nvim
├── init.lua
├── lazy-lock.json
└── lua
    └── robbylew
        ├── core
        │   ├── init.lua
        │   ├── keymaps.lua
        │   └── options.lua
        ├── lazy.lua
        └── plugins
            ├── alpha.lua
            ├── auto-session.lua
            ├── autopairs.lua
            ├── bufferline.lua
            ├── colorscheme.lua
            ├── comment.lua
            ├── dressing.lua
            ├── formatting.lua
            ├── gitsigns.lua
            ├── indent-blankline.lua
            ├── init.lua
            ├── lazygit.lua
            ├── linting.lua
            ├── lsp
            │   ├── lspconfig.lua
            │   └── mason.lua
            ├── lualine.lua
            ├── nvim-cmp.lua
            ├── nvim-tree.lua
            ├── nvim-treesitter-text-objects.lua
            ├── substitute.lua
            ├── surround.lua
            ├── telescope.lua
            ├── todo-comments.lua
            ├── treesitter.lua
            ├── trouble.lua
            ├── vim-maximizer.lua
            └── which-key.lua
```

## Core Configuration

- **`init.lua`**: Main entry point for Neovim configuration.
- **`keymaps.lua`**: Contains custom key mappings.
- **`options.lua`**: Sets various Neovim options.

## Plugins

The plugin configurations are modularized within the `plugins` directory. Below is a brief overview of each plugin and its purpose:

- **`alpha.lua`**: Configures the Alpha startup screen, providing a customizable dashboard.
- **`auto-session.lua`**: Manages sessions automatically, saving and restoring your workspaces.
- **`autopairs.lua`**: Provides automatic closing of pairs like brackets, quotes, etc.
- **`bufferline.lua`**: Enhances the buffer line, offering better navigation between buffers.
- **`colorscheme.lua`**: Sets the colorscheme for a visually appealing interface.
- **`comment.lua`**: Adds easy commenting functionality with keyboard shortcuts.
- **`dressing.lua`**: Enhances default UI elements for a better user experience.
- **`formatting.lua`**: Configures code formatting to maintain consistent style.
- **`gitsigns.lua`**: Integrates Git with buffer, showing changes and providing Git commands.
- **`indent-blankline.lua`**: Adds indentation guides to improve code readability.
- **`lazygit.lua`**: Integration with LazyGit for a powerful Git UI within Neovim.
- **`linting.lua`**: Configures linting to catch errors and enforce coding standards.
- **`lspconfig.lua`**: Sets up Neovim's built-in LSP (Language Server Protocol) for language-specific features.
- **`mason.lua`**: Manages LSP servers, DAP servers, linters, and formatters.
- **`lualine.lua`**: Configures the status line for a more informative and stylish look.
- **`nvim-cmp.lua`**: Provides autocompletion setup for faster coding.
- **`nvim-tree.lua`**: File explorer for easy navigation of the file system.
- **`nvim-treesitter-text-objects.lua`**: Treesitter-based text objects for better code manipulation.
- **`substitute.lua`**: Enhanced substitute functionality.
- **`surround.lua`**: Surround functionality for quick text editing.
- **`telescope.lua`**: Fuzzy finder for searching files, buffers, and more.
- **`todo-comments.lua`**: Highlight and search TODO comments in your code.
- **`treesitter.lua`**: Treesitter configuration for better syntax highlighting and code navigation.
- **`trouble.lua`**: Diagnostics list for better error tracking.
- **`vim-maximizer.lua`**: Maximizes and restores the current window for focused coding.
- **`which-key.lua`**: Displays possible key bindings in a popup for easier discovery.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.


---

Feel free to customize this configuration to suit your needs. Happy coding!
