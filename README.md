
# Gestión de Tareas

Este es un proyecto de gestión de tareas desarrollado con Ruby on Rails y postgreSQL. El proyecto permite a los usuarios crear, editar y eliminar tareas, así como organizarlas en categorías.

## Características

- Crear, editar y eliminar tareas.
- Crear, editar y eliminar categorías.
- Asignar tareas a categorías.
- Listar tareas por categoría.

## Modelos

### Task

- **id**: Integer
- **title**: String
- **description**: Text
- **due_date**: Date
- **completed**: Boolean
- **category_id**: Integer (Referencia a Category)

### Category

- **id**: Integer
- **name**: String

## Requisitos

- Ruby 3.0.0 o superior
- Rails 6.1.0 o superior
- PostgreSQL

## Instalación

1. Clona el repositorio:

    ```sh
    git clone https://github.com/tu-usuario/gestion-de-tareas.git
    cd gestion-de-tareas
    ```

2. Instala las gemas necesarias:

    ```sh
    bundle install
    ```

3. Configura la base de datos (ajusta el archivo config/database.yml con las credenciales de tu base de datos):

    ```sh
    rails db:create
    rails db:migrate
    ```

4. Inicia el servidor:

    ```sh
    rails server
    ```

5. Abre tu navegador y ve a `http://localhost:3000`.

## Uso

En el menú, puedes dirigirte a la página de categorías o directamente a la página de gestión de tareas.

### Tareas

- **Crear una tarea**: Ve a `/tasks/new` y completa el formulario.
- **Editar una tarea**: Ve a `/tasks/:id/edit` y modifica los campos necesarios.
- **Eliminar una tarea**: Ve a `/tasks/:id` y haz clic en el botón de eliminar.
- **Listar tareas**: Ve a `/tasks` para ver todas las tareas.

### Categorías

- **Crear una categoría**: Ve a `/categories/new` y completa el formulario.
- **Editar una categoría**: Ve a `/categories/:id/edit` y modifica los campos necesarios.
- **Eliminar una categoría**: Ve a `/categories/:id` y haz clic en el botón de eliminar.
- **Listar categorías**: Ve a `/categories` para ver todas las categorías.


