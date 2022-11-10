# Uso de los comandos git push

* Vamos a la terminal y subiremos los cambios.

* Ejecuta los comandos <span style="color: blue; font-family: Babas; font-size: 1.12em;">git push</span>

* Aquí empiezan algunos problemas!

* Te saldrá el siguiente error:
    * fatal: The current branch feature_1 has no upstream branch.
    To push the current branch and set the remote as upstream, use
    git push --set-upstream origin feature_1

    * fatal: La rama actual feature_1 no tiene una rama upstream.
    Para realizar un push de la rama actual y configurar el remoto como upstream, use
    git push --set-upstream origin feature_1

* Nos dice esto porque la rama en la que estamos es local y no se ha subido al repositorio online en GitHub. Si te fijas en GitHub, ahí sólo tienes una sola rama que la rama main.

* Entonces, copia en terminal ese comando que te apareció: git push --set-upstream origin feature_1

* Y ejecútalo!

* Te pedirá tus credenciales

* Y veamos git status

* Te debería decir que todo está actualizado

* Ve ahora a GitHub y actualiza tu página



