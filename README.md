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
$ git add README.md
$ git commit -m 'Primer Commit!'
```

### Verificamos :)

```
$ git status
```
