# mkdocs
MkDocs es una herramienta estática de generación de sitios web, ideal para crear documentación y páginas personales

**1. Instalación de MkDocs**

Primero, necesitas instalar MkDocs. Si no tienes pip instalado, instala pip primero.
```bash
pip install mkdocs
```
Para verificar que la instalación fue exitosa, puedes ejecutar:

```bash
mkdocs --version
```

**2. Crear un Nuevo Proyecto MkDocs**

Crea un nuevo proyecto utilizando el comando mkdocs new. Esto generará la estructura básica del proyecto.

```bash
mkdocs new my-personal-site
cd my-personal-site
```

**3. Editar el Archivo de Configuración mkdocs.yml**  

Edita el archivo mkdocs.yml para personalizar tu sitio. Aquí tienes un ejemplo básico:

```bash
site_name: My Personal Site
nav:
    - Home: index.md
    - About: about.md
    - Projects: projects.md
    - Contact: contact.md
theme:
    name: material
```

Este archivo define el nombre del sitio, la navegación y el tema. En este caso, estamos usando el tema material, que es un tema popular y atractivo para MkDocs.

Para instalar el tema material, necesitas instalar el paquete correspondiente:

```bash
pip install mkdocs-material
```

**4. Crear Contenido**  

Dentro del directorio docs/, puedes crear archivos Markdown (.md) para las diferentes secciones de tu sitio. Por ejemplo:

**5. Servir el Sitio Localmente**  

Para ver tu sitio en acción, puedes servirlo localmente utilizando el siguiente comando:

```bash
mkdocs serve
```

Abre tu navegador web y ve a http://127.0.0.1:8000/ para ver tu sitio en funcionamiento.

**6. Desplegar el Sitio**  

Cuando estés listo para desplegar tu sitio, puedes usar el comando mkdocs build para generar los archivos estáticos en el directorio site.

```bash
mkdocs build
```
El contenido del directorio site/ puede ser desplegado en cualquier servidor web. Para desplegar en GitHub Pages, puedes usar el comando gh-deploy de MkDocs:

```bash
mkdocs gh-deploy
```

## Personalización Adicional  

Puedes agregar estilos personalizados y scripts adicionales creando archivos CSS y JavaScript en los directorios docs/stylesheets/ y docs/javascripts/ respectivamente, y luego referenciándolos en el archivo mkdocs.yml.
