---
author: kalib
comments: true
date: 2009-08-19 13:12:02+00:00
layout: post
slug: erro-com-a-libjpeg-resolvendo-no-archlinux
title: Erro com a libjpeg.. resolvendo no archlinux
wordpress_id: 556
categories:
- Arch Linux
- Linux
- Software Livre
---

![](http://www.adslgr.com/forum/picture.php?albumid=214&pictureid=1984)



**Q**uem está utilizando o [Archlinux](http://archlinux.org) devidamente atualizado, pode ter percebido alguns erros relacionados à libjpeg.so ao tentar executar alguma aplicação, como foi o meu caso com o [floola](http://www.floola.com), um gerenciador para meu ipod com o qual transfiro e manipulo minhas músicas pelo linux.

**O** problema se deu pelo fato de o Archlinux já ter adotado a nova libjpeg. Esta versão 7 possui algumas vantagens em relação a versão anterior, porém muitos aplicativos ainda não foram atualizados para esta nova versão. Este foi o caso do floola por exemplo, que só funciona com a libjpeg6.

**S**egue uma dica simples e rápida para resolver este pequeno problema.

**1-** Baixe o pacote da libjpeg6 diretamente do [AUR](http://aur.archlinux.org) através do seguinte link:


> http://aur.archlinux.org/packages/libjpeg6/libjpeg6.tar.gz


**2-** Descompacte o arquivo:


> [kalib@tuxcaverna downloads]$ tar -xvzf libjpeg6.tar.gz


**3-** Entre no diretório libjpeg6, crie e instale o pacote a partir do PKGBUILD extraído:


> [kalib@tuxcaverna downloads]$ cd libjpeg6/

[kalib@tuxcaverna libjpeg6]$ makepkg

[kalib@tuxcaverna libjpeg6]$ pacman -U libjpeg6-6b-6-i686.pkg.tar.gz


**F**eito isto, pode executar novamente o software que estava apontando o erro. No meu caso foi o floola. Isto resolverá o seu problema. ;]

**A**braços


![](http://www.marcelocavalcante.net/portal/imgs/userbar.gif)




