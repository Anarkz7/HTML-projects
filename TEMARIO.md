
### **Apuntes de HTML: La Guía Definitiva**

---

1. Estructura Básica del Documento (Esqueleto de tu Web)
<!DOCTYPE html>

<html>

<head>

<meta charset="UTF-8">

<title>Título del Head</title>

<link rel="icon" href="imagenes/favicon.png" type="image/png">: Esta etiqueta enlaza un icono de página (conocido como favicon) que aparece en la pestaña del navegador, en los marcadores y en los resultados de búsqueda.

rel="icon": Especifica que el recurso enlazado es el icono de la página.

href="imagenes/favicon.png": La ruta donde se encuentra tu archivo de icono. Puede ser .ico, .png, .gif, etc.

type="image/png": Indica el tipo de archivo de la imagen, ayudando al navegador a interpretarlo correctamente.

<body>

#### **2. Estructura Semántica y Contenedores (Organizando tu Contenido)**

Estas etiquetas dan significado a las diferentes partes de tu página, lo que mejora la accesibilidad y el SEO.

* `<header>`: Representa el **contenido introductorio o de navegación** de una sección o de toda la página (ej: logo, título principal, menú de navegación).
* `<nav>`: Contiene los **enlaces de navegación** principales de tu sitio.
* `<main>`: Define el **contenido principal o central** del documento. Solo debe haber uno por página.
* `<article>`: Encapsula **contenido independiente y auto-contenido**, como una entrada de blog, una noticia o un comentario.
* `<section>`: Define una **sección genérica** de contenido temáticamente agrupado. Un `article` puede contener varias `section`s, y viceversa.
* `<aside>`: Representa contenido que está **indirectamente relacionado con el contenido principal**, como una barra lateral, un glosario o anuncios.
* `<footer>`: Contiene el **pie de página** de una sección o de toda la página (ej: información de copyright, enlaces de contacto, autor).
* `<div>`: Un **contenedor genérico en bloque** para agrupar elementos y aplicarles estilos con CSS. No tiene significado semántico por sí mismo.
* `<span>`: Un **contenedor genérico en línea** para aplicar estilos a una parte del texto o a pequeños elementos. No tiene significado semántico por sí mismo.

---

#### **3. Texto y Títulos (Dando Jerarquía y Formato)**

Etiquetas para estructurar y presentar el texto.

* `<h1>` a `<h6>`: Definen **encabezados** de diferente nivel. `<h1>` es el más importante y `<h6>` el menos. Usar correctamente la jerarquía es crucial para la accesibilidad y el SEO.
* `<p>`: Define un **párrafo** de texto.
* `<br>`: Inserta un **salto de línea**. Es un elemento vacío.
* `<hr>`: Crea una **línea horizontal** temática, usada para separar contenido. Es un elemento vacío.

**Formato de Texto Específico:**

* `<b>Texto b</b>`: Pone el texto en **negrita**, pero sin implicar importancia adicional (más por estilo visual).
* `<strong>Texto strong</strong>`: Pone el texto en **negrita** e indica que es **importante** o tiene una fuerte relevancia semántica.
* `<i>Texto i cursiva</i>`: Pone el texto en *cursiva*, sin implicar énfasis adicional (más por estilo visual).
* `<em>`: Pone el texto en *cursiva* e indica **énfasis**.
* `<u>Texto subrayado</u>`: **Subraya** el texto. Generalmente, se desaconseja para evitar confusiones con enlaces.
* `<sub>`: Define **texto de subíndice** (ej: H₂O). Útil para fórmulas químicas o notas al pie.
* `<sup>`: Define **texto de superíndice** (ej: X²). Útil para potencias o medidas de la superficie de un suelo.
* `<q>`: Define una **cita corta en línea**. El navegador suele añadir comillas. Ejemplo: `<q>comillas</q>`.
* `<abbr title="World Health Organitacion, Organización Mundial de la salud.">WHO, OMS</abbr>`: Representa una **abreviatura o acrónimo**. El atributo `title` proporciona la descripción completa al pasar el ratón.
* `<cite>Resumen anual estadístico</cite>`: Se usa para el **título de una obra creativa** (libro, película, canción, etc.).
* `<address>`: Define la **información de contacto** del autor/propietario de un documento o sección. Ejemplo: `<address>contacto o sección de direcciones</address>`.
* `<bdo dir="rtl">`: Sobrescribe la dirección del texto actual. `rtl` (right-to-left) para idiomas que se escriben de derecha a izquierda.
* `<blockquote>`: Se usa para **citas largas** que ocupan varias líneas o un párrafo completo.
* `<ins>`: Indica texto que ha sido **insertado** en el documento.
* `<del>`: Indica texto que ha sido **eliminado** del documento.

---

4. Enlaces e Imágenes (Navegación y Elementos Visuales)
Cómo conectar tu página a otros recursos y mostrar contenido gráfico.

<a href="https://enlace">Enlace web</a>: Crea un hipervínculo.

href: Especifica la URL de destino del enlace.

target="_blank": Un atributo común para <a> que abre el enlace en una nueva pestaña del navegador.

