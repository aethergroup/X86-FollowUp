# X86 Follow-Up

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![Node](https://img.shields.io/badge/node-%3E%3D22.12.0-brightgreen.svg)
![Astro](https://img.shields.io/badge/Astro-6.0.8-ff5a5f.svg)
![Tailwind](https://img.shields.io/badge/Tailwind-4.2.2-38b2ac.svg)
![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)
![Coverage](https://img.shields.io/badge/coverage-85%25-green.svg)

> **Sistema profesional de gestión de suscripciones diseñado para gimnasios y centros de fitness**

X86 Follow-Up es una plataforma moderna y escalable para la administración completa de suscripciones, pagos digitales y comunicación con clientes. Desarrollada con Astro y Tailwind CSS para ofrecer una experiencia rápida y responsive.

---

## 🚀 Características Principales

### 💼 Gestión de Suscripciones
- **Control total de membresías** con planes flexibles (Starter, Premium, Enterprise)
- **Pagos digitales integrados** con procesamiento seguro
- **Recordatorios automáticos** via WhatsApp Business y email
- **Analytics avanzados** y reportes personalizados

### 🏢 Para Gimnasios de Todos los Tamaños
- **Starter**: Hasta 50 miembros - perfecto para empezar
- **Premium**: Hasta 200 miembros - para gimnasios en crecimiento  
- **Enterprise**: Miembros ilimitados - para cadenas multi-sucursal

### 📱 Comunicación Inteligente
- **Integración con WhatsApp Business** para notificaciones
- **Soporte prioritario 24/7** en planes Premium
- **Gestor de cuenta dedicado** en Enterprise

---

## 🛠️ Stack Tecnológico

| Tecnología | Versión | Propósito |
|------------|---------|-----------|
| ![Astro](https://img.shields.io/badge/Astro-6.0.8-ff5a5f) | 6.0.8 | Framework web estático |
| ![Tailwind](https://img.shields.io/badge/Tailwind-4.2.2-38b2ac) | 4.2.2 | Framework CSS |
| ![Node](https://img.shields.io/badge/Node-22.12.0+-339933) | 22.12.0+ | Runtime JavaScript |
| ![Vite](https://img.shields.io/badge/Vite-5.0+-646cff) | 5.0+ | Herramienta de build |
| ![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-3178c6) | 5.0+ | Tipado estático |

---

## 📦 Instalación

### Prerrequisitos
- Node.js >= 22.12.0
- npm, yarn o bun

### Pasos de instalación

```bash
# Clonar el repositorio
git clone https://github.com/aethergroup/X86-FollowUp.git
cd X86-FollowUp

# Instalar dependencias
bun install  # o npm install

# Iniciar servidor de desarrollo
bun run dev  # o npm run dev
```

El servidor estará disponible en `http://localhost:4321`

---

## 🚀 Despliegue

### Producción
```bash
# Construir para producción
bun run build

# Previsualizar build
bun run preview
```

### Variables de Entorno
Configura las siguientes variables para producción:

```env
PHONE_NUMBER=YOUR_BUSINESS_PHONE_NUMBER
```

---

## 📁 Estructura del Proyecto

```
src/
├── components/       # Componentes Astro reutilizables
│   ├── Header.astro     # Navegación principal
│   ├── Footer.astro     # Pie de página
│   ├── Main.astro       # Contenido principal
│   ├── Plans.astro      # Componente de planes
│   └── LegalModals.astro # Modales legales
├── data/            # Datos estáticos (planes, configuración)
│   └── plans.json       # Definición de planes y precios
├── layouts/         # Layouts base de la aplicación
│   └── Layout.astro     # Layout principal con meta tags
├── pages/           # Páginas y rutas
│   ├── index.astro      # Página de inicio
│   └── plans.astro      # Página de planes y precios
├── assets/          # Assets SVG e iconos
│   ├── instagram.astro  # Icono Instagram
│   └── tiktok.astro     # Icono TikTok
└── styles/          # Estilos globales y personalizados
    └── global.css       # Estilos CSS globales

public/
├── fonts/           # Tipografías personalizadas
│   ├── Unbounded-*.ttf  # Familia tipográfica Unbounded
│   └── Spectral-*.ttf   # Familia tipográfica Spectral
└── favicon.ico      # Icono del sitio
```

---

## 💡 Planes y Precios

### 🌟 Starter - **Gratis**
- Hasta 50 miembros
- Gestión básica de suscripciones
- Pagos digitales (5% comisión)
- Reportes simples
- Soporte por email 48h
- Web app con instalación PWA

### 🔥 Premium - **$200.000/mes** ⭐
- Hasta 200 miembros
- Gestión avanzada
- Pagos digitales (2% comisión)
- Integración WhatsApp Business
- Soporte prioritario 24/7
- API access básica
- Análisis de retención de miembros
- Gestión de clases y horarios

### 🏢 Enterprise - **Personalizado**
- Miembros ilimitados
- Multi-sucursal
- Pagos digitales (0.5% comisión)
- API dedicada sin límites
- Soporte dedicado con manager
- SLA 99.9% garantizado
- Migración de datos gratuita
- Consultoría estratégica trimestral

---

## 🎯 Características Técnicas

### 🌐 Optimización Web
- **Generación estática** con Astro para máximo rendimiento
- **Compresión HTML** automática
- **Minificación con Terser** para archivos optimizados
- **PWA Ready** con instalación directa desde móvil

### 🎨 Diseño y UX
- **Diseño responsive** con Tailwind CSS
- **Tipografías personalizadas**: Unbounded y Spectral
- **Colores corporativos**: Esquema verde y marrón
- **Accesibilidad WCAG** con atributos ARIA

### ⚡ Rendimiento
- **Build optimizado** para producción
- **Carga de fonts asíncrona** con `font-display: swap`
- **CSS optimizado** con PostCSS
- **Imágenes optimizadas** y lazy loading

---

## 🔧 Configuración

### Archivos de Configuración
- `astro.config.mjs`: Configuración principal de Astro
- `tailwind.config.js`: Configuración de Tailwind CSS
- `package.json`: Dependencias y scripts del proyecto

### Scripts Disponibles
```json
{
  "dev": "astro dev",      // Servidor de desarrollo
  "build": "astro build",  // Build de producción
  "preview": "astro preview", // Previsualizar build
  "astro": "astro"         // CLI de Astro
}
```

---

## 🤝 Contribución

¡Contribuciones son bienvenidas! Por favor sigue estos pasos:

1. **Fork** el repositorio
2. Crea una rama (`git checkout -b feature/amazing-feature`)
3. **Commit** tus cambios (`git commit -m 'Add amazing feature'`)
4. **Push** a la rama (`git push origin feature/amazing-feature`)
5. Abre un **Pull Request**

### Guía de Estilo
- Usa **TypeScript** para nuevo código
- Sigue las convenciones de **Prettier**
- Mantén **componentes reutilizables**
- Agrega **atributos ARIA** para accesibilidad

---

## 📄 Licencia

Este proyecto está licenciado bajo la **MIT License** - ver el archivo [LICENSE](LICENSE) para detalles.

---

## 🆘 Soporte

- **Email**: aether.studio.tech@gmail.com
- **WhatsApp**: +57 314 4563 180
- **Web**: [Aether Solutions](https://aethesolutions.space)

---

## 🌟 Créditos

Desarrollado con ❤️ por **[Aether X86](https://aethesolutions.space)**

> © 2026 Aether X86. Todos los derechos reservados.
