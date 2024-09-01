# mkdoc-test
Prueba de Mkdoc para generar documentación 

## Instalación de Mkdoc

### Prerrequisitos
- Contar con Python instalado [aquí](https://www.python.org/downloads/)

### Pasos
- Ejecutar los siguientes comandos para instalar Mkdoc
```bash
pip install mkdocs
pip install mkdocs-material
```
El segundo comando es para instalar material y poderlo usar como tema.

### Crear proyecto
- Para crear un proyecto de documentación con Mkdoc, se debe ejecutar con el comando
```bash
mkdocs new mkdocs-test
```
- Ingresamos a la carpeta generada
```bash
cd mkdocs-test
```

- Debe tener una estructura 

```plainttext
├── docs/
│   ├── index.md
├── mkdocs.yml
```

- Dentro de `docs/` se deben colocar todos los archivos `.md` que van a contener toda la documentación a mostrar.
- En el archivo mkdocs.yml se configura el sitio de documentación.



