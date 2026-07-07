# INMUEBLES-BROKERS
**Consulta de Inventario de Inmuebles — Activos por Colombia**

SPA estática (HTML + CSS + JS vanilla) conectada a Supabase como backend.

---

## Requisitos

- nvm (Node Version Manager)
- Node.js 18.20.4 (gestionado por nvm vía `.nvmrc`)
- npm >= 9.x

## Instalación

```bash
nvm use          # activa Node 18.20.4 desde .nvmrc
npm install      # instala dependencias de desarrollo
```

## Levantar el servidor local

```bash
npm run dev
```

Abre automáticamente `http://localhost:5500` en el navegador.

## Estructura del proyecto

```
INMUEBLES-BROKERS/
├── index.html              → Login + interfaz de búsqueda
├── src/
│   ├── js/app.js           → Lógica de autenticación, consulta Supabase y KMZ
│   └── css/styles.css      → Estilos globales
├── public/
│   └── logos/              → Assets de imagen y SVG
├── .nvmrc                  → Versión de Node fijada (entorno virtual)
├── package.json            → Configuración npm y scripts
├── DEPENDENCIAS.txt        → Documentación completa de dependencias
├── .gitignore
└── README.md
```

## Roles de acceso

| Usuario        | Rol        | Acceso especial                        |
|----------------|------------|----------------------------------------|
| broker2026     | broker     | Consulta básica (sin avalúo comercial) |
| comercial2026  | comercial  | Consulta completa + panel admin KMZ    |
