# Git 101 +

## Primer tiempo

### Configuramos nuestra instancia de GIT

```
$ git config --global user.name "Roberto Pettinato"
$ git config --global user.email robertito@gmail.com
$ git config --list
```

### Creamos nuestas firmas :)

- [GPG key](https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key)
- [SSH key](https://docs.github.com/es/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

```
$ ssh-keygen -t ed25519 -C "robertito@gmail.com"
$ eval "$(ssh-agent -s)"
$ ssh-add ~/.ssh/id_ed25519
```

```
$ gpg --full-generate-key
$ gpg --list-secret-keys --keyid-format=long
/Users/hubot/.gnupg/secring.gpg
------------------------------------
sec   4096R/3AA5C34371567BD2 2016-03-10 [expires: 2017-03-10]
uid                          Hubot <hubot@example.com>
ssb   4096R/4BB6D45482678BE3 2016-03-10
$ gpg --armor --export 3AA5C34371567BD2
```

### Instalamos GIT

- [GIT Download Page](https://git-scm.com/downloads)

### Creamos un Repo

```
$ mkdir -p ~/Repos/git101
$ cd ~/Repos/git101
$ git init
```

### Creamos contenido

```
$ $editor README.md
# Mi primer Readme en Git
```

### Añadimos el codigo al repo y commiteamos

```
$ git status
$ git add README.md
$ git status
$ git commit -m 'Primer Commit!'
```

### Verificamos :)

```
$ git status

```
