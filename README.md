
Millions of years ago, a race of hyper-intelligent beings built the most powerful computer ever conceived—Deep Thought—to answer the greatest mystery of all: What is the meaning of life, the universe, and everything? After eons of humming, blinking, and thinking (very deeply), Deep Thought finally emerged from its contemplative trance and declared the answer was… 42. The architects were stunned. “Forty-two what?” they asked. Deep Thought blinked again and shrugged—in its very supercomputer way. You see, it had given the answer, but no one had ever figured out the question. And so began the most wonderfully ridiculous search for meaning in the galaxy: not for life itself, but for the question that made 42 the answer. It’s a brilliant cosmic punchline, reminding us that maybe the universe isn’t just strange—it’s in on the joke.

# Vim42 Configuration

> ⚙️  A customized Vim setup designed for efficient development at Ecole 42 and beyond, developed by students, with full integration for Norminette, Git, snippets, fuzzy search, smooth scrolling, and more.

```
===========================================================
██████      ██████     ██████████████████████████
██████      ██████     ██████████████████████████
██████      ██████     ██████              ██████
██████      ██████     ██████              ██████
██████      ██████                         ██████
██████      ██████                         ██████
██████      ██████     Vim                 ██████
██████████████████                         ██████
██████████████████       ████████████████████████
██████████████████       ████████████████████████
            ██████       ██████
            ██████       ████████████████████████
            ██████       ████████████████████████
```

---

## 📦 Plugin Manager: Vim-Plug

This configuration uses [vim-plug](https://github.com/junegunn/vim-plug) for plugin management. Plugins are installed in `~/.vim/plugged`.

### Install `vim-plug` (if not installed):
```bash
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
     https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

---

## 🔌 Included Plugins

| Category          | Plugins |
|-------------------|---------|
| **File Explorer** | `preservim/nerdtree` |
| **Fuzzy Finder**  | `junegunn/fzf`, `junegunn/fzf.vim` |
| **Commenting**    | `tpope/vim-commentary` |
| **Start Screen**  | `mhinz/vim-startify` |
| **Brackets**      | `jiangmiao/auto-pairs` |
| **Git Tools**     | `tpope/vim-fugitive`, `lewis6991/gitsigns.nvim` |
| **Linting**       | `vim-syntastic/syntastic` |
| **AI Coding**     | `github/copilot.vim` |
| **Scrolling**     | `terryma/vim-smooth-scroll` |
| **YAML Support**  | `stephpy/vim-yaml` |
| **Terminal**      | `kassio/neoterm` |
| **Themes**        | `nordtheme/vim`, `akiicat/vim-github-theme`, `greenvision` |
| **Completion**    | `neoclide/coc.nvim` |
| **42 Norms**      | `alexandregv/norminette-vim` |

---

## 🧠 Key Mappings

| Mode | Keys                  | Action                                      |
|------|------------------------|---------------------------------------------|
| Normal | `<leader>ft`         | Toggle NERDTree                             |
| Normal | `<leader><ff>`        | Open FZF file search                        |
| Normal | `cc`                 | Comment/uncomment line                      |
| Visual | `cc`                | Comment/uncomment selected lines            |
| Normal | < ` >                | toggle Copilot On-Off                       |
| Normal | `<A-Left>`           | Move to left window                         |
| Normal | `<A-Right>`          | Move to right window                        |
| Normal | `<A-Up>`             | Move to upper window                        |
| Normal | `<A-Down>`           | Move to lower window                        |
| Normal | `<leader>sw`         | Swap windows                                |
| Terminal | `<C-n><C-n>`       | Escape terminal mode                        |
| Normal | `<S-Down>`           | Smooth scroll down                          |
| Normal | `<S-Up>`             | Smooth scroll up                            |
| Normal | `<S-Right>`          | Scroll right by 5 characters                |
| Normal | `<S-Left>`           | Scroll left by 5 characters                 |
| Normal | `<leader>nn`         | Run Norminette on current file              |

> Note: `<leader>` is the spacebar in this config.

---

## 🧪 42 Norminette Integration

- Runs both `norminette` and `gcc` via Syntastic.
- Errors shown on file open.
- Location list auto-populated.

To run Norminette manually:
```vim
<leader>nn
```

---

## 🎨 Theme: Nord (Customized)

Uses the `nord` colorscheme with overridden highlights for vivid C development colors. Requires `termguicolors`.

---

## ✅ Installation Guide (If you don't have a vim configuration installed such as SpaceVim, in that case, you need to remove that configuration first)

Follow these steps to set up your custom Vim configuration:

1. **Make sure `vim-plug` is installed**
   Run the following command to check:

   ```bash
   ls ~/.vim/autoload/plug.vim
   ```

   If the file does **not** exist, install it with:

   ```bash
   curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
   https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
   ```

2. **Clone this repository**
   Use `git` to clone the configuration files:

   ```bash
   git clone https://github.com/malhyasa/Vim42.git
   cd Vim42
   ```

3. **Move the `.vimrc` file to your home directory**

   ```bash
   mv .vimrc ~/
   ```

4. **Install the plugins**
   Open Vim and run the following command:

   ```vim
   :PlugInstall
   ```

5. ✅ You're all set!
   Your Vim is now configured with your custom settings and plugins.


## 🧰 Recommended Tools

- [`norminette`](https://github.com/42School/norminette)
- `gcc`, `ctags`, `ripgrep`

Disclaimers:
- This configuration was tailored by students and is not an official 42 configuration.
- This configuration is a work in progress and may not be fully optimized. Contributions and suggestions are welcome!
```

Made with love @ 42Amman
