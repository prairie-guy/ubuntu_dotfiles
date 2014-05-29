ubuntu_dotfiles.git
============
Clone and run this on a new instance running Ubuntu 14.02 LTS to
configure your `bash` and `emacs` development environment as follows:

```sh
cd $HOME
git clone https://github.com/prairie-guy/ubuntu_dotfiles.git .dotfiles
ln -sb .dotfiles/.screenrc .
ln -sb .dotfiles/.bash_profile .
ln -sb .dotfiles/.bashrc .
ln -sb .dotfiles/.bashrc_custom .
mv .emacs.d .emacs.d~
ln -s .dotfiles/.emacs.d .
```

See also https://github.com/prairie-guy/ubuntu_setup.git to install prerequisite
programs. If all goes well, in addition to a more useful prompt, now you can
do `emacs -nw hello.js` and hitting `C-c!` to launch an interactive SSJS
REPL, among many other features. See the
[Startup Engineering Video Lectures 4a/4b](https://class.coursera.org/startup-001/lecture/index)
for more details.
