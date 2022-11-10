# Uso de git add, para agregar los cambios.

* Recuerda que en principio, tenemos iguales la rama <span style="color: blue; font-family: Babas; font-size: 1.12em;">main</span> y la rama <span style="color: blue; font-family: Babas; font-size: 1.12em;">feature_1</span>

* Solamente has editado códigos de manera local

* Ahora, en la rama feature_1, vas a agregar los cambios que has hecho y se actualizará esta rama 

* Lo primero que haremos es usar: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git add</span>

* Existen dos opciones 

* La primera es hacer git add, de cada uno de los archivos que han cambiado: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git add tutorial_1.py tutorial_2.py</span>

* La segunda, es hacer lo mismo pero usando un punto: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git add .</span>

* Recomendamos ir haciendo esto uno por uno

* Agrega uno solo de los archivos: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git add tutorial_1.py</span>

* Y revisa el estado del repositorio: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git status</span>

* Vemos que el que agregamos dice: 

<img src="../figures/confirmados_committed.png" alt="fishy" class="bg-primary" width="550px" align="center"/>

<br/><br/>

* También, el mensaje puede decir: <span style="color: blue; font-family: Babas; font-size: 1.12em;">Changes to be committed</span>

* Esto quiere decir que tienes un solo cambio a confirmar, que si le hacemos <span style="color: blue; font-family: Babas; font-size: 1.12em;">commit</span> estaría listo para ser subido a la rama <span style="color: blue; font-family: Babas; font-size: 1.12em;">feature_1</span>

* En cambio, puedes observar que tutorial_2.py todavía no está trackeado. Todavía no se le puede hacer <span style="color: blue; font-family: Babas; font-size: 1.12em;">commit</span> porque no ha sido <span style="color: blue; font-family: Babas; font-size: 1.12em;">agregado</span> a los archivos trackeados.

