# DESAFÍO

```
Objetivo
```
Determinarsielcandidatoestáencondicionesdeinteractuarconunabasededatos
a través de una aplicación web, implementando cliente y servidor.
Esteejercicio,notieneningúnfincomercialniestratégico,sóloqueremosmedirtus
habilidades...

```
Ejercicio
```
Construirunatiendaonlinequedespliegueproductosagrupadosporlacategoríaa
la que pertenecen, generando por separado backend (API REST) y frontend
(aplicaciónquelaconsuma)yutilizandolabasededatosquesedisponibilizapara
su desarrollo.

Además,hayqueagregarunbuscador,elcual **tienequeestarimplementadoanivel
deservidor** ,medianteuna ApiRest **cuyolenguajeyframeworkpuedeserdelibre
elección.** Es decir, los datos de productos deben llegarfiltrados al cliente.

Opcionalmente, puedes implementar filtros por atributo, ordenar productos y
paginación.

La aplicación de cliente tiene que estar desarrollada con **vanilla javascript
(javascript puro),sin ningún framework,** sipuedes usar libreríasocomponentes
específicos, tales como; boopstrap, material, Jquery, entre otros.

Finalmente, disponibilizarlaaplicacióny elrepositorioconelcódigoenunhosting
comoamododeejemplo,puedeser;Heroku,Netlity uotro.Tambiénpuedeslevantar
el sitio en una cuenta AWS.


### Acceso a la base de datos de uso obligatorio

Base de datos

```
● Motor: MySQL
● Host: mdb-test.c 6 vunyturrl 6 .us-west- 1 .rds.amazonaws.com
● Usuario: bsale_test
● Contraseña: bsale_test
● Nombre db: bsale_test
```
**Tip para la conexión** : El servidor está configurado para que todas aquellas
conexiones inactivas por más de 5 segundos sean abortadas, por lo que te
recomendamos utilizar alguna estrategia de “keep alive”

Tablas

```
product
id Identificador único del producto (int)
name Nombre del producto (varchar)
url_image URL de la imagen asociada al producto (varchar)
price Precio de venta del producto (float)
discount Porcentaje de descuento del producto (int)
category Identificador de la categoría (int)
```
```
category
id Identificador único de la categoría (int)
name Nombre de la categoría (varchar)
```

**Ejemplos de las imágenes que se encuentran en la BD**


#### CONOCE LA PAUTA DE EVALUACIÓN

```
Categoría Acción que evaluaremos Ponderación
Requisito obligatorio Se debe utilizar control de versiones Obligatorio
Requisito obligatorio La aplicación debe tener deploy Obligatorio
Programación El código debe ser limpio, ordenado y
seguir buenas prácticas
40 %
Programación La aplicación debe ser eficiente y controlar
errores
Documentación Documentar la aplicación* 20 %
Funcionalidad Que se entregue buena usabilidad y
experiencia al usuario.^40 %
TOTAL 100 %
```
```
● ¿Quéesdocumentar? implicaexplicarejercicio,Apirest,FrontendyReadmeen
el repositorio de ambos proyectos (back y front).
```
Ejemplo de documentación:
https://apichile.bsalelab.com/lista-de-endpoints/productos-y-servicios/stocks

## Mucho éxito!!!


