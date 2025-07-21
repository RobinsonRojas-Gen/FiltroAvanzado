# **Actividad Grupal – CRUD Usuarios Versión 5 (v5)**

## **Objetivo**
El objetivo de esta versión es **mejorar el CRUD de usuarios (v4)** añadiendo nuevas funcionalidades, validaciones, animaciones y mejoras de UI/UX.  
Cada grupo trabajará en **la actividad que le corresponde según su número de grupo**.

---

## **Dinámica de Trabajo**
- **Grupos:** 7 grupos.
- **Tiempo Total:** 1 hora (con 5 min de presentación de la actividad realizada).
- **Apoyo:** Se permite consultar IA o documentación, pero deben entender y explicar el código durante la presentación.
- **Presentador:** La persona que presentará será elegida por el profesor.
- **Repositorio:** Cada grupo debe subir **un solo repositorio grupal**.  
  *No es necesario que cada persona suba su código individualmente.*
---

## **Instrucciones Generales**
- Cada grupo **debe completar únicamente la tarea que le corresponde**.  
- **Si desean hacer otras actividades como práctica, es opcional.**  


## **Actividades por Grupo**

### **Grupo 1: Validaciones Mejoradas**
- Implementar validaciones dinámicas:
  - Mostrar mensajes de error en tiempo real mientras el usuario escribe.
  - Resaltar campos inválidos con borde rojo.
- **Tip:** Usar eventos `input` y manipulación de clases (`classList.add/remove`).

---

### **Grupo 2: Filtro Avanzado**
- Agregar un filtro por **dominio de email** (ejemplo: `@gmail.com`, `@yahoo.com`).
- Botones predefinidos para mostrar:
  - Solo usuarios con Gmail.
  - Solo usuarios con Yahoo.
- **Tip:** Usar `filter()` con `endsWith()`.  

---

### **Grupo 3: Paginación Simple**
- Mostrar solo **5 usuarios por página**.
- Agregar botones **Anterior** y **Siguiente** para cambiar de página.
- **Tip:** Controlar un índice `currentPage` y usar `slice()` para renderizar.

---

### **Grupo 4: Sistema de Favoritos**
- Agregar un botón **"⭐ Favorito"** en cada tarjeta.
- Crear un filtro para mostrar solo los favoritos.
- Guardar el estado con una propiedad `isFavorite` en cada usuario.

---

### **Grupo 5: Subida de Imagen de Perfil**
- Permitir que el usuario suba una imagen desde su computadora.
- Mostrar una **vista previa** antes de guardar usando `FileReader`.
- Reemplazar la imagen por defecto (`profileImage`) con la seleccionada.

---

### **Grupo 6: Animaciones y Transiciones**
- Agregar animaciones CSS al agregar, editar o eliminar usuarios.
  - Ejemplo: animar entrada de una tarjeta con `@keyframes fadeIn`.
  - Animación de "deslizamiento" al eliminar una tarjeta.
- **Plus:** Mostrar un **loading spinner** mientras se cargan usuarios.

---

### **Grupo 7: Mejora del Diseño**
- Rediseñar la interfaz usando **Bootstrap avanzado**:
  - **Tooltips** para botones Editar/Eliminar.
  - **Badges** con número de usuarios favoritos.
  - Mejorar la estética con `cards`, sombras y colores.

---

---

## **Entrega**
Cada grupo debe:
1. Subir **un único repositorio grupal** con la actividad completada.
2. Mostrar en vivo su funcionalidad.
3. Explicar su código y cómo manipularon el DOM.
---
