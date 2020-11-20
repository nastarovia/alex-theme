# El problema

Cuando comenzamos en el misterioso mundo de la publicación web, lo más común es utilizar un CMS, pongamos por caso Wordpress. Parece una elección razonable: es _open source_, hay miles de plantillas disponibles para ahorrarnos el trabajo de escribir código nosotros mismos, y _plugins_ a punta de pala para añadir todas las funcionalidades imaginables. Sin embargo, no todo es perfecto: cuando llega la hora de hacer algo que nuestra plantilla no tiene previsto, comienzan los problemas. Wordpress es un software estupendo, pero es increíblemente pesado y complejo. Y está escrito en PHP, que es un lenguaje de programación como mínimo opaco. Cuando construimos el primer sitio de la editorial, me debo de haber pasado sus buen par de meses haciendo ajustes: cuando acabé sabía exactamente lo mismo de PHP que al principio (o sea: nada) y tenía la frustrante sensación de que nada de lo que había construido se podía reutilizar en el trabajo de la editorial. Escribir contenido en Wordpress supone hacerlo en su editor y almacenar nuestros contenidos en una base de datos, algo que es práctico al principio, pero que cuando tu sitio web crece (y tu editorial también) supone una cantidad de información duplicada almacenada en archivos de word que si bien puedes importar en wordpress significa que cada corrección supone corregir en varios archivos (indesign, wordpress, etc...) con el consiguiente problema de mantenimiento y sostenibilidad. 

Pasó el tiempo. Aprendimos algunas cosas más (Github entró en nuestra vida) y comenzamos de a poco a crear un mecanismo para repetir lo menos posible y almacenar todo en cuanto menos lugares mejor. Desterramos Word y comenzamos a utilizar venerables archivos de texto plano, que tienen la nada desdeñable ventaja de no esconderte nada. Lo que ves es lo que hay, lo cual resulta muy útil para resolver problemas cuando se te desarregla un diseño o algo se resiste en InDesign (que es algo que cualquiera que trabaje con InDesign y Word sabe que pasa todo el tiempo). Pero Wordpress se resistía a casi cualquier intento de ser integrado en nuestro flamante _Workflow_ de alguna manera que en lugar de añadir trabajo extra nos lo ahorrara. Eso, sin contar las actualizaciones del tema (que una vez si, y otra también, rompían la web) y las actualizaciones de _plugins_ (la misma historia).

Total, que llegó la pandemia y el confinamiento y decidí encarar el asunto.
La idea era crear desde cero un tema con el foco puesto en la publicación de libros. Escogí Jekyll, un generador de sitios estáticos escrito en Ruby, y probablemente el más popular de los que existen, por varias razones: está muy bien documentado, es rápido, es ligero, y el tipo de tecnología que utiliza es extremadamente simple:  MarkDown para formatear los archivos de texto plano, YAML para almacenar los datos, CSS para tunear la presentación del sitio y Git para hacer el control de versiones, mantener los archivos y alojarlos en la web (o sea, más o menos lo mismo que ya utilizábamos para producir libros). Es todo lo que hace falta; eso, y algo de liquid para escribir las plantillas, y paciencia.

## Manos a la obra

### Instalar software y dependencias

Para trabajar con jekyll hay dos cosas que son importantes: la primera, saber usar el terminal (el terminal en Mac y Linux, PowerShell en Windows). Si necesitas una intro al uso del terminal, [aquí](https://programminghistorian.org/es/lecciones/introduccion-a-bash) hay una estupenda.

Lo siguiente es un editor de texto plano. Hay muchos, cada cual con sus pequeñas maravillas incorporadas. Yo utilizo [Atom](https://atom.io/), pero cualquiera vale.

Entonces, podemos instalar el software que vamos a necesitar (las instrucciones pueden variar según el sistema operativo que utilicemos):

#### Git

Lo primero es Git. Lo podemos descargar [aquí](https://git-scm.com/). Una vez lo hemos instalado, abrimos el terminal para comprobar que está todo en orden y escribimos:

````git --version````

Si está todo OK, en la pantalla del terminal aparecerá algo así:

`git version 2.26.0.windows.1`

#### Ruby
#### Jekyll

### Crear el esqueleto de nuestro sitio

podemos scaffold

`jekyll new`

o bien, podemos clonar un tema de github. Para ahorrame algo de trabajo, pero aún empezar de los más básico, yo cloné el repo de mínima, que es el tema por defecto de Jekyll.

para esto:

Una vez que tenemos los archivos en algun lugar del disco duro, podemos agregar la carpeta entera a nuestro editor de texto, de manera que tengamos una vista panorámica de lo que pasa ahí
