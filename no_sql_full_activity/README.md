# Actividad Completa NoSQL (MongoDB + Redis)

Este repositorio contiene:
- Respuestas teóricas
- Comandos usados en MongoDB y Redis
- Reportes en PDF
- Caso de uso propio implementado

## Respuestas

### 1. ¿Qué es una base de datos NoSQL?
Las bases NoSQL permiten modelos flexibles como documentos, clave–valor, grafos o columnas.  
Diferencias clave: escalamiento horizontal y esquemas flexibles.

### 2. Rol de MongoDB
Base documental orientada a JSON/BSON. Excelente para datos semiestructurados.

### 3. Base de datos, colección y documento
Base → Colecciones → Documentos JSON.  
Ejemplo:
{
  "nombre": "Sara",
  "edad": 20,
  "skills": ["node", "mongo"],
  "ciudad": { "nombre": "Lima" }
}

### 4. Ventajas del esquema flexible
- No requiere migraciones complejas  
- Evoluciona con la aplicación  
Riesgo: inconsistencia si no se valida

### 5. Redis
Servidor de estructuras en memoria. Tipos: Strings, Hashes, Lists, Sets, Sorted Sets.

### 6. Dos tipos de datos de Redis
Hashes: representación de objetos ligeros.  
Lists: colas ordenadas.

### 7. Laboratorio de turnos
MongoDB → turnos persistentes  
Redis → cola rápida y turnos inmediatos

### 8. Laboratorio tamagochi
MongoDB → datos permanentes  
Redis → estados variables como energía o hambre

### 9. Diseño propio
Caso: Tienda online  
MongoDB → productos, usuarios, órdenes  
Redis → carrito temporal, sesiones, ranking de productos

### 10. Reflexión
MongoDB para datos complejos y permanentes.  
Redis para cache, sesiones y operaciones rápidas.
