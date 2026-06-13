# Instalación

TaskList corre sobre [Node.js](https://nodejs.org), así que es lo único que necesitas
tener instalado antes de empezar. Si ya lo tienes, salta directo a
[Instalar las dependencias](#instalar-las-dependencias).

## Qué necesitas

| Requisito | Versión mínima | Para qué lo usa la app    |
| --------- | -------------- | ------------------------- |
| Node.js   | 18.x           | Ejecutar el servidor      |
| npm       | 9.x            | Bajar las dependencias    |
| Navegador | Cualquiera     | Abrir la interfaz         |

Para comprobar qué versión de Node tienes, ejecuta `node --version` en tu terminal.

## Instalar las dependencias

Clona el repositorio y deja que npm baje los paquetes. Los comandos son casi iguales
en todos los sistemas; cambia solo la terminal que uses:

=== "Linux / macOS"

    ```bash
    git clone https://github.com/usuario/tasklist.git
    cd tasklist
    npm install
    ```

=== "Windows"

    ```powershell
    git clone https://github.com/usuario/tasklist.git
    cd tasklist
    npm install
    ```

## Arrancar la app

Con las dependencias instaladas, levántala con:

```bash
npm start
```

Abre `http://localhost:3000` en el navegador y ya deberías ver la lista vacía, lista
para usar.

!!! tip "Si el puerto está ocupado"
    El 3000 es de los puertos más solicitados. Si otra app lo está usando, indícale
    a TaskList que arranque en otro: `PORT=4000 npm start`.

!!! warning "Si `npm install` falla"
    Casi siempre es por una versión de Node demasiado vieja. Revisa con
    `node --version` que tengas la 18 o superior antes de volver a intentarlo.
