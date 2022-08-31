# bsale-test


## Comandos de ejecución
En caso de no tener docker compose instalado dejo un enlace de la documentación oficial [aquí](https://docs.docker.com/compose/install/).

Lo primero es clonar el repositorio y dirigirnos a la carpeta de bsale-test, finalmente cargar los comandos de ejecución.
```console
git clone https://github.com/OscarVargas97/BesTestEver.git
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
A la hora de pasar de un entorno a otro, si bien los archivos docker están configurados para utilizar distintas imágenes y containers dependiendo de los entornos, siempre se puede prevenir limpiando gracias al comando mostrado a continuación: 
```console
pdownall
```
Tambien es posible realizar el building de las imágenes y contenedores gracias al comando:
```console
#para development
pbuild dev
#para test
pbuild test
#para producción
pbuild
```

Una vez iniciado el comando en producción es necesario dirigirse a la siguiente ruta para acceder al cliente:
[http://localhost:3000](http://localhost:3000)

En caso de ingresar al modo de development se levanta un contenedor con phpmyadmin, ademas de exponerse los puertos de la api, teniendo acceso a estos utilizando los siguientes enlaces:

- phpmyadmin: [http://localhost:8081](http://localhost:8081)
- api: [http://localhost:4000](http://localhost:4000)
## Enunciado


Para leer el enunciado completo, te invito a dar click en el siguiente enlace: [Test.md](./docs/Test.md)

## Docs
Se puede acceder a la documentación de la aplicación atravesé del siguiente enlace:
