# Autostart a Bash Script on Linux

## Example Script

```bash
#!/bin/bash

# Load the .bashrc file
source /root/.bashrc

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

# ========== NodeJS Servers ==========

# AstragoDE Website 
tmux new-session -s "nodeAstragoDeNuxt" -d "cd /root/nodeServers/AstragoDE_Technologies/astrago_de-nuxt && bash /root/nodeServers/AstragoDE_Technologies/astrago_de-nuxt/run.sh"
```

This script starts a tmux session with a node server running inside. First the `.bashrc` file is loaded, then the `nvm` environment is loaded. After that the tmux session is started, which will first cd into the correct folder and then start the `run.sh` file in the same folder.

## Autostart the Script
We will use crontab to autostart the script. To edit the crontab file, run the following command:

```bash
crontab -e
```

then you need to append the following line to the file:

```bash
@reboot sh /root/autostart.sh
```

we assume that the script is located in the root folder and is called `autostart.sh`. If you want to use a different path or filename, you need to change the path in the line above.

## Credits
This guide was inspired by [this](https://www.baeldung.com/linux/run-script-on-startup#1-using-cron) article.