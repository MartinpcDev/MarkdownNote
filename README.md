# Markdown Notes-Taking App

Challenge basado en [Markdown Notes](https://roadmap.sh/projects/markdown-note-taking-app)
Esta aplicación permite a los usuarios subir archivos en formato Markdown, verificar su gramática,
guardar las notas y renderizarlas en HTML. El objetivo es ofrecer una herramienta simple para
gestionar y visualizar notas en formato Markdown y, al mismo tiempo, aprender a manejar la carga de
archivos en una API RESTful.

## Características

La aplicación incluye las siguientes funcionalidades:

1. **Verificación de gramática**: Endpoint para verificar la gramática de una nota en Markdown.
2. **Guardar notas**: Endpoint para guardar una nota ingresada en texto Markdown.
3. **Listar notas**: Endpoint para listar las notas guardadas (archivos Markdown subidos).
4. **Renderizar notas**: Endpoint para devolver la versión HTML de una nota en Markdown,
   convirtiéndola a HTML para su visualización.

## Endpoints

1. **Verificar gramática**

    * **Descripción**: Permite analizar el texto en Markdown para identificar errores gramaticales.
    * **Método**: POST
    * **Ruta**: /notes/check-grammar
    * **Parámetro**: text (contenido de la nota en Markdown).
2. **Guardar nota**

    * **Descripción**: Permite guardar una nota en texto Markdown en el sistema.
    * **Método**: POST
    * **Ruta**: /notes/save
    * **Parámetro**: text (contenido de la nota en Markdown).
3. **Listar notas**

    * **Descripción**: Muestra una lista de las notas guardadas.
    * **Método**: GET
    * **Ruta**: /notes
4. **Renderizar nota**

    * **Descripción**: Convierte una nota en Markdown a HTML para su visualización.
    * **Método**: GET
    * **Ruta**: /notes/{id}
    * **Parámetro**: {id} (identificador de la nota guardada).