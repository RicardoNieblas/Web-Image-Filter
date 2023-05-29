# **Web Image Filter**

Proyecto realizado por Ricardo Nieblas y John Nemeth.

### **Resumen**

Web Image Filter es una página web diseñada para proporcionar a los usuarios una experiencia interactiva de edición de fotos. Esta página ofrece varios filtros y herramientas para manipular las imágenes. Esto permite a los usuarios transformar sus fotografías a un resultado creativo. Nos enfocamos en una interfaz intuitiva y fácil de usar para que el proceso se vuelva libre de frustraciones y accesible para cualquier persona, sin importar el nivel de habilidad o experiencia.

#

### **Descripción del problema**

Con Web Image Filter, una de las problemáticas que buscamos resolver es la accesibilidad a herramientas de edición de imágenes. Estamos conscientes de que en el mercado existen muchas alternativas, pero nuestro enfoque principal es proveer una herramienta libre de restricciones como suscripciones, anuncios, o interfaces complicadas. Al hablar de herramientas en línea, las opciones disponibles resultan ser escasas. Por lo tanto, nuestro objetivo es proporcionar una solución en línea que sea accesible, intuitiva y visualmente atractiva para los usuarios que deseen editar sus fotos de manera rápida y sencilla.

#

### **Objetivos**

- Desarrollar una página web interactiva para la edición de imágenes que sea fácil de usar y accesible para usuarios de diferentes niveles de habilidad. El objetivo principal es proporcionar una interfaz intuitiva y amigable, con controles claros y funcionales, para que los usuarios puedan realizar ediciones de imágenes sin dificultad.

- Proporcionar una variedad de filtros y herramientas de edición de imágenes para que los usuarios puedan mejorar, transformar y personalizar sus fotos de manera creativa. El objetivo es ofrecer una amplia gama de opciones de edición, como filtros de color, ajustes de tono y saturación, efectos de desenfoque, recorte y redimensionamiento de imágenes, entre otros. Además, se buscará implementar opciones avanzadas para aquellos usuarios con conocimientos técnicos más profundos.

- Permitir a los usuarios cargar y guardar imágenes de forma segura en la aplicación. En la actualidad la seguridad es un factor muy importante al momento de estar en línea. No está de más mencionar, que nuestra aplicación web no recolecta información de ningún tipo de los usuarios. Las imágenes son procesadas mediante los gráficos integrados de la computadora en la que se accede, y no se manda nada a servidores externos.

- Utilizar Inteligencia Artificial (objetivo a largo plazo) para identificar automáticamente la escena de una fotografía y aplicar ajustes adecuados a través de algoritmos de visión por computadora y aprendizaje automático. Esto permite mejorar la calidad de la imagen al resaltar aspectos clave como contraste, saturación y balance de blancos. Al automatizar este proceso, los usuarios obtienen resultados precisos y rápidos en la edición de sus fotografías, ahorrando tiempo y esfuerzo en ajustes manuales.

#

### **Marco teórico**

El proyecto se basa en los principios de procesamiento digital de imágenes, que abarcan técnicas para manipular y mejorar la calidad de las imágenes. Esto incluye operaciones como filtrado, ajuste de color, corrección de brillo/contraste, manipulación de píxeles, etc. Para las tecnologías implementadas, nuestro proyecto se debe gracias a la librería de glfx.js. Esta es la encargada de realizar los cambios a las imágenes, permitiéndonos acceder a los parámetros de edición encontrados en nuestro proyecto.

#

### **Descripción de la implementación**

A continuación, una descripción breve de algunos de los puntos más importantes de nuestra implementación del código:

- `loadImage(src)`: Esta función se utiliza para cargar una imagen en la aplicación. Cuando se carga una imagen, se realizan una serie de acciones, como contraer cualquier elemento seleccionado, restablecer el filtro seleccionado y ocultar el diálogo actual. Luego, se llama a la función init(image) para inicializar la imagen cargada.

- `showDialog()` y `hideDialog()`: Estas funciones se utilizan para mostrar y ocultar un diálogo en la aplicación.


- `contractItem(item)` y `expandItem(item)`: Estas funciones se utilizan para contraer o expandir un elemento en la barra lateral de la aplicación.

- `setSelectedFilter(filter)`: Esta función se utiliza para establecer el filtro seleccionado en la aplicación. Borra cualquier contenido dibujado previamente en el contexto 2D del lienzo `(canvas2d)`, actualiza los elementos de la interfaz de usuario y dibuja el filtro seleccionado.

- `init(image)`: Esta función se utiliza para inicializar la imagen cargada en la aplicación. Crea una textura a partir de la imagen y la dibuja en el lienzo (canvas). También establece los límites del área de arrastre para que los elementos de control no se puedan arrastrar fuera de la imagen.

- `$(window).load(function() { ... })`: Esta función se ejecuta cuando se carga completamente la página web. Se utiliza para realizar la inicialización inicial de la aplicación. Intenta obtener un lienzo WebGL utilizando la biblioteca glfx.js. Si tiene éxito, genera el HTML para la barra lateral de la aplicación y establece los controladores de eventos para varios elementos.

#

### **Resultados finales y demostración**

Para una mejor comprensión del funcionamiento de nuestro proyecto, consideramos ideal que se pueda interactuar con él, a comparación de mostrar varias capturas del mismo.

Entra a [Web Image Filter](https://ricardonieblas.github.io/Web-Image-Filter/)

#

### **Conclusiones**

En resumen, el proyecto Web Image Filter proporciona una experiencia interactiva y accesible en la edición de imágenes en línea. Ofrece una interfaz intuitiva y atractiva, variedad de filtros y herramientas de edición, seguridad en las imágenes cargadas y el objetivo a largo plazo de incorporar inteligencia artificial para mejorar la calidad de las imágenes automáticamente.

Nos encontramos contentos con el resultado final, pues a pesar de todas las dificultades que encontramos durante nuestro camino, tenemos en nuestras manos el conocimiento necesario y un proyecto en el cual tenemos claras ideas de cómo nos gustaría seguir trabajando en él, con la posibilidad de incluirlo en futuras materias que tomaremos en los siguientes semestres.
