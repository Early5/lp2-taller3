# Lenguaje de Programación 2 - Taller 3

![Commits](https://badgen.net/github/commits/clubdecomputacion/lp2-taller3)
![Last Commit](https://img.shields.io/github/last-commit/clubdecomputacion/lp2-taller3)

## Autor

* Early Andrés Erazo

## Descripción del proyecto

El proyecto consiste en desarrollar una tienda virtual de productos tecnológicos utilizando Flask para la interfaz web y FastAPI para crear una API REST. La información de los productos y las categorías se almacena en una base de datos PostgreSQL.

La aplicación permite visualizar un catálogo de productos, consultar sus detalles y acceder a la información mediante endpoints de la API.

## Tecnologías utilizadas

* **Python:** lenguaje de programación utilizado para desarrollar la aplicación.
* **Flask:** framework utilizado para construir la tienda virtual.
* **FastAPI:** framework utilizado para desarrollar la API REST.
* **PostgreSQL:** sistema de gestión de bases de datos.
* **Docker Compose:** herramienta utilizada para ejecutar los servicios del proyecto.
* **HTML y CSS:** tecnologías utilizadas para construir y dar estilo a las páginas web.

## Funcionalidades

* Visualización del catálogo de productos.
* Consulta de los detalles de cada producto.
* Visualización de fotografías, marcas, SKU, precios y stock.
* Consulta de productos mediante la API REST.
* Filtrado de productos por categoría.
* Consulta de categorías.
* Almacenamiento de la información en PostgreSQL.

## Endpoints de la API

| Método | Endpoint           | Descripción                                             |
| ------ | ------------------ | ------------------------------------------------------- |
| GET    | `/`                | Consulta la ruta principal de la API.                   |
| GET    | `/productos/`      | Lista los productos y permite filtrarlos por categoría. |
| GET    | `/productos/{sku}` | Consulta un producto por su SKU.                        |
| GET    | `/categorias/`     | Lista las categorías disponibles.                       |

## Instalación y ejecución

### Requisitos

* Python.
* Docker y Docker Compose.
* Git.

### Pasos

1. Clonar el repositorio:

   ```bash
   git clone https://github.com/clubdecomputacion/lp2-taller3.git
   ```

2. Entrar a la carpeta del proyecto:

   ```bash
   cd lp2-taller3
   ```

3. Construir las imágenes e iniciar los servicios:

   ```bash
   docker compose up -d --build
   ```

4. Comprobar el estado de los servicios:

   ```bash
   docker compose ps
   ```

## Acceso a la aplicación

Cuando los servicios estén ejecutándose localmente, se puede acceder a:

* **Tienda virtual:** http://localhost:5000/
* **Documentación de la API:** http://localhost:8000/docs
* **Productos en formato JSON:** http://localhost:8000/productos/
* **Categorías en formato JSON:** http://localhost:8000/categorias/

## Documentación adicional

Consulta la guía del proyecto para obtener información complementaria sobre su desarrollo y funcionamiento:

[Ver GUIA.md](docs/GUIA.md)

## Detener los servicios

Para detener los contenedores del proyecto, ejecuta:

```bash
docker compose down
```
