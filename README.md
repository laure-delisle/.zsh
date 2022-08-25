# zsh_config

### for colors in man pages:

`sudo apt-get install most`

### run:

`./deploy.sh`

## New laptop setup
Essential packages

- `sudo apt-get install vim python3-pip git` !!! do not install virtualenv via apt-get
- `pip3 install virtualenv; pip install --upgrade virtualenv

Generate ssh-key for github

- generate key `ssh-keygen -t rsa -b 4096 -C "laure.delisle@gmail.com"` with path `/home/laure/.ssh/github_id_rsa` and passphrase of choice.
- activate SSH agent `eval "$(ssh-agent -s)"`
- add newly created key to agent `ssh-add ~/.ssh/github_id_rsa`.
- add key to https://github.com/settings/keys by clicking "new SSH key" (use `cat .ssh/github_id_rsa.pub` and copy into field)

Virtualenv

- folder for all venvs `mkdir /home/laure/venvs`
- create with python3 `virtualenv -p python3 venvs/comp-vis`
- `source venvs/comp-vis/bin/activate`
- install from reqs `pip3 install -r venvs/reqs_comp-vis.txt`

