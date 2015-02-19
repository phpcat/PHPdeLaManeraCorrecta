---
title:   Configuració per Mac
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

### Instal·lar PHP amb phpbrew

[phpbrew] és una eina per a la instal·lació i gestió de múltiples versions de PHP. Això pot ser molt útil si dos
[aplicacions / projectes diferents, requereixen diferents versions de PHP, i no s'estan utilitzant màquines virtuals.

### Compilar des del codi font

Una altra opció que et deixa tenir control sobre la versió de PHP que s'instal·la, és [compilar-la tu mateix][mac-
compile]. En aquest cas, assegura't d'haver instal·lat qualsevol [Xcode][xcode-gcc-substitution] o substitut d'Apple
"Eines de línia d'ordres per XCode" descarregables des del Centre de desenvolupadors d'Apple.

### Instal·ladors Tot-en-Un

Les solucions esmentades anteriorment manegen principalment PHP únicament i no proporcionen coses com Apache, Nginx o un
servidor SQL. Solucions "Tot-en-un" com [MAMP][mamp-downloads] i [XAMPP][xampp] instal·len aquests altres programes i
els configura entre ells. De totes maneres la facilitat que aporta potser no compensa amb la poca flexibilitat que
ofereixen.


[Homebrew]: http://brew.sh/
[Homebrew PHP]: https://github.com/Homebrew/homebrew-php#installation
[MacPorts]: https://www.macports.org/install.php
[phpbrew]: https://github.com/phpbrew/phpbrew
[mac-compile]: http://php.net/install.macosx.compile
[xcode-gcc-substitution]: https://github.com/kennethreitz/osx-gcc-installer
["Command Line Tools for XCode"]: https://developer.apple.com/downloads
[mamp-downloads]: http://www.mamp.info/en/downloads/
[xampp]: http://www.apachefriends.org/en/xampp.html
