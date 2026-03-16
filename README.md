# 🍃 MONGODB DESDE CERO - GUÍA COMPLETA

**MongoDB desde Cero** es un sitio educativo completo diseñado para enseñar MongoDB desde los fundamentos hasta conceptos avanzados, con explicaciones claras, ejemplos prácticos y código listo para usar.

> *"MongoDB es la base de datos NoSQL más popular para aplicaciones modernas."*

---

## 🎯 ¿Qué es este Proyecto?

Este proyecto proporciona un recurso educativo gratuito para aprender MongoDB, incluyendo:

- **Documentación completa** de cada tema
- **Ejemplos de código** listos para ejecutar
- **Ejercicios prácticos** para reforzar el aprendizaje
- **Sitio web educativo** con navegación intuitiva

---

## 📚 Contenido del Curso

### Módulo 1: Fundamentos

1. **Introducción**
   - ¿Qué es NoSQL?
   - Diferencias entre SQL y NoSQL
   - Casos de uso de MongoDB

2. **Instalación**
   - MongoDB Community Server
   - MongoDB Compass (GUI)
   - MongoDB Atlas (Cloud)
   - Configuración inicial

3. **Conceptos básicos**
   - Documentos BSON
   - Colecciones
   - Tipos de datos
   - Operaciones CRUD

### Módulo 2: Intermedio

4. **Ejemplos prácticos**
   - Consultas con find()
   - Operadores de consulta
   - Índices
   - Agregaciones

5. **Buenas prácticas**
   - Modelado de datos
   - Indexación estratégica
   - Optimización de consultas
   - Schema design patterns

### Módulo 3: Avanzado

6. **Casos reales**
   - Replica Sets
   - Sharding
   - Backup y recovery
   - Monitoreo

7. **Proyecto final**
   - Aplicación MEAN/MERN completa
   - Implementación en producción

---

## 🗂️ Estructura del Proyecto

```
Practica-Nro02/
├── index.html          # Página principal
├── css/
│   └── styles.css      # Estilos del sitio
├── js/
│   └── main.js         # JavaScript del sitio
└── README.md
```

---

## 🚀 Cómo Usar este Proyecto

### Opción 1: Navegar el Sitio Web

1. Abre `index.html` en tu navegador
2. Navega por las secciones del curso
3. Haz clic en los temas para ver la documentación detallada

### Opción 2: Ejecutar los Ejemplos

1. Abre MongoDB Compass o mongosh
2. Conéctate a tu instancia de MongoDB
3. Ejecuta los scripts de ejemplo

### Requisitos

- **MongoDB 6.0** o superior
- **MongoDB Compass** o **mongosh**
- Navegador web moderno (Chrome, Firefox, Edge)

---

## 📝 Ejemplos Rápidos

### Insertar Documento

```javascript
db.usuarios.insertOne({
    nombre: "Juan",
    email: "juan@email.com",
    edad: 30,
    fechaRegistro: new Date()
});
```

### Consultar Documentos

```javascript
db.usuarios.find({
    edad: { $gte: 25 }
}).sort({ nombre: 1 });
```

### Actualizar Documento

```javascript
db.usuarios.updateOne(
    { email: "juan@email.com" },
    { $set: { edad: 31 } }
);
```

### Agregación

```javascript
db.ventas.aggregate([
    { $group: {
        _id: "$categoria",
        total: { $sum: "$monto" }
    }}
]);
```

---

## 🎓 Metodología de Aprendizaje

### 1. Leer la Teoría
Cada tema comienza con una explicación clara del concepto.

### 2. Ver Ejemplos
Los ejemplos de código muestran la aplicación práctica.

### 3. Practicar
Los ejercicios te permiten aplicar lo aprendido.

### 4. Experimentar
Modifica los ejemplos para entender cómo funcionan.

---

## 🔧 Comandos Esenciales

### Gestión de Bases de Datos

```javascript
// Listar bases de datos
show dbs;

// Usar una base de datos
use miBaseDeDatos;

// Eliminar base de datos
db.dropDatabase();
```

### Gestión de Colecciones

```javascript
// Listar colecciones
show collections;

// Ver estructura de documento
db.coleccion.findOne();

// Eliminar colección
db.coleccion.drop();
```

### Consultas Comunes

```javascript
// Contar documentos
db.coleccion.countDocuments();

// Ver primeros documentos
db.coleccion.find().limit(10);

// Buscar con patrón
db.coleccion.find({ nombre: /juan/i });
```

---

## 📖 Recursos Adicionales

### Documentación Oficial

- [MongoDB Documentation](https://docs.mongodb.com/)
- [MongoDB University](https://university.mongodb.com/)
- [MongoDB Blog](https://www.mongodb.com/blog)

### Herramientas Recomendadas

- **MongoDB Compass** - GUI oficial gratuito
- **mongosh** - Shell moderno
- **MongoDB Atlas** - Servicio cloud gratuito

### Comunidades

- [MongoDB Community](https://www.mongodb.com/community/)
- [Stack Overflow - MongoDB](https://stackoverflow.com/questions/tagged/mongodb)
- [Reddit r/mongodb](https://www.reddit.com/r/mongodb/)

---

## 💡 Consejos para Principiantes

1. **Entiende los documentos**: Piensa en JSON, no en tablas.
2. **Modela para tus consultas**: Diseña según cómo leerás los datos.
3. **Usa índices**: Mejoran drásticamente el rendimiento.
4. **Aprende el aggregation framework**: Poderoso para análisis.
5. **Considera Atlas**: Para desarrollo rápido sin instalación.

---

## ⚠️ Mejores Prácticas

### Rendimiento

- Indexa campos de consulta frecuente
- Usa proyecciones para limitar datos
- Evita $where y funciones JavaScript

### Modelado

- Embed vs Reference: depende del acceso
- Considera el crecimiento de datos
- Planifica para escalabilidad

### Seguridad

- Habilita autenticación
- Usa roles con privilegios mínimos
- Encripta datos sensibles

---

## 🧪 Ejercicios Prácticos

### Nivel Básico

1. Instala MongoDB y Compass
2. Crea una base de datos `Tienda`
3. Inserta documentos en colecciones
4. Realiza consultas básicas

### Nivel Intermedio

1. Crea índices para optimizar consultas
2. Usa el aggregation framework
3. Implementa validación de esquema

### Nivel Avanzado

1. Configura un replica set
2. Implementa sharding
3. Crea backups automatizados

---

## 👨‍💻 Desarrollado por Isaac Esteban Haro Torres

**Ingeniero en Sistemas · Full Stack · Automatización · Data**

- 📧 Email: zackharo1@gmail.com
- 💻 GitHub: https://github.com/ieharo1

---

© 2026 Isaac Esteban Haro Torres - Todos los derechos reservados.
