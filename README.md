# Pattern Recognition using Labview

Búsqueda de patrones por medio de una cámara web usando Labview el cual busca un patrón determinado dentro de un entorno. El presente proyecto se realizó con la finalidad de investigar la visión artificial para determinar en qué sectores podremos utilizar nuestro proyecto a futuro.
Labview es una herramienta gráfica de test, control y diseño mediante la programación. El lenguaje que usa se llama lenguaje G.
El método usado para nuestra búsqueda de patrones es por medio de vectorización el cual consiste representar las imágenes como si fueran vectores y así facilitar nuestra búsqueda.
Las limitantes de nuestro proyecto es que solo abarca imágenes o video para el reconocimiento de patrones.

###Modelo o patrón.
Un modelo es una descripción global del conjunto de datos. Toma una perspectiva completa y total. En contraste un patrón es una propiedad local de los datos, tal vez sólo la tienen ciertas instancias o atributos.
Un patrón es la descripción de la región segmentada
El patrón se forma, usualmente, a partir de una combinación de propiedades (x1, x2, ..., xn), la cual define el espacio de propiedades en la que actúa el clasificador.
El clasificador no reconoce objetos, reconoce el patrón que define al objeto y si se conoce el patrón que define a un objeto cierto, asigna la región al objeto.

###Búsqueda de patrones
Un sistema de reconocimiento de patrones completo consiste en:
•	Un sensor que recoge las observaciones a clasificar.
•	Un sistema de extracción de características transforma la información observada en valores numéricos o simbólicos.
•	Un sistema de clasificación o descripción que, basado en las características extraídas, clasifica la medición.
Por ejemplo se pueden clasificar imágenes digitales de letras en las clases «A» a «Z» dependiente de sus píxeles o se pueden clasificar huellas dactilares.

Las características de la imagen pueden ser:
	*Topológicas: número de componentes conexas, agujeros,…
	*Geométricas: área, perímetro, curvatura,…
	*Estadísticas: momentos,…
  
Un patrón es un conjunto de características.
Una clase de patrones es un conjunto de patrones “similares”.
El objetivo del reconocimiento de patrones es asignar un patrón a la clase a la que pertenece (lo más automáticamente posible).

Desarrollo
El algoritmo
Un diagrama genérico del algoritmo se presenta en la siguiente figura: ver manual-tecnico.pdf

En el primer bloque están concentradas las inicializaciones de los dispositivos y de los bloques de memoria que se reservarán para los cálculos y procesos del algoritmo. En cualquier lenguaje de programación será necesario este proceso.
El segundo bloque está destinado a comenzar el ciclo ininterrumpido de la búsqueda de la trama que necesariamente debe comenzar con la especificación de la misma, luego esta se tiene que almacenar para las futuras búsquedas.
El siguiente bloque es en donde el algoritmo entra en funcionamiento; en él se busca la trama en cada una de las imágenes y con ello se hacen los cálculos para la ubicación del objeto en el espacio.
El bloque de pregunta fin determina si se debe o no salir del ciclo ininterrumpido.
El bloque de pregunta de nueva búsqueda permite salir del ciclo de búsqueda y regresa al bloque de inserción de la trama para la nueva búsqueda que se supone se tomará como un nuevo objeto.


