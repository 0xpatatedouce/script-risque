#!/bin/bash
exists()
{
  command -v "$1" >/dev/null 2>&1
}
if exists curl; then
echo ''
else
  sudo apt update && sudo apt install curl -y < "/dev/null"
fi


# Télécharger le script d'installation de NVM depuis GitHub
curl -sL https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.0/install.sh -o install_nvm.sh

# Installer NVM en exécutant le script d'installation
sh install_nvm.sh

# Si l'installation de NVM nécessite d'accepter des conditions de licence, suivre les instructions pour accepter
# Par exemple, sur macOS, cela peut nécessiter d'exécuter la commande suivante
# sudo xcodebuild -license

# Installer la version spécifique de NodeJS (16.20) avec NVM
nvm install 16.20

# Utiliser la version spécifique de NodeJS (16.20) installée avec NVM
nvm use 16.20

# Créer un répertoire temporaire pour exécuter la cérémonie
mkdir ~/p0tion-tmp

# Naviguer vers le répertoire temporaire créé
cd ~/p0tion-tmp
