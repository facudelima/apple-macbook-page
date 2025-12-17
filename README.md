# Apple MacBook Page

Una página web interactiva estilo Apple que muestra productos MacBook con modelos 3D animados, efectos de scroll avanzados y animaciones fluidas.

🌐 **Demo en vivo**: [https://facu-apple-macbook-page.vercel.app/](https://facu-apple-macbook-page.vercel.app/)

## 📖 Descripción del Proyecto

Este proyecto es una landing page moderna inspirada en el diseño de Apple, que presenta productos MacBook mediante:

- **Modelos 3D interactivos**: Visualización de MacBook en 3D con diferentes tamaños (14", 16" y modelo estándar)
- **Animaciones avanzadas**: Efectos de scroll sincronizados con animaciones GSAP
- **Secciones fijas (pinned)**: Secciones que permanecen visibles mientras el contenido se anima
- **Transiciones suaves**: Efectos de máscara de imágenes y animaciones de timeline
- **Diseño responsive**: Adaptado para diferentes tamaños de pantalla

## 🛠️ Tecnologías y Herramientas

### Frontend Framework
- **React 19.1.1**: Biblioteca de JavaScript para construir interfaces de usuario interactivas
- **React DOM 19.1.1**: Renderizado de componentes React en el navegador

### Animaciones
- **GSAP 3.13.0**: Biblioteca de animación JavaScript de alto rendimiento
- **@gsap/react 2.1.2**: Integración de GSAP con React mediante hooks personalizados
- **ScrollTrigger**: Plugin de GSAP para crear animaciones basadas en el scroll

### Gráficos 3D
- **Three.js 0.180.0**: Biblioteca JavaScript para crear gráficos 3D en el navegador
- **@react-three/fiber 9.3.0**: Renderizador React para Three.js
- **@react-three/drei 10.7.6**: Utilidades y helpers para react-three/fiber (iluminación, texturas, etc.)

### Estilos
- **Tailwind CSS 4.1.13**: Framework CSS utility-first para diseño rápido
- **@tailwindcss/vite 4.1.13**: Plugin de Vite para Tailwind CSS

### Gestión de Estado
- **Zustand 5.0.8**: Biblioteca ligera de gestión de estado para React

### Utilidades
- **clsx 2.1.1**: Utilidad para construir strings de clases CSS condicionalmente
- **react-responsive 10.0.1**: Hook para detectar el tamaño de pantalla y crear diseños responsive

### Herramientas de Desarrollo
- **Vite 7.1.7**: Build tool y servidor de desarrollo rápido
- **ESLint 9.36.0**: Linter para mantener la calidad del código
- **TypeScript types**: Tipos para React y React DOM

## 🚀 Instalación y Ejecución

### Prerrequisitos

Asegúrate de tener instalado:
- [Node.js](https://nodejs.org/) (versión 18 o superior)
- [npm](https://www.npmjs.com/) o [yarn](https://yarnpkg.com/)

### Pasos para ejecutar

1. **Clonar el repositorio** (si aplica):
```bash
git clone https://github.com/facudelima/apple-macbook-page
cd apple_macbook_page
```

2. **Instalar dependencias**:
```bash
npm install
```

3. **Ejecutar el servidor de desarrollo**:
```bash
npm run dev
```

4. **Abrir en el navegador**:
   - El proyecto estará disponible en `http://localhost:5173`

### Scripts disponibles

- `npm run dev`: Inicia el servidor de desarrollo con Vite
- `npm run build`: Construye la aplicación para producción
- `npm run preview`: Previsualiza la build de producción
- `npm run lint`: Ejecuta ESLint para verificar el código

## 📁 Estructura del Proyecto

```
src/
├── components/          # Componentes React
│   ├── Features.jsx    # Sección de características
│   ├── Footer.jsx      # Pie de página
│   ├── Hero.jsx        # Sección hero principal
│   ├── Highlights.jsx  # Sección de destacados
│   ├── NavBar.jsx      # Barra de navegación
│   ├── Performance.jsx # Sección de rendimiento
│   ├── ProductViewer.jsx # Visor de productos 3D
│   ├── Showcase.jsx    # Showcase de productos
│   └── models/         # Modelos 3D de MacBook
│       ├── Macbook.jsx
│       ├── Macbook-14.jsx
│       └── Macbook-16.jsx
├── constants/          # Constantes y configuraciones
├── store/              # Store de Zustand para estado global
├── App.jsx             # Componente principal
└── main.jsx            # Punto de entrada de la aplicación
```

## 🎨 Características Principales

- **Visualización 3D**: Modelos interactivos de MacBook con diferentes configuraciones
- **Animaciones de scroll**: Efectos sincronizados con el desplazamiento del usuario
- **Secciones fijas**: Contenido que permanece visible durante las animaciones
- **Transiciones de imágenes**: Efectos de máscara y fade para transiciones suaves
- **Diseño responsive**: Adaptación automática a diferentes dispositivos
- **Timeline animations**: Animaciones complejas que abarcan múltiples secciones

## 📝 Notas

- Los modelos 3D están ubicados en `public/models/`
- Las animaciones utilizan GSAP ScrollTrigger para sincronización con el scroll
- El estado global se gestiona con Zustand para controlar colores, texturas y configuraciones del modelo
