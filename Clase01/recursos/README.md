# ⚙️ Recursos y Configuración Inicial del Curso ⚙️

---

¡Bienvenido! Para asegurar un inicio fluido en el curso de Web Scraping, es fundamental configurar tu entorno de trabajo correctamente. Esta guía te ayudará paso a paso con la instalación de **Quarto**, la configuración de tu editor y la gestión de dependencias con entornos virtuales.

## 🚀 1. Instalación de Quarto

**Quarto** es una herramienta esencial que utilizaremos para la creación de cuadernos interactivos y la documentación.

Puedes descargarlo e instalarlo siguiendo las instrucciones oficiales en el siguiente enlace:

* **Descargar Quarto**: [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)

---

## 💻 2. Configuración del Editor de Código

Una vez que tengas Quarto instalado, te recomendamos instalar una **extensión o plugin** en tu editor de código preferido. Esto mejorará significativamente tu experiencia al trabajar con archivos Quarto (`.qmd`), facilitando la edición, previsualización y renderizado.

**Recomendaciones para editores populares:**

* **Visual Studio Code**: Busca la extensión oficial de Quarto en el Marketplace.
* **Neovim**: Existen varios plugins comunitarios que ofrecen soporte para Quarto.

---

## 🐍 3. Entorno Virtual y Dependencias de Python

Para mantener tu espacio de trabajo limpio y evitar conflictos entre diferentes proyectos de Python, es **altamente recomendable** usar un **entorno virtual**. El repositorio incluye un archivo `requirements.txt` con todas las librerías de Python necesarias para el curso.

---

### ➡️ 3.1. Creación y Activación del Entorno Virtual

Para mantener tus proyectos de Python organizados y sin conflictos, vamos a usar un **entorno virtual**. Sigue estos sencillos pasos para crearlo y activarlo. Nombraré tu entorno `.venv`:

1.  **Crea el entorno virtual:**

    ```bash
    python3 -m venv .venv
    ```

2.  **Activa el entorno virtual:**

    * **Para Linux / macOS:**

        ```bash
        source .venv/bin/activate
        ```

    * **Para Windows PowerShell:**

        ```powershell
        .venv\Scripts\Activate.ps1
        ```

---

### ➡️ 3.2. Instalación de las Librerías Necesarias

Una vez que tu entorno virtual esté **activado** (verás `(.venv)` al inicio de tu línea de comandos), puedes instalar todas las librerías necesarias para el curso. Estas están listadas en el archivo `requirements.txt`:

```bash
pip install -r requirements.txt