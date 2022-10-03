# Comenzando con ACUS220

## ¿Por qué es importante aprender Python en acústica?
+ `Python` ha surgido en las últimas dos décadas como una herramienta de primera clase para tareas de `computación científica`.

+ Esto ha incluido la posibilidad de analizar y explorar grandes conjuntos de datos (incluiodo los datos de origen acústico). 

+ Lo anterior puede haber resultado toda una sorpresa para los primeros defensores del lenguaje `Python`. Porque el lenguaje en sí mismo no fue diseñado específicamente para el análisis de datos o la computación científica en mente.

## ¿Cuál es la utilidad de Python?
+ La utilidad de Python para el campo de la acústica proviene principalmente del gran y activo `ecosistema` de paquetes de terceros: `Numpy` para la manipulación de datos homogéneos basados ​​en matrices; `Pandas`  para la manipulación de datos heterogéneos y etiquetados; `SciPy` para tareas comunes de computación científica; `Matplotlib` para visualización de calidad de publicación; `IPython/Jupyter` que proporcionan un terminal mejorado y un entorno para interacción de cuadernillo que es muy útil para el análisis exploratorio, visualización, así como también, para la creación de documentos interactivos y ejecutables. Por ejemplo, este libro de curso está compuesto enteramente de cuadernillos Jupyter; y `Scikit-Learn` para aprendizaje de máquinas y muchas herramientas más que se irán mencionando durante el curso.

## Datos en acústica
+ En acústica usamos una gran variedad de datos los que nos permiten la posibilidad de explorarlos científicamente y aplicar la propia perspectiva de la ingeniería acústica. 
+ Hay una amplia variedad diferente de campos que están relacionados: señales de audio provenientes por ejemplo de procesos de la voz, de origen médico, vibraciones sísmicas, contextos diversos en ecoacústica y biodiversidad, para la interpretación de vocalizaciones de los animales (aves, anfibios), en la localización de fuentes sonoras y en el análisis de imágenes en diferentes escenas acústicas, en espacios interiores, espacios urbanas y rurales. Entre otros $\ldots$

+ En todos estos campos, el análisis de datos se ve complicado por una serie de desafíos, que incluyen ruido que podría aparecer en los datos, el escaso número de mediciones o ejemplos, la reverberación o bien, el manejo de grandes volúmenes de datos. 

+ En muchos casos, se podrían revisar manualmente hasta una cierta cantidad datos acústicos, lo que demandará sin duda un esfuerzo humano.

+ Pero este esfuerzo se hace mayor y se vuelve rápidamente una limitante, cuando aumenta el tamaño de los conjuntos de datos. 

+ Además, pueden existir ciertos `patrones característicos` en los datos que no son fácilmente reconocidos por una revisión humana y que sería de interés poderlos descubrir para analizar.

