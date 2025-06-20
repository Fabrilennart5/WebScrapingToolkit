# 📦 Recursos de la Clase 4: Persistencia de Datos y Formatos de Salida 📦


¡Hola! Bienvenido/a a los recursos para la **Clase 4** de nuestro curso.

En esta sesión, nos centraremos en un paso crucial del web scraping: **cómo y dónde almacenar los datos** que extraemos. La elección del formato adecuado es clave para que tu información sea útil y accesible.

## 📊 Formatos Comunes para Almacenar Datos Web

Una vez que extraes datos de la web, la siguiente pregunta es: **¿dónde los guardas?** Aquí te presentamos un resumen de los formatos más utilizados en web scraping y por qué son valiosos:

* **JSON (JavaScript Object Notation)**:
    * **¿Qué es?**: Un formato ligero y legible para intercambiar datos, ideal para estructuras de datos anidadas.
    * **¿Cuándo usarlo?**: Para datos con jerarquía compleja, integración con APIs, o transmitir datos entre servicios.
    * **Recurso**: [https://www.json.org/json-es.html](https://www.json.org/json-es.html)

* **CSV (Comma Separated Values)**:
    * **¿Qué es?**: Un formato de texto simple donde los valores están separados por comas. Ideal para datos tabulares.
    * **¿Cuándo usarlo?**: Para datos simples de filas y columnas, fácil de abrir en hojas de cálculo como Excel o Google Sheets.
    * **Recurso**: [Wikipedia - Valores separados por comas](https://es.wikipedia.org/wiki/Valores_separados_por_comas)

* **Excel (Archivos .xlsx)**:
    * **¿Qué es?**: Formato propietario de Microsoft Excel que permite datos tabulares con formato, múltiples hojas y fórmulas.
    * **¿Cuándo usarlo?**: Para compartir datos con usuarios no técnicos, análisis directos en la hoja de cálculo o cuando se requiere formato visual. Necesita librerías Python como `openpyxl` o `pandas` para exportar.
    * **Recurso**: [Microsoft Office - Acerca de los formatos de archivo de Excel](https://support.microsoft.com/es-es/office/acerca-de-los-formatos-de-archivo-de-excel-1a980967-73d8-4e89-af0e-316279f53e6b)

* **Bases de Datos (ej., SQL, NoSQL)**:
    * **¿Qué son?**: Sistemas organizados para almacenar y gestionar grandes volúmenes de datos de forma eficiente.
    * **¿Cuándo usarlas?**: Para proyectos a gran escala, consultas complejas, integridad de datos o acceso concurrente. (Este es un tema más avanzado).
    * **Recurso (Ejemplo SQL)**: [PostgreSQL - Documentación oficial](https://www.postgresql.org/docs/)

---

## 🚀 Próximos Pasos

Una vez que revises estos formatos, te invitamos a sumergirte en el material principal de la clase:

* Dirígete al cuaderno interactivo: `quarto/Clase04.qmd`. Allí verás ejemplos prácticos sobre cómo guardar los datos extraídos en algunos de estos formatos.

¡A seguir explorando el apasionante mundo del web scraping y la persistencia de datos!