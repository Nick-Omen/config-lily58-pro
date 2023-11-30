# config-lily58-pro
My lily58 pro keymap without LED

### 1. Link folder with qmk project
```bash
ln -s ./omen666 [path_to_qmk]/keyboards/lily58/keymaps/omen666
```

### 2. Convert JSON to C-compatible keymap
```bash
qmk json2c ./omen666/omen_keymap.json
```
and update keymap.c with the output

### 3. Flash
```bash
qmk flash -kb lily58 -km omen666
```