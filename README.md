# desarrollo_91370

# MÓDULO 1 — INTRODUCCIÓN A HTML
## Desarrollo Web | Coderhouse

**Modalidad:** Live Coding con Visual Studio Code y Google Chrome.

**Objetivo:** Aprender a construir la estructura de un sitio web utilizando HTML5, comprendiendo la función de las etiquetas, los atributos, la organización semántica del contenido y la navegación entre páginas.

**Proyecto del módulo:** Construiremos progresivamente un sitio web personal que servirá como base para las siguientes clases.

---

# 1. HERRAMIENTAS FUNDAMENTALES

## 1.1. Introducción al desarrollo web

### 🎤 Para comenzar la clase

Antes de escribir código, pensemos en algo que hacemos todos los días: entrar a una página web.

Cuando abrimos una red social, un sitio de noticias o una tienda online, vemos textos, imágenes, botones y enlaces.

Pero ¿alguna vez se preguntaron cómo sabe el navegador qué tiene que mostrar?

### 💬 Preguntas para el grupo

- ¿Qué diferencia creen que hay entre Internet y una página web?
- ¿Qué creen que hace un navegador?
- ¿Alguien escribió código alguna vez?
- ¿Qué creen que necesitamos para construir una página web?

## 1.2. Conceptos fundamentales

### ¿Qué es Internet?

Internet es una red mundial de dispositivos interconectados que permite compartir información.

### ¿Qué es la web?

La World Wide Web es uno de los servicios que funciona sobre Internet y permite acceder a páginas y otros recursos mediante navegadores.

### ¿Qué es un navegador?

Es un programa que interpreta y presenta los recursos de un sitio web.

Ejemplos:
- Google Chrome
- Mozilla Firefox
- Microsoft Edge
- Brave

### ¿Qué es un editor de código?

Es una herramienta que utilizamos para escribir, organizar y modificar el código fuente de nuestros proyectos.

Durante este curso vamos a utilizar **Visual Studio Code**.

Sitio oficial: https://code.visualstudio.com/

## 1.3. Tecnologías fundamentales

### HTML — HyperText Markup Language

Es un lenguaje de marcado que permite definir la estructura y el significado del contenido de una página web.

Por ejemplo:
- Títulos
- Párrafos
- Imágenes
- Enlaces
- Formularios

**HTML no es un lenguaje de programación.**

### CSS — Cascading Style Sheets

Es un lenguaje de estilos que permite definir la presentación visual de una página web.

Por ejemplo:
- Colores
- Tipografías
- Tamaños
- Márgenes
- Distribución de elementos
- Adaptación a diferentes pantallas

### JavaScript

Es un lenguaje de programación que permite incorporar comportamientos dinámicos e interactividad.

### Para recordar

- **HTML:** estructura y significado.
- **CSS:** presentación visual.
- **JavaScript:** comportamiento e interactividad.

---

## 1.4. Inspeccionamos una página web

### 💻 Demostración en Chrome

1. Abrir cualquier sitio web.
2. Hacer clic derecho sobre un elemento.
3. Seleccionar **Inspeccionar**.
4. Mostrar el panel Elements.
5. Identificar etiquetas HTML.
6. Modificar temporalmente algún texto.

### 🎤 Explicación

Todo lo que vemos en una página web tiene una representación en el documento.

Las palabras que aparecen entre los signos `<` y `>` son etiquetas HTML.

Estas etiquetas permiten indicar qué función cumple cada contenido.

**Importante:** los cambios realizados desde DevTools son locales y temporales. No estamos modificando el sitio original.

---

# 2. ESTRUCTURA BÁSICA DE UN DOCUMENTO HTML5

## 2.1. Nuestro primer proyecto

### 💻 En Visual Studio Code

1. Crear una carpeta llamada `mi-primer-sitio`.
2. Abrir la carpeta desde VS Code.
3. Crear un archivo llamado `index.html`.
4. Escribir lo siguiente:

```html
Hola, mundo.
```

Abrir el archivo en Chrome.

### 💬 Pregunta

¿Por qué el navegador puede mostrar este texto si todavía no escribimos ninguna etiqueta?

### 🎤 Explicación

Los navegadores pueden interpretar incluso documentos incompletos.

