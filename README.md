# NKN-auto-installation
This script is based on the Docker environment and is used to achieve fully automatic one-click deployment of NKN programs.

Reference website/document:
1. https://github.com/nknorg/nkn
2. https://hub.docker.com/r/nknorg/nkn

# Main features
1. All programs involved use official sources, without additional additions.
2. Determine whether the Docker program already exists. If not, Docker is automatically installed.
3. Determine whether the NKN container based on Docker already exists. If not, the container is automatically created.
4. If the NKN container already exists, the old version is automatically deleted and the latest version is re-pulled.
5. The NKN container will use the HOST network configuration and set automatic start/restart.
6. Use custom parameters through this script to set the beneficiary wallet.
7. Automatically create the NKN folder and automatically set the mapping NKN data folder.
8. During the installation process, you will be required to enter the wallet file and password, which need to be prepared in advance.

# Script parameter description


# Notice
Please check the code yourself before use to confirm whether it meets your own usage requirements.
Please note that I am not responsible for any problems that arise from using this script.
