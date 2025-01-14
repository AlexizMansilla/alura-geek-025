# AluraGeek

AluraGeek es un proyecto creado para el curso **Alura | ONE**. Es una aplicación de una sola página que muestra una lista de productos geek y permite a los usuarios agregar nuevos productos a través de un formulario. El proyecto utiliza **HTML**, **CSS**, **JavaScript** y **json-server** para manejar el envío de nuevos productos.

## Características

- **Diseño Responsivo**: Totalmente compatible con dispositivos móviles, se adapta a diferentes tamaños de pantalla.
- **Modo Oscuro/Claro**: Alterna entre temas oscuro y claro para una mejor experiencia de usuario.
- **Lista de Productos**: Muestra una colección de productos geek con elementos interactivos.
- **Formulario para Agregar Producto**: Los usuarios pueden agregar nuevos productos a la lista a través de un formulario.
- **Funcionalidad del Lado del Servidor**: El envío del formulario se procesa a través de **json-server**, que simula un back-end para manejar los productos.

## Tecnologías

- **HTML5**: Estructura y maquetado de las páginas web.
- **CSS3**: Estilos y diseño (usando Flexbox).
- **JavaScript**: Interactividad, manipulación del DOM y manejo de formularios.
- **json-server**: Herramienta para simular un back-end y manejar el almacenamiento de productos,

## Configuración de Lanzamiento

```json
{
  "configurations": [
    {
      "type": "node",
      "request": "launch",
      "name": "Launch Program",
      "program": "${workspaceFolder}/${input:programPath}",
      "preLaunchTask": "npm: run"
    }
  ],
  "inputs": [
    {
      "type": "pickString",
      "id": "programPath",
      "description": "Select the entry point for your application",
      "options": [
        "js/api.js",
        "js/dom.js",
        "js/main.js"
      ]
    }
  ]
}
