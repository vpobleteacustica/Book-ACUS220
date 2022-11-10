# Uso de git checkout -b <nombre_de_la_nueva_rama>

## Actualiza tu repositorio.

* Queremos ahora hacer una actualización de tu repositorio.

* Como ya sabes, estás en tu rama <span style="color: blue; font-family: Babas; font-size: 1.12em;">main</span>. Porque es la única que hasta ahora existe.

* Vamos a crear una nueva <span style="color: blue; font-family: Babas; font-size: 1.12em;">rama</span>. 

* En ocasiones a esta nueva rama se le llama <span style="color: blue; font-family: Babas; font-size: 1.12em;">rama de producción</span>, porque será la rama que quieres mostrar y que deseas subir a GitHub como la versión funcional de tu proyecto.

* Supongamos que tu proyecto considera realizar algún tipo de proceso de señales, por ejemplo, procesar una señal de audio para extraer <span style="color: blue; font-family: Babas; font-size: 1.12em;">features</span> o características de la señal. 

* Vamos a nombrar a la nueva rama <span style="color: blue; font-family: Babas; font-size: 1.12em;">feature_1</span>. 

* Para esto, ejecuta <span style="color: blue; font-family: Babas; font-size: 1.12em;">git checkout -b</span> y agrega a continuación, el nombre que le quieres dar a tu nueva rama:

```console
kasparov@kasparov-MS-7B58:~/Escritorio/github/uso_git$ git checkout -b feature_1
```

* La idea es que el nombre de la rama sea siempre lo más descriptivo posible de lo que contiene esa rama. 

* Si todo está bien, deberías ver:

<img src="../figures/nueva_rama.png" alt="fishy" class="bg-primary" width="550px" align="center"/>

<br/><br/>

* Ve el estado de tu repositorio: <span style="color: blue; font-family: Babas; font-size: 1.12em;">git status</span>.

* Lo que has hecho al crear una nueva rama, es copiar todo el código que se encuentra en la rama <span style="color: blue; font-family: Babas; font-size: 1.12em;">main</span> y lo has llevado a tu nueva rama que se llama <span style="color: blue; font-family: Babas; font-size: 1.12em;">feature_1</span>. 

* Imagínenselo como que ambas ramas ahora están con el mismo nivel de código, porque todavía no hemos hecho ningún cambio.

* Ahora en tu rama nueva empezarás a trabajar. Vamos a crear archivos y le pondremos algo de código.

## Crea un archivo nuevo de Python.

* Usemos el comando <span style="color: blue; font-family: Babas; font-size: 1.12em;">touch</span>.

* En tu terminal, ejecuta el siguiente comando que te permite crear el archivo nuevo de Python. Nómbralo como: tutorial_1.py:

```console
kasparov@kasparov-MS-7B58:~/Escritorio/github/uso_git$ touch tutorial_1.py
```

* Abre el archivo recién creado usando Visual Studio Code.

* A modo de juego, agrega el siguiente cógido Python:

```
def hello_world(name):
    print(f'Hello world {name}')

hello_world('Víctor') # aquí vamos a llamar a nuestra función
```

* Para probar cómo quedó tu código, ejecuta desde la terminal 

```
python tutorial_1.py
```

* Si todo está bien, deberías ver:

<img src="../figures/hello_world.png" alt="fishy" class="bg-primary" width="550px" align="center"/>

<br/><br/>

* En este ejemplo que ya funciona, vemos que estaríamos listos con nuestro <span style="color: blue; font-family: Babas; font-size: 1.12em;">feature_1</span>.

## Uso de terminal y de Visual Studio Code (VSC).

* Hay dos opciones. La más importante es seguir trabajando en la terminal pero, podemos aprender a trabajar en VSC. 

* Se recomienda manejar ambas opciones.

* En VSC, la función <span style="color: blue; font-family: Babas; font-size: 1.12em;">Source Control</span> está integrada y se conecta a <span style="color: blue; font-family: Babas; font-size: 1.12em;">Git</span>.

* Desde VSC ubica la carpeta que llamamos: <span style="color: blue; font-family: Babas; font-size: 1.12em;">github</span>, y que contiene tu repositorio: <span style="color: blue; font-family: Babas; font-size: 1.12em;">uso_git</span>.

* Abre tu repositorio <span style="color: blue; font-family: Babas; font-size: 1.12em;">uso_git</span>.

* En VSC verás todos los archivos que están en tu repositorio.

* Pero, también a mano izquierda, verás una pestaña que se llama <span style="color: blue; font-family: Babas; font-size: 1.12em;">Source Control</span>.

* <span style="color: blue; font-family: Babas; font-size: 1.12em;">Source Control</span> te muestra todos los cambios que has ido realizando. 

* Debería decir que solamente hemos cambiado <span style="color: blue; font-family: Babas; font-size: 1.12em;">tutorial_1.py</span>.

* Otra cosa importante que observar es que al fondo de VSC nos dice en qué rama nos encontramos, en este caso, <span style="color: blue; font-family: Babas; font-size: 1.12em;">feature_1</span>.