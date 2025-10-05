# Amanto Landing

Landing page con efecto de texto animado usando Astro + Aceternity UI

## 🚀 Stack

- **Astro 5.14** - Framework
- **React 19** - Componentes interactivos
- **Tailwind CSS 4** - Estilos
- **Framer Motion** - Animaciones
- **Aceternity UI** - Componente de texto con efecto hover

## 📦 Desarrollo

```bash
# Instalar dependencias
pnpm install

# Iniciar servidor de desarrollo
pnpm dev

# Construir para producción
pnpm build

# Vista previa de producción
pnpm preview
```

## 🐳 Deploy en Dokploy

Este proyecto está configurado para desplegarse en Dokploy usando Nixpacks.

### Requisitos:
- **Node.js**: 20.18.0 o superior
- **pnpm**: 9.0.0 o superior

### Configuración:

Los siguientes archivos están configurados para el deployment:

- `.node-version` - Especifica la versión de Node.js
- `.nvmrc` - Versión para NVM
- `nixpacks.toml` - Configuración de Nixpacks para Dokploy
- `.dockerignore` - Optimiza el build de Docker

### Variables de entorno:

No se requieren variables de entorno para el despliegue básico.

## 📁 Estructura

```
/
├── public/              # Archivos estáticos
├── src/
│   ├── components/      # Componentes React y Astro
│   │   ├── ui/         # Componentes UI de Aceternity
│   │   └── *.tsx       # Componentes React
│   ├── layouts/        # Layouts de Astro
│   ├── lib/            # Utilidades
│   ├── pages/          # Páginas de Astro
│   └── styles/         # Estilos globales
├── astro.config.mjs    # Configuración de Astro
├── components.json     # Configuración de shadcn/ui
├── nixpacks.toml       # Configuración de Nixpacks
└── package.json
```

## 🎨 Componentes

### TextHoverEffect

Efecto de texto animado con gradiente que sigue el cursor.

```tsx
import { TextHoverEffect } from "@/components/ui/text-hover-effect";

<TextHoverEffect text="AMANTO" />
```

## 📄 Licencia

MIT
