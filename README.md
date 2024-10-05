# Script ETL de Ingredientes

## Descripción

Este script implementa un proceso ETL (Extracción, Transformación y Carga) que extrae datos desde una base de datos MongoDB, los procesa y actualiza una base de datos MariaDB utilizando campos JSON. Específicamente, actualiza los datos de `ingredientGroup` en el campo `extended_data` de la tabla `Recipes`.

## Autor
**Santiago Salvioli**

## Funcionalidades
- **Fuente de Datos:** Extrae datos de ingredientes de una colección en MongoDB.
- **Transformación de Datos:** Genera sentencias SQL `UPDATE` para actualizar la información de los ingredientes.
- **Destino de Datos:** Actualiza los campos JSON (`ingredientDescription`, `ingredientGroup`) en la tabla `Recipes` de MariaDB.

## Requisitos
Para ejecutar este script necesitas:
- Python 3.x
- MongoDB
- MariaDB

### Librerías de Python:
- `pymongo` para la integración con MongoDB
- `mysql-connector-python` para la conexión con MariaDB
- `dotenv` para gestionar las variables de entorno

Instala las dependencias con:
```bash
pip install pymongo mysql-connector-python python-dotenv
