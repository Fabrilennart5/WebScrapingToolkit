# Recursos para la configuración del curso

## Instalación de Quarto

Para seguir este curso, necesitarás tener **Quarto** instalado en tu computadora. Puedes descargarlo e instalarlo desde el siguiente enlace oficial:  
https://quarto.org/docs/get-started/

---

## Configuración del editor

Después de instalar Quarto, instala un plugin o extensión para tu editor de código favorito, ya sea Visual Studio Code, Neovim u otro, que te permita manejar archivos Quarto (`.qmd`). Esto facilitará la creación, edición y renderizado de tus documentos.

---

## Entorno virtual y dependencias

En el repositorio encontrarás un archivo `requirements.txt` con todas las librerías que usaremos durante el curso.

Antes de instalar estas librerías, es recomendable crear un **entorno virtual** para aislar las dependencias y evitar conflictos con otras instalaciones de Python en tu sistema.

### Comandos para crear y activar el entorno virtual

Crear entorno virtual llamado .venv
python3 -m venv .venv

Activar entorno virtual (Linux/macOS)
source .venv/bin/activate

Activar entorno virtual (Windows PowerShell)
..venv\Scripts\Activate.ps1

---

### Instalar las librerías necesarias

Con el entorno virtual activado, instala todas las dependencias del archivo `requirements.txt` con el siguiente comando:

pip install -r requirements.txt

---

Con esta configuración estarás listo para comenzar a trabajar en tus tareas de web scraping y documentación con Quarto de forma organizada y reproducible.