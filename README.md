
# Proyecto de Inteligencia de Negocios: Análisis de Datos de Store

## Descripción General

Este proyecto tiene como objetivo principal desarrollar un sistema de inteligencia de negocios basado en la información proveniente de una base de datos de una tienda (Store). A través de este proyecto, se implementó un flujo completo de **ETL (Extract, Transform, Load)** para la integración, limpieza y transformación de los datos, con el fin de construir un repositorio optimizado para el análisis de información.

Posteriormente, se diseñó e implementó un **Cubo OLAP (Online Analytical Processing)**, permitiendo realizar consultas analíticas multidimensionales sobre los datos de ventas, productos, clientes y empleados. Gracias al cubo OLAP, los usuarios pueden explorar la información desde distintas perspectivas, como tiempo, ubicación, categoría de productos, entre otras.

## Tecnologías Utilizadas

* **Base de Datos Relacional:** SQL Server (o la base que estés usando)
* **ETL:** SQL Server Integration Services (SSIS) / Herramienta de ETL utilizada
* **Cubo OLAP:** SQL Server Analysis Services (SSAS) / Herramienta OLAP utilizada
* **Lenguaje de Consulta:** SQL y MDX (para consultas multidimensionales)

## Proceso ETL

1. **Extracción:** Se extrajeron datos desde la base de datos operativa de la tienda, la cual contiene información sobre ventas, clientes, productos y empleados.
2. **Transformación:** Se realizaron procesos de limpieza, normalización de formatos, unificación de claves, manejo de datos nulos, y derivación de nuevas métricas de análisis.
3. **Carga:** Los datos transformados fueron cargados en el Data Warehouse, diseñando un esquema en estrella para facilitar el análisis.

## Cubo OLAP

El cubo OLAP fue diseñado para proporcionar análisis rápidos y eficientes sobre grandes volúmenes de datos. Las principales dimensiones del cubo son:

* **Tiempo:** Año, Mes, Día
* **Producto:** Categoría, Subcategoría, Nombre del Producto
* **Cliente:** Ubicación geográfica, Tipo de Cliente
* **Empleado:** Departamento, Cargo

Las principales métricas analizadas incluyen:

* Ventas Totales
* Cantidad de Productos Vendidos
* Descuentos Aplicados
* Utilidades

## Beneficios

* Exploración dinámica de datos mediante consultas multidimensionales.
* Identificación de tendencias de ventas por periodos, productos o regiones.
* Mejora en la toma de decisiones estratégicas para el negocio.
