git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.7.4

echo -e '\n. $HOME/.asdf/asdf.sh' >> ~/.bashrc
echo -e '\n. $HOME/.asdf/completions/asdf.bash' >> ~/.bashrc

sudo apt install \
  automake autoconf libreadline-dev \
  libncurses-dev libssl-dev libyaml-dev \
  libxslt-dev libffi-dev libtool unixodbc-dev \
  unzip curl
  
## re-open the terminal  
asdf update

## install python
asdf plugin-add python
asdf install python 3.6.2
asdf install python 2.7.13
asdf global python 3.6.2 2.7.13

## install nodejs
sudo apt-get install dirmngr gpg --yes
asdf plugin-add nodejs
bash ~/.asdf/plugins/nodejs/bin/import-release-team-keyring
asdf install nodejs 12.13.0
asdf global nodejs 12.13.0
