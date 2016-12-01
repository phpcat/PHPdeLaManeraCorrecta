---
title: Guia d'estil del codi
anchor: code_style_guide
---

# Guia d'estil del codi {#code_style_guide_title}

La comunitat de PHP és gran i diversa, composta per una infinitat de biblioteques (libraries), marcs de treball (frameworks), i components. És habitual pels desenvolupadors de PHP el fet d'escollir molts d'aquests i combinar-los en un sol projecte.

El [Framework Interop Group][fig] ha proposat i aprovat una sèrie de recomanacions d'estil. No totes elles relacionades amb l'estil de codi, però les que ho són: [PSR-0][psr0], [PSR-1][psr1], [PSR-2][psr2] i [PSR-4][psr4]. Aquestes recomanacions són merament un conjunt de regles que a alguns projectes com Drupal, Zend, Symfony, CakePHP, phpBB, AWS SDK,
FuelPHP, Lithium, etc comencen a adoptar. Podeu utilitzar-les pels vostres projectes o continuar amb les vostres propies guies d'estil de codi.

Per això és important que el codi PHP s'adhereixi (el més a prop possible) a un estil de codi comú perquè es faciliti el treball dels desenvolupadors en combinar una varietat de llibreries per als seus projectes.

Idealment hauríeu d'escriure codi PHP seguint un estàndard reconegut. Podria ser una combinació dels estàndards PSR's o algun dels estàndards creats per PEAR o Zend. Seguint aquests estàndards aconseguirem que altres desenvolupadors puguin de manera senzilla llegir el teu codi i aplicacions que implementin components, ja que tindran consistència encara que implementin codi de tercers.

* [Llegir sobre PSR-0][psr0]
* [Llegir sobre PSR-1][psr1]
* [Llegir sobre PSR-2][psr2]
* [Llegir sobre PSR-4][psr4]
* [Llegir sobre PEAR Coding Standards][pear-cs]
* [Llegir sobre Symfony Coding Standards][symfony-cs]

Podeu utilitzar [PHP_CodeSniffer][phpcs] per comprovar si el vostre codi segueix alguna d'aquestes recomanacions i també podeu fer servir connectors (plugins) per tenir editors com [Sublime Text 2][st-cs] llest per detectar-los.

També podeu utilitzar una d'aquestes dues eines per arreglar de manera automàtica l'estil del codi. La primera és [PHP Coding Standards Fixer][phpcsfixer], la qual està molt provada. L'altre és [php.tools][phptools], que s'ha fet molt popular pels usuaris de [sublime-phpfmt][sublime-phpfmt]. 

Podeu executar phpcs manualment des de la vostra consola:

    phpcs -sw --standard=PSR2 file.php

Us mostrarà els errors i les descripcions de com arreglar-los.
Seria de molt bona ajuda pels vostres projectes si ho teniu configurat per executar-se des de un git hook.
D'aquesta manera no permetríem que entrés codi al repositori que violés els estàndards que hem definit pel projecte..

Els símbols i infraestructures de codi hauran de fer-se amb anglès. Els comentaris podran ser escrits amb altres idiomes.


[fig]: http://www.php-fig.org/
[psr0]: http://www.php-fig.org/psr/psr-0/
[psr1]: http://www.php-fig.org/psr/psr-1/
[psr2]: http://www.php-fig.org/psr/psr-2/
[psr4]: http://www.php-fig.org/psr/psr-4/
[pear-cs]: http://pear.php.net/manual/en/standards.php
[symfony-cs]: http://symfony.com/doc/current/contributing/code/standards.html
[phpcs]: http://pear.php.net/package/PHP_CodeSniffer/
[phpcbf]: https://github.com/squizlabs/PHP_CodeSniffer/wiki/Fixing-Errors-Automatically
[st-cs]: https://github.com/benmatselby/sublime-phpcs
[phpcsfixer]: http://cs.sensiolabs.org/
