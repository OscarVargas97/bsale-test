# bsale-test
Bsale-test consiste en la prueba técnica para postulara a la empresa bsale. En este repositorio se encuentra tanto el back-end como el front-end bien organizados y dockerizados para una rápida implementación. En las siguientes secciones se detallara tanto los pasos para la puesta en marcha de los distintos contextos (dev, prod, test) como la documentación asociada al back-end y al front-end

## Comandos de ejecución
**Opcional**
En caso de no tener docker compose instalado dejo un enlace de la documentación oficial [aquí](https://docs.docker.com/compose/install/).
Se recomienda revisar las ultimas versiones de docker-compose desde el enlace oficial de github que se encuentra justo [aquí](https://github.com/docker/compose/releases).

Tras purgar el repositorio o bien eliminar el script utilizado anteriormente para instalar docker compose, se deben utilizar los siguientes comandos para instalar la version minima recomendable para ejecutar este proyecto:
```console
sudo curl -L "https://github.com/docker/compose/releases/download/2.10.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```
**Opcional terminado**

Lo primero es clonar el repositorio y dirigirnos a la carpeta de bsale-test, finalmente cargar los comandos de ejecución.
```console
git clone https://github.com/OscarVargas97/bsale-test.git
cd bsale-test
source commands.sh
```
Para el caso de lanzar la aplicación a producción se debe ejecutar el siguiente comando: 
```console
pstart
```
Para el caso de utilizar la aplicación en development, lo cual permite carga en caliente de los archivos modificados, se debe utilizar el siguiente comando.
```console
pstart dev
```
A la hora de pasar de un entorno a otro, si bien los dockerfiles y docker-compose están configurados para utilizar distintas imágenes y containers dependiendo de los entornos, siempre se puede prevenir limpiando toda la información asociada con el comando mostrado a continuación: 
```console
pdownall
```
Tambien es posible realizar el building de las imágenes y contenedores gracias al comando:
```console
# para development
pbuild dev
# para test
pbuild test
# para producción
pbuild
```

Una vez iniciado el comando en producción es necesario dirigirse a la siguiente ruta para acceder al cliente:
[http://localhost:3000](http://localhost:3000)

En caso de ingresar al modo de development se levanta un contenedor con phpmyadmin, ademas de exponerse los puertos de la api, teniendo acceso a estos utilizando los siguientes enlaces:

- phpmyadmin: [http://localhost:8081](http://localhost:8081)
- api: [http://localhost:4000](http://localhost:4000)
## Enunciado
### Resumen

Construir una tienda online que despliegue productos agrupados por la categoría a la que pertenecen, generando por separado backend (API REST) y frontend (aplicación que la consuma) y utilizando la base de datos que se disponibiliza para su desarrollo.

Además, hay que agregar un buscador, el cual **tiene que estar implementado a nivel de servidor**, mediante una Api Rest **\_cuyo lenguaje y framework puede ser de libre elección\_**. Es decir, los datos de productos deben llegar filtrados al cliente. Opcionalmente, puedes implementar filtros por atributo, ordenar productos y paginación.

La aplicación de cliente tiene que estar desarrollada con vanilla javascript (javascript puro), sin ningún framework, si puedes usar librerías o componentes específicos, tales como; boopstrap, material, Jquery, entre otros. Finalmente, disponibilizar la aplicación y el repositorio con el código en un hosting como a modo de ejemplo, puede ser; Heroku, Netlity u otro. También puedes levantar el sitio en una cuenta AWS.

Para leer el enunciado completo, te invito a dar click en el siguiente enlace: [Test.md](docs/test.md)

## Docs
Se puede acceder a la documentación de la api a traves del siguiente enlace:
Se puede acceder a la documentación del cliente a traves del siguiente enlace:
