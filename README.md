# keep

Simple directory encryption using GnuPG `--symmetric`.

## Usage

Encrypt `files` to `files.gpg`:

```sh
keep encrypt files
```

Decrypt `files.gpg` to `files`:

```sh
keep decrypt files.gpg
```

Encrypt `files` to `foo/bar.gpg`, then remove `files`:

```
keep enc -u files foo/bar.gpg
```

Decrypt `foo/bar.gpg` to `a/b/c`, overwriting files in that directory:

```sh
keep dec -f foo/bar.gpg a/b/c
```

More usage information:

```sh
keep --help
```

## Install

```sh
sudo apt-get install bash gnupg # or sudo yum install bash gnupg
sudo wget -O /usr/local/bin/keep \
  https://raw.githubusercontent.com/vjagaro/keep/main/keep
sudo chmod 755 /usr/local/bin/keep
```
