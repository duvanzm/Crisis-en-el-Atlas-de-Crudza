# Crisis-en-el-Atlas-de-Crudza
Proyecto Grupal
Duvan A. Zuluaga

# WorldHub — Crisis en el Atlas de Crudzaso
Hola soy luis, me extraña araña que siendo mosca no me conozca.
## 1. El problema

Crudzaso lleva meses soñando con publicar un **Atlas visual** donde se puedan explorar diferentes **mundos, sistemas o realidades posibles**: ciudades imposibles, comunidades de desarrolladores, planetas inventados, escuelas extrañas, juegos teóricos, civilizaciones tecnológicas, etc.

La idea inicial era simple:

> “Una colección de páginas web que cualquiera pueda visitar para conocer estos mundos.”

El problema es que el equipo de diseño de Crudzaso colapsó:

* No hay estructura unificada para las páginas.
* No hay una guía clara de qué secciones debe tener cada mundo.
* Nadie ha preparado todavía una forma ordenada de colaborar con Git.
* Nada está publicado para que otros lo vean.

Por ahora solo saben esto:

* El Atlas debe construirse con **tecnología sencilla y accesible**.
* Tiene que ser **fácil de leer**, **semántico** y **responsivo**.
* Debe ser posible **colaborar varias personas en el mismo proyecto** sin pisarse el trabajo.
* Cada mundo debe tener su **propia página web estática**, **sin JavaScript ni frameworks**, pero bien pensada.

Crudzaso les entrega el problema y espera que ustedes definan **cómo** lo resuelven.
Lo único que sí deja cerrado son los **requerimientos mínimos** del resultado.

---

## 2. Lo que Crudzaso necesita que resuelvan

### 2.1 Equipos

* Organizarse en **equipos de 4 coders**.
* Cada equipo:

  * Elige un **nombre de equipo**.
  * Elige el **tema/concepto de su mundo** (libre).
  * Se organiza como quiera internamente: quién toca qué, quién investiga qué, etc.

> Crudzaso no asigna roles formales. Solo le importa que el resultado final exista y que se note el trabajo colaborativo.

---

## 3. Condiciones técnicas del Atlas

Crudzaso define estas restricciones:

### 3.1 Tecnología permitida

* **Obligatorio:**

  * HTML.
  * CSS.
* **Prohibido:**

  * JavaScript.
  * Librerías o frameworks CSS (Bootstrap, Tailwind, etc.).
  * Preprocesadores de CSS (SASS, SCSS, LESS, etc.).
  * Herramientas externas que generen toda la interfaz por ustedes.

---

## 4. Estructura mínima de cada mundo (la página)

Cada equipo debe crear una página principal `index.html` que represente **un mundo** dentro del Atlas de Crudzaso.

El tema es completamente libre, pero la página debe tener como mínimo:

### 4.1 Encabezado del mundo

* Un `<header>` con:

  * Nombre oficial del mundo.
  * Subtítulo o frase que lo resuma.
  * Opcional: logo, símbolo o icono del mundo.

### 4.2 Navegación interna

* Un bloque de navegación (`<nav>`) que:

  * Permita moverse entre secciones de la misma página.
  * Tenga al menos **3 enlaces** que apunten a secciones relevantes del mundo (usando anchors con `href="#algo"`).

### 4.3 Cuerpo principal (`<main>`)

Dentro de `main`, Crudzaso quiere ver al menos estas piezas:

#### a) Introducción al mundo

* Una **sección** que cuente:

  * De qué va este mundo.
  * Qué lo hace especial.
* Debe tener al menos:

  * Un título de sección.
  * Uno o más párrafos explicativos.

#### b) Atlas / catálogo de elementos (tarjetas)

Crudzaso quiere que cada mundo tenga una especie de “galería” o “atlas” de cosas importantes:

* Puede ser un catálogo de:

  * Lugares, personajes, reglas, artefactos, eventos, clanes, etc.
* Debe existir una sección dedicada a esto con:

  * Al menos **8 elementos** representados como tarjetas o bloques.
  * Cada elemento con:

    * Título.
    * Texto descriptivo corto.
    * Algún detalle visual (borde, fondo, icono, etc.).

Maquetación:

* Esta sección debe verse como un **mosaico o cuadrícula** en pantallas grandes.
* En pantallas pequeñas, debe reorganizarse para seguir siendo legible (por ejemplo, una columna).

#### c) Sistema / reglas / lógica del mundo

Crudzaso también necesita entender **cómo funciona** cada mundo:

* Una sección que describa:

  * Reglas del sistema,
  * normas internas,
  * fases,
  * jerarquías,
  * o lo que tenga sentido para ese mundo.
