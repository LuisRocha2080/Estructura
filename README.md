📁 System/
│
├── 📁 app/                      🧠 Lógica del Back-end
│   ├── 📁 Http/
│   │   ├── 📁 Controllers/      🎯 Controladores (lógica de negocio)
│   │   └── 📁 Middleware/       🔐 Filtros, seguridad y control de acceso
│   ├── 📁 Models/               🗄️ Modelos de base de datos (Eloquent ORM)
│   └── 📁 Providers/            ⚙️ Proveedores de servicios del sistema
│
├── 📁 public/                   🌐 Archivos accesibles públicamente
│   ├── 📁 css/                  🎨 Hojas de estilo del sistema
│   ├── 📁 js/                   ⚡ Scripts JavaScript
│   ├── 📁 images/               🖼️ Recursos gráficos
│   └── 📄 index.php             🚪 Punto de entrada de la aplicación
│
├── 📁 resources/                🎨 Recursos del Front-end
│   └── 📁 views/                🧩 Plantillas Blade
│       ├── 📁 admin/            👑 Vistas del Administrador
│       ├── 📁 recepcionista/    📋 Vistas del Recepcionista
│       ├── 📁 veterinario/      🩺 Vistas del Veterinario
│       ├── 📁 vendedor/         🛒 Vistas del Vendedor
│       ├── 📁 layouts/          🧱 Plantillas base (layouts)
│       └── 📁 others/           🔑 Autenticación, perfil, errores, etc.
│
├── 📁 routes/                   🧭 Definición de rutas del sistema
│   └── 📄 web.php               🌍 Rutas web y navegación
│
├── 📁 database/                 🗃️ Gestión de la base de datos
│   ├── 📁 migrations/           🧬 Estructura y versionado de tablas
│   └── 📁 seeders/              🌱 Datos de prueba e iniciales
│
├── 📁 config/                   ⚙️ Archivos de configuración
├── 📁 tests/                    🧪 Pruebas automatizadas
├── 📁 vendor/                   📦 Dependencias PHP (Composer)
└── 📄 .env                      🔐 Variables de entorno (DB, claves, entorno)
