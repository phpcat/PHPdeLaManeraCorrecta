---
title:   Configuració per Windows
isChild: true
anchor:  windows_setup
---

## Configuració per Windows {#windows_setup_title}

PHP està disponible en diverses formes per Windows. Podeu [descarregar els binaris][php-downloads] i fins fa poc es
podia utilitzar un instal·lador .msi '. L'instal·lador ja no es manté i es deté en PHP 5.3.0.

Per l'aprenentatge i el desenvolupament local pots utilitzar el servidor enpaquetat amb PHP 5.4+ perquè no necessitaràs
preocupar-te de la configuració del mateix. Si prefereixes un "tot-en-un" que inclou un servidor web amb tota regla i
MySQL, llavors necessites eines com el [Web Platform Installer][wpi], [XAMPP][xampp], [EasyPHP][easyphp] i [WAMP][wamp],
t'ajudarà a aconseguir un entorn de desenvolupament per Windows ràpidament. Dit això, aquestes eines seran una mica
diferents de les de producció així que vés amb compte amb les diferències d'entorn si s'està treballant amb Windows i a
producció es fa servir Linux.

Si necessites un entorn estable de producció amb Windows, pots utilitzar IIS7. Pots utilitzar [phpmanager][phpmanager]
(un plugin GUI per IIS7) per la configuració i administració de PHP de manera senzilla. IIS7 ve amb FastCGI incorporat i
llest per funcionar, només has de configurar PHP com a gestor. Per a suport i recursos addicionals hi ha una [zona
dedicada a iis.net][php-iis] per a PHP.


[php-downloads]: http://windows.php.net
[wpi]: http://www.microsoft.com/web/downloads/platform.aspx
[xampp]: http://www.apachefriends.org/en/xampp.html
[easyphp]: http://www.easyphp.org/
[wamp]: http://www.wampserver.com/en/
[phpmanager]: http://phpmanager.codeplex.com/
[php-iis]: http://php.iis.net/