## Distribución Anaconda y entorno virtual.
+ ¿Por qué necesitamos configurar un entorno virtual?
+ Muchas de las `aplicaciones` de Python requieren `paquetes` y `módulos` que no son parte de la `librería` estándar. 
+ Además, cualquiera aplicación necesitará una `versión` específica de una `librería`.
+ Qué significa ésto? Que podría ocurrir que no sea posible que una instalación de Python cumpla con los todos los requisitos de una aplicación. Por ejemplo, si la aplicación `acus_1` necesita la versión 1.0 de un módulo en particular, pero la aplicación `acus_2` necesita la versión 2.0, entonces los requisitos están en `conflicto de versiones` y la instalación de la versión 1.0, ó 2.0, dejará una aplicación `incapaz` de ejecutarse.
+ La solución para este problema de `conflicto de versiones` es crear un `entorno virtual`, esto es, se trata de un árbol de directorios, autocontenido que contenga una instalación de Python para una versión específica.
+ Distintas `aplicaciones` pueden utilizar diferentes entornos virtuales. Por ejemplo, para solucionar el conflicto anterior de requisitos, la aplicación `acus_1` puede tener su propio entorno virtual con la versión 1.0 instalada. Mientras que, la aplicación `acus_2` tiene otro entorno virtual con la versión 2.0 instalada. Además, en el caso hipotético que la aplicación `acus_2` pudiera requerir que una `librería` se actualice a la versión 3.0, `esto no afectará` el entorno de la aplicación `acus_1`.
+ Anaconda ofrece la forma más fácil de usar Python en diversas aplicaciones, por ejemplo, en minería de datos, aprendizaje de máquinas, en una sola máquina. Podemos comenzar a trabajar con muchos paquetes y librerías de código abierto: Ver [Anaconda](https://www.anaconda.com/), y para apoyar estos conceptos ver [Administración de ambientes](https://www.anaconda.com/products/distribution).

## Manejador de paquetes Conda por medio de la instalación de Miniconda.
+ `Conda` es un sistema de gestión de entornos y paquetes de código abierto que se ejecuta en Windows, macOS y Linux. 
+ Conda instala, ejecuta y actualiza rápidamente los paquetes y sus dependencias. 
+ También crea, guarda, carga y cambia fácilmente entre entornos en nuestro computador local. Fue creado para programas de Python, pero puede empaquetar y distribuir software para cualquier idioma.
+ `Miniconda` es un instalador mínimo gratuito para `conda`. Es una pequeña versión de arranque de Anaconda que incluye sólo conda, Python, los paquetes de los que dependen y una pequeña cantidad de otros paquetes útiles, incluidos pip, zlib y algunos otros. 
+ Utilicemos [Miniconda](https://docs.conda.io/en/latest/miniconda.html)

## Creando un entorno virtual e instalando paquetes y librerías
+ Los `entornos` son uno de los conceptos más útiles en conda. Son instalaciones autónomas, es decir, `todo lo que está dentro de un entorno sólo depende de las cosas que están dentro de ese entorno.`

+ El `entorno base` es creado cuando uno instala `Miniconda` o `Anaconda`. 
+ Y contiene: `conda` y los paquetes necesarios para operaciones `básicas`.

::::{important}
:::{note}
Un error típico es instalar paquetes en el entorno `base`. **NO HAGAS ESO**. Si lo haces, podrías crear conflictos con otros entornos que pudieras crear. 
:::
::::

+ Para crear un entorno nuevo:
```
conda create --name <nombre_de_mi_entorno>
```
+ O bien:
```
conda create -n <nombre_de_mi_entorno>
```

```{admonition} Nota:
Reemplazar **<nombre_de_mi_entorno>** con el nombre que le quieres dar a tu entorno.
```

+ Por ejemplo, crear el entorno virtual llamado `acus220`:
```
conda create -n acus220
```

+ Puedes activar un entorno usando:
```
conda activate <nombre_de_mi_entorno>
```

+ Para desactivar un entorno, escribe:
```
conda deactivate
```

+ Paquetes pueden ser instalados usando el comando:

```
conda install [el nombre de un paquete]
```

`````{admonition} Nota:
:class: tip
Reemplazar **[el nombre de un paquete]** por el nombre del paquete que necesitas!
`````

+ Para ver una lista de todos tus entornos, en tu terminal, ejecuta:
```
conda env list
```

+ Si tu entorno está activado y quieres ver una lista de todos los paquetes que tienes instalados en tu entorno específico, en tu terminal, ejecuta:
```
conda list
```

+ Para eliminar un entorno, en tu terminal, ejecuta:
```
conda remove --name <nombre_de_mi_entorno> --all
```
+ O bien, 
```
conda env remove --name <nombre_de_mi_entorno>
```

### Paquetes IPython y Jupyter
+ Estos paquetes nos proporcionan el entorno computacional en el cual trabajan con Python muchos usuarios científicos de datos.
+ `IPython` (abreviación de **Interactive Python**) fue creado en 2001 por [Fernando Pérez](https://bids.berkeley.edu/people/fernando-p%C3%A9rez). Se puede pensar que `IPython` es un panel de control de Python interactivo.     
+ `Jupyter` nos ofrecen una base interactiva de entornos informáticos, en donde la computación científica, la ciencia y análisis de datos (`audio, imágenes, o textos`), se pueden desarrollar utilizando una amplia gama de lenguajes de programación. 

### Jupyter Notebook
+ Es una aplicación basada en web, que nos permite crear documentos donde podemos combinar código en vivo, con texto narrativo, ecuaciones en $\LaTeX$, videos y explorar y visualizar datos. 

:::{note}
[Documentación](https://github.com/jupyter/notebook)
[Repo](https://github.com/jupyter/notebook)
:::

### Kernels (lenguajes de programación) y ipykernel
+ En Jupyter, los `kernels` representan procesos específicos de lenguajes de programación que se ejecuta, de forma independiente y que interactúan con las aplicaciones de `Jupyter` y sus interfaces de usuario.

+ El equipo de `Jupyter` mantiene el proyecto [`IPython`](https://github.com/ipython/ipython) el que se asigna como kernel predeterminado (como [`ipykernel`](https://docs.jupyter.org/en/latest/projects/kernels.html#term-ipykernel)) en varios clientes de Jupyter. Sin embargo, en el `cuadernillo` es posible usar diferentes lenguajes de programación además de `Python` [lista disponible](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels).

+ Nosotros podemos crear múltiples `kernels` de `IPython` para distintos entornos virtuales que vayamos creando (nos referimos a entornos `conda`). Para realizar esto, se debe especificar un nombre único del kernel.

+ Nos debemos asegurar primero que hemos instalados en nuestro entorno virtual el paquete `ipykernel`.
+ `ipykernel` se puede considerar como lo que envuelve a IPython y que nos permitirá usar IPython en un kernel específico.

+ Para instalar `ipykernel` en nuestro entorno, ejecutar en el terminal:
```
python -m ipykernel install --user --name=<nombre_del_kernel>
```

## Canales de Conda
+ Un canal de Conda es una ubicación donde se alojan `paquetes de Conda` de forma remota.
+ Un canal es un equivalente a un `repositorio`. 
+ Los paquetes de Conda se descargan desde direcciones URL.
+ El comando `conda` busca un conjunto de canales. 
+ Los canales predeterminados (o simplemente, canales `por defecto`) son los que se van a utilizar si no especificamos ningún parámetro $--channel$ durante la instalación.
+ Por ejemplo, un comando como el siguiente, buscará el paquete `scipy` en el canal `conda-forge` así como también en los canales por defecto:
```
conda install scipy --channel conda-forge
```
+ Diferentes canales pueden tener el mismo paquete, por lo que conda debe manejar estas colisiones de canales.

## Buscando paquetes
+ ¿Cómo se busca un paquete? Simplemente, ejecutar en el terminal
```
conda search
```
+ Para ver si un paquete específico, como SciPy, está disponible en el entorno, ejecutar en el terminal:
```
conda search scipy
```
+ Conda tiene una lista de canales. Consultemos cuáles canales existen en el entorno:
```
conda config --show channels
```
+ El canal [`conda-forge`](https://conda-forge.org/) es una organización de GitHub que contiene repositorios con recetas de conda, repetibles en Windows, Linux y OSX.
+ Para instalar conda-forge en un entorno conda existente, ejecutar en el terminal:
```
conda config --append channels conda-forge
```