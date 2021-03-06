# My vim setup

Simple neovim setup with colors and lsp.

<img width="1200px" alt="My workflow photos" src="images/img1.png">

- [My vim setup](#my-vim-setup)
- [Requirements](#requirements)
- [Installation](#installation)
- [Installing the plugin manager](#installing-the-plugin-manager)
- [Usage](#Usage)
  - [Keybindings](#keybindings)
  - [Color Scheme](#colorscheme)
- [Plugins](#plugins)
  - [nvim-lspconfig](#nvim-lspconfig)
  - [nvim-lsp-installer](#nvim-lsp-installer)
  - [lspsaga.nvim](#lspsaganvim)
  - [lsp-colors.nvim](#lsp-colorsnvim)
  - [lsp-kind](#lsp-kind)
  - [vim-devicons](#vim-devicons)
  - [vim-startify](#vim-startify)
  - [lualine.nvim](#lualinenvim)
  - [specs.nvim](#specsnvim)
  - [nvim-treesitter](#nvim-treesitter)
  - [cmp-buffer](#cmp-buffer)
  - [nvim-cmp](#nvim-cmp)
  - [nvim-web-devicons](#nvim-web-devicons)
  - [nerdtree](#nerdtree)
  - [nvim-bufferline.lua](#nvim-bufferlinelua)
  - [vim-fugitive](#vim-fugitive)
  - [LuaSnip](#luasnip)
  - [vim-prettier](#vim-prettier)
  - [nvim-ts-autotag](#nvim-ts-autotag)
  - [vim-rhubarb](#vim-rhubarb)
- [Credits](#credits)

# Requirements

- [Neovim](https://neovim.io) v0.5 at least.
- [Prettier](https://prettier.io) (optional)
- [Git](https://git-scm.com/)

# Installation

```bash
# Move to .config directory
cd ~/.config
# Back up our current config (Recommended)
cp -r nvim nvim.backup
# Clone repository
git clone https://github.com/pauchiner/chiner.nvim ~/.config/nvim
```

Or [download the repository](https://github.com/pauchiner/chiner.nvim/archive/refs/heads/main.zip) and copy the folder on your config directory.

# Installing the plugin manager

This neovim config uses [vim-plug](https://github.com/junegunn/vim-plug) as plugin manager.

## Why doesn't work ⁉️
By default when you run the configuration for the first time, vim-plug is autoloaded.
If you have any problem see the [vim-plug installation guide](https://github.com/junegunn/vim-plug#installation).
# Usage

## Keybindings

### Basic key binds

|                 |               |
|-----------------|---------------|
| Leader Key      |      `;`      |
| Escape Key      |`<leader> ;`   |

### Buffers

|  Function       |  keybind      |
|-----------------|---------------|
| Buffer Next     |`<tab>`        |
| Buffer Previous |`<Shift> <tab>`|

### Browser

|  Function       |  keybind      |
|-----------------|---------------|
| Toggle Nerdtree | `<leader> l`  |


To see all check [maps.vim](https://github.com/pauchiner/chiner.nvim/blob/main/maps.vim).

## Color Scheme

This configuration uses [One](https://github.com/joshdick/onedark.vim) color scheme.


To change the color scheme go to [init.vim](https://github.com/pauchiner/chiner.nvim/blob/0cd9cd08eb006c615be2e9a65eb3016e3cca0724/init.vim#L142) on the line 142:
```vim 
colorscheme one
```
and change `one` with your color scheme.

All color schemes are stored in the [`colors/`](https://github.com/pauchiner/chiner.nvim/tree/main/colors) directory.

# Plugins

All of the plugins of the configuration file are here:

## [nvim-lspconfig](https://github.com/neovim/nvim-lspconfig)

The neovim built-in lsp client with some plugins.

[View on github ↩︎](https://github.com/neovim/nvim-lspconfig)

## [nvim-lsp-installer](https://github.com/williamboman/nvim-lsp-installer)

Neovim plugin that allows you to seamlessly manage LSP servers with :LspInstall.

<img width="500px" alt="lsp-installer preview" src="images/img2.png">

## Installing Language support clients

To see a full list of the supported Languages see [this](https://github.com/williamboman/nvim-lsp-installer/tree/main/lua/nvim-lsp-installer/servers).

To install a Language server just enter this:
`:LspInstall` followed by `<TAB>` to see all the options.


[View on github ↩︎](https://github.com/williamboman/nvim-lsp-installer)

## [lspsaga.nvim](https://github.com/tami5/lspsaga.nvim)

Is a light-weight lsp plugin based on neovim built-in lsp with highly a performant UI.

<img width="500px" alt="lspsaga preview" src="images/img3.gif">

[View on github ↩︎](https://github.com/tami5/lspsaga.nvim)

## [lsp-colors.nvim](https://github.com/folke/lsp-colors.nvim)

Plugin that creates missing LSP diagnostics highlight groups for color schemes.

<img alt="lsp-colors preview" src="images/img4.png">

[View on github ↩](https://github.com/folke/lsp-colors)

## [lsp-kind](https://github.com/onsails/lspkind.nvim)

Pictograms for neovim built-in lsp.

<img alt="lsp-kind preview" src="images/img5.png">

[View on github ↩](https://github.com/onsails/lsp-kind)

## [vim-devicons](https://github.com/ryanoasis/vim-devicons)

Adds file type icons to Vim plugins.

<img alt="vim-devicons preview" src="images/img6.png">

[View on github ↩](https://github.com/ryanoasis/vim-devicons)

## [vim-startify](https://github.com/mhinz/vim-startify)

[View on github ↩](https://github.com/mhinz/vim-startify)

## [lualine.nvim](https://github.com/nvim-lualine/lualine.nvim)

[View on github ↩](https://github.com/nvim-lualine/lualine.nvim)

## [specs.nvim](https://github.com/edluffy/specs.nvim)

[View on github ↩](https://github.com/edluffy/specs.nvim)

## [nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter)

[View on github ↩](https://github.com/nvim-treesitter/nvim-treesitter)

## [cmp-buffer](https://github.com/hrsh7th/cmp-buffer)

[View on github ↩](https://github.com/hrsh7th/cmp-buffer)

## [nvim-cmp](https://github.com/hrsh7th/nvim-cmp)

[View on github ↩](https://github.com/hrsh7th/nvim-cmp)

## [nvim-web-devicons](https://github.com/kyazdani42/nvim-web-devicons)

[View on github ↩](https://github.com/kyazdani42/nvim-web-devicons)

## [nerdtree](https://github.com/preservim/nerdtree)

[View on github ↩](https://github.com/preservim/nerdtree)

## [nvim-bufferline.lua](https://github.com/akinsho/bufferline.nvim)

[View on github ↩](https://github.com/akinsho/bufferline.nvim)

## [vim-fugitive](https://github.com/tpope/vim-fugitive)

[View on github ↩](https://github.com/tpope/vim-fugitive)

## [LuaSnip](https://github.com/L3MON4D3/LuaSnip)

[View on github ↩](https://github.com/L3MON4D3/LuaSnip)

## [vim-prettier](https://github.com/prettier/vim-prettier)

[View on github ↩](https://github.com/prettier/vim-prettier)

## [nvim-ts-autotag](https://github.com/windwp/nvim-ts-autotag)

[View on github ↩](https://github.com/windwp/nvim-ts-autotag)

## [vim-rhubarb](https://github.com/tpope/vim-rhubarb)

[View on github ↩](https://github.com/tpope/vim-rhubarb)

# Credits

<img style="border-radius: 50%" width='90px' src="https://avatars.githubusercontent.com/u/1332805?v=4">

This vim workflow is forked from [craftzdog](https://github.com/craftzdog/dotfiles-public) dotfiles. Thanks! 🙏
