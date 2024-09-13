# NKN-auto-installation
This script is based on the Docker environment and is used to achieve fully automatic one-click deployment of NKN programs.

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

# Script parameter description


# Notice
Please check the code yourself before use to confirm whether it meets your own usage requirements.
Please note that I am not responsible for any problems that arise from using this script.
