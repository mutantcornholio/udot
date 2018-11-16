# udot

**udot**: upload dotfiles!
Runs manually, uses rsync under the hood.

### Installation

1. Download `udot` to your favorite place for user-defined-binaries. e.g.
```bash
sudo curl https://raw.githubusercontent.com/mutantcornholio/udot/master/udot -o /usr/local/bin/udot
sudo chmod +x /usr/local/bin/udot
```
2. Create `.udot` configs in your home dir. e.g.
```bash
mkdir "$HOME/.udot"

echo "- ***/.git" >> "$HOME/.udot/dotfiles"
echo "+ .vimrc" >> "$HOME/.udot/dotfiles"
echo "+ .vim/***" >> "$HOME/.udot/dotfiles"

echo "my-server1.org" >> "$HOME/.udot/servers"
echo "my-server2.org" >> "$HOME/.udot/servers"
```
3. Run `udot`:  
![screencast.gif](http://mcornholio-s3.s3.amazonaws.com/udot.gif)
