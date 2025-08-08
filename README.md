# Todo VibeCoding - Lista de Tareas Moderna

Aplicación de gestión de tareas desarrollada con React, TypeScript y Vite siguiendo los principios de **Vibe Coding** para crear código eficiente, mantenible y con estándares profesionales.

## 🚀 Stack Tecnológico

### Framework y Librerías Principales
- **React 19.1.0** - Biblioteca principal para la interfaz de usuario
- **TypeScript 5.8.3** - Tipado estático para mayor seguridad y mantenibilidad
- **Vite 7.0.4** - Build tool y dev server ultrarrápido

### Estilos y UI
- **Tailwind CSS v4.1.11** - Framework de CSS utility-first para diseño moderno
- **@tailwindcss/vite** - Plugin oficial de Tailwind para Vite

### Testing y Calidad de Código
- **Jest 30.0.5** - Framework de testing principal
- **Testing Library** - Suite completa para testing de componentes React
  - `@testing-library/react 16.3.0`
  - `@testing-library/jest-dom 6.6.3`
  - `@testing-library/user-event 14.6.1`
- **ESLint 9.30.1** - Linter para mantener calidad de código
- **TypeScript ESLint 8.35.1** - Reglas específicas para TypeScript

### Herramientas de Desarrollo
- **Babel** - Transpilador con presets para React y TypeScript
- **ts-jest** - Soporte de TypeScript en Jest
- **jest-environment-jsdom** - Entorno DOM para testing

## 🏗️ Arquitectura del Proyecto

El proyecto sigue una arquitectura modular y escalable basada en los principios de **Clean Architecture** y **Component-Driven Development**:

```
src/
├── components/          # Componentes reutilizables
│   └── ui/             # Componentes base de interfaz
│       ├── FilterButtons.tsx
│       ├── Footer.tsx
│       ├── Header.tsx
│       ├── StatsCard.tsx
│       ├── StatsSection.tsx
│       ├── TodoItem.tsx
│       ├── TodoList.tsx
│       └── index.ts    # Barrel exports
├── hooks/              # Custom hooks para lógica reutilizable
│   └── useTodo.ts     # Hook principal para gestión de todos
├── types/              # Definiciones de tipos TypeScript
│   └── svg.d.ts       # Tipos para archivos SVG
├── utils/              # Funciones utilitarias
│   ├── dateUtils.ts   # Utilidades para manejo de fechas
│   └── index.ts       # Barrel exports
├── assets/             # Recursos estáticos
├── __tests__/          # Tests unitarios e integración
│   ├── App.test.tsx
│   └── setup.ts       # Configuración de testing
├── App.tsx            # Componente principal
├── main.tsx           # Punto de entrada
├── todos.ts           # Datos y lógica de todos
└── index.css          # Estilos globales
```

### Patrones de Diseño Implementados

- **Container/Presentational Pattern**: Separación clara entre lógica y presentación
- **Custom Hooks Pattern**: Encapsulación de lógica de estado en `useTodo`
- **Barrel Exports**: Importaciones limpias mediante archivos `index.ts`
- **Composition Pattern**: Componentes modulares y reutilizables
- **TypeScript Strict Mode**: Tipado estricto para mayor seguridad

### Características Técnicas

- ✅ **TypeScript Strict**: Tipado estricto en toda la aplicación
- ✅ **Responsive Design**: Diseño adaptativo con Tailwind CSS
- ✅ **Dark Mode Support**: Soporte nativo para modo oscuro
- ✅ **Accessibility**: Componentes accesibles con ARIA labels
- ✅ **Testing Coverage**: Tests unitarios e integración
- ✅ **ESLint Configuration**: Reglas estrictas de calidad de código
- ✅ **Performance Optimized**: Uso de `useMemo` para optimización

## 🛠️ Instalación y Configuración

### Prerrequisitos

- **Node.js** >= 18.0.0
- **npm** >= 9.0.0 o **yarn** >= 1.22.0
- **Git** para clonar el repositorio

### Proceso de Instalación

1. **Clonar el repositorio**
   ```bash
   git clone <repository-url>
   cd todo-vibecoding
   ```

2. **Instalar dependencias**
   ```bash
   npm install
   # o usando yarn
   yarn install
   ```

3. **Ejecutar en modo desarrollo**
   ```bash
   npm run dev
   # o usando yarn
   yarn dev
   ```
   La aplicación estará disponible en `http://localhost:3000`

### Scripts Disponibles

```bash
# Desarrollo
npm run dev          # Inicia servidor de desarrollo
npm run build        # Construye la aplicación para producción
npm run preview      # Vista previa de la build de producción

# Testing
npm run test         # Ejecuta tests una vez
npm run test:watch   # Ejecuta tests en modo watch
npm run test:coverage # Ejecuta tests con reporte de cobertura
npm run test:ci      # Ejecuta tests para CI/CD

# Calidad de Código
npm run lint         # Ejecuta ESLint para verificar código
```

### Configuración del Entorno

El proyecto está configurado con:

- **Vite Config**: Puerto 3000, plugins de React y Tailwind
- **TypeScript**: Configuración estricta con referencias de proyecto
- **ESLint**: Reglas para React, TypeScript y hooks
- **Jest**: Entorno JSDOM con soporte para TypeScript
- **Tailwind**: Configuración v4 con soporte para dark mode

### Estructura de Testing

Los tests están organizados en:
- `src/__tests__/` - Tests principales
- `setup.ts` - Configuración global de testing
- Cobertura automática con Jest

## 🚀 Despliegue

Para desplegar en producción:

1. **Construir la aplicación**
   ```bash
   npm run build
   ```

2. **Los archivos estáticos se generarán en `/dist`**

3. **Servir los archivos estáticos** con cualquier servidor web (Nginx, Apache, Vercel, Netlify, etc.)

---

**Desarrollado con ❤️ siguiendo los principios de Vibe Coding**
