---
author: kalib
comments: true
date: 2009-01-07 15:57:00+00:00
layout: post
slug: repositorio-brasileiro-arch-linux
title: Repositório Brasileiro Arch Linux
wordpress_id: 57
categories:
- Arch Linux
- Linux
- Software Livre
---
{% img center /imgs/repobr.png 'Repositório Archlinux Brasil' %}
Saudaçes pessoal,




A comunidade [Archlinux-br](http://www.archlinux-br.org/) criou um repositório nacional para o Archlinux. Nele colocaremos alguns pacotes que ainda não foram colocados no repositório do [archlinux.org](http://archlinux.org/), por ainda serem pouco populares, ou que não podem ser incluídos (por serem experimentais, por exemplo). Para utilizá-lo, basta adicionar essas duas linhas no pacman.conf antes dos outros repositórios.




[archlinuxbr]  

Server = http://repo.archlinux-br.org/i686




ou




[archlinuxbr]  

Server = http://repo.archlinux-br.org/x86_64




A política do repositório é: Adicionar qualquer pacote que esteja no [AUR](http://aur.archlinux.org/), desde que não seja malicioso ou tenha muitas falhas de segurança (por isso nada de yaourt :-)) ou tenha problema de licença (por exemplo o Virtual Box). Pacotes de softwares experimentais serão adicionados com nomes diferentes, seguindo a mesma política do AUR (ex.: o Qt Technology Preview se chama qt-tp).




Para adicionar um pacote, mande um e-mail para repo@archlinux-br.org, dando uma breve explicação e o link para o AUR do pacote.