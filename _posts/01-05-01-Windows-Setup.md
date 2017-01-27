---
title:   Configuració per Windows
isChild: true
anchor:  windows_setup
---

## Configuració per Windows {#windows_setup_title}

Podeu [descarregar els binaris][php-downloads]. Després de l'extracció de PHP, es recomana ajustar la [ruta][windows-
path] a l'arrel de la carpeta de PHP (on es troba php.exe) perquè pugui executar PHP des de qualsevol lloc.

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

En general, executar les teves aplicacions en entorns diferents entre el de desenvolupament i el de producció pot donar lloc a errors causats per la diferència d'aquests dos. Si està desenvolupant en Windows i la implementació és per a Linux (o qualsevol cosa que no sigui Windows), llavors hauria de considerar l'ús d'un [Màquina Virtual] (/ # virtualization_title).

Chris Tankersley té un bloc molt útil on explica les seves eines per [el desenvolupament de PHP sobre Windows] [windows-tools].

[easyphp]: http://www.easyphp.org/
[phpmanager]: http://phpmanager.codeplex.com/
[openserver]: http://open-server.ru/
[wamp]: http://www.wampserver.com/en/
[php-downloads]: http://windows.php.net/download/
[php-iis]: http://php.iis.net/
[windows-path]: http://www.windows-commandline.com/set-path-command-line/
[windows-tools]: http://ctankersley.com/2016/11/13/developing-on-windows-2016/
[wpi]: https://www.microsoft.com/web/downloads/platform.aspx
[xampp]: http://www.apachefriends.org/en/xampp.html
