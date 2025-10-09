# Prepare script

### Make script executable
```
sudo chmod +x <path>/tmux-sessionizer.sh
```

### Make script accesible globally
```
sudo ln -s <path>/tmux-sessionizer.sh /usr/local/bin/tmux-sessionizer
```

# How to keybind the script for quick access

## Neovim
`keymap.set("n", "<C-f>", ":silent !tmux neww tmux-sessionizer<CR>", opts)`

## Bash
`bind -x '"\C-f":"tmux-sessionizer"'`

## Zsh
`bindkey -s ^f "tmux-sessionizer\n"`
