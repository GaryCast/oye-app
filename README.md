# Oye! - Organize Your Expenses

Aplicación móvil para el control y organización de gastos personales, desarrollada en Kodular.

## Información de la actividad

- **Autor:** Gary Castaño
- **Universidad:** Universidad de Cartagena — Ingeniería de Software
- **Corte 1:** Kodular con persistencia en el dispositivo (TinyDB) y uso de sensores
- **Ejercicio asignado:** N° 6 — Gastos

## Tecnología

- Kodular Creator
- Persistencia local con TinyDB
- Sensores utilizados: Clock (temporizador de splash) y LocationSensor (ubicación GPS)

## Estructura del repositorio

oye-app/
├── apk/
│   └── oye.apk          # Aplicación instalable
├── source/
│   └── oye.aia           # Proyecto fuente de Kodular
└── README.md

## Funcionalidades

- **Login y registro** de usuarios, con roles de Usuario General y Administrador
- **CRUD completo de Gastos**: crear, listar, editar y eliminar
- **CRUD completo de Usuarios**: cada usuario gestiona su propio perfil; el administrador puede gestionar cualquier usuario
- **Reportes parametrizados de Gastos**: por fecha y por lugar
- **Reportes parametrizados de Usuarios**: por rol y por nombre
- **Recuperación de usuario y contraseña** por email
- Uso de sensor de ubicación (GPS) para autocompletar el lugar del gasto

## Cómo instalar y probar la aplicación

### Opción 1: instalar el APK directamente (recomendado)

1. Descarga el archivo `apk/oye.apk` de este repositorio.
2. En tu celular Android, ve a **Ajustes → Seguridad** y activa **"Instalar apps de fuentes desconocidas"** (o acéptalo cuando el sistema te lo pida al abrir el archivo).
3. Abre el archivo `.apk` descargado y sigue las instrucciones de instalación.
4. Abre la app "Oye!" desde tu pantalla de inicio.

### Opción 2: abrir el proyecto fuente en Kodular

1. Ve a creator.kodular.io e inicia sesión (o crea una cuenta gratuita).
2. Ve a **Project → Import project (.aia) from my computer**.
3. Selecciona el archivo `source/oye.aia` de este repositorio.
4. Una vez cargado, puedes probarlo en vivo con **Kodular Companion** (Test → conectar por código QR) o exportar tu propio APK (Export → App .apk).

## Credenciales de prueba

- **Administrador:** usuario `admin`, contraseña `admin123` (se crea automáticamente la primera vez que se abre la app)
- Para probar como usuario general, regístrate desde la pantalla de login.

## Permisos requeridos

La app solicita permiso de **ubicación** (para autocompletar el lugar de cada gasto) y necesita conexión a internet para el envío de correos de recuperación de contraseña.