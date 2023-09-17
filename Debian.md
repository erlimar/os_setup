Debian 12, codinome bookworm
============================

Alguns dados:

* GNOME 43
* Wayland
* Arquitetura amd64
* Tema escuro

Primeiros softwares instalados:

* GCC 12.2
```sh
root@$ apt install gcc
```

* GNU Make 4.3
```sh
root@$ apt install make
```

* CMake 3.25.1
```sh
root@$: apt install cmake
```

* Ninja Build 1.11.1
```sh
root@$ apt install ninja-build
```

* Curl 7.88.1
```sh
root@$ apt install curl
```

* Alguns utilitários e bibliotecas de desenvolvimento
```sh
root@$ apt install dh-autoreconf \
  libcurl4-gnutls-dev \
  libexpat1-dev \
  gettext \
  libz-dev \
  libssl-dev \
  asciidoc \
  xmlto \
  docbook2x \
  install-info
```

* Git 2.42 - à partir do código fonte
```sh
# Baixa código fonte
$ curl -O https://mirrors.edge.kernel.org/pub/software/scm/git/git-2.42.0.tar.gz

# Descompacta conteúdo
$ tar -xzf git-2.42.0.tar.gz

# Compila código
$ cd git-2.42.0
$ make configure
$ make all doc info

root@$ make install install-doc install-html install-info
```

* Neovim 0.9 - à partir do código fonte
```sh
# Baixa código fonte
$ git clone https://github.com/neovim/neovim
$ cd neovim
$ git checkout release-0.9

# Compila código
$ make CMAKE_BUILD_TYPE=Release CMAKE_INSTALL_PREFIX=/usr
root@$ make install
```
  - Minhas configurações do Neovim: https://github.com/erlimar/astronvim_config

