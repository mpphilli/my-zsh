my-zsh
======

####Git Setup:
```
git config --global user.name “Mike P”
git config --global user.email “mpphilli@users.noreply.github.com"
```
Add SSH key to Github 
https://help.github.com/articles/generating-ssh-keys


####My zsh configuration:
Clone this into ~/my-zsh, and then symlink the zshrc.local file to ~/.zshrc.local:

```
git clone https://github.com/mgdm/zsh-antigen.git ~/.zsh-antigen
cd
ln -s .zsh-antigen/zshrc .zshrc
```

Then pull the GRML zsh config into ~/.zshrc
```
wget -O .zshrc http://git.grml.org/f/grml-etc-core/etc/zsh/zshrc
```
