sudo rm -fr /usr/local/bin/archey /usr/local/bin/archey-en /usr/local/archey-osx

cd $HOME
[[ -s .zshrc ]] && sed -i ".bak" '/archey/d' .zshrc

 [[ -s .bashrc ]] && sed -i ".bak" '/archey/d' .bashrc 

[[ -s .bash_profile ]] && sed -i ".bak" '/[[ -s ~\/.bashrc ]] && source ~\/.bashrc/d' .bash_profile