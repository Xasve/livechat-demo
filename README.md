# 💬 App de Mensajería en Vivo

Aplicación de chat en tiempo real con interfaz profesional. Construida con HTML, CSS y JavaScript. Simula la experiencia completa de una plataforma de mensajería incluyendo conversaciones, respuestas automáticas, archivos adjuntos e indicadores de estado.

## ✨ Funcionalidades

- **Lista de contactos** con estado en línea/ausente/desconectado y badges de no leídos
- **Mensajes en tiempo real** — Envía y recibe respuestas automáticas simuladas
- **Indicador de escritura** — Animación de puntos mientras el contacto "escribe"
- **Confirmación de lectura** — Doble check ✓✓ en mensajes enviados
- **Adjuntar archivos** — Simula el envío de .zip, .pdf, .sql con nombre y tamaño
- **Compartir imágenes** — Envío de capturas de pantalla
- **Insertar código** — Botón para insertar bloques de código en el chat
- **Canales de equipo** — Sección de canales (#general, #proyectos, #diseño)
- **Panel de información** — Estadísticas del contacto, archivos recientes y miembros online
- **Búsqueda de contactos** — Filtro en tiempo real en la lista
- **Diseño responsive** — Panel lateral colapsable en móvil

## 🧰 Stack Técnico

| Capa | Tecnología |
|------|-----------|
| Frontend | HTML5, CSS3, JavaScript ES6+ |
| Layout | CSS Grid, Flexbox, sticky positioning |
| Tipografía | Inter + JetBrains Mono |
| Animaciones | CSS keyframes (typing dots, pulse) |

> **Stack en producción:** JavaScript · Socket.io · Express · MySQL · JWT Auth · Node.js

## 🚀 Cómo correr el proyecto

```bash
# Clonar el repositorio
git clone https://github.com/Xasve/livechat-demo.git

# Abrir en el navegador (no requiere servidor)
open index.html
```

O visita el **[Demo en vivo →](https://xasve.github.io/livechat-demo)**

## 📁 Estructura

```
livechat-demo/
└── index.html      # App completa (HTML + CSS + JS)
```

## 🗂️ Arquitectura en producción

```
Cliente (Browser)
    │
    ├── Socket.io client  ──→  Node.js + Express server
    │                              │
    │                              ├── Socket.io server (eventos en vivo)
    │                              ├── REST API (historial, usuarios)
    │                              └── MySQL (mensajes, salas, usuarios)
    │
    └── JWT Token  ──→  Middleware de autenticación
```

## 📸 Lo que verás en el demo

- Panel izquierdo con 6 contactos y sus estados
- Chat central con historial de conversación
- Respuestas automáticas al enviar mensajes
- Animación de "escribiendo..." antes de cada respuesta
- Panel derecho con info del contacto y miembros online

## 👨‍💻 Autor

**Ethan Barboza** — Full Stack Developer Freelance
📧 ethan.barboza10@gmail.com
🌐 [xasve.github.io](https://xasve.github.io)
