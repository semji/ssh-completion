# ssh-completion

Auto-magically add completion on your ssh command from remote configs file.

## get started

- clone repository
- Source `.ssh_completion` file in your `.bashrc`
```
f [ -f /path/to/.ssh_completion ]; then
        source /path/to/.ssh_completion
fi
```
- list your base ssh config files in `.ssh_config_shared_files`

## own config

The projet concat files into `~/.ssh/config-generate` in the following order :

- `~/.ssh/config-before`
- `~/.ssh/config`
- All config file list in `.ssh_config_shared_files`
- `~/.ssh/config-after`
