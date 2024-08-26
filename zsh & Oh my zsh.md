# zsh & Oh my zsh

Install zsh dan oh my zsh pada ubuntu 

## Installation

```bash
apt install zsh curl
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## Install Powerlevel10k

```bash
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k

# Edit file .zshrc
nano .zshrc

# rubah ZSH_THEM
ZSH_THEME="robbyrussell"

# menjadi
ZSH_THEME="powerlevel10k/powerlevel10k"

# jalankan perintah source 
sourche .zshrc

```
## Install Plugin zsh-autosuggestions & zsh-syntax-highlighting

```bash
# jalankan perintah dibawah ini 
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions

git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting

# Edit file .zshrc
nano .zshrc

# Edit pada bagian plugins= menjadi
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

# jalankan perintah source 
sourche .zshrc
