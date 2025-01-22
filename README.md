Avance 1 - 15% (Definición de alternativa - Diagramas de clases - Solución preliminar)

# 🗒️ Aplicación Web de Toma de Notas

## 🌐 Colaboradores

```
├── Santiago Gamboa Martínez
├── Samuel Eduardo Fajardo Quintero
└── Manuel Felipe Torres Gamboa
```

## 🏆 Introducción

Como equipo, hemos elegido desarrollar la `alternativa 5`, proponiendo un proyecto que aborda necesidades específicas compartidas por algunos estudiantes: **_una aplicación web de toma de notas_** 📝. Esta herramienta permitirá a los usuarios llevar un seguimiento organizado de sus tareas, ideas y pensamientos, e incluso redactar textos más largos.

💫 El **objetivo principal** del proyecto es facilitar el aprendizaje y la gestión del aparendizaje en el ámbito educativo, brindando una solución personalizada para estudiantes. Nuestra aplicación no busca replicar proyectos tradicionales que usan librerías como Tkinter ni basarse directamente con plataformas comerciales como Notion o Joplin, diseñadas para un uso general. En cambio, queremos enfocarnos en las necesidades específicas del entorno académico, ofreciendo una herramienta que permita a los usuarios organizar sus apuntes de manera eficiente, sintetizar conceptos clave y compartir ideas en un entorno accesible.

En términos de desarrollo, la aplicación será creada bajo los principios de la programación orientada a objetos (POO), lo que nos facilitará la modularidad, el mantenimiento y la escalabilidad del proyecto.

## ➕ Definición de Alternativa

**Nombre del Proyecto**: Bloc de Notas para Estudiantes

Nuestra alternativa propone el desarrollo de una **aplicación web de toma de notas** diseñada específicamente para satisfacer las necesidades de los estudiantes. Esta herramienta permitirá organizar y gestionar sus apuntes, ideas y tareas de manera eficiente, integrando funcionalidades avanzadas y tecnologías modernas que la diferencian de las soluciones existentes en el mercado.

El objetivo principal es ofrecer una solución práctica, segura y escalable que sea fácil de usar y personalizable. El proyecto se desarrollará bajo los principios de la **programación orientada a objetos (POO)**, garantizando un diseño modular y de alta calidad.

---

### Funcionalidades de la Aplicación

#### Funcionalidades Básicas:

- **Gestión de Notas**: Crear, leer, actualizar y eliminar notas de forma intuitiva.
- **Sistema de Inicio de Sesión**: Permitir que los usuarios se registren, inicien y cierren sesión de manera segura.
- **Organización de Notas**: Agrupar notas mediante etiquetas o categorías para facilitar la búsqueda.
- **Búsqueda Avanzada**: Filtrar notas por palabras clave, etiquetas o fechas.

#### Funcionalidades Avanzadas:

- **Modo Oscuro/Claro**: Adaptar la interfaz según las preferencias del usuario.
- **Sincronización en Tiempo Real**: Habilitar la colaboración entre usuarios en las notas compartidas.
- **Notificaciones**: Enviar alertas sobre cambios en notas colaborativas o recordatorios.
- **Exportación de Notas**: Descargar notas en formatos como PDF o Markdown para mayor flexibilidad.
- **Adjuntos**: Posibilidad de cargar y asociar archivos a las notas.

---

### Enfoque Técnico

El proyecto será desarrollado utilizando tecnologías modernas:

- **Backend**: Django, con Django REST Framework para la creación de API y SQLite como base de datos en producción.
- **Frontend**: React, utilizando Tailwind CSS para un diseño atractivo y Redux para la gestión del estado global.
- **Seguridad**: Autenticación mediante JWT, protección contra CSRF y encriptación avanzada para datos sensibles.

---

### Diferenciadores de la Alternativa

A diferencia de otras aplicaciones de notas generalistas como Notion o Joplin, nuestro proyecto está diseñado específicamente para estudiantes, con un enfoque en:

- **Productividad Académica**: Herramientas que facilitan el aprendizaje y la organización de apuntes.
- **Personalización**: Funcionalidades como el modo oscuro y etiquetas personalizables.
- **Simplicidad y Usabilidad**: Interfaz moderna y fácil de usar para que los estudiantes puedan enfocarse en lo importante.

---

### Alcance de la Alternativa

En su primera versión, la aplicación incluirá las funcionalidades básicas de gestión de notas y autenticación de usuarios. Las funcionalidades avanzadas se implementarán en fases posteriores, permitiendo iterar sobre la solución para agregar más valor al proyecto con base en la retroalimentación de los usuarios.

## 📈 Diagrama de Clases

## 💿 Solución Preliminar

### **Objetivo del Proyecto**

Desarrollar una aplicación web para gestionar notas, utilizando buenas prácticas de programación orientada a objetos (POO) y tecnologías modernas. La aplicación debe destacar por su:

