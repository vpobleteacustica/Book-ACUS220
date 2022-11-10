# Uso del comando commit:

* Hay dos opciones para hacer los commits :

    * Archivo por archivo
    * Todos de una vez

* Por ahora, veamos archivo por archivo:

* En terminal ejecuta: git commit tutorial_1.py -m "Hello world function added" 

**(NOTA: después del comando "-m", usar comillas para el mensaje)**.

<img src="../figures/commit_1.png" alt="fishy" class="bg-primary" width="550px" align="center"/>

<br/><br/>

* El comando "-m" es para ingresar un mensaje, que describirá qué es lo que se hizo en ese commit

* En nuestro ejemplo, en tutorial_1.py hicimos una función llamada Hello world

* La palabra added es importante de colocar porque te dice que se agregó una función.

* Otros verbos típicos en mensajes de commit son: removed; fixed; etc

* Si observas Source Control en VSC y recuerdas que había una acción que devuelve el archivo desde el <span style="color: blue; font-family: Babas; font-size: 1.12em;">add</span>, en VSC se puede hacer simplemente usando el signo "-" (menos) que aparece.

* Y el git add se puede hacer simplemente con el signo "+"

* Para hacer un commit en VSC, basta agregar un mensaje en la zona de <span style="color: blue; font-family: Babas; font-size: 1.12em;">message</span>

* Describimos en message lo que hicimos en tutorial_2.py: Good bye world function added

<img src="../figures/message.png" alt="fishy" class="bg-primary" width="750px" align="center"/>

<br/><br/>

* Hacemos: control+enter y este commit está listo!

* En resumen, aparentemente en VSC es simple de hacer los committs pero, recomendamos para entender un poquito más, saber cómo se hacen estos committs en terminal. 

* Ahora que los cambios están agregados y committeados, el próximo paso es subirlos al repositorio. Porque todos los cambios están de manera local.






