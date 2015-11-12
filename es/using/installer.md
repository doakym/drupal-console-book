# Usando el instalador de Drupal Console
Puedes instalar el Drupal Console localmente ejecutando el instalador en el directorio de tu proyecto, el instalador se encargará de descargar los archivos necesarios para ejecutar Drupal Console en tu computador.

## Usando curl:
```
$ curl -LSs http://drupalconsole.com/installer | php
```
## O si no tienes curl:
```
$ php -r "readfile('http://drupalconsole.com/installer');" | php
```

El script instalador sólo comprobará algunas configuraciones en el php.ini, se advierte si están incorrectos, y luego descarga la última versión de console.phar en el directorio actual.


## Ahora puedes ejecutar la consola usando:
```
$ php console.phar generate:module
```

Puedes colocar este archivo donde quieras. Si lo pones en su PATH, puedes accederlo globalmente. En los sistemas unixy puedes incluso hacerlo ejecutable e invocarlo sin php.

### Acceso a la console desde cualquier lugar de tu sistema
```
$ mv console.phar /usr/local/bin/drupal
```

#### Ahora puedes ejecutar console usando:
```
$ drupal generate:module
```

**NOTA:** El nombre `drupal` es sólo un alias, puedes nombrarlo como quieras. 
