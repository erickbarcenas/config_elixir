# config_elixir

## Clone
git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.9.0

## Configure Your Shell

echo -e '\n. $HOME/.asdf/asdf.sh' >> ~/.bash_profile

echo -e '\n. $HOME/.asdf/completions/asdf.bash' >> ~/.bash_profile

## Plugins
asdf plugin-add elixir https://github.com/asdf-vm/asdf-elixir.git

asdf plugin add erlang https://github.com/asdf-vm/asdf-erlang.git



#asdf list-all erlang
#asdf list elixir

## Installation
asdf install erlang 24.2

asdf install elixir 1.13

## Enviroment
mkdir my_fonder_with_enviroment

asdf local erlang 24.2

asdf local elixir 1.13

## Use
elixir -v
iex


## VSCode

https://marketplace.visualstudio.com/items?itemName=JakeBecker.elixir-ls

https://marketplace.visualstudio.com/items?itemName=saratravi.elixir-formatter
