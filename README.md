# **CRUD Usuarios – Versión 4 (con JSON Server)**

## **Descripción**
La **versión 4** del CRUD de usuarios incorpora persistencia real usando un archivo **`data/users.json`** gestionado a través de **`json-server`**.  
Esto permite que las operaciones **Crear, Editar y Eliminar** modifiquen directamente el archivo JSON, simulando un backend real.

---

## **Nuevas Funcionalidades**
- **Persistencia en JSON Server:**  
  Los datos se almacenan en el archivo `data/users.json` y se manejan mediante endpoints REST (`GET`, `POST`, `PUT`, `DELETE`).

- **Identificación por ID:**  
  Cada usuario tiene un campo `id` único generado automáticamente por `json-server`.

- **Integración híbrida:**  
  - `api.js` sigue proporcionando datos aleatorios desde **RandomUser** para autocompletar formularios.
  - `scripts.js` gestiona el CRUD real a través de **http://localhost:3000/users**.

---

## **Requisitos**
- **Node.js** instalado.
- **json-server** (se instala una sola vez).

### **Instalar json-server**
```bash
npm install -g json-server
```

---

## **Estructura del Proyecto**
```
/v4
│
├── index.html
├── data/
│   └── users.json
├── assets/
│   ├── js/
│   │   ├── scripts.js
│   │   ├── api.js
│   │   └── filter.js
│   └── css/
│       └── style.css
└── README.md
```

---

## **Iniciar el servidor**
Ejecuta este comando desde la carpeta del proyecto (donde está `data/users.json`):

```bash
json-server --watch data/users.json --port 3000
```

- El endpoint principal será:  
  **`http://localhost:3000/users`**

- Abre el navegador en tu archivo **`index.html`** para usar la aplicación.

---

## **Características heredadas**
- **Formulario de Registro:** Permite ingresar nombre, email y teléfono.
- **Auto-rellenado:** Botón que obtiene datos aleatorios de la API [RandomUser](https://randomuser.me/).
- **Lista de Usuarios:** Muestra tarjetas con datos de cada usuario.
- **Edición y Eliminación:** Modales para editar o confirmar eliminación.
- **Búsqueda y Ordenamiento:** A-Z y Z-A (gracias a `filter.js`).
- **Validaciones y Notificaciones:** Validación básica de datos y notificaciones con Bootstrap Toast.

---

## **Notas Importantes**
- Si `json-server` no está corriendo, las operaciones CRUD (guardar, editar, eliminar) darán error.
- Si cambias el puerto o la ruta del servidor, actualiza la constante `USERS_API_URL` en **scripts.js**:
  ```javascript
  const USERS_API_URL = 'http://localhost:3000/users';
  ```