Pero eso no significa que nuestro documento tenga una estructura correcta.

Vamos a construir una estructura HTML válida.

## 2.2. Estructura básica HTML5

### 💻 Live Coding

Escribir progresivamente:

```html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi primer sitio web</title>
</head>

<body>
    <h1>¡Hola, mundo!</h1>
    <p>Esta es mi primera página web.</p>
</body>

</html>
```

## 2.3. Explicación de cada elemento

### `<!DOCTYPE html>`

Indica al navegador que el documento utiliza el estándar moderno de HTML.

### `<html>`

Es el elemento raíz del documento.

El atributo `lang="es"` indica que el idioma principal del documento es español.

### `<head>`

Contiene metadatos e información de configuración del documento.

Generalmente, esta información no se muestra dentro del contenido visible de la página.

### `<meta charset="UTF-8">`

Define la codificación de caracteres utilizada por el documento.

Permite representar correctamente caracteres como tildes, ñ y otros símbolos.

### `<meta name="viewport">`

Permite controlar cómo se adapta la visualización del documento a diferentes tamaños de pantalla.

### `<title>`

Define el título que aparece en la pestaña del navegador.

### `<body>`

Contiene el contenido visible de nuestra página web.

## 2.4. ¿Qué son las etiquetas HTML?

Las etiquetas permiten describir la función de los elementos.

La mayoría tiene una etiqueta de apertura y una de cierre.

```html
<p>Este es un párrafo.</p>
```

- `<p>`: apertura.
- `Este es un párrafo.`: contenido.
- `</p>`: cierre.

Algunos elementos, como `<img>` y `<meta>`, no necesitan etiqueta de cierre.

## 2.5. Títulos y párrafos

### Encabezados

HTML proporciona seis niveles de encabezado:

```html
<h1>Título principal</h1>
<h2>Título secundario</h2>
<h3>Subtítulo</h3>
<h4>Encabezado de nivel cuatro</h4>
<h5>Encabezado de nivel cinco</h5>
<h6>Encabezado de nivel seis</h6>
```

Los niveles indican jerarquía, no solamente tamaño visual.

### Párrafos

```html
<p>Este es un párrafo de texto.</p>
```

Se utiliza para representar bloques de texto.

### 💻 Demostración

Cambiar el contenido del `<title>` y observar la pestaña.

Cambiar el contenido del `<h1>` y observar la página.

### 💬 Preguntas

- ¿Qué diferencia hay entre `head` y `body`?
- ¿Dónde colocarían un título que debe ver el usuario?
- ¿Por qué no deberíamos utilizar un `h3` solamente porque se ve más pequeño?

## 2.6. Actividad práctica

### ✍️ Nuestra primera página personal

Crear una página HTML que incluya:

1. El nombre del estudiante como título principal.
2. Un párrafo de presentación.
3. Un título secundario sobre sus intereses.
4. Un párrafo donde explique qué le gustaría aprender.
5. Un tercer título con su actividad favorita.

**Objetivo:** practicar la estructura base y la jerarquía de títulos.

---

# 3. ETIQUETAS SEMÁNTICAS Y ATRIBUTOS

## 3.1. ¿Qué es HTML semántico?

### 🎤 Introducción

Ya sabemos incorporar contenido, pero imaginemos una página que tiene muchos elementos.

Una tienda online, por ejemplo, tiene un encabezado, un menú, productos, distintas secciones y un pie de página.

¿Cómo podemos organizar toda esa información?

HTML incluye etiquetas que permiten describir qué función cumple cada parte de una página.

Esto se conoce como **semántica HTML**.

### Ejemplo de código poco semántico

```html
<div>
    <div>Menú principal</div>
</div>

<div>
    <div>Contenido de la página</div>
</div>
```

Aunque `div` es una etiqueta válida, no indica específicamente qué función cumple cada contenido.

### Ejemplo semántico

```html
<header>
    <nav>Menú principal</nav>
</header>

<main>
    <section>Contenido de la página</section>
</main>
```

En este caso, las etiquetas expresan qué representa cada parte.

## 3.2. Principales etiquetas semánticas

### `<header>`

Representa contenido introductorio de una página o sección.

