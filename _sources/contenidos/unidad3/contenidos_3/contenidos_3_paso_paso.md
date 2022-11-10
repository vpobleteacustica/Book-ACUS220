# Paso a paso para actualizar: 

* Para actualizar los cambios entonces, primero haces: 1) git add; y en segundo lugar, haces: 2) git commit

<img src="../figures/paso_paso.png" alt="fishy" class="bg-primary" width="550px" align="center"/>

<br/><br/>

* Aún falta un paso más, pero por ahora, veamos estos dos primeros pasos.

* Por otra parte, veamos los comandos: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git restore</span>

* La palabra: <span style="color: blue; font-family: Babas; font-size: 1.12em;">staging</span> se usa para representar el lugar donde están listos los archivos para ser committeados

* Uno puede ejecutar <span style="color: blue; font-family: Babas; font-size: 1.12em;">git restore</span> para sacarlos del stage

* Vamos a hacer solamente para efectos del tutorial <span style="color: blue; font-family: Babas; font-size: 1.12em;">git restore --staged tutorial_1.py</span>

* Esta acción se interpreta como que el archivo tutorial_1.py, lo devolvimos desde el <span style="color: blue; font-family: Babas; font-size: 1.12em;">add</span>

* Ahora observa lo sucedido, puedes hacer: git status

* Puedes ver que el archivo tutorial_1.py, volvió a estar en color rojo.

* Esto significa que si realizaste algún cambio que no querías, entonces lo puedes restaurar.

* Ahora, como ya se entiende, de una sola ejecución agrega los dos archivos: tutorial_1.py junto con tutorial_2.py

* Ejecuta: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git add .</span>

* Y observa lo sucedido, puedes hacer: git status

* Verás que están los dos archivos listos para ser <span style="color: blue; font-family: Babas; font-size: 1.12em;">committeados</span>
