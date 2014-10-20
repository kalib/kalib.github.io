---
author: kalib
comments: true
date: 2008-05-07 16:14:00+00:00
layout: post
slug: configurando-a-jre-para-funcionar-no-buntu-804-com-firefox-3-configuring-jre-on-buntu-804-to-work-with-firefox-30
title: Configurando a JRE para funcionar no *buntu 8.04 com firefox 3 / Configuring
  JRE on *buntu 8.04 to work with Firefox 3.0
wordpress_id: 13
categories:
- Firefox
- Java
- Kubuntu
- Linux
- Software Livre
---

### 

Versão em Português BR / Portuguese Version




Saudações galera..




Aqui segue uma rápida dica que poderá ajudar aqueles que, assim como eu, instalaram o *buntu 8.04 e perceberam que o mesmo possui o Firefox 3.0 em seus repositórios como o navegador padrão.




Bom, ao tentar instalar, desde ontem, o plugin do java para poder acessar minha página do banco, encontrei uma solução bem simples depois de várias tentativas frustradas.




Após tentar tudo que sempre utilizei como por exemplo baixar o pacote jre diretamente do site da sun, descompactar no diretório /usr/java (como sempre fiz por questão de organização), instalar e criar um link simbólico para o mesmo no diretório de plugins do Firefox, e mesmo assim não ter nenhum resultado concreto, pesquisei um pouco e achei uma solução bem mais simples e rápida.




Basta descomentar as linhas referentes aos mirrors multiverse nos seus repositórios (/etc/apt/sources.list), dar um update (# aptitude update) e em seguida instalar os pacotes com o seguinte comando:




# aptitude install sun-java6-jre sun-java6-plugin sun-java6-fonts




Feito isto reinicie o firefox e digite em sua barra de endereços:




about:plugins




Deverá agora constar em sua lista de plugins os referentes ao java. ;]




Outro teste é digitar no seu console: $ java -version




Você deverá ter um retorno similar a este:




java version "1.6.0_06"  

Java(TM) SE Runtime Environment (build 1.6.0_06-b02)  

Java HotSpot(TM) Client VM (build 10.0-b22, mixed mode, sharing)




Ou mesmo acessando alguma página que se utilize de java como o teclado virtual do Banco do Brasil por exemplo.  

;]




Bom, espero ter ajudado com esta simples, porém eficiente dica.




Abraços




-----------------------------------------------------

Versão em Inglês / English Version




Hey Guys..




Here I'll describe a simple and quickly way that can help those people who, like me, are trying to use *buntu 8.04 and have realized that it comes with Firefox 3.0 beta 5 on its repositories as the default web browser.




Well, trying to install the java plugin since yesterday to access my bank account, I could find a simple way after some frustrated tries.




After trying every ways i had always use, like for example downloading the jre package directly from the sun's website, install it and create a symbolic link at Firefox plugin's directory and have no positive answer, I decided to search on the web until realize that a simple aptitude's use could solve my problem and make it work correctly.




All you have to do is uncomment (remove the # from the beggining of the line) the multiverse mirror's lines at your sources file (/etc/apt/sources.list). The next step is to make an upload on your mirrors and repositories (# aptitude update) and then install the necessary packages with the following line command:




# aptitude install sun-java6-jre sun-java6-plugin sun-java6-fonts




It's done!




Can't believe? Restart your Firefox and put the following command on your address bar:




about:plugins




You should find some lines describing your java plugin on the plugins page, like all your other plugins on Firefox.




Another way to test and check it is typing the following command on a terminal or console:




$ java -version




You should receive some return like this:




java version "1.6.0_06"  

Java(TM) SE Runtime Environment (build 1.6.0_06-b02)  

Java HotSpot(TM) Client VM (build 10.0-b22, mixed mode, sharing)




Or, if you still not believing, you can try to access some website that uses java like some bank sites for example. ;]




Well, i hope this text could help some of you guys.




Take Care