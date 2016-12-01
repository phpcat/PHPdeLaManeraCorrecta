---
title: Hashing de Contrasenyes
isChild: true
anchor:  password_hashing
---

## Hashing de Contrasenyes {#password_hashing_title}

Tard o d'hora tothom acaba creant aplicacions PHP que depenen de credencials d'usuari. Els noms d'usuari i les contrasenyes són desades a una base de dades per tal de ser emprades més tard en el procés d'autenticació de l'usuari que es *logineja*. És important d'aplicar tècniques de [_hash_][3] a les contrasenyes abans no les desem. 

El Hashing de contrasenyes és un procés de xifrat irreversible, d'una sola direcció, aplicada a les contrasenyes dels usuaris. Això produexi una cadena de llargaria fixa que és molt difícil de transformar en la cadena original.

Això significa que podeu comparar un *hash* contra un altre *hash* per tal de determinar si ambdos provenen de la mateixa cadena original.

Si les contrasenyes no són *hashejades* i la vostra base de dades és accedida per terceres persones no autoritzades, tots els comptes d'usuari estaran compromesos. Alguns usuaris empren (desafortunadament) la mateixa contrasenya en d'altres serveis. És per això que és molt important ser molt curos amb la seguretat de les nostres aplicacions.


**Hashing de contrasenyes amb `password_hash`**

La comanda `password_hash()` va ser introduida a la versió 5.5 de PHP. Actualment està emprant BCrypt, el més fort algoritme de *hash* actualment suportat per PHP. Més endavant serà actualitzat per suportar més algoritmes així es necessitin. La biblioteca `password_compat` fou creada per oferir post-compatibilitat per a les versión >= 5.3.7 de PHP.

A l'exemple *hasejarem* una cadena i llavors comprovarem el *hash* resultant contra una nova cadena. Com que les dues cadenes d'origen són diferents ('secret-password' vs. 'bad-password') el procés de login fallarà.

{% highlight php %}
<?php
require 'password.php';

$passwordHash = password_hash('secret-password', PASSWORD_DEFAULT);

if (password_verify('bad-password', $passwordHash)) {
    // Correct Password
} else {
    // Wrong password
}
{% endhighlight %}  

s'encarrega del "salt" de la contrasenya per tu. El "salt" s'emmagatzema durant el transcurs de l'algoritme i té el cost com a part del "hash". 'password_verify()' extreu aquest per determinar com s'ha de comprovar la contrasenya, llavors no necessites separar el camp de la base de dades per emmagatzemar els "salts" 

* [Per saber més sobre `password_hash()`] [1] (en anglès)
* [`password_compat` per PHP >= 5.3.7 && < 5.5] [2] (en anglès)
* [Learn about hashing in regards to cryptography] [3] (en anglès)
* [PHP `password_hash()` RFC] [4] (en anglès)


[1]: http://php.net/function.password-hash
[2]: https://github.com/ircmaxell/password_compat
[3]: http://en.wikipedia.org/wiki/Cryptographic_hash_function
[4]: https://wiki.php.net/rfc/password_hash
[5]: https://en.wikipedia.org/wiki/Salt_(cryptography)
