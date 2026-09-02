# DataProject: Lógica y Consultas SQL

Proyecto práctico de análisis y manipulación de datos relacionales utilizando la base de datos **Sakila / DVD Rental** sobre **PostgreSQL**, gestionado a través de **DBeaver**.

---

## 📋 Descripción del Proyecto

El objetivo de este proyecto es demostrar el dominio de la lógica SQL mediante la resolución de 64 ejercicios prácticos:

* Consultas monotabla con filtros condicionales y agregaciones (`GROUP BY`, `HAVING`).
* Relaciones relacionales entre tablas (`INNER JOIN`, `LEFT JOIN`, `CROSS JOIN`).
* Subconsultas escalares y correlacionadas.
* Creación de vistas persistentes (`VIEW`).
* Definición y manipulación de tablas temporales (`TEMPORARY TABLE`).
* Estandarización y buenas prácticas en sintaxis SQL.

---

## 🛠️ Tecnologías y Entorno

* **Motor de Base de Datos:** PostgreSQL
* **Cliente de Gestión / IDE:** DBeaver Community Edition
* **Base de Datos:** Sakila (esquema `public`)
* **Control de Versiones:** Git / GitHub

---

## 🗂️ Estructura del Repositorio

* `consultas_data_project.sql`: Script SQL completo con las 64 consultas resueltas y ordenadas.
* `postgres - proyecto_sql - público.png`: Diagrama Entidad-Relación (ER) exportado de la base de datos.
* `BBDD_Proyecto_shakila_sinuser.sql`: Script original con la estructura e inserción de datos de la base de datos.
* `LÉAME.md`: Documentación del proyecto.

---

## 📊 Diagrama Entidad-Relación (ER)

Esquema visual generado desde DBeaver correspondiente al **Ejercicio 1**:

![Esquema de la BBDD](./postgres%20-%20proyecto_sql%20-%20p%C3%BAblico.png)

---

## 🚀 Instrucciones de Ejecución

1. **Cargar la base de datos:** Ejecutar el archivo `BBDD_Proyecto_shakila_sinuser.sql` sobre una base de datos PostgreSQL vacía llamada `proyecto_sql`.
2. **Consultas analíticas:** Abrir el archivo `consultas_data_project.sql` en DBeaver y ejecutar individualmente cada consulta (`Ctrl + Enter`).

---

## 📝 Aspectos Técnicos Destacados

* **Ejercicio 44 (CROSS JOIN):** Se incluye la consulta y la justificación teórica sobre por qué un producto cartesiano no aporta valor analítico real entre estas dos tablas.
* **Aritmética de fechas (Ejercicio 57):** Uso de intervalos nativos de PostgreSQL (`return_date - rental_date > INTERVAL '8 days').
* **Vistas y tablas temporales (Ejercicios 48, 51 y 52):** Uso de `CREATE VIEW` y `CREATE TEMPORARY TABLE` para persistir estructuras reutilizables.