Suele utilizarse para encabezados y, en muchos sitios, contiene la identidad visual y la navegación principal.

### `<nav>`

Representa una sección destinada a enlaces de navegación importantes.

### `<main>`

Contiene el contenido principal del documento.

Normalmente debe existir un único elemento `main` visible por página.

### `<section>`

Representa una sección temática de contenido.

Generalmente debe tener un encabezado que identifique su tema.

### `<article>`

Representa contenido autónomo que tiene sentido por sí mismo.

Por ejemplo:
- Una noticia.
- Una publicación de blog.
- Una reseña.
- Una tarjeta de producto independiente.

### `<aside>`

Representa contenido relacionado indirectamente con el contenido principal.

Por ejemplo, una barra lateral con información complementaria.

### `<footer>`

Representa el pie de página o de una sección.

Puede incluir información de contacto, derechos de autor y enlaces complementarios.

---

## 3.3. Construimos la estructura de nuestro portafolio

### 💻 Live Coding

Conservar el `head` del documento anterior y reemplazar el contenido del `body`.

```html
<body>

    <header>
        <p>Mi Portafolio</p>

        <nav>
            <ul>
                <li>Inicio</li>
                <li>Sobre mí</li>
                <li>Proyectos</li>
                <li>Contacto</li>
            </ul>
        </nav>
    </header>

    <main>

        <section>
            <h1>Hola, soy Ana</h1>
            <p>Estoy aprendiendo desarrollo web.</p>
        </section>

        <section>
            <h2>Mis proyectos</h2>

            <article>
                <h3>Mi primer sitio web</h3>
                <p>Una página construida con HTML5.</p>
            </article>

        </section>

    </main>

    <footer>
        <p>2026 - Mi portafolio personal</p>
    </footer>

</body>
```

### 💬 Preguntas durante el Live Coding

- ¿Por qué utilizamos `header`?
- ¿Qué diferencia hay entre `header` y `head`?
- ¿Dónde ubicaríamos el menú principal?
- ¿Por qué el contenido principal está dentro de `main`?
- ¿Qué diferencia hay entre `section` y `article`?
- ¿Qué información colocarían en el footer?

### Para destacar

**`section` organiza contenido por temas, mientras que `article` representa una unidad de contenido que puede tener sentido de forma independiente.**

---

## 3.4. Atributos HTML

Los atributos permiten agregar información adicional a los elementos HTML.

Se escriben dentro de la etiqueta de apertura.

### Atributo `id`

Permite identificar un elemento de forma única dentro del documento.

```html
<section id="sobre-mi">
    <h2>Sobre mí</h2>
</section>
```

### Atributo `class`

Permite asignar una o más clases a un elemento.

Una misma clase puede utilizarse en diferentes elementos.

```html
<article class="proyecto">
    <h3>Proyecto 1</h3>
</article>

<article class="proyecto">
    <h3>Proyecto 2</h3>
</article>
```

### Diferencia principal

- `id`: identificador único.
- `class`: permite agrupar elementos bajo una misma clasificación.

Más adelante utilizaremos estos atributos para trabajar con CSS.

## 3.5. Actividad práctica

### ✍️ Estructura de un emprendimiento

Crear la estructura HTML de una página para un emprendimiento ficticio.

Puede ser:
- Cafetería.
- Tienda de ropa.
- Librería.
- Restaurante.
- Tienda de tecnología.

La página debe contener:

1. Encabezado.
2. Menú de navegación.
3. Contenido principal.
4. Dos secciones temáticas.
5. Al menos un artículo.
6. Pie de página.

**Objetivo:** elegir etiquetas por su significado y no por su apariencia.

---

# 4. ENLACES Y NAVEGACIÓN

## 4.1. ¿Cómo conectamos las páginas?

### 🎤 Introducción

Nuestro sitio ya tiene contenido organizado, pero todavía hay algo que no funciona.

Tenemos un menú con distintas opciones, pero no podemos navegar.

¿Cómo hacemos para que un usuario pueda pasar de una página a otra?

Para eso utilizamos los enlaces HTML.

## 4.2. La etiqueta `<a>`

La etiqueta `<a>` permite crear hipervínculos.

El atributo `href` indica el destino del enlace.

### Enlace externo

