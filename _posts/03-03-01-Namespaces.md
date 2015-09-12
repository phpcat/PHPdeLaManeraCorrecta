---
isChild: true
title: Namespaces
anchor:  namespaces
---

## Namespaces {#namespaces_title}

Com ja hem esmentat anteriorment, la comunitat de PHP té molts desenvolupadors creant una gran quantitat de codi. Això vol dir que existeix la possibilitat que dues llibreries diferents utilitzin el mateix nom per a una classe en el seu codi. Quan les dues llibreries s'usen dins del mateix _namespace_ això es denomina com una col·lisió i pot causar problemes.

Els _namespaces_ resolen aquest problema. Com es descriu en el manual de referència de PHP, els _namespaces_ són similars als directoris que separen els arxius en el sistema operatiu. Dos arxius amb el mateix nom poden coexistir en directoris separats. Igualment, dues classes de PHP amb el mateix nom poden coexistir en _namespaces_ separats, és tan simple com això.


És important que separeu el vostre codi amb un _namespace_ perquè pugui ser usat per altres desenvolupadors sense la preocupació que causi conflictes amb altres llibreries.

Un dels mètodes recomanats per a l'ús de namespaces està indicat amb el PSR-0, el qual es proposa proveir una convenció estàndard per als arxius, classes i els namespaces, la qual cosa facilita l'intercanvi i ús del codi en diferents projectes.

Us recomanem utilitzar els namespaces amb la convenció [PSR-4][psr4], ja que proporciona els estàndards de classes, arxius i namespaces que ens facilitaran molt la vida.

A l'octubre de 2014 des de PHP-FIGA es va considerar obsolet l'ús de l'estàndard [PSR-0][psr0], el qual ha estat reemplaçat per [PSR-4][psr4]. Encara es pot fer servir PSR-0, però amb versió de PHP 5.2. Per tant recomanem no sols que actualitzeu les vostres versions de PHP, sinó que també utilitzeu [PSR-4][psr4].


* [Llegir sobre Namespaces][namespaces]
* [Llegir sobre PSR-0][psr0]
* [Llegir sobre PSR-4][psr4]


[namespaces]: http://php.net/language.namespaces
[psr0]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md
[psr4]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-4-autoloader.md
