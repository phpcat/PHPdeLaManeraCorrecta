---
isChild: true
title: Paradigmes de programació
anchor:  programming_paradigms
---

## Paradigmes de programació {#programming_paradigms_title}

PHP és un llenguatge de programació flexible i dinàmic que permet aplicar una varietat de tècniques de programació. Ha evolucionat de forma molt positiva amb els anys adaptant-se a la programació orientada a objectes amb la versió de PHP 5.0 (2004), funcions anònimes i els namespaces amb la versió de PHP 5.3 (2009) o finalment amb els traits a la versió 5.4 (2012).

### Programació Orientada a Objectes

PHP té un conjunt molt complet d'aspectes que faciliten la programació orientada a objectes com ara: classes, classes abstractes, interfícies, herència, constructors, clonació, excepcions i d'altres.

* [Llegir sobre Object-oriented PHP][oop]
* [Llegir sobre Traits][traits]

### Programació funcional

PHP té la capacitat de declarar funcions de primera classe, és a dir, una funció pot ser assignada a una variable. Les funcions definides per l'usuari, així com les funcions internes (incloses), tenen l'habilitat de ser referenciades per una variable i invocades dinàmicament. Les funcions poden ser passades com a arguments a altres funcions (un aspecte anomenat _funcions d'ordre superior_) i funcions poden retornar altres funcions.

La recursivitat és un aspecte que li permet a una funció a cridar-se a si mateixa. El llenguatge PHP habilita aquest tipus d'algorismes, no obstant això, la majoria del codi PHP s'enfoca en iteració.

Les funcions anònimes (amb suport per closures) estan presents en PHP des de la versió 5.3 (2009).

A la versió de PHP 5.4 es va afegir l'habilitat per vincular _closure_ a l'àmbit d'un objecte i també es va millorar el suport de funcions de tipus _callable_ perquè puguin intercanviar-se amb funcions anònimes en gairebé tots els casos.

* Seguiu llegint [Functional Programming in PHP](/pages/Functional-Programming.html)
* [Llegir sobre Anonymous Functions][anonymous-functions]
* [Llegir sobre the Closure class][closure-class]
* [Més detellas a the Closures RFC][closures-rfc]
* [Llegir sobre Callables][callables]
* [Llegir sobre dynamically invoking functions with `call_user_func_array()`][call-user-func-array]

### Meta Programació

PHP suporta diverses maneres de meta programació per mitjà de mecanismes com l'API de Reflexió i els Mètodes Màgics com ara: `__get()`, `__set()`, `__clone()`, `__toString()`, `__invoke()`, etc.
Amb aquests mètodes podreu connectar-vos amb el funcionament de la classe. Sovint, desenvolupadors amb Ruby diuen que a PHP li falta la funció de `method_missing`, no obstant això, els aspectes d'aquesta funció estan disponibles amb `__call()` and `__callStatic()`.

* [Llegir sobre Magic Methods][magic-methods]
* [Llegir sobre Reflection][reflection]
* [Llegir sobre Overloading][overloading]


[oop]: http://php.net/language.oop5
[traits]: http://php.net/language.oop5.traits
[anonymous-functions]: http://php.net/functions.anonymous
[closure-class]: http://php.net/class.closure
[closures-rfc]: https://wiki.php.net/rfc/closures
[callables]: http://php.net/language.types.callable
[call-user-func-array]: http://php.net/function.call-user-func-array
[magic-methods]: http://php.net/language.oop5.magic
[reflection]: http://php.net/intro.reflection
[overloading]: http://php.net/language.oop5.overloading

