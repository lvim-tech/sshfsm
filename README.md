# SSHFS Manager

## INFO

SSHFS Manager is a cli tool to mount and unmount remote directories.

1. Predefined options (default explorer and editor) and sshfs configs
2. Intuitive menu
3. Exploring mounted directory
4. Editing configuration file from menu

---

![SSHFSM SCREENSHOT](https://github.com/lvim-tech/sshfsm/blob/main/media/sshfs-manager-creenshot.png)

---

> Requirements: `rjshon`, `sshfs`, `unmount`

## HOW TO USE

Just download sshfsm and runing it (script automaticaly create config file - ~/.config/sshfsm/config.json).

If you want to add sshfsm to your PATH, add this to your bashrc:

```bash
export PATH=$PATH:/path/to/sshfsm
```

### Default options

```bash
"options": {
    "editor": "xdg-open", // you can choice "vim"
    "explorer": "xdg-open" // you can choice "vifm"
}
```

### How to write points

```bash
"points": {
    "NAME OF YOUR POINT": {
        "host": "example.com", // required
        "port": "22", // not required, default 22
        "user": "user_name", // required
        "remote_directory": "example.com", // required
        "local_directory": "example.com", // required
        "options": "allow_other" // not required, default null
    }
}
```
