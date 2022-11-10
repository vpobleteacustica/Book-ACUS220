# Uso de comando git pull

* Actualiza los cambios hechos en GitHub en tu repositorio local

* En la terminal ejecuta: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git pull</span>

* Observas con: ls que ya están en local los archivos tutorial_1.py  tutorial_2.py

* Con eso ya estás actualizado con lo que hay en la rama main del repositorio de GitHub

* Si haces git status, te darás cuenta en tu repositorio local que no hay ninguna rama a excepción de la rama main, porque ya se eliminó la otra rama

* Vamos a crear ahora otra rama que llamaremos feature_2

* Ejecuta los comandos: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git checkout -b feature_2</span>

* Si ejecutas git status te dirá que te cambiaste a la rama feature_2 con el mismo código de main

* Vamos a VSC y vamos a hacer unos cambios a los archivos

* Hacer un cambio al archivo README

    * <span style="color: blue; font-family: Babas; font-size: 1.12em;">## Run</span>
    * <span style="color: blue; font-family: Babas; font-size: 1.12em;">```</span>
    * <span style="color: blue; font-family: Babas; font-size: 1.12em;">python tutorial_1.py</span>
    <span style="color: blue; font-family: Babas; font-size: 1.12em;">python tutorial_2.py</span>
    * <span style="color: blue; font-family: Babas; font-size: 1.12em;">```</span>
* Cambiamos en los archivos tutorial_1.py y tutorial_2.py:

```console
def hello_world(name):
    print(f'Hello world {name}')
name = 'Víctor'
hello_world(name) # aquí vamos a llamar a nuestra función
```

```console
def good_bye_world(name):
    print(f'Good bye world {name}')
name = 'Víctor'
good_bye_world(name) # aquí vamos a llamar a nuestra función
```
* Lo genial es que VSC te muestra los archivos a los que le has hecho cambios en color amarillo

* Para ver los cambios que has hecho en VSC, te vas a Source Control

* Puedes ver los archivos que se han modificado, línea a línea

* Vamos a la terminal y ejecutamos git status para ver el estado de la rama feature_2

* Nos muestra los archivos que se han modificado

* Pero que todavía no han sido movidos al area <span style="color: blue; font-family: Babas; font-size: 1.12em;">staging</span>, no han sido agregados

* Para agregarlos, ejecuta: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git add .</span>

* Ejecuta: git status

* Podrás que ver que todos los cambios en los archivos ahora están en el área de stage

* En la terminal, has un committ del archivo README

* Para eso ejecuta: git commit README.md -m 'Run instructions added'

* Ejecuta: git status y verás que ya no está en el área de stage

* Para committear todos los archivos que quedan, ejecuta git commit -m 'Hello and bye world functions updated'

* Ejecuta: git status y verás que ya no hay ningún archivo en el área de staging

* Esto quiere decir que está listo para hacer push

* Otra vez te va a decir que: git push --set-upstream origin feature_2

* Recuerda que te dice que feature_2 no ha sido creada en GitHub y que solo es una rama local

* Para crearla en GitHub ejecutamos este comando: git push --set-upstream origin feature_2

* Te pedirá tus credenciales

* Hacemos git status

* Nos vamos a cambiar ahora a la rama main (local!)

* Ejecutamos: git checkout main

* Aquí en main no hay nada actualizado porque los cambios los hicimos en la otra rama

* Nos vamos a GitHub y actualizamos

* Nos dice que: feature_2 had recent pushes 4 minutes ago

* También vemos que hay otra rama: feature_2

* Observas los cambios

* Pero estos cambios aún no están en main

* Para hacer estos vamos a Compare & pull request

* Observa: los cambios va a ser actualizados de la rama feature_2 a main

* Ejecuta: Merge and pull request 

* Ejecuta: Confirm merge

* Borra la rama feature_2 y te vas al código

* te podrás dar cuenta que no hay ninguna otra rama, solamente main

* Y observas que los cambios están actualizados en main

* Revisa los committs para que veas los cambios que se hicieron

* Y puedes ver todos los committs que se han hecho!












