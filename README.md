# keep

Simple directory encryption using GnuPG `--symmetric`.

## Usage


```sh
# encrypt secrets directory to secrets.gpg
keep encrypt secrets

# decrypt secrets.gpg to secrets directory
keep decrypt secrets.gpg

# encrypt secrets directory to foo/bar.gpg, then remove secrets
keep enc -u secrets foo/bar.gpg 

# decrypt foo/bar.gpg to a/b/c directory, overwriting any files therein
keep dec -f foo/bar.gpg a/b/c

# additional help
keep --help
```

## Install

```sh
sudo apt-get install bash gnupg
# or sudo yum install bash gnupg
sudo wget -O /usr/local/bin/keep \
  https://raw.githubusercontent.com/vjagaro/keep/main/keep
sudo chmod 755 /usr/local/bin/keep
```
