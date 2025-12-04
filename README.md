# 📊 Power BI – Análisis de Ventas para Tienda de Libros

Este proyecto consiste en un informe profesional de Power BI enfocado en analizar las ventas de una **tienda de libros**. Incluye un proceso completo de ETL, modelado de datos, creación de medidas DAX y desarrollo de un dashboard interactivo.

## 📁 Fuentes de Datos
- Archivo **CSV** con información de ventas (Orders, Customers, Books).
- Tabla **Calendar** generada en Power BI para soporte de inteligencia de tiempo.

## 🔧 Proceso ETL (Power Query)
Se realizaron transformaciones clave para preparar los datos:
- Corrección del formato decimal en precios.
- Conversión de columnas de fecha a tipo *Date*.
- Estandarización y limpieza general de campos.

## 🗄️ Modelo de Datos
Se utilizó un **esquema en estrella**, compuesto por:
- **Tabla de Hechos:** `Orders`
- **Tablas de Dimensión:** `Customers`, `Books`, `Calendar`
- Relaciones adecuadas con cardinalidad 1:* y la tabla Calendar marcada como tabla de fechas.

## 📐 Medidas DAX
Se crearon medidas explícitas para análisis:
- `Total Ventas`
- `Cantidad de Órdenes`
- `Ticket Promedio`
- Otras medidas complementarias para KPIs y visualizaciones

## 📊 Dashboard
El informe incluye:
- KPIs principales
- Gráfico de líneas de tendencia
- Gráfico de barras por categoría/producto
- Mapa por país/ciudad
- Segmentadores (fecha, ciudad, categoría)
- Botón de reinicio de filtros
