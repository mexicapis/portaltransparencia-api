API del Portal de Transparencia Mx
================
[![Build Status](https://travis-ci.org/mexicapis/portaltransparencia-api.svg)](https://travis-ci.org/mexicapis/portaltransparencia-api)

Para probar: http://api.mexicapis.org.mx/portaltransparencia/index.php/

### Instituciones y sectores

| Endpoint                                   | Ejemplo                              |
| ------------------------------------------ | ------------------------------------ |
| /instituciones                             | http://api.mexicapis.org.mx/portaltransparencia/index.php/instituciones                       |
| /instituciones?nombre=[NOMBRE INSTITUCION] | http://api.mexicapis.org.mx/portaltransparencia/index.php/instituciones?nombre=casa+de+moneda |
| /sectores                                  | http://api.mexicapis.org.mx/portaltransparencia/index.php/sectores                            |

### Contrataciones

| Endpoint                                                                           | Ejemplo                                                       |
| ---------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| /contrataciones?clave_institucion=[CLAVE INSTITUCION]                              | http://api.mexicapis.org.mx/portaltransparencia/index.php/consulta?tipo=contrataciones&institucion=06305               |
| /contrataciones?clave_institucion=[CLAVE CONTRATO]&clave_contrato=[CLAVE CONTRATO] | http://api.mexicapis.org.mx/portaltransparencia/index.php/consulta?tipo=contrataciones&institucion=06305&contrato=1/12 |

### Remuneraciones

| Endpoint                                                    | Ejemplo                                    |
| ----------------------------------------------------------- | ------------------------------------------ |
| /remuneraciones?clave_institucion=[CLAVE INSTITUCION]       | http://api.mexicapis.org.mx/portaltransparencia/index.php/contrataciones?clave_institucion=06305    |
| /remuneraciones?clave_institucion=[NOMBRE INSTITUCION]      | http://api.mexicapis.org.mx/portaltransparencia/index.php/contrataciones?nombre_institucion=hacienda |

### Deployea tu copia

En Ubuntu por ejemplo:

1. Instalar cURL para PHP 
``` sudo apt-get install curl libcurl3 libcurl3-dev php5-curl```
2. Clonar repo
```git clone https://github.com/mexicapis/portaltransparencia-api.git ```
3. Instalar composer
``` $ curl -s https://getcomposer.org/installer | php ```
Si no con wget
``` $ wget http://getcomposer.org/composer.phar ```
O con
```php -r "readfile('https://getcomposer.org/installer');" | php ```
4. Instalar dependencias con Composer
```php composer.phar install```
5. Listo para usar en http://localhost/portaltransparencia-api/index.php/portaltransparencia/

### TODO

 - Filtrado
 - Mas info

##### Fuente de la info: http://portaltransparencia.gob.mx/