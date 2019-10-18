Forked from ![mathiasbynens/dotfiles](https://github.com/mathiasbynens/dotfiles)

## Installation

### Using Git and the bootstrap script

Clone the repository wherever you want. (I prefer /Documents)

```
cd ~/Documents
mkdir "Some folder name"
cd "Some folder name"

git clone git@github.com:startupheroes/dotfiles.git && cd dotfiles
```

Check the files and change them if necessary to your preference.
Change git settings in .extra with any editor you like
```
vim .extra
```
```
# Git credentials
GIT_AUTHOR_NAME="your username"
GIT_COMMITTER_NAME="$GIT_AUTHOR_NAME"
git config --global user.name "$GIT_AUTHOR_NAME"
GIT_AUTHOR_EMAIL="your@email"
GIT_COMMITTER_EMAIL="$GIT_AUTHOR_EMAIL"
git config --global user.email "$GIT_AUTHOR_EMAIL"
```

After you are done editing, run the script
```
source bootstrap.sh
```

### Sensible macOS defaults

When setting up a new Mac, you may want to set some sensible macOS defaults:

```bash
./.macos
```

### Install Homebrew formulae

When setting up a new Mac, you may want to install some common [Homebrew](http://brew.sh/) formulae (after installing Homebrew, of course):

For Command Line Software
```bash
./brew.sh
./extra-brew.sh
```

For Graphical Applications
```bash
./extra-cask.sh
```
