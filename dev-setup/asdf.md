# asdf Version Manager

`asdf` is an extendable version manager that can be used to manage Ruby, NodeJS, and many others in a single unified version manager.

## Why

### Why you need a version manager

1. It makes it easy to install ruby and node.
1. If you're working with > 1 project, they might not use the same rubies, for instance. If you wanted to do this by hand, it would take awhile to switch rubies every time you wanted to swap versions.

### Why asdf?

1. asdf provides a unified interface to all packages you might want to install
1. asdf is easy to use
1. I've never had an issue with asdf, but I have had plenty of issues with both rvm and rbenv

## Installation

```bash
git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.3.0
# install asdf version manager
echo -e '\n\n# load asdf version manager (https://github.com/asdf-vm/asdf)' >> ~/.profile
echo -e '\n. $HOME/.asdf/asdf.sh' >> ~/.bashrc
echo -e '\n. $HOME/.asdf/completions/asdf.bash' >> ~/.bashrc
# reboot

# install asdf plugins
asdf plugin-add ruby https://github.com/asdf-vm/asdf-ruby.git
asdf plugin-add nodejs https://github.com/asdf-vm/asdf-nodejs.git

# install 2 latest rubies
asdf install ruby 2.4.1
asdf install ruby 2.3.4

# install latest nodejs lts (at time of writing guide)
asdf install nodejs 6.11.0
```

## Alternatives

Ruby: rvm, rbenv
NodeJS: nvm