```html
<a href="https://github.com">
    Visitar GitHub
</a>
```

### Abrir en una pestaña nueva

```html
<a
    href="https://github.com"
    target="_blank"
    rel="noopener noreferrer"
>
    Visitar GitHub
</a>
```

### Enlace interno dentro del documento

```html
<a href="#contacto">
    Ir a contacto
</a>
```

El enlace apunta a un elemento cuyo `id` sea `contacto`.

```html
<section id="contacto">
    <h2>Contacto</h2>
</section>
```

## 4.3. Construimos nuestro menú

### 💻 Live Coding

```html
<nav>
    <ul>
        <li>
            <a href="index.html">Inicio</a>
        </li>
        <li>
            <a href="#sobre-mi">Sobre mí</a>
        </li>
        <li>
            <a href="#proyectos">Proyectos</a>
        </li>
        <li>
            <a href="pages/contacto.html">Contacto</a>
        </li>
    </ul>
</nav>
```

Recordar agregar los identificadores correspondientes a las secciones.

### 💬 Preguntas

- ¿Qué sucede si hacemos clic en un enlace con `#proyectos`?
- ¿Qué pasa si no existe un elemento con ese `id`?
- ¿Qué diferencia hay entre un enlace externo y uno interno?

---

## 4.4. Rutas relativas

Una ruta indica dónde se encuentra un recurso.

### Estructura inicial de carpetas

```text
mi-primer-sitio/
│
├── index.html
│
├── pages/
│   ├── sobre-mi.html
│   ├── proyectos.html
│   ├── servicios.html
│   └── contacto.html
│
└── img/
    └── foto.jpg
```

### Desde index.html hacia una página secundaria

```html
<a href="pages/contacto.html">
    Contacto
</a>
```

### Desde contacto.html hacia index.html

```html
<a href="../index.html">
    Volver al inicio
</a>
```

### ¿Qué significa `../`?

Indica que debemos subir un nivel en la estructura de carpetas.

### 💻 Demostración de un error

Escribir intencionalmente una ruta incorrecta.

Por ejemplo, desde `pages/contacto.html`:

```html
<a href="index.html">Inicio</a>
```

Mostrar que el navegador busca el archivo dentro de `pages`.

Corregir la ruta:

```html
<a href="../index.html">Inicio</a>
```

### 💬 Pregunta

¿Por qué una misma ruta no necesariamente funciona desde todos los archivos?

---

# 5. INSERCIÓN DE IMÁGENES Y MULTIMEDIA

## 5.1. La etiqueta `<img>`

Permite insertar imágenes dentro de una página HTML.

### Ejemplo

```html
<img
    src="img/foto.jpg"
    alt="Persona trabajando frente a una computadora"
>
```

### Atributos fundamentales

**`src`:** indica dónde se encuentra la imagen.

**`alt`:** proporciona un texto alternativo que describe la imagen según su función y contexto.

El atributo `alt` es importante para la accesibilidad, especialmente para personas que utilizan lectores de pantalla.

Cuando una imagen es puramente decorativa, normalmente utilizamos `alt=""`.

### 💻 Demostración

1. Insertar una imagen desde la carpeta `img`.
2. Abrir la página en Chrome.
3. Cambiar intencionalmente el nombre del archivo en `src`.
4. Observar qué sucede.
5. Corregir la ruta.

### 💬 Pregunta

¿Por qué `alt="imagen"` no sería una alternativa textual suficientemente descriptiva?

---

## 5.2. Las etiquetas `<figure>` y `<figcaption>`

Estas etiquetas permiten agrupar contenido ilustrativo y agregarle una leyenda.

### `<figure>`

Representa contenido autónomo, como una fotografía, un gráfico, una ilustración o un ejemplo de código.

### `<figcaption>`

Permite agregar una leyenda visible asociada al contenido de `figure`.

### Ejemplo

```html
<figure>
    <img
        src="img/equipo.jpg"
        alt="Equipo de trabajo reunido"
    >

    <figcaption>
        Nuestro equipo durante una jornada de capacitación.
    </figcaption>
</figure>
```

### Diferencia entre `alt` y `figcaption`

