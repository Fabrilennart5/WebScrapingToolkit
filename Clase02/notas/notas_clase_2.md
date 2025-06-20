# 📝 Notas de la Clase 2: Explorando Beautiful Soup y Códigos de Estado HTTP

¡Hola! En esta segunda sesión de nuestro curso de Web Scraping, nos adentraremos en el fascinante mundo de la extracción de datos web. Prepárate para aprender sobre una de las librerías más populares y potentes para esta tarea: **Beautiful Soup**. Además, abordaremos un tema crucial para cualquier web scraper: los **códigos de estado HTTP**, que nos informan sobre la respuesta de los servidores web.

---

## 🥣 Beautiful Soup: Tu Aliado para Analizar HTML

**Beautiful Soup** es una librería de Python diseñada para **analizar documentos HTML y XML**. Es increíblemente útil para el web scraping porque te permite navegar, buscar y modificar el árbol de análisis (parse tree) como si fuera una estructura de datos anidada de Python. Esto facilita enormemente la extracción de información específica de una página web, sin importar cuán compleja sea su estructura.

Con Beautiful Soup, podrás:

* **Encontrar elementos HTML** por su nombre de etiqueta, atributos (clases, IDs, etc.) o incluso por el texto que contienen.
* **Navegar por la estructura de la página** subiendo y bajando por el árbol HTML (padres, hijos, hermanos).
* **Extraer el texto o los atributos** de cualquier elemento que te interese.

Para que puedas profundizar y sacar el máximo provecho de esta herramienta, te dejamos el enlace a su **documentación oficial**:

* **Documentación de Beautiful Soup**: [https://www.crummy.com/software/BeautifulSoup/bs4/doc/](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
    * ¡Te recomendamos encarecidamente explorarla! Contiene ejemplos detallados y explicaciones claras que te serán de gran ayuda.

---

## 🚦 Entendiendo los Códigos de Estado HTTP: Las Señales de la Web

Cuando tu script de web scraping intenta acceder a una página web, el servidor de esa página responde con un **código de estado HTTP**. Estos códigos son como un semáforo o una señal que te indica si la solicitud fue exitosa, si hubo un error, si la página se movió, etc. Conocerlos es **fundamental** para diagnosticar problemas y escribir scripts de scraping robustos.

A continuación, te presentamos un resumen de los códigos de estado más comunes y su significado. ¡Cada uno de ellos te cuenta una historia sobre lo que pasó con tu solicitud!

| Código | Categoría           | Descripción General                                         | Qué Significa para ti (Web Scraping)                                                 |
| :----- | :------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------- |
| **1xx**| **Informativa** | La solicitud fue recibida y el proceso continúa.            | Raros de ver en scraping. Indican que el servidor está pensando.                     |
| **2xx**| **Éxito** | La acción fue recibida, entendida y aceptada.               | **¡Lo que buscas!** La página se cargó correctamente y puedes empezar a extraer datos. |
| **`200 OK`** | Éxito           | La solicitud ha tenido éxito.                               | **Ideal.** Significa que el contenido está disponible para ser procesado.             |
| **3xx**| **Redirección** | Es necesario tomar acciones adicionales para completar la solicitud.| La página se ha movido. Necesitas seguir la nueva URL para obtener el contenido.   |
| **`301 Moved Permanently`** | Redirección | La página solicitada ha sido movida permanentemente.        | Debes actualizar la URL en tu script si quieres acceder al contenido final.          |
| **`302 Found`** | Redirección | La página solicitada ha sido encontrada en una ubicación diferente.| La página se ha movido temporalmente. Tu script debería seguir la redirección.       |
| **4xx**| **Error del Cliente**| La solicitud contiene una sintaxis incorrecta o no puede ser cumplida.| **¡Atención!** Tu script o tu solicitud tienen un problema.                          |
| **`400 Bad Request`** | Error del Cliente | El servidor no pudo entender la solicitud debido a una sintaxis inválida.| Tu script envió una solicitud mal formada. Revisa los encabezados o parámetros.     |
| **`401 Unauthorized`** | Error del Cliente | Se requiere autenticación para acceder al recurso.         | Necesitas credenciales (usuario/contraseña, token) para acceder a esta página.      |
| **`403 Forbidden`** | Error del Cliente | El servidor se niega a autorizar la solicitud.             | El servidor te está bloqueando, quizás por no ser un navegador real o por políticas. |
| **`404 Not Found`** | Error del Cliente | El recurso solicitado no se encontró en el servidor.       | **La URL es incorrecta.** La página no existe o ha sido eliminada.                   |
| **`429 Too Many Requests`** | Error del Cliente | Has enviado demasiadas solicitudes en un tiempo determinado. | **¡Te están bloqueando por abuso!** Necesitas implementar pausas (delays) entre tus solicitudes. |
| **5xx**| **Error del Servidor**| El servidor falló al completar una solicitud aparente y válida.| **Problema en el sitio web.** No es tu culpa, el servidor tiene un fallo interno.     |
| **`500 Internal Server Error`** | Error del Servidor | El servidor encontró una condición inesperada que le impidió cumplir la solicitud.| Un error general del servidor. Podrías reintentar más tarde.                       |
| **`503 Service Unavailable`** | Error del Servidor | El servidor no está listo para manejar la solicitud.       | El servidor está sobrecargado o en mantenimiento. Reintenta más tarde.             |

---

¡Dominar estos conceptos te dará una base sólida para crear web scrapers más inteligentes y eficientes! En la práctica, aprenderás a manejar estas respuestas para que tus scripts puedan adaptarse a diferentes escenarios. ¿Listo para empezar a extraer datos?