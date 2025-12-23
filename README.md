# 📁 Estructura del Sistema de Gestión Veterinaria

## 🗂️ Organización Completa del Proyecto
```
📦 Sistema/
│
├── 📂 app/                          # 🔧 Lógica del Back-end
│   ├── 📂 Http/
│   │   ├── 📂 Controllers/          # 🎮 Controladores (Lógica de negocio)
│   │   └── 📂 Middleware/           # 🔒 Filtros de peticiones y seguridad
│   ├── 📂 Models/                   # 🗄️ Modelos de Base de Datos (Eloquent ORM)
│   └── 📂 Providers/                # ⚙️ Proveedores de servicios del sistema
│
├── 📂 resources/                    # 🎨 Recursos del Front-end
│   └── 📂 views/                    # 📄 Plantillas Blade (HTML dinámico)
│       ├── 📂 layouts/              # 🏗️ Plantillas base (Master layouts)
│       ├── 📂 admin/                # 👨‍💼 Vistas del Administrador
│       ├── 📂 veterinario/          # 👨‍⚕️ Vistas del Veterinario
│       ├── 📂 recepcionista/        # 👩‍💼 Vistas del Recepcionista
│       ├── 📂 vendedor/             # 🛒 Vistas del Vendedor
│       ├── 📂 auth/                 # 🔐 Autenticación (login, registro, recuperación)
│       ├── 📂 profile/              # 👤 Perfil de usuario
│       └── 📂 errors/               # ⚠️ Páginas de error (404, 500, etc.)
│
├── 📂 public/                       # 🌐 Archivos accesibles públicamente
│   ├── 📄 index.php                 # 🚀 Punto de entrada de la aplicación
│   ├── 📂 css/                      # 🎨 Hojas de estilo (organizadas por módulos)
│   ├── 📂 js/                       # ⚡ Scripts JavaScript (organizados por módulos)
│   ├── 📂 images/                   # 🖼️ Imágenes y recursos gráficos públicos
│   └── 📂 uploads/                  # 📤 Archivos subidos por usuarios
│
├── 📂 routes/                       # 🛣️ Definición de rutas del sistema
│   └── 📄 web.php                   # 🌐 Rutas web y navegación de la aplicación
│
├── 📂 database/                     # 💾 Gestión de Base de Datos
│   ├── 📂 migrations/               # 🔄 Estructura y versionado de tablas
│   └── 📂 seeders/                  # 🌱 Datos de prueba e iniciales
│
├── 📂 config/                       # ⚙️ Archivos de configuración del sistema
├── 📂 tests/                        # 🧪 Pruebas unitarias y de integración
├── 📂 storage/                      # 💿 Almacenamiento (logs, cache, sesiones)
│   ├── 📂 app/                      # 📦 Archivos generados por la aplicación
│   ├── 📂 framework/                # 🔧 Cache, sesiones y vistas compiladas
│   └── 📂 logs/                     # 📋 Archivos de registro (logs)
│
├── 📂 vendor/                       # 📚 Dependencias de PHP (Composer)
│
├── 📄 .env                          # 🔑 Variables de entorno (DB, claves, configuración)
├── 📄 .env.example                  # 📋 Ejemplo de configuración de entorno
├── 📄 composer.json                 # 📦 Gestión de dependencias PHP
├── 📄 composer.lock                 # 🔒 Versiones exactas de dependencias
├── 📄 artisan                       # 🔨 CLI de Laravel (comandos de consola)
├── 📄 package.json                  # 📦 Dependencias JavaScript (npm)
└── 📄 README.md                     # 📖 Documentación del proyecto
```

---

## 📋 Descripción Detallada de Carpetas

### 🔧 Backend (app/)

