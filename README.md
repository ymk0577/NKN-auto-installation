# NKN-auto-installation
This script is used to implement the automatic one-click deployment function of the NKN program.

After execution, NKN will be run based on the Docker container.

After the NKN program is running, it will automatically generate a default configuration file and a new wallet file.

However, the automatically generated configuration file is not suitable for hosts with low storage space and low memory, and the new wallet file cannot be used unless 10 NKN is manually transferred to activate it because it has no ID.

Therefore, the script has a step to detect the NKN data folder before installation. If the NKN folder already exists, it will automatically proceed to the next step; if it does not exist, it will be required to enter the configuration file and wallet file related content.

Reference website/document:
1. https://github.com/nknorg/nkn
2. https://hub.docker.com/r/nknorg/nkn

# Main features
1. All programs involved use official channels without any additions.
2. Determine whether the Docker program already exists. If not, Docker will be automatically installed.
3. Determine whether the NKN container based on Docker already exists. If not, it will be automatically created.
4. If the NKN container already exists, the old version will be automatically deleted and the latest version will be re-pulled.
5. The NKN container will use the HOST network configuration and set automatic start/restart.
6. If the NKN data folder already exists, the configuration stage will be skipped. If not, the configuration will need to be written manually, that is, config.json / wallet.json / wallet.pswd files.
7. The installation process will automatically create the NKN folder (skip if it already exists) and set the data folder mapping of the NKN container.
8. Please check the source code for more specific details.

# Install
```
curl -L https://raw.githubusercontent.com/ymk0577/NKN-auto-installation/main/nkn.sh -o nkn.sh && chmod +x nkn.sh && bash nkn.sh
```
Execute the above command to execute the installation script.

# Uninstall
```
bash nkn.sh -u
```
Uninstall nkn service.

# Notice
Please check the code yourself before use to confirm whether it meets your own usage requirements.
Please note that I am not responsible for any problems that arise from using this script.