* Debe contener:

  * Un título.
  * Una lista (`<ul>` o `<ol>`) con al menos **5 puntos** claramente redactados.

#### d) Contenido complementario (opcional pero valorado)

* `aside`, glosario, curiosidades, notas, citas, etc.

### 4.4 Pie de página

Un `<footer>` que incluya:

* Nombre del equipo.
* Nombres completos de los integrantes.
* Año.
* Enlace al repositorio de GitHub.
* Enlace a la versión publicada (cuando exista).

---

## 5. Requisitos de HTML y semántica

Crudzaso no quiere solo divs apilados.

* Deben **investigar y aplicar** semántica HTML.
* En la página se espera ver, al menos:

  * `header`, `nav`, `main`, `section`, `article`, `footer`.
  * Opcionalmente `aside` u otras etiquetas semánticas si tienen sentido.

Además:

* En el `README.md` del proyecto, debe existir una sección llamada **“Semántica usada”** donde expliquen con sus palabras (muy breve):

  * Para qué usaron cada etiqueta semántica importante.
  * Mínimo 5 etiquetas explicadas.

---

## 6. Requisitos de CSS

Crudzaso solo especifica **qué quiere ver**, no cómo lograrlo (eso deben investigarlo ustedes):

* Debe existir al menos:

  * Un layout con **flexbox o grid** para las tarjetas del mundo.
  * Una **media query** para ajustar la visual a pantallas pequeñas.
  * Un efecto `:hover` en algún elemento (tarjetas, enlaces, etc.).
  * Una **clase reutilizable** (ej: un estilo de botones, etiquetas, etc.) usada en múltiples partes.

El diseño visual debe estar alineado con el tema de su mundo: colores, tipografías, espaciados, etc.

---

## 7. Colaboración con Git y ramas

Crudzaso quiere comprobar que los equipos no trabajan “todos en el mismo archivo a lo bruto”.

Reglas mínimas:

* Deben usar **Git y GitHub** para colaborar.
* Deben usar **ramas** de manera activa.
* La rama principal se llamará `main`.

### 7.1 Lo que Crudzaso espera ver en ramas

* Cada integrante del equipo debe haber trabajado en **al menos una rama distinta**.
* Se deben usar nombres de rama que tengan sentido, por ejemplo:

  * `feature/estructura-html`
  * `feature/estilos-base`
  * `feature/atlas-tarjetas`
  * `feature/responsivo`
  * `feature/footer`
* Cada rama representa una parte del trabajo y luego se integra a `main`.

No se exige seguir un Git Flow formal, pero sí:

* Evitar trabajar todo directo en `main`.
* Que existan **varias ramas** con cambios significativos.
* Que se vea un historial de merges donde el equipo haya unido su trabajo.

Cómo crear, cambiar, subir y fusionar ramas es parte de lo que deben **investigar y acordar** como equipo.

---

## 8. Publicación (“despliegue”) con GitHub Pages

Crudzaso no quiere que el Atlas viva solo en el código.
Cada mundo debe estar disponible como **página pública**.

* El proyecto debe **publicarse usando GitHub Pages**.
* El resultado debe ser una URL del estilo:

  * `https://usuario.github.io/nombre-del-repo`
* Esa URL debe aparecer en:

  * El `README.md` del repo del equipo.
  * El portafolio individual de cada coder.

Cómo activar GitHub Pages y configurarlo correctamente forma parte de lo que deben **investigar y resolver**.

---

## 9. Entrega esperada por Crudzaso

### 9.1 A nivel de equipo

Un repositorio público en GitHub que contenga:

* `index.html`
* `styles.css` (o los `.css` que definan, respetando las restricciones).
* `README.md` con:

  * Nombre del equipo.
  * Nombre del mundo.
  * Breve descripción del mundo.
  * Listado de integrantes con nombre completo.
  * Sección **“Semántica usada”** (mínimo 5 etiquetas).
  * Breve explicación (2–4 líneas) de cómo organizaron el trabajo con ramas.
  * URL pública del sitio en GitHub Pages.

En el historial del repositorio se debe notar:

* Uso de **ramas diferentes**.
* Varios commits con mensajes decentes (no solo “update” o “cosas”).

### 9.2 A nivel individual

Cada coder debe:

* Registrar este proyecto en su **repositorio personal de portafolio de Crudzaso**, indicando:

  * Nombre del mundo / proyecto.
  * En qué partes aportó (secciones, estilos, ramas).
  * Enlace al repositorio del equipo.
  * Enlace al sitio publicado.

---
