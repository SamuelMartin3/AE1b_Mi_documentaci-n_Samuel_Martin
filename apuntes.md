# Github

Esta es una documentacion basica sobre Github.

Github es un sistema de control de versiones, que nos ayuda a llevar un orden completo de las modificaciones y avances de un trabajo. Sirve para poder trabajar un proyecto en diferentes ordenadores y poder acceder a lo que has hecho anteriormente con muchas más opciones.

En Github podemos hacer muchas cosas pero las más significativas y importantes son las siguientes:

- Podemos hacer que podamos tirar hacia atrás en un trabajo subiendo commits por si ocurre algún problema y no sabemos qué hacer volvemos a como lo teníamos antes.
- Trabaja con ramas para poder editar cosas sin tener que tocar el trabajo principal.
- Se pueden crear clones de los repositorios para poder hacer trabajo simultáneo en diferentes ordenadores y después juntarlo todo.
- Puedes trabajar sin conexión a la red.
- Trabaja con plataformas de desarrollo colaborativo para poder tener los repositorios en la nube.
- Una vez instalado Github tendremos que configurar nuestro nombre de usuario y email con estos comandos en la consola.

git config--global user.name “Tu nombre”
git config--global user.email tugmail@gmail.com
Para crear un repositorio solo tendremos que darle al botón de "Nuevo" en "Crear un nuevo repositorio".

![Imagen1.png](img/Imagen1.png)

Una vez tenemos el repositorio creado tenemos que clonarlo en nuestra máquina local para poder trabajar y después subirlo a Github para hacer las pruebas fuera por si ocurre algo. Primero de todo tendremos que copiar la URL del repositorio.

![Imagen2.png](img/Imagen2.png)

Y después en nuestra consola en la raíz del repositorio tendremos que poner los siguientes comandos

1. -git clone URL del repositorio
2. -git init (para iniciarlo)
3. -git add “archivo” o git add . (para subir el archivo o todo)
4. -git commit-m “nombre del commit” (para saber que hemos subido por si tenemos que ir hacía atrás saber que es lo último que hemos hecho)
5. -git push origin main (para subirlo a la rama principal del repositorio)

Todo esto si ya tenemos el repositorio inicializado por el README si no hemos marcado esta opción tendremos que poner antes de lo anterior estos comandos

1. -git init
2. -git add README.md (para iniciar el repositorio en el local)
3. -git branch-M main (para asociarlo a una rama)-git commit-m "first commit”
4. -git remote add origin https://github.com/TuNombre/Prueba.git. (para asociar el local con el remoto)
5. -git push-u origin main

Y para sincronizarlo tendremos que poner los comandos de diferente forma git init

1. -git remote add origin https://github.com/TuNombre/Prueba.git.
2. -git branch-M main-git add .
3. -git commit-m "first commit"
4. -git push-u origin

Y por último para importar un repositorio ya creado solo tenemos que copiar la URL y a la hora de crear el nuevo repositorio nos dará la opción de importar un repositorio y tendremos que copiar la URL allí.

![Imagen3.png](img/Imagen3.png)

Si queremos utilizar Github Pages tendremos que ir al repositorio y en sus opciones de ajustes tendremos que ir al apartado de Pages y poner la rama principal y la carpeta root cuando hayamos hecho eso nos saldrá la URL del Pages y ya. Es muy importante que tengamos el index.html para que lo reconozca y podamos acceder

![Imagen4.png](img/Imagen4.png)