| Carpeta | Descripción |
|---------|-------------|
| **Controllers/** | 🎮 Contiene la lógica de negocio y maneja las peticiones HTTP |
| **Middleware/** | 🔒 Filtros para autenticación, autorización y validación de peticiones |
| **Models/** | 🗄️ Modelos Eloquent que representan las tablas de la base de datos |
| **Providers/** | ⚙️ Registro y configuración de servicios del sistema |

### 🎨 Frontend (resources/views/)

| Carpeta | Descripción |
|---------|-------------|
| **layouts/** | 🏗️ Plantillas base compartidas (header, footer, sidebar) |
| **admin/** | 👨‍💼 Dashboard y funcionalidades del administrador |
| **veterinario/** | 👨‍⚕️ Panel de control para veterinarios (consultas, historiales) |
| **recepcionista/** | 👩‍💼 Interfaz para gestión de citas y atención al cliente |
| **vendedor/** | 🛒 Sistema de ventas de productos y servicios |
| **auth/** | 🔐 Formularios de login, registro y recuperación de contraseña |
| **profile/** | 👤 Edición de perfil y configuración de usuario |
| **errors/** | ⚠️ Páginas personalizadas de error (404, 403, 500) |

### 🌐 Recursos Públicos (public/)

| Carpeta | Descripción |
|---------|-------------|
| **css/** | 🎨 Archivos de estilos organizados por módulos y componentes |
| **js/** | ⚡ Scripts JavaScript organizados por funcionalidad |
| **images/** | 🖼️ Logos, iconos, banners y recursos gráficos |
| **uploads/** | 📤 Imágenes de mascotas, documentos y archivos de usuarios |
| **index.php** | 🚀 Archivo principal que inicia la aplicación Laravel |

### 💾 Base de Datos (database/)

| Carpeta | Descripción |
|---------|-------------|
| **migrations/** | 🔄 Archivos que definen la estructura de las tablas (versionado) |
| **seeders/** | 🌱 Scripts para poblar la BD con datos iniciales o de prueba |

### 💿 Almacenamiento (storage/)

| Carpeta | Descripción |
|---------|-------------|
| **app/** | 📦 Archivos generados por la aplicación (PDFs, reportes) |
| **framework/** | 🔧 Cache del sistema, sesiones y vistas compiladas |
| **logs/** | 📋 Registros de errores y eventos de la aplicación |

---

## 🚀 Tecnologías Utilizadas

| Tecnología | Uso |
|------------|-----|
| **Laravel** | 🔧 Framework PHP principal |
| **MySQL** | 💾 Sistema de gestión de base de datos |
| **Blade** | 📄 Motor de plantillas de Laravel |
| **Eloquent ORM** | 🗄️ Mapeo objeto-relacional para la BD |
| **Bootstrap/Tailwind** | 🎨 Framework CSS para diseño responsive |
| **JavaScript** | ⚡ Interactividad y validaciones del lado cliente |
| **Composer** | 📦 Gestor de dependencias PHP |

---

## 🔐 Archivos de Configuración Importantes

| Archivo | Descripción |
|---------|-------------|
| **.env** | 🔑 Variables de entorno (DB, mail, API keys) |
| **composer.json** | 📦 Definición de dependencias PHP del proyecto |
| **artisan** | 🔨 Herramienta CLI para comandos de Laravel |
| **web.php** | 🛣️ Definición de todas las rutas web |

---

## 📝 Roles del Sistema

| Rol | Funcionalidades Principales |
|-----|------------------------------|
| 👨‍💼 **Administrador** | Gestión de usuarios, reportes, configuración del sistema |
| 👨‍⚕️ **Veterinario** | Historiales clínicos, diagnósticos, recetas |
| 👩‍💼 **Recepcionista** | Agendamiento de citas, registro de clientes |
| 🛒 **Vendedor** | Ventas de productos, inventario, facturación |

---

## 💡 Convenciones de Desarrollo

- ✅ **PSR-4**: Autoloading de clases
- ✅ **PSR-12**: Estándares de código PHP
- ✅ **Blade**: Separación de lógica y presentación
- ✅ **MVC**: Arquitectura Modelo-Vista-Controlador
- ✅ **RESTful**: Rutas y endpoints bien estructurados

---

## 📦 Instalación y Configuración
```bash
# 1. Clonar el repositorio
git clone <url-del-repositorio>

# 2. Instalar dependencias
composer install

# 3. Configurar entorno
cp .env.example .env
php artisan key:generate

# 4. Configurar base de datos en .env
DB_DATABASE=veterinaria
DB_USERNAME=root
DB_PASSWORD=

# 5. Ejecutar migraciones
php artisan migrate

# 6. Poblar base de datos (opcional)
php artisan db:seed

# 7. Iniciar servidor
php artisan serve
```

---

## 📞 Contacto y Soporte

Para dudas o contribuciones, contactar al equipo de desarrollo.

---

**🏥 Sistema de Gestión Veterinaria - Versión 1.0**
