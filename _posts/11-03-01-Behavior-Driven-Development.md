---
isChild: true
anchor:  behavior_driven_development
---

## Desenvolupament Guiat per Comportament (BDD) {#behavior_driven_development_title}

Hi ha dos tipus diferents de Desenvolupament Guiat per Comportament (BDD): SpecBDD i StroyBDD. SpecBDD es centra en el comportament tècnic del codi, en canvi StoryBDD es centra en la part de negoci o de futurs comportaments o interaccions. PHP té frameworks per ambdós tipus de BDD.

Amb StoryBDD, s'escriuen històries d'usuari -llegibles per humans- que descriuen el comportament de la teva aplicació. Aquestes històries d'usuari poden executar-se com a tests contra la teva aplicació. El framework de PHP per StoryBDD és el [Behat], inspirat pel projecte [Cucumber] provinent de Ruby i implementa el llenguatge Gherkin DSL per descriure el comportament de les funcionalitats.

Amb SpecBDD, s'escriuen especificacions que descriuen com s'hauria de comportar el codi. En comptes de provar una funció o un mètode, es descriu com s'hauria de comportar una funció o mètode. PHP ofereix el framework [PHPSpec] per a aquest propòsit. Aquest framework està inspirat per [RSpec project][Rspec] de Ruby.


### Enllaços BDD

* [Behat], el framework StoryBDD per a PHP, inspirat pel projecte [Cucumber] de Ruby;
* [PHPSpec], el framework SpecBDD per a PHP, inspirat pel projecte [RSpec] de Ruby;
* [Codeception] és un framework complet de test que fa ús de principis BDD.

[Behat]: http://behat.org/
[Cucumber]: http://cukes.info/
[PHPSpec]: http://www.phpspec.net/
[RSpec]: http://rspec.info/
[Codeception]: http://codeception.com/
