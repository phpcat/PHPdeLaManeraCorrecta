---
isChild: true
anchor:  mac_setup
---

## Configuració per Mac {#mac_setup_title}

El sistema OS X ve prèviament configurat amb una versió de PHP que no és l'actual. El sistema Mountain Lion ve
configurat amb PHP 5.3.10, el sistema Mavericks amb la versió 5.4.17 i el sistema Yosemite amb l'versió 5.5.9.

Hi ha diverses maneres d'instal·lar PHP a l'OS X.

### Instal·lar PHP amb Homebrew

[Homebrew] és un gestor de paquets per OS X, que et pot ajudar a instal·lar PHP i diverses extensions fàcilment.
[Homebrew PHP] és un repositori que conté fitxers per Homebrew relacionats amb PHP, i també et permetrà instal·lar PHP.

En aquest punt, pots instal·lar `php53`, `php54`, `php55` o `php56` escrivint la comanda `brew install`, i podràs
canviar entre les versions modificant la variable `PATH`.

### Instal·lar PHP amb Macports

El projecte [MacPorts], és una iniciativa de la comunitat de codi obert per dissenyar un sistema fàcil d'utilitzar,
instal·lar i actualitzar qualsevol programari de línia d'ordres, X11 o Aqua per al sistema OS X.

MacPorts suporta binaris pre-compilats, per la qual cosa no cal tornar a compilar totes les dependències del codi font
original, et salvarà la vida si no tens els paquets instal·lats al teu sistema.

En aquest punt, pots instal·lar `php53`, `php54`, `php55` o `php56` escrivint la comanda `port install`, per exemple:

    sudo port install php54
    sudo port install php55

I pots escriure la comanda `select` per canviar entre les teves versions actives de php:

    sudo port select --set php php55

### Install PHP via phpbrew

[phpbrew] is a tool for installing and managing multiple PHP versions. This can be really useful if two different
applications/projects require different versions of PHP, and you are not using virtual machines.

### Compile from Source

Another option that gives you control over the version of PHP you install, is to [compile it yourself][mac-compile].
In that case be sure to have installed either [Xcode][xcode-gcc-substitution] or Apple's substitute
["Command Line Tools for XCode"] downloadable from Apple's Mac Developer Center.

### All-in-One Installers

The solutions listed above mainly handle PHP itself, and do not supply things like Apache, Nginx or a SQL server.
"All-in-one" solutions such as [MAMP][mamp-downloads] and [XAMPP][xampp] will install these other bits of software for
you and tie them all together, but ease of setup comes with a trade-off of flexibility.


[Homebrew]: http://brew.sh/
[Homebrew PHP]: https://github.com/Homebrew/homebrew-php#installation
[MacPorts]: https://www.macports.org/install.php
[phpbrew]: https://github.com/phpbrew/phpbrew
[mac-compile]: http://php.net/install.macosx.compile
[xcode-gcc-substitution]: https://github.com/kennethreitz/osx-gcc-installer
["Command Line Tools for XCode"]: https://developer.apple.com/downloads
[mamp-downloads]: http://www.mamp.info/en/downloads/
[xampp]: http://www.apachefriends.org/en/xampp.html