- **Funcionalidad**: CRUD de notas (Crear, Leer, Actualizar, Eliminar).
- **Estética**: Interfaz amigable y moderna.
- **Seguridad**: Gestión segura de datos y contraseñas.
- **Escalabilidad**: Código modular y estructurado para futuras ampliaciones.

---

### **1. Definición de Requisitos**

### **1.1. Funcionalidades Básicas**

- **Gestión de Notas**: CRUD completo de notas.
- **Sistema de Inicio de Sesión**: Registro, inicio de sesión y cierre de sesión seguro.
- **Organización de Notas**: Posibilidad de agrupar notas por etiquetas o categorías.
- **Búsqueda y Filtros**: Permitir búsqueda avanzada por palabras clave, etiquetas o fechas.

### **1.2. Funcionalidades Avanzadas**

- **Modo Oscuro/Claro**: Personalización de la interfaz para mejorar la experiencia del usuario.
- **Sincronización en Tiempo Real**: Colaboración en notas entre usuarios mediante WebSockets.
- **Notificaciones**: Alertas por cambios en notas colaborativas o recordatorios automáticos.
- **Exportación de Notas**: Descargar notas en formatos como PDF o Markdown.
- **Adjuntos**: Posibilidad de cargar y asociar archivos multimedia a las notas.

---

### **2. Tecnologías y Herramientas**

### **Backend**

- **Framework**: Django (con Django REST Framework para la creación de APIs).
- **Base de Datos**: PostgreSQL para producción y SQLite para desarrollo.
- **Autenticación**: Gestión con Django-Auth y tokens JWT.
- **Notificaciones en Tiempo Real**: Implementadas mediante Django Channels y WebSockets.

### **Frontend**

- **Framework**: React.
- **Estilos**: Tailwind CSS o Bootstrap para un diseño moderno y responsivo.
- **Estado Global**: Redux para manejar datos de usuario y notas.

### **Seguridad**

- **Contraseñas**: Hashing con bcrypt o Argon2.
- **Protección**: Middleware para prevenir ataques CSRF y XSS.
- **Encriptación**: Uso de bibliotecas como `cryptography` para proteger notas sensibles.

### **Despliegue**

- **Backend**: Heroku o AWS para el entorno de producción.
- **Frontend**: Vercel o Netlify para hosting de la interfaz de usuario.

---

### **3. Diseño de la Arquitectura**

### **3.1. Estructura del Proyecto**

**Backend (Django):**

```
/mi_aplicacion
    /app
        /models
            user.py      # Modelo de Usuario.
            note.py      # Modelo de Nota.
        /routes
            auth_routes.py  # Rutas de autenticación.
            note_routes.py  # Rutas del CRUD de notas.
        /templates
        /static
    /tests
        test_auth.py
        test_note.py
    manage.py
```

**Frontend (React):**

```
/src
    /components
        NoteCard.js       # Componente para mostrar una nota.
        NoteForm.js       # Formulario para crear o editar notas.
    /pages
        LoginPage.js      # Página de inicio de sesión.
        NotesPage.js      # Página principal con todas las notas.
    /redux
        store.js          # Configuración del estado global.
        slices/
            notesSlice.js  # Gestión de estado de las notas.
            authSlice.js   # Gestión de estado de autenticación.
    index.js
```

### **3.2. Modelos de Datos**

**Usuario (User):**

- Atributos: `id`, `username`, `email`, `password_hash`, `fecha_creación`.
- Relaciones: Un usuario tiene muchas notas.

**Nota (Note):**

- Atributos: `id`, `título`, `contenido`, `fecha_creación`, `etiquetas`, `usuario_id`.
- Relaciones: Cada nota pertenece a un usuario.

---

### **4. Cronograma de Desarrollo**

### **Fase 1: Configuración y Diseño**

- Configurar el entorno de desarrollo (Django, React).
- Crear los modelos básicos (Usuario y Nota).
- Definir las rutas y vistas iniciales.
- Diseñar la estructura del frontend.

### **Fase 2: Desarrollo de Funcionalidades**

- Implementar CRUD de notas.
- Desarrollar el sistema de autenticación.
- Añadir etiquetas y filtros para la organización de notas.

### **Fase 3: Mejoras y Funcionalidades Avanzadas**

- Implementar sincronización en tiempo real.
- Añadir exportación de notas a PDF o Markdown.
- Desarrollar el sistema de notificaciones.
- Integrar modo oscuro y opciones de personalización.

### **Fase 4: Pruebas y Despliegue**

- Escribir pruebas unitarias para backend y frontend.
- Desplegar la aplicación para su uso.

---

### **5. Valor Agregado del Proyecto**

- **Diseño Responsive**: Uso de herramientas modernas para asegurar compatibilidad en dispositivos móviles.
- **Seguridad**: Gestión robusta de contraseñas y protección contra ataques comunes.
- **Escalabilidad**: Arquitectura modular y preparada para añadir nuevas funcionalidades en el futuro.
