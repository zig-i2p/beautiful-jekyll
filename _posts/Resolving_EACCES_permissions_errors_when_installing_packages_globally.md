---
layout: post
title: npm error EACCES
subtitle: Resolving EACCES permissions errors when installing packages globally
cover-img: 
thumbnail-img: 
share-img: 
gh-repo: 
gh-badge: [star, fork, follow]
tags: [npm, node]
comments: true
---

Устранение ошибок разрешений EACCES при глобальной установке пакетов

Если вы видите ошибку `EACCES` при попытке установить пакет глобально, вы можете: переустановить `npm` с помощью диспетчера версий узлов (рекомендуется) или вручную изменить каталог `npm` по умолчанию. Переустановить `npm` с помощью диспетчера версий узлов. Это лучший способ избежать  проблемы с разрешениями.

 Чтобы переустановить `npm` с помощью диспетчера версий узлов, выполните действия, описанные в разделе [Загрузка и установка Node.js и npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm).

 You do not need to remove your current version of npm or Node.js before installing a node version manager.

 Manually change npm's default directory Note: This section does not apply to Microsoft Windows.

 To minimize the chance of permissions errors, you can configure npm to use a different directory.

 In this example, you will create and use hidden directory in your home directory.

 Back up your computer.

 On the command line, in your home directory, create a directory for global installations: Configure npm to use the new directory path: npm config set prefix '~/.npm-global' In your preferred text editor, open or create a ~/.profile file and add this line: export PATH=~/.npm-global/bin:$PATH On the command line, update your system variables: To test your new configuration, install a package globally without using sudo: Instead of steps 2-4, you can use the corresponding ENV variable (e.g.

 if you don't want to modify ~/.profile): NPM_CONFIG_PREFIX=~/.npm-global npx: an alternative to running global commands If you are using npm version 5.2 or greater, you may want to consider npx as an alternative way to run global commands, especially if you only need a command occasionally.

 For more information, see this article about npx.