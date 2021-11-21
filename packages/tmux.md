[< Back](../readme.md)


### New window
```bash
tmux new -s <NAME>
```

---

### List windows
```bash
tmux ls
```

---

### Attach to window
```bash
tmux a -t <NAME>
```

---

### Detach from window (in window)
<kbd>Ctrl</kbd> + <kbd>B</kbd> --> <kbd>D</kbd>

---

### Rename window
```bash
tmux rename-window -t <WINDOW> <NEWNAME>
```

### Rename window (in window)
<kbd>Ctrl</kbd> + <kbd>B</kbd> --> <kbd>$</kbd>

---

### Kill Session
```bash
tmux kill-session -t <WINDOW>
```

### Kill Session (in window)
<kbd>Ctrl</kbd> + <kbd>B</kbd> --> ```:kill-session```

---

### Kill all Sessions
```bash
tmux kill-server
```