<img src="imagen.jpg" alt="Kiko Palomares">: Incrusta una imagen.

src: Ruta de la imagen.

alt: Texto alternativo para la imagen, esencial para la accesibilidad y si la imagen no carga. Siempre debe incluirse.

Imagen como Enlace (NUEVO): Para hacer que una imagen funcione como un enlace, simplemente tienes que colocar la etiqueta <img> dentro de una etiqueta <a>.

Estructura:

HTML

<a href="https://www.pagina-destino.com">
  <img src="ruta/de/tu/imagen.png" alt="Descripción de la imagen y el enlace">
</a>
Ejemplo práctico:

HTML

<a href="index.html">
  <img src="imagenes/logo.svg" alt="Logo de la empresa, enlace a la página principal">
</a>
El usuario puede hacer clic en cualquier parte de la imagen para navegar a la URL especificada en el href del enlace <a>.

<figure> y <figcaption>: Para agrupar imágenes con su leyenda.

#### **5. Listas (Organizando Información)**

Para presentar datos de forma estructurada.

* `<ol>`: Crea una **lista ordenada** (los elementos se numeran automáticamente).
    * `<li>Nombre 1</li>`: Define cada **elemento** de una lista ordenada o no ordenada.
* `<ul>`: Crea una **lista no ordenada** (los elementos se marcan con viñetas).
    * `<li>Nombre 1</li>`: Define cada **elemento** de una lista ordenada o no ordenada.
* `<dl>`: Define una **lista de descripciones**.
* `<dt>`: Define el **término** o nombre en una lista de descripciones.
* `<dd>`: Define la **descripción** del término en una lista de descripciones.

---

#### **6. Tablas (Datos en Filas y Columnas)**

Para mostrar datos tabulares.

* `<table>`: Define una **tabla**.
    * `border="1"`: Un atributo HTML antiguo para añadir un borde (se recomienda hacer esto con CSS).
    * `cellpadding="6"`: Espacio entre el contenido de la celda y su borde (mejor con CSS).
    * `cellspacing="1"`: Espacio entre las celdas de la tabla (mejor con CSS).
* `<tr>`: Define una **fila** en la tabla (table row).
* `<th>`: Define una **celda de encabezado** de la tabla (table header). Por defecto, el texto es negrita y centrado.
    * `rowspan="2"`: Un atributo para `<th>` o `<td>` que hace que la celda **ocupe dos o más filas**.
    * `colspan="2"`: Un atributo para `<th>` o `<td>` que hace que la celda **ocupe dos o más columnas**.
* `<td>`: Define una **celda de datos** en la tabla (table data).
* `<thead>`: Agrupa las **filas de encabezado** de la tabla.
* `<tbody>`: Agrupa las **filas del cuerpo** de la tabla.
* `<tfoot>`: Agrupa las **filas del pie** de la tabla.

---

#### **7. Multimedia (Vídeos y Otros)**

Cómo integrar contenido audiovisual.

* `<video width="820" height="400" controls>`: Incrusta un **reproductor de vídeo**.
    * `width`, `height`: Dimensiones del reproductor.
    * `controls`: Añade los controles de reproducción estándar (pausa, volumen, etc.).
    * `autoplay`: El vídeo comienza a reproducirse automáticamente al cargar la página.
    * `muted`: El vídeo se reproduce automáticamente, pero silenciado.
    * `loop`: El vídeo se reinicia automáticamente al finalizar.
* `<source src="video.mp4" type="video/mp4">`: Define **múltiples fuentes de vídeo** para el navegador, permitiendo elegir el formato compatible.
* `<iframe>`: Incrusta **otra página HTML** dentro de la página actual. Se puede usar para insertar vídeos de YouTube, mapas, etc. (Ejemplo: insertar un par de vídeos en el periódico).

---

#### **8. Formularios (Interacción con el Usuario)**

(No has incluido etiquetas de formulario en tu código, pero son fundamentales y las mencionamos en la guía anterior. Asegúrate de repasarlas).

* `<form>`: El contenedor de un formulario.
* `<input>`: Elemento de entrada de datos (text, password, email, number, checkbox, radio, submit, date, etc.).
* `<textarea>`: Área de texto multilinea.
* `<label>`: Etiqueta descriptiva para un control de formulario.
* `<select>`: Lista desplegable.
* `<option>`: Opción dentro de un `<select>`.
* `<button>`: Botón interactivo.

---

### **Consejos Adicionales para tu Examen**

* **Atributos**: Recuerda que muchas etiquetas tienen atributos que modifican su comportamiento (ej: `href` en `<a>`, `src` y `alt` en `<img>`). Presta atención a los más comunes.
* **Semántica**: Piensa en el "significado" de cada etiqueta. Usar `<h1>` para el título principal es mejor que usar `<b>` y un tamaño de fuente grande, porque `<h1>` comunica que es un título importante, mientras que `<b>` solo cambia el estilo.
* **Practica con ejemplos**: Intenta crear pequeñas páginas usando estas etiquetas. La memoria muscular de escribir el código es muy efectiva.
* **Validación**: Aunque no lo has mencionado, en un entorno profesional es importante validar el HTML para asegurar que es correcto.

