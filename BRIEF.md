# Brief del proyecto: Fooddie
<!---
El brief de proyecto es un documento breve que explica qué vas a construir, para quién y cómo sabrás si el diseño funciona. Tiene una particularidad: es el primero que empiezas y el último que terminas. Lo comienzas el primer día con tu hipótesis y lo cierras cuatro semanas después, cuando ya puedes apoyar cada afirmación con los datos de tu investigación. Si al final de la órbita tu brief se parece demasiado a lo que escribiste el primer día, conviene que te preguntes si la investigación ha cambiado algo de lo que pensabas.
-->

En éste proyecto vamos a plantear la construcción de una aplicación Web o aplicación para dispositivos móviles en la que gran variedad de usuarios puedan encontrar una manera fácil de escoger que comida a domicilio o a qué establecimiento acudir en grupo. 
No se pretende crear una plataforma de pedido a domicilio ni un agente IA que recomiende platos, nos apoyamos directamente en el concepto de tener una plataforma para crear listas de deseo y colecciones de comida con diferentes temas para ponerlas en común con otros usuarios y ya sea por propia conciliación o por hacer un pequeño sorteo con las opciones propuestas, se pueda decidir que tomar.

Se considerará el diseño como funcional si tras realizar un pequeño prototipo y ponerlo a prueba como plantearemos posteriormente en este documento encontramos satisfactoria la experiencia del usuario, proponiendo un flujo y diseños intuitivos y que se adapten a las necesidades de potenciales usuarios.

## El problema que resuelve la aplicación
<!---
El problema que resuelve tu aplicación, contado desde el punto de vista de tus personas y respaldado por la investigación. Para comprobar si está bien planteado, imagina que no tienes ninguno de los datos que has recogido y vuelve a leer la frase. Si sigue pareciendo igual de convincente, es probable que describa un problema que has supuesto, porque los problemas que se descubren investigando vienen siempre acompañados de datos.
-->
El análisis-parálisis al pensar que comer cuando estas fuera o vas a pedir para llevar con tus amigos/familiares. El hecho de que salgas y siempre te pidas lo mismo de comer.

## El alcance
<!---
El alcance, es decir, qué entra en esta versión y qué se queda fuera. Ya lo decidiste al definir el MVP, así que en el brief solo tienes que recogerlo.
--->
Por el momento, el MVP va a englobar las funcionalidades de asignación de costes por comensal y de sorteo de temas o platos para poner de acuerdo a los usuarios de la aplicación.
Algunas funcionalidades como la creación de colecciones de comida (básicamente, gestión de etiquetas) o la exploración de estas, no estarán implementadas en el MVP.

## Las personas
<!---
Las personas, con un enlace a cada ficha y una línea que resuma quién es cada una y qué papel tiene en el diseño.
--->
[Enlace a FigJam](https://www.figma.com/board/g1oVTlD5MZU38cBQuDMn8h/Foodapp-FigJam?node-id=0-1&t=XVWRDXXDSCulieWB-1)

## Los criterios de éxito
<!---
Los criterios de éxito, que indican cómo sabrás si el diseño funciona. En este módulo se escriben como frases que se puedan comprobar sobre tus personas, por ejemplo "Lucía puede reservar una pista para el jueves sin ayuda y en menos de un minuto" o "Manuel puede completar la misma reserva con la letra ampliada al 200 % sin que ningún botón se salga de la pantalla". Estos criterios servirán de guion para las pruebas de la Órbita 5, de modo que al escribirlos ahora estás preparando tú mismo la forma en que se evaluará tu diseño (RA6-e, RA6-f).
--->
Los usuario podrán gestionar pedidos y gastos de forma rápida e intuitiva, así como tomar decisiones en grupo de forma satisfactoria y sin distracciones.

## Las restricciones
<!---
Las restricciones, que son los límites con los que tienes que trabajar: los tecnológicos (los del proyecto que coordinamos con DWEC y DWES), los de tiempo y los que imponen tus propias personas, como los dispositivos que usan, la conexión a internet que tienen o las tecnologías de apoyo que necesitan. Incluye también al menos una restricción ambiental, por ejemplo un peso máximo por página pensado para la persona que tiene peor conexión. Así aplicas desde el principio el criterio 2.4 de las Web Sustainability Guidelines, que pide integrar la sostenibilidad en todas las etapas del proceso de diseño, y tendrás una referencia concreta cuando empieces a maquetar en la Órbita 3.
--->
| Categoría | Restricción clave | Límite / Criterio |
| :--- | :--- | :--- |
| **Tecnológica** *(DWEC / DWES)* | Stack y compatibilidad | JS vanilla/Stack MERN. |
| | Arquitectura de API | Comunicación mediante **REST/JSON (MongoDB)**. Sin dependencias externas no aprobadas. |
| **Usuario** *(Personas)* | Dispositivos y soporte | Sensible a responsive (*Mobile-first* a Escritorio). Interfaz adaptable a **lectores de pantalla** y **magnificación**, **plantear text to speech como posibilidad pero sin implementación real**. |
| | Accesibilidad | **Navegación 100% por teclado**. Sin gestos táctiles complejos ni avisos exclusivamente sonoros. |
| **Ambiental** *(Red y Entorno)* | Peso de página *(Performance Budget)* | **Máximo 2 MB por vista** (imágenes optimizadas y minificación) para conexiones débiles (3G). |
| | Tiempos de carga | **FCP < 2 segundos** con throttling de red activado. |

# Órbita 2: sistema visual de [nombre de tu aplicación]

## Enlaces

| Qué | Enlace |
|---|---|
| Mockup + Estilos Web |[Mockup Web](https://www.figma.com/design/bECq10MRgdyF5GqBcu4VmR/MockupWeb-7-11?node-id=5027-344) |
| Prototipo Web |[Prototipo Web](https://www.figma.com/proto/bECq10MRgdyF5GqBcu4VmR/MockupWeb-7-11?node-id=5027-347&p=f&t=Gu6GuNdfFW6TfJat-0&scaling=scale-down&content-scaling=fixed&page-id=5027%3A344&starting-point-node-id=5027%3A347)|

## Dónde está cada cosa en Figma

| Entregable | Página y sección del archivo |
|---|---|
| Inventario de decisiones |  |
| Wireframes rediseñados con sus notas | [Wireframe](https://www.figma.com/design/bECq10MRgdyF5GqBcu4VmR/MockupWeb-7-11?node-id=0-1&p=f&t=Gu6GuNdfFW6TfJat-0) |
| Componentes | Componentes web | [En la página de componentes del mockup web](https://www.figma.com/design/bECq10MRgdyF5GqBcu4VmR/MockupWeb-7-11?node-id=5027-344&p=f&t=Gu6GuNdfFW6TfJat-0) 
| Mockups del happy path | Web | [Mockup de la web] (https://www.figma.com/design/bECq10MRgdyF5GqBcu4VmR/MockupWeb-7-11?node-id=5027-344&p=f&t=Gu6GuNdfFW6TfJat-0)
| Pantalla principal en el segundo ancho | x |
| Pantallas en modo oscuro | [Usar variable Dark Mode en el menú de variables](https://www.figma.com/design/bECq10MRgdyF5GqBcu4VmR/MockupWeb-7-11?node-id=5027-344&p=f&t=fB6Uj0cOClbnog6F-0) |
| Guía de estilo | Página de manual de la Web | [Manual de identidad visual en Figma](https://www.figma.com/design/bECq10MRgdyF5GqBcu4VmR/MockupWeb-7-11?node-id=3044-56&p=f&t=Gu6GuNdfFW6TfJat-0)

## Lista de comprobación de Figma

- [x] Variables en dos colecciones (primitivos y semánticos), con alias, modos claro y oscuro, ámbito, descripción y sintaxis de código.
- [x] Estilos de texto, efecto y retícula vinculados a las variables.
- [~] Componentes con Auto layout, variables, propiedades y variantes de estado.
- [~] Mockups construidos enteros con Auto layout y espacios sacados de variables.
- [ ] Pantalla principal en un segundo ancho, con los mismos componentes.
- [x] Modo oscuro aplicado con el selector de modo.
- [x] Prototipo que recorre el happy path completo.
- [x] Prueba 1 superada: al cambiar `color/primary`, cambian todas las pantallas a la vez.
- [x] Prueba 2 superada: con todos los mockups en modo oscuro, nada desaparece contra el fondo.

## Resumen de decisiones

### Rediseño de los wireframes
Sobre todo la pantalla de login, se han ajustado algunos menús desplegables y se han ajustado los espacios entre elementos de la página.

### Color
Definidos en la [guía de estilos](https://www.figma.com/design/bECq10MRgdyF5GqBcu4VmR/MockupWeb-7-11?node-id=3044-56&p=f&t=Gu6GuNdfFW6TfJat-0).

### Tipografía
Definidos en la [guía de estilos](https://www.figma.com/design/bECq10MRgdyF5GqBcu4VmR/MockupWeb-7-11?node-id=3044-56&p=f&t=Gu6GuNdfFW6TfJat-0).

### Espaciado y retícula
Definidos en la [guía de estilos](https://www.figma.com/design/bECq10MRgdyF5GqBcu4VmR/MockupWeb-7-11?node-id=3044-56&p=f&t=Gu6GuNdfFW6TfJat-0).

### Componentes
En el apartado componentes.

### Responsive y modo oscuro
ALgunos elementos al usar padding, se ha tenidoq ue corregir todo su tamañó, distribución en general de los elementos en la página de login.

## Uso de IA
Asistencia en la definición del formato de token semánticos y a la hora de realizar el modo oscuro. Se realizó una variación a mano de una pantalla del modo oscuro y se le pidió al agente de Figma que asignara las variables . El detalle está en el [CHANGELOG.md](CHANGELOG.md).

## Lo que ha quedado pendiente
Uso de estilos de espaciado, mockup de la APP, mejor nomenclatura de los componentes.
