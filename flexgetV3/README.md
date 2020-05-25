Para poder realizar la integración con trakt se deben realizar los siguientes pasos:

- Crear una cuenta en trakt.
- Crear una lista para las series
- Crear una lista para las peliculas
- Crear una aplicación para api (Usuario > Settings > your API) //Este usuario se usa para autenticar en la configuración, y no el de la cuenta
- Autorizar flexget para conectarse a trakt:
	- docker exec -it idcontainer sh
	- flexget trakt auth <account> //El resultado de manda a autenticar, con el código que entrega al link https://trakt.tv/activate

Realizados estos pasos, flexget debería poder extraer la información desde trakt.

Para poder utilizar la funcionalidad de descargas, se deben crear cuentas en las siguientes páginas:

- https://www.addic7ed.com/
- https://www.opensubtitles.org/es/index.com

Para utilizar el archivo config.yml, se deben ajustar los valores en el archivo secrets.yml de acuerdo a la configuración utilizada.
