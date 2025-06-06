
# 🧪 Workflow & Command Reference

## 🔐 Daily Startup

### Start Your Day
```bash
startday
```
- Initializes today's daily note and log file.
- Loads your current focus from `.current` if set.

---

## 🔁 Focus Management

### Switch Focus (no logging)
```bash
switchfocus [folder]
```
- Updates your `.current` focus silently.

### Refocus (log + note update)
```bash
focus [folder/path]
```
- Updates `.current` and logs the switch.
- Appends a working link to your Daily note.

Examples:
```bash
focus Courses/Cloud+
focus HTB/Machines/fawn
focus Planner
```

---

## 🕹️ HTB Machine Operations

### 🔌 Connect to HTB VPN
```bash
htbvpn
```
- Uses permanent config at `~/VPNs/htb.ovpn`
- Must keep the terminal open to stay connected

### 🖥️ Manage tmux Sessions

- Start new session:
  ```bash
  htbmux
  ```

- Detach from session:
  - Press `Ctrl + b`, then `d`

- Reattach:
  ```bash
  tmux attach -t htb
  ```

- Kill session:
  ```bash
  tmux kill-session -t htb
  ```

---

## 📦 Common tmux Shortcuts

- Split window vertically: `Ctrl + b`, then `%`
- Split window horizontally: `Ctrl + b`, then `"`
- Switch panes: `Ctrl + b`, then arrow keys
- Resize panes: `Ctrl + b`, hold `Ctrl` + arrow keys
- New window: `Ctrl + b`, then `c`
- Next/prev window: `Ctrl + b`, then `n` / `p`

---

## 🛑 End Your Day

### Push changes to GitHub
```bash
endday
```
- Commits and pushes notes + logs
- Finalizes your daily log

---

## 📝 Notes

- VPN file now lives in `~/VPNs/htb.ovpn`
- `startday`, `focus`, and `endday` are all customized aliases
- Maintain consistent folder names for Obsidian link