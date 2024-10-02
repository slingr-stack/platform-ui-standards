+++
title = 'First Page'
date = 2024-10-02T12:03:48-03:00
draft = true
+++

# Guia de UX para desarolladores
![Slingr logo](https://platform-docs.slingr.io/images/vendor/slingr_blue.png)

## **Objetivo**

Esta guía tiene como propósito principal establecer y documentar recomendaciones y mejores prácticas para diseñar y evaluar nuestro producto (SLINGR) centrado en el usuario. Esta debe ser un soporte para nuestros desarrolladores Front-End, así mantener consistencia en toda la plataforma, también reducir errores y simplificar los tiempos de desarrollo.

## **Principios Generales**

Es necesario seguir lo que llamamos "Principios Generales de Diseño" para asegurar que la aplicación sea eficiente, intuitiva y agradable tanto para los usuarios asi como tambien los clientes finales. Estos principios ayudan a mantener la coherencia y la calidad en todo el proceso de desarrollo. A continuación, se describen algunos de los principios más importantes:

#### 1. **Consistencia**
La consistencia es crucial para crear una experiencia de usuario intuitiva. Los usuarios deben poder anticipar el comportamiento del sistema en base a interacciones previas. La consistencia se aplica en varios niveles:
- **Visual:** Uso uniforme de colores, tipografías, y estilos de botones, headers, contenedores, etc... en toda la aplicación.
- **Funcional:** Comportamiento predecible de las interacciones, como clics, deslizamientos y toques.
- **Terminología:** Uso coherente de términos y mensajes en toda la aplicación.
 
**Ejemplo:** Si un botón de "Guardar" siempre esta del lado derecho en una sección del runtime, debe debe estar del lado derecho en todas las secciones.

#### **2. Usabilidad**
La usabilidad se refiere a qué tan fácil y eficiente es para los usuarios alcanzar sus objetivos en la aplicación. Un buen diseño debe facilitar una curva de aprendizaje rápida y minimizar los errores del usuario.
- **Intuición:** La aplicación debe ser fácil de aprender sin la necesidad de una extensa capacitación.
- **Accesibilidad:** El diseño debe considerar a todos los usuarios.
- **Retroalimentación:** Proporcionar indicaciones claras de las acciones realizadas, como confirmaciones o mensajes de error.

**Ejemplo:** Un formulario con validación en tiempo real que muestre mensajes de error claros y específicos facilita a los usuarios completar la tarea correctamente.

#### **3. Retroalimentación y Visibilidad**
Los usuarios deben recibir retroalimentación inmediata de sus acciones y deben poder ver el estado actual del sistema.
- **Retroalimentación inmediata:** Confirmar acciones, como clics en botones, con indicaciones visuales o auditivas.
- **Visibilidad del estado:** Mostrar información del sistema relevante, como el progreso de una tarea o notificaciones de error.

**Ejemplo:** Una barra de progreso que muestra el estado de una descarga o actualización.

#### **4. Diseño Centrado en el Usuario**
Los desarrolladores deben poner a los usuarios en el centro del proceso de diseño, entendiendo sus necesidades y comportamientos.
- **Investigación de usuarios:** Conducir pruebas de usuario y estudios para entender las necesidades reales de los usuarios.
- **Iteración:** Revisar y mejorar el diseño continuamente basado en la retroalimentación del usuario.

#### **5. Simplicidad y Minimalismo**
La simplicidad en el diseño reduce la carga cognitiva de los usuarios y facilita la navegación.
- **Eliminar lo innecesario:** Mantener solo los elementos esenciales y eliminar la complejidad innecesaria.
- **Claridad:** Diseñar interfaces limpias y claras con un enfoque en las tareas principales.

**Ejemplo:** Un diseño de pantalla de inicio con acceso directo a las funciones más usadas y una navegación mínima.

### _Importancia de estos Principios_

Seguir estos principios no solo mejora la experiencia del usuario, sino que también:
- **Fomenta la uniformidad:** Facilita la colaboración entre equipos de desarrollo y diseño.
- **Reduce errores:** Minimiza los errores y la frustración del usuario.
- **Mejora la eficiencia:** Aumenta la productividad del usuario y reduce la carga de soporte técnico.
- **Incrementa la satisfacción del usuario:** Conduce a una mayor adopción y retención de la aplicación.

# Lineamientos de diseño visual para Runtime
## **Fuente**

Como fuente principal en Slingr utilizamos *Open Sans* en 14px.

## **Temas y colores**

Los temas se componen del siguiente listado de colores:
- Primary ()
- Secondary
- Terciary
- Info

Estos generalmente son previstos por clientes y nos van a dar las indicaciones necesarias para poder identificar cada color.
Lo recomendable es que para los colores de **Warning, Danger y Success**, utilicemos amarillos rojos y verdes que hagan buen contraste con el color. Esto lo podemos obtener del cliente o bien consultando con UX.


## **Botones**
En cuanto los botones utilizamos una medida estandard de 30px de alto y el width dependera del contenido del mismo

La fuente debe respetar el lineamiento general (14px Open Sans)

Uso de color primary como color principal

slingr-button

Alineamiento de icono a la izquierda, 16px con un padding de 4px

## **Alertas**

Medidas: Full width x 52px

Estilos: Usaremos los colores por defeto de BS3 (NO BS5); es decir: info success danger warning. 

Contenido: el texto en dichas alertas debera estar en 14px, estilo bold (strong). Tambien puede contar con contenido secundario con la misma fuente pero en estilo normal, no bold.

## **Header principal de aplicación**

Medidas: full width x 50px (extensible segun el contenido, +12px por linea)

Este header es el que contiene el que proovera contexto al usuario para decirle en qué aplicacion se encuentra, a la vez de permitirle al desarrollador alocar acciones globales.

Elementos fijos:
- Menú hamburguesa: 

## **Header**

Medidas: full width x 50px.

Estilos: "Header Title" y  "Header Subtitle".

Padding:

En cuanto los estilos se divide en dos:
 - Title: Fuente de 16px, estilo bold (Strong) con fondo gris.
 - Subtitle: Fuente de 16px, estilo bold (Strong) con linea divisora gris, sin fondo.

 El color de fondo es el de por defecto #F1F1F1 y no agregamos customizacion de color al momento ya que es dificil hacer coincidir con el tema. 

## **Contenedores**

## **Modales**

Medidas:
- Auto
- SM
- LG
- XL


## **Labels**

Para los labels, hemos decidido modificar el comportamiento del responsive (wrappeo) para los HTML Tags. Si se llegase a hacer un ajuste a los labels por defecto, deberiamos alinearlos con estos cambios.

Le hemos agregado una mejoria para cortar los labels con la propiedad **word-break** setteada en **auto-phrase**. Esto se debe a que estabamos cortando las palabras para aprovechar espacio y no siendo concientes de la usabilidad de la misma. Respecto a grandes strings lo logico es poder ver toda la palabra en linea (por ejemplo un ID), asique este cambio se alinea con nuestra politica.

