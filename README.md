# medialab-invisible.github.io
medialab webpages

[Foro de desarrollo](https://github.com/orgs/medialab-invisible/discussions/1)

## Instrucciones de uso

### Pre-requisitos
- Instalar Hugo [https://gohugo.io/installation/](https://gohugo.io/installation/)
- Instalar git y clonar este repositorio `git clone git@github.com:medialab-invisible/medialab-invisible.github.io.git`
- Iniciar submódulos con `git submodule update --init --recursive`

### Añadir una nueva entrada

```
hugo new content content/posts/nueva-entrada.md
$EDITOR content/posts/nueva-entrada.md
```

En este archivo podemos editar el título (title), y añadir el contenido en formato markdown bajo la cabecera autogenerado. Una vez la entrada esté lista, indicamos que no es un borrador poniendo el valor de `draft` a `false`.

### Generar sitio

- Para iniciar un servidor usar el comando `hugo server -D` (-D incluye entradas en borrador).
- Para generar el sitio estático usar el comando `hugo` (no incluye entradas en borrador).

### Publicar sitio

Para publicar el sitio solo hace falta subir las nuevas entradas al repositorio de git, y la pipeline se encargará de publicar el sitio automágicamente en [medialab-invisible.github.io](https://medialab-invisible.github.io).

NO subas el directorio public/ al repositorio (la ruta está ignorada por defecto).