**`alt`:**
- Es un atributo de `img`.
- Ofrece una alternativa textual para la imagen.
- Es importante para la accesibilidad.
- No aparece normalmente como leyenda visible.

**`figcaption`:**
- Es una etiqueta HTML.
- Es una leyenda visible en la página.
- Puede aportar contexto o información adicional.

### ¿Es obligatorio utilizar figure?

No.

Podemos insertar imágenes directamente:

```html
<img src="img/logo.png" alt="Logo de la empresa">
```

Conviene utilizar `figure` cuando la imagen o contenido ilustrativo constituye una unidad con sentido propio, especialmente si necesita una leyenda.

### Ejemplos de uso

- Fotografías con epígrafes.
- Gráficos estadísticos.
- Capturas de pantalla en tutoriales.
- Ilustraciones acompañadas de explicaciones.

---

# 6. FORMULARIOS HTML

## 6.1. ¿Para qué sirven los formularios?

### 🎤 Introducción

Hasta ahora aprendimos a mostrar información.

Pero muchas veces necesitamos que las personas ingresen datos en nuestro sitio.

### 💬 Preguntas

- ¿Dónde utilizan formularios habitualmente?
- ¿Qué campos tiene una pantalla de registro?
- ¿Qué información pedirían en una página de contacto?

## 6.2. Principales etiquetas

### `<form>`

Agrupa los controles de un formulario.

### `<label>`

Identifica y describe un campo.

### `<input>`

Permite introducir diferentes tipos de datos.

Algunos tipos comunes:

- `text`
- `email`
- `password`
- `number`
- `date`
- `checkbox`
- `radio`

### `<textarea>`

Permite ingresar textos de varias líneas.

### `<button>`

Permite crear un botón, que puede utilizarse para enviar el formulario.

---

## 6.3. Construimos un formulario de contacto

### 💻 Live Coding

Dentro de `pages/contacto.html`:

```html
<main>

    <h1>Contacto</h1>

    <p>Completá el formulario para escribirme.</p>

    <form action="#" method="get">

        <div>
            <label for="nombre">Nombre</label>

            <input
                type="text"
                id="nombre"
                name="nombre"
                required
            >
        </div>

        <div>
            <label for="email">Correo electrónico</label>

            <input
                type="email"
                id="email"
                name="email"
                required
            >
        </div>

        <div>
            <label for="mensaje">Mensaje</label>

            <textarea
                id="mensaje"
                name="mensaje"
                rows="5"
            ></textarea>
        </div>

        <button type="submit">
            Enviar
        </button>

    </form>

</main>
```

### Explicación de atributos

**`for`:** vincula un `label` con el campo que tiene el `id` correspondiente.

**`type`:** define el tipo de control.

**`name`:** identifica el dato cuando se envía el formulario.

**`required`:** indica que el campo es obligatorio.

**`placeholder`:** permite mostrar una pista dentro de un campo. No reemplaza al `label`.

**`action`:** indica el destino al que se envían los datos.

**`method`:** indica el método HTTP utilizado para enviar el formulario.

- `get`: los datos suelen incorporarse a los parámetros de la URL.
- `post`: los datos se envían en el cuerpo de la solicitud HTTP.

**Importante:** este formulario es demostrativo y todavía no cuenta con un servicio que procese los mensajes. No debe utilizarse para recopilar información sensible.

### 💻 Demostraciones en Chrome

1. Intentar enviar el formulario vacío.
2. Observar la validación de `required`.
3. Ingresar un correo con formato incorrecto.
4. Hacer clic en el `label`.
5. Observar cómo se activa el campo correspondiente.

### 💬 Preguntas

- ¿Qué sucede si eliminamos `required`?
- ¿Por qué es importante relacionar el `label` con el `input`?
- ¿Qué diferencia hay entre `placeholder` y `label`?

---

# 7. AUDIO Y VIDEO EN HTML5

HTML permite incorporar contenido multimedia utilizando etiquetas nativas.

## 7.1. Video

```html
<video controls width="400">
    <source
        src="video/presentacion.mp4"
        type="video/mp4"
    >

    Tu navegador no admite este video.
</video>
```

## 7.2. Audio

```html
<audio controls>
    <source
        src="audio/presentacion.mp3"
        type="audio/mpeg"
    >

    Tu navegador no admite este audio.
</audio>
```

