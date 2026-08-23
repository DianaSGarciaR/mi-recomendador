# README.md — Página de Recomendaciones

## 📌 Descripción

Este proyecto consiste en el desarrollo de una página web de recomendaciones, diseñada para presentar contenido de forma clara, atractiva y sencilla de consultar.

La página busca facilitar al usuario la exploración de diferentes recomendaciones mediante una interfaz visual, organizada y adaptable a distintos dispositivos.

El proyecto también documenta el uso de herramientas de inteligencia artificial durante el proceso de desarrollo, mostrando cómo la IA puede utilizarse como apoyo para generar ideas, resolver problemas, mejorar código y acelerar determinadas etapas del desarrollo web.

---

## 🛠️ Tecnologías utilizadas

### HTML
Utilizado para construir la estructura y organización del contenido de la página web.

### CSS
Utilizado para personalizar la apariencia visual, distribución, tamaños, espacios, colores y estilos de los diferentes elementos.

### Bootstrap
Framework utilizado para facilitar el diseño responsive y utilizar componentes y utilidades prediseñadas.

### JavaScript
Utilizado para agregar interactividad y comportamiento dinámico a la página.

### Git
Utilizado para llevar un control de versiones del proyecto y registrar los diferentes cambios realizados durante el desarrollo.

### GitHub
Utilizado como repositorio remoto para almacenar, administrar y compartir el código fuente del proyecto.

### IA — ChatGPT
Utilizado como herramienta de apoyo durante el desarrollo para generar ideas, consultar dudas, proponer soluciones, revisar código y apoyar en diferentes etapas del proyecto.

---

## 🤖 Proceso de IA

Durante el desarrollo del proyecto se utilizó inteligencia artificial como herramienta de apoyo, principalmente mediante ChatGPT.

El proceso de trabajo con IA se puede resumir de la siguiente manera:

1. **Definición de la idea:** se establecieron las características y objetivos principales de la página.
2. **Planeación:** se solicitaron propuestas para organizar la estructura y contenido del sitio.
3. **Desarrollo:** se utilizó IA para consultar ejemplos y posibles implementaciones utilizando HTML, CSS, Bootstrap y JavaScript.
4. **Resolución de problemas:** cuando surgieron errores o dudas durante el desarrollo, se realizaron consultas específicas para encontrar posibles soluciones.
5. **Revisión:** se compararon las sugerencias proporcionadas por la IA con el código desarrollado manualmente.
6. **Adaptación:** las soluciones generadas por IA fueron modificadas cuando fue necesario para adaptarlas a las necesidades reales del proyecto.
7. **Validación:** finalmente, se probaron las funcionalidades implementadas para comprobar que funcionaran correctamente.

La IA se utilizó como una herramienta de asistencia y aprendizaje, manteniendo la revisión y toma de decisiones por parte del desarrollador.

---

## 💬 4 Prompts principales

Promp Uno
1.	¿Qué necesitábamos?
Darle contexto a la IA 
2.	¿Que intente hacer?
Quería poner en contexto a la IA antes consultar mis dudas, ya que al no tener contexto me daba soluciones donde usaba angular o funcione, en este caso no estaba permitido usar más que html, boostarp, javascrip y css.
3.	Prompt utilizado
Tu rol es ser mi tutor de desarrollo web para alguien que apenas es principiante. Mi proyecto es crear un sitio web llamado "Mis recomendaciones de video juegos" solo utilizaremos HTML, CSS, Bootstrap y variables básicas de JavaScript. Mi tema es juegos multijugador. Ya tengo conocimientos en HTML, CSS, Bootstrap y variables en JavaScript básicos. Para el desarrollo de este sitio está prohibido usar function, for, while, addEventListener, querySelector, map, filter. Importante cuando te consulte no generes todo el código del proyecto. Explícamelo paso a paso por favor y con ejemplos sencillos.
4.	¿Que respondió?
Medio un resumen de cómo me responderá, indicándome también que podrá empezar con declarar variables en el javaScrip.
5.	¿Qué parte utilizare?
Empecé con declarar mis variables en el archivo scrip.js
 
Promp Dos
1.	¿Qué necesitábamos?
HTML y Boostrap Al presionar un botón este me redirecciones a una sección específica del sitio.
2.	¿Que intente hacer?
Asigné un ID a cada sección a la que a la cual quería navegar y en la etiqueta botón usé data-target="seccion1", esto lo quise hacer como se abre un modal sin embargo no funciono.
3.	Prompt utilizado:
Explícame de manera clara, sencilla si es posible navegar dentro de una misma página HTML.
Tengo una página que al inicio contiene un menú con varios botones. Por ejemplo:
•	Opción 1
•	Opción 2
•	Opción 3
Más abajo, dentro de la mismo html, tengo diferentes secciones:
•	Sección 1
•	Sección 2
•	Sección 3
Quiero que, cuando se seleccione el botón "Opción 2" del menú, la página se desplace automáticamente hasta donde se encuentra la Sección 2 pero sin abrir otra página HTML.
Solo usando HTML.
4.	¿Que respondió?
1. Identifica tu Sección 2
En la parte de tu HTML donde está la sección 2, coloca un id:
<section id="seccion2">
    <h2>Sección 2</h2>
    <p>Aquí está el contenido de la sección 2.</p>
</section>
El id="seccion2" funciona como una especie de punto de destino.

