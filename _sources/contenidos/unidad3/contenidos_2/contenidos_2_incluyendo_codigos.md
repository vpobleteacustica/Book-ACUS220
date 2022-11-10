# Seguimiento de los cambios.

* * En tu terminal, crea otro archivo nuevo de Python. Nómbralo como: tutorial_2.py:

```console
kasparov@kasparov-MS-7B58:~/Escritorio/github/uso_git$ touch tutorial_2.py
```
* Abre el archivo recién creado usando Visual Studio Code.

* Como antes, a modo de juego, agrega el siguiente cógido Python:

```
def good_bye_world(name):
    print(f'Good bye world {name}')

good_bye_world('Víctor') # aquí vamos a llamar a nuestra función
```

* Ahora tienes dos archivos nuevos. 

* Si ves Source Control, puedes observar los cambios. Te dice que hay dos archivos nuevos en los que has hecho cambios!

* Pero también en tu terminal puedes ver el estado de tu repositorio y observar los cambios que has hecho.

* Anda a tu terminal y ejecuta los comandos: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git status</span>.

* Te muestra que hay dos archivos que no han sido <span style="color: blue; font-family: Babas; font-size: 1.12em;">trackeados</span>, o en otras palabras, están sin seguimiento.

* Quiere decir que hay dos archivos que no se han agregado y necesitan ser actualizados para poder subir los cambios.


