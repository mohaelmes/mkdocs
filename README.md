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

5. Crear Contenido
Dentro del directorio docs/, puedes crear archivos Markdown (.md) para las diferentes secciones de tu sitio. Por ejemplo:
