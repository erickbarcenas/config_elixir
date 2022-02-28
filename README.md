# config_elixir


- Instalar asdf https://github.com/asdf-vm/asdf 
- Instalar plugin asdf para erlang https://github.com/asdf-vm/asdf-erlang 
- Instalar plugin asdf para elixir https://github.com/asdf-vm/asdf-elixir 

## Super user
sudo su

##Config
sudo apt update
sudo apt install curl

apt-get -y install build-essential autoconf m4 libncurses5-dev libwxgtk3.0-gtk3-dev libgl1-mesa-dev libglu1-mesa-dev libpng-dev libssh-dev unixodbc-dev xsltproc fop libxml2-utils libncurses-dev openjdk-11-jdk

## Clone
git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.9.0

## Configure Your Shell


echo -e '\n. $HOME/.asdf/asdf.sh' >> ~/.bash_profile

echo -e '\n. $HOME/.asdf/completions/asdf.bash' >> ~/.bash_profile

asdf --version

source ~/.bash_profile

## Plugins
asdf plugin-add elixir https://github.com/asdf-vm/asdf-elixir.git

asdf plugin add erlang https://github.com/asdf-vm/asdf-erlang.git


## Installation
asdf install erlang 24.2

#asdf list-all erlang

asdf install elixir 1.13

#asdf list elixir

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
