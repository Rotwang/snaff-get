# Python utility to assume available roles in AWS

`!!!!! Notice !!!!!`
`snaff-get` will update your `~/.aws` configuration files removing all the comments in the process (it shouldn't touch your current credentials though)!

Tested with Python 3.5.2

## TL;DR

```
# Note that you may require root priviledges to install packages via pip3
curl https://raw.githubusercontent.com/Rotwang/snaff-get/master/requirements.txt > /tmp/reqs.txt
pip3 install -r /tmp/reqs.txt
# put snaff-get somewhere in your $PATH
curl https://raw.githubusercontent.com/Rotwang/snaff-get/master/snaff-get > ~/bin/snaff-get
chmod +x ~/bin/snaff-get
$ snaff-get # run snaff-get -h for details
```

To upgrade:

```
$ snaff-get -e # checks if new version is available in the upstream repository
New version is available!
$ snaff-get -u # fetches snaff-get from the upstream and replaces it on disk
I'm upgraded (or at least refreshed).

## Install

### Mac OSX

python 3.5.2

```
brew install pyenv
pyenv install 3.5.2
```

snaff-get

```
git clone git@github.com:Rotwang/snaff-get.git
cd snaff-get
virtualenv -p /usr/local/Cellar/pyenv/1.1.3/versions/3.5.2/bin/python env
source ./env/bin/activate
pip install -r requirements.txt
./snaff-get -h
```
