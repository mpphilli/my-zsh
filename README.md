my-zsh
======

Pull the GRML zsh config into ~/.zshrc
```
wget -O ~/.zshrc http://git.grml.org/f/grml-etc-core/etc/zsh/zshrc
```

####Git Setup:
```
git config --global user.name "Mike P"
git config --global user.email "mpphilli@users.noreply.github.com"
```
Add SSH key to Github 
https://help.github.com/articles/generating-ssh-keys


####My zsh configuration:
Clone my zsh config into ~/my-zsh, and then symlink the zshrc.local file to ~/.zshrc.local:

```
git clone git@github.com:mpphilli/my-zsh.git ~/my-zsh
cd ~/my-zsh
git submodule init
git submodule update
cd
ln -s ~/my-zsh/zshrc.local ~/.zshrc.local
```


####Git Commands
git help <command> - read about a specific subcommand or concept
git status - Show the working tree status
git add - Add file contents to the index
git rm - Remove files from the working tree and from the index
git mv - Move or rename a file, a directory, or a symlink
git diff - Show changes between commits, commit and working tree, etc
git commit - Record changes to the repository
       -a - Tell the command to automatically stage files that have been modified and deleted, but new files you have not told Git about are not affected.
git push - Update remote refs along with associated objects
git log - Show commit logs  http://git-scm.com/book/en/Git-Basics-Viewing-the-Commit-History
git fetch origin - fetches any new work that has been pushed to that server since you cloned (or last fetched from) it
git pull - fetches data from the server you originally cloned from and automatically tries to merge it into the code you’re currently working on

- Submodules
git submodule update - Update the registered submodules