### ¿Qué hace el atributo controls?

Permite que el navegador muestre controles de reproducción, como reproducir, pausar y ajustar el volumen.

### 💻 Demostración

Agregar archivos multimedia de ejemplo y observar cómo se reproducen desde Chrome.

---

# 8. ACTIVIDAD INTEGRADORA DEL MÓDULO

## Construimos nuestro sitio web personal

### Objetivo

Aplicar los conceptos aprendidos durante el módulo y preparar la estructura inicial del proyecto del curso.

### Estructura del proyecto

```text
mi-primer-sitio/
│
├── index.html
│
├── pages/
│   ├── sobre-mi.html
│   ├── proyectos.html
│   ├── servicios.html
│   └── contacto.html
│
└── img/
    └── foto.jpg
```

### Consigna

Construir un sitio web personal sobre una temática elegida.

Puede ser un portafolio, un emprendimiento, una marca o un proyecto personal.

El sitio debe contar con una página principal y cuatro páginas secundarias.

### Requisitos

- Estructura HTML5 válida.
- Etiquetas `html`, `head` y `body`.
- Uso de etiquetas semánticas.
- Encabezado y navegación.
- Contenido principal organizado en secciones.
- Jerarquía correcta de títulos.
- Una imagen dentro de `figure`, con `figcaption`.
- Imágenes con texto alternativo.
- Enlaces funcionales entre las cinco páginas.
- Código ordenado e indentado.
- Archivos secundarios dentro de la carpeta `pages`.

### Checklist de revisión

- [ ] El archivo `index.html` está en la raíz.
- [ ] Existen cuatro páginas secundarias.
- [ ] Todas las páginas tienen una estructura HTML válida.
- [ ] Los enlaces funcionan correctamente.
- [ ] Se utilizan etiquetas semánticas.
- [ ] Los títulos mantienen una jerarquía coherente.
- [ ] Las imágenes cargan correctamente.
- [ ] Las imágenes tienen atributos `alt` apropiados.
- [ ] Se incluye `figure` y `figcaption`.
- [ ] El código está correctamente organizado.

### Entrega

Según el programa del curso, se deberá compartir el enlace a un repositorio público de GitHub con el proyecto.

---

# 9. REPASO Y CIERRE DEL MÓDULO

## Actividad: Encontrar los errores

### 💻 Demostración

Abrir el proyecto y provocar intencionalmente algunos errores:

1. Eliminar el cierre de una etiqueta.
2. Escribir incorrectamente una ruta.
3. Utilizar un `id` que no existe.
4. Cambiar el nombre de una imagen.
5. Colocar contenido visible dentro del `head`.
6. Alterar la jerarquía de encabezados.

### 💬 Preguntas para resolver en conjunto

- ¿Qué está fallando?
- ¿Dónde buscarían el error?
- ¿Cómo podrían comprobar qué sucede?
- ¿Qué herramientas del navegador utilizarían?

## Reflexión final

Al comenzar el módulo teníamos un archivo con un texto que decía "Hola, mundo".

Ahora tenemos un sitio con distintas páginas, contenido organizado, enlaces, imágenes y formularios.

### Pregunta de cierre

**¿Qué creen que todavía le falta a nuestro sitio para parecerse a las páginas que utilizamos todos los días?**

Con esta pregunta introducimos el siguiente módulo: **CSS**.

---

# 10. RECOMENDACIONES PARA EL LIVE CODING

## Durante las explicaciones

- Escribir el código progresivamente.
- Evitar pegar grandes fragmentos de código ya resueltos.
- Explicar por qué se utiliza cada etiqueta.
- Mostrar constantemente el resultado en Chrome.
- Preguntar antes de resolver un error.
- Relacionar cada concepto con sitios reales.

## Durante las actividades

- Dar consignas breves y claras.
- Dejar tiempo para que los estudiantes escriban código.
- Revisar errores comunes.
- Resolver ejemplos en conjunto.
- Priorizar la comprensión por encima de memorizar etiquetas.

## Idea central del módulo

**No se trata solamente de aprender etiquetas HTML. Se trata de comprender cómo se estructura la información de una página web y cómo el navegador interpreta ese contenido.**
