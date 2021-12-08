# Installation of Java (17)

## Before Installation

Uninstall previous Java installations, as otherwise they might interfere with the new Java version.

## Download
Follow the steps for a manual installation shown on [this website](https://www.linuxcapable.com/how-to-install-java-17-lts-jdk-17-on-ubuntu-20-04/#ftoc-heading-8).

Remember to check if every command ran successfully. The name of the downloaded or unzipped file might differ from the one shown in the tutorial. Adjust the following commands accordingly.

## Set $PATH permanently
In order to set the $PATH permanently, you must **append** both "export-commands" to the end of the .bashrc file. This file is found in the home directory of the user.

 
### Edit the .bashrc-file for the root user:
```bash
nano /root/.bashrc
``` 

### Example:
```bash
# set $PATH for Java 17
export JAVA_HOME=/opt/jdk17
export PATH=$PATH:$JAVA_HOME/bin
```