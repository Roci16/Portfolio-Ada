# Observaciones

Ro, felicitaciones por tu trabajo. Me encanta como quedó tu portfolio, se ve muy lindo, limpio y profesional. Me gustan los colores y tipografías, y tengo que destacar la increíble atención al detalle que demostrás y lo bien que anda tu responsive. 

Como dije en clase, este trabajo no se hace para que constates conocimientos, sino para que aprendas: en ese sentido, mi intencion es que estos comentarios te sirvan para aprender, mejorar tu codigo a futuro e ir apreciando mejor qué se espera de nosotras como desarrolladoras front end.

## Estructura correcta de documento HTML

Tu HTML esta realmente excelente. Claro, prolijo, muy bien comentado e identado. Lo único a comentar es que dejar un salto de linea entre cada etiqueta hace muy dificil la lectura. Privilegiá escribir uno debajo del otro sin un espacio entre cada uno. 

Algo que me llama la atención es tu `head`, dado que allí repetís innecesariamente el link de css. No es necesario escribilo dos veces

```html
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/devicons/devicon@v2.11.0/devicon.min.css">
    <link rel="stylesheet" href="style.css">
```

Agregar muchos de estos links innecesarios impacta negativamente en la velocidad de carga de tu web, ya que por cada uno de ellos se hace un llamado a un css externo y se lo carga. 

Tenés cierta tendencia a tener divs de más. Algunas estructuras de tu web se podrían resolver con menos divs. Dicho esto, yo prefiero que los divs sobren antes de que falten: un div de más se soluciona muy fácil, un div menos puede ser un gran dolor de cabeza cuando estamos recién arrancando. Este sería un comentario que quizá me reservaría para futuros trabajos, pero veo tan bien tu código que me siento confiada en recomendarte que empieces a ver estas cosas desde ya. 

Si tenés ganas, con tiempo, te diría que valdría la pena recorrer tu html y notar que estructuras como esta se pueden hacer más breves. Te diria que podriamos hacerlo solo el nav, el ul, los li y los a. 

```html
    <nav class="nav-barra">
        <!-- *Empieza el menú* -->
        <ul>
            <div class="nav-derecha">
                <div class="box-nav">
                    <li><a href="#Hola" class="color-nav">HOLA</a></li>
                    <li><a href="#Conocimiento" class="color-nav">CONOCIMIENTO</a></li>
                    <li><a href="#Proyecto" class="color-nav">PROYECTOS</a></li>
                    <li><a href="#Contacto" class="color-nav boton-1">CONTACTO</a></li>
                </div>


            </div>
        </ul>
        <!-- *Termina el menú* -->
    </nav>
```

## Respeta la consigna

- El portfolio cuenta con las secciones solicitadas
- Al clickear en los links de navegación, debe llevar a la sección correspondiente
- Al clickear en los links de contacto, debe llevar a la página externa
  correspondiente
- El portfolio debe tener un diseño responsivo y verse correctamente en distintos dispositivos
- El portfolio debe estar deployado y ser accesible desde una URL
- El repositorio en GitHub debe tener un readme adecuado

Todos estos puntos están cumplidos. Menciono especialmente tu responsive: es increíble lo bien que solucionaste las distintas resoluciones, siguiendo casi a la perfección el modelo y preocupandote para que todo se vea hermoso, veamos tu web desde cualquier dispositivo.

### Respeta el diseño dado

Cumplido a la perfección. El único comentario es que tus elementos de formulario necesitan algo de `padding`: los textos y placeholders se ven como pegoteados a los bordes. 

### Buena estructura de proyecto

Cumplido casi a la perfección, pero el favicon deberia llamarse favicon.ico, ya que asi lo van a buscar la mayoria de los servicios de hosting. Notá también que tenés una carpeta innecesaria, `vscode`, que es agregada a veces automáticamente por Visual Studio. Es buena práctica borrarla antes de una entrega. 

### Código bien indentado

Tabulas muy bien, lo cual parece un detalle extra cuando una recien comienza pero ayuda un monton a su legibilidad, y que lo hayas logrado en esta etapa es un gran mérito. 

### Comentarios que permiten mejorar la legibilidad del código

Perfecto. 

### Uso correcto de etiquetas semánticas

En general usas bien las etiquetas semánticas. Me llama la atención que hayas usado `div` para las tarjetas de Mis Conocimientos: yo diría que deberían ser `article`. Pero es el único detalle a comentar aquí (y hay quien podría discutirme que deberían ser divs)

### Buenos nombres de clases

Cumplido la mayoría de las veces: en otras ocasiones se nota que te rendiste. La clase "box-lorem-2" o la clase ".color-hover-2" no me dicen nada, no me ayudan a saber a qué elementos se refieren. 

Cuando decimos que un nombre de clase debe ser descriptivo, lo decimos en un sentido funcional: qué rol cumple este elemento en el código. Los colores de los elementos, su etiqueta de html, su forma, su estilo, su posición, todas esas cosas pueden cambiar y efectivamente cambian todo el tiempo en las webs que hacemos. El botón que hoy es violeta mañana será azul; la sección que estaba primera mañana estará tercera. Por lo tanto esos factores sos no son buenos descriptores, y no deberían ser parte de nuestros nombres de clases.

### Código CSS bien estructurado

Cumplido, te dejo algunos comentarios en el archivo. 

### Reutilización de estilos

<!-- Cumplido en general, aunque hay muchisimas oportunidades perdidas de reciclar estilos para que se usen en muchos elementos a la vez. Es necesario por ejemplo tener estilos distintos en los contenedores de Mis Proyectos, Mis Conocimientos, etc? Quiza puedan tener dos clases que hagan que no se repitan tanto todas las ordenes de flex? -->

### Cumple con criterios básicos de accesibilidad

- Los colores tienen un contraste adecuado

Cumplido 

- Las imágenes tiene el atributo `alt` que corresponde

Incumplido. Si te pareció innecesario agregar `alt` para las imagenes de Mis Proyectos, correspondía un aria-hidden en lugar de dejar el alt vacío (que indica que la imagen es decorativa: aquí claramente es ilustrativa). Dejarlo vacía es decirle al usuario que depende del lector de pantalla "aquí hay una imagen y no te voy a decir qué es", lo que no es una buena experiencia. 

- Los íconos y elementos que no presentan texto agregan la información correspondiente por otros medios (etiquetas aria, texto oculto)

Cumplido

- Los íconos y elementos que no necesitan ser anunciados por un lector de pantalla tienen la etiqueta aria
  correspondiente

Cumplido

- Commits con mensajes adecuados

Cumplido, noto muchos y buenos commits en tu proyecto, lo que siempre se agradece.

- Cuenta con un favicon

Cumplido, aunque debería llamarse favicon.ico

### Nota: 9