2. Haz que "Opción 2" apunte hacia ella
En tu menú:
<a href="#seccion2">Opción 2</a>
Cuando el usuario haga clic, el navegador buscará:
id="seccion2"
dentro del mismo HTML y se desplazará hasta allí.

5.	¿Qué parte utilizare?
Así construí mis botones:
            <div class="card-footer">
                <a href="#seccion1" class="btn btn-success">Ver mas</a>
            </div>
Y aso están mis secciones:
<section id="seccion1">
 
Promp Tres
1.	¿Qué necesitábamos?
Ajustar el tamaño de las imagines que se muestran en un carrusel.
  
2.	¿Que intente hacer?
Cree una clase en los styles.css para modificar el alto y ancho de mis imágenes. Sin embargo, el ancho de la imagen no se modificaba al tamaño de la ventana.

4.	Prompt utilizado:
Estoy intentando modificar mi carrusel para que ocupe todo el ancho de la ventana. Sin embargo, cuando modifico su ancho mediante CSS, no llega a ocupar todo el espacio disponible. Ya intenté utilizar diferentes valores en píxeles y también probé centrando el carrusel automáticamente, pero ninguna de estas opciones funcionó. ¿Cómo puedo hacer que el carrusel ocupe correctamente todo el ancho de la ventana sin modificar el alto?

5.	¿Que respondió?
Sí. 😊 Si el alto de tu carrusel ya está bien y solamente quieres que ocupe todo el ancho de la ventana, el problema probablemente no está en la imagen, sino en el contenedor que envuelve al carrusel.
1. Usa width: 100%
Para las imágenes puedes tener:
.imgCarusel {
    width: 100%;
    height: 500px;
    object-fit: cover;
}
No necesitas poner valores como 1200px, 1500px, etc. 100% permite que se adapte al tamaño de la ventana.

5.	¿Qué parte utilizare?
Solo cambie el valor de width.
.imgCarusel {
    width: 100%;
    /* Alto fijo deseado */
    height: 500px;
    /* Evita la distorsión */
    object-fit: cover;
    position: center;
}

Promp Cuatro
1.	¿Qué necesitábamos?
JavaScrip y html, mostrar la información de una variable en html.
2.	¿Que intente hacer?
Anterior mente ya había eche este tipo de trabajos pero solo usando angular, y por medio de document.getElementById(). Sin embargo, quise saber si hay otra manera de aplicarlo siguiendo las instrucciones de la actividad.
3.	Prompt utilizado:
Explícame si es posible mostrar en mi archivo index.html en cualquier etiqueta (div, a, p, etc) el valor de una variable que tengo declarada en mi archivo script.js. Recuerda únicamente estamos utilizando HTML, CSS, JavaScript y Bootstrap.
4.	¿Que respondió?
Sí, es posible. Pero hay un punto importante según lo que ya hemos establecido para tu proyecto:
Para mostrar el valor de una variable de script.js dentro de una etiqueta de index.html, necesitas que JavaScript modifique ese elemento HTML. Eso es manipulación del DOM.
Como todavía estás aprendiendo JavaScript y no quieres utilizar DOM, funciones ni ciclos, entonces todavía no puedes hacerlo de esa manera.
5.	¿Qué parte utilizare?
Por ahora solo mostré el mensaje por consola:
let listVideoGame = ["1. Project zomboid", "2. Pokemon Unite", "3. Dont strave", "4. Overcooked", "5. Terraria", "6. Elsword", "7. GTA 5", "8. Heatopia", "9. Roblox", "10. Among us"];

let mensaje = "Hola, puedes ver mi página web";
let miVideoGameFavorito = "Project zomboid";
let numeroVideoGame = 1;
let numeroMiFavorito = 10;
let bandera = true;
console.log(mensaje);
console.log("Vista activa: ", bandera)
console.log("Mi video juego favorito: es el Top ", numeroVideoGame, "y su nombre es: ", miVideoGameFavorito);
console.log("Cuantos juegos recomiendo: ", numeroVideoGame);
console.log("Lista de todos los juegos: ", listVideoGame);

## 🔄 Comparativa: código generado por IA vs código propio

La IA me ayudó con consultas sobre cómo mejorar mi código HTML y cómo manejar de una mejor manera la navegación entre páginas, sin necesidad de utilizar JavaScript ni implementar soluciones demasiado robustas.

Las consultas que realizaba principalmente me daban referencias y explicaciones sobre cómo hacerlo, con el objetivo de comprender su funcionamiento y aprender a utilizarlas. Finalmente, yo mismo podía implementar estas soluciones en mi código.

## 📚 Aprendizaje

Aprendí que existen muchas funcionalidades y diferentes usos para los atributos de HTML. También comprendí que la IA puede ayudarme a orientarme sobre cómo comenzar a desarrollar una determinada estructura de código, qué conceptos necesito comprender y qué aspectos puedo mejorar a partir de los conocimientos que ya tengo.

Además, entendí que utilizar la IA como una herramienta de orientación y aprendizaje me permite encontrar diferentes formas de resolver un problema sin depender completamente de que genere el código por mí.


## 💭 Reflexión

Hubo conceptos que al principio no comprendía completamente, pero al realizar consultas y recibir explicaciones sobre su funcionamiento pude entender mejor cómo aplicarlos. Esto me permitió no solo obtener una solución, sino también aprender el motivo por el cual se utiliza cada elemento y cómo puedo implementarlo por mi cuenta.
