# 🏥 PharmaSafe - Sistema Inteligente de Control de Medicamentos

![PharmaSafe](https://img.shields.io/badge/PharmaSafe-IoT%20Medical%20Device-6FDA9E?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Prototipo-3D6B5E?style=for-the-badge)
![Tech](https://img.shields.io/badge/Tech-ESP32%20%7C%20RFID%20%7C%20Android-0A0F0D?style=for-the-badge)

## 📋 Descripción del Proyecto

**PharmaSafe** es un sistema inteligente de control y monitoreo de medicamentos que combina hardware IoT (ESP32 + RFID) con una aplicación móvil Android para ofrecer una solución integral de gestión de medicamentos. El proyecto busca mejorar la adherencia a tratamientos médicos mediante tecnología accesible y automatizada.

### 🎯 Objetivo Principal

Facilitar el control, monitoreo y recordatorio de medicamentos mediante un sistema integrado que notifique a los usuarios sobre horarios de toma y fechas de caducidad, reduciendo errores en la medicación.

---

## ✨ Características Principales Implementadas

### ✅ Página Web Futurista
- **Hero Section** con animación de partículas y efectos visuales futuristas
- **Diseño Glassmorphism** con efectos de vidrio esmerilado y neón
- **Animaciones suaves** al hacer scroll y hover
- **Responsive Design** adaptable a dispositivos móviles y tablets
- **Sistema de navegación** con scroll suave y menú móvil hamburguesa

### 🎨 Estilo Visual
- **Paleta de colores médica:**
  - Verde Esmeralda: `#3D6B5E`
  - Verde Menta: `#6FDA9E`
  - Negro Azulado: `#0A0F0D`
  - Blanco Puro: `#FFFFFF`
- **Tipografía moderna:** Poppins y Orbitron
- **Efectos especiales:** Neón, glassmorphism, animaciones 3D

### 📱 Secciones de la Página

1. **Hero/Inicio**
   - Mensaje principal: "Tu botiquín inteligente, siempre conectado"
   - Badges tecnológicos y estadísticas clave
   - Botones de acción (CTA)

2. **¿Cómo Funciona?**
   - Timeline interactiva con 3 pasos
   - Lector RFID → App Móvil → ESP32
   - Diagrama de sistema con conexiones animadas
   - Tags tecnológicos para cada componente

3. **Características**
   - 6 tarjetas con efectos glassmorphism
   - Gestión automática de medicamentos
   - Alertas de caducidad
   - Recordatorios de toma
   - Conexión Bluetooth y RFID
   - Historial y estadísticas

4. **Galería**
   - Showcases del dispositivo físico
   - Aplicación móvil Android
   - Sistema RFID
   - Panel de control
   - Placeholder para video demo

5. **Equipo**
   - Perfiles de desarrolladores
   - Enlaces sociales (LinkedIn, GitHub, Email)
   - Información institucional

6. **Contacto**
   - Formulario de contacto funcional
   - Métodos de contacto
   - Mapa de ubicación (placeholder)

7. **Footer**
   - Links de navegación
   - Redes sociales
   - Información del proyecto

---

## 🚀 Tecnologías Utilizadas

### Frontend
- **HTML5** - Estructura semántica
- **CSS3** - Estilos avanzados con variables CSS
- **JavaScript (ES6+)** - Interactividad y animaciones
- **Font Awesome** - Iconografía
- **Google Fonts** - Tipografías Poppins y Orbitron

### Hardware (Proyecto IoT)
- **ESP32** - Microcontrolador principal
- **RFID RC522** - Lector de etiquetas (13.56 MHz)
- **LCD 16x2** - Display de información
- **Buzzer** - Alertas sonoras
- **Bluetooth BLE** - Comunicación con smartphone

### Software
- **Android (Java/Kotlin)** - Aplicación móvil nativa
- **SQLite** - Base de datos local
- **Bluetooth API** - Comunicación con ESP32

---

## 📂 Estructura del Proyecto Web

```
pharmasafe/
│
├── index.html              # Página principal
│
├── css/
│   └── style.css           # Estilos principales con efectos futuristas
│
├── js/
│   ├── particles.js        # Sistema de partículas animadas
│   └── main.js             # Funcionalidad principal e interactividad
│
└── README.md               # Documentación
```

---

## 🎨 Características Técnicas de la Web

### Animaciones Implementadas
- **Partículas interactivas** con Canvas API
- **Scroll reveal** con Intersection Observer
- **Efecto parallax** en elementos hero
- **Hover effects 3D** en tarjetas
- **Transiciones suaves** con cubic-bezier
- **Pulsos luminosos** en iconos tecnológicos

### Interactividad
- **Menú móvil responsivo** tipo hamburguesa
- **Navegación con scroll suave** entre secciones
- **Botón "scroll to top"** con fade-in/out
- **Formulario de contacto** con validación
- **Sistema de notificaciones** para feedback
- **Efecto tilt 3D** en tarjetas glassmorphism

### Rendimiento
- **Lazy loading** de animaciones
- **Optimización de CSS** con variables
- **Event delegation** para mejor performance
- **RequestAnimationFrame** para animaciones fluidas

---

## 🌐 URIs Funcionales

### Navegación Principal
- `/` o `index.html` - Página principal
- `#inicio` - Sección Hero
- `#como-funciona` - Timeline del sistema
- `#caracteristicas` - Características del producto
- `#galeria` - Galería y demo
- `#equipo` - Información del equipo
- `#contacto` - Formulario de contacto

---

## 🔧 Instalación y Uso

### Requisitos
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- No requiere instalación de dependencias

### Ejecución Local
1. Clona o descarga el repositorio
2. Abre `index.html` en tu navegador
3. ¡Listo! La página se carga automáticamente

### Despliegue
Para publicar en producción:
1. Ve a la pestaña **Publish** en el panel
2. Haz clic en **Deploy**
3. Obtén tu URL pública

---

## 📊 Componentes del Sistema IoT (Hardware)

### Arquitectura del Dispositivo

```
┌─────────────────────────────────────┐
│         DISPOSITIVO PHARMASAFE      │
│                                     │
│  ┌──────────┐      ┌──────────┐   │
│  │  ESP32   │◄────►│ RFID-RC522│   │
│  └────┬─────┘      └──────────┘   │
│       │                             │
│       ├─────► LCD 16x2              │
│       ├─────► Buzzer                │
│       └─────► Bluetooth BLE         │
│                       │              │
└───────────────────────┼─────────────┘
                        │
                        ▼
              ┌──────────────────┐
              │   APP ANDROID    │
              │                  │
              │  • Gestión de    │
              │    medicamentos  │
              │  • Alertas       │
              │  • Estadísticas  │
              │  • SQLite DB     │
              └──────────────────┘
```

---

## 🎯 Funcionalidades del Sistema Completo

### Hardware (ESP32 + RFID)
✅ Detección automática de medicamentos vía RFID  
✅ Visualización de información en LCD  
✅ Alertas sonoras con buzzer  
✅ Comunicación Bluetooth con smartphone  
✅ Bajo consumo energético  

### Aplicación Móvil (Android)
✅ Registro de medicamentos  
✅ Programación de horarios de toma  
✅ Alertas de caducidad  
✅ Notificaciones push  
✅ Historial de adherencia  
✅ Gráficos y estadísticas  
✅ Sincronización con dispositivo ESP32  

---

## 🔮 Características No Implementadas (Roadmap)

### Próximas Funcionalidades
- [ ] Integración con API de base de datos de medicamentos
- [ ] Reconocimiento óptico de códigos de barras (OCR)
- [ ] Sistema de múltiples usuarios
- [ ] Panel web de administración
- [ ] Integración con wearables (smartwatches)
- [ ] Exportación de reportes médicos en PDF
- [ ] Conexión WiFi para sincronización en la nube
- [ ] Asistente por voz con comandos
- [ ] Integración con Google Calendar
- [ ] Modo offline completo en la app

### Mejoras Técnicas Pendientes
- [ ] Backend con API REST (Node.js/Python)
- [ ] Base de datos en la nube (Firebase/MongoDB)
- [ ] Autenticación de usuarios
- [ ] Dashboard web para médicos
- [ ] Sistema de notificaciones por email/SMS
- [ ] Análisis predictivo con Machine Learning

---

## 🛠️ Desarrollo del Proyecto

### Equipo de Desarrollo
**Desarrolladores:**
- Desarrollo IoT & Hardware (ESP32, RFID)
- Desarrollo de Software & App Android
- Diseño UI/UX de la web

**Institución:**
- Universidad / Centro de Estudios

### Contacto
- **Email:** pharmasafe@proyecto.edu
- **GitHub:** github.com/pharmasafe
- **LinkedIn:** [Perfil del equipo]

---

## 📝 Pasos Recomendados para Continuar

### Fase 1: Desarrollo Web ✅ (Completada)
- [x] Diseño y maquetación de la página web
- [x] Implementación de animaciones futuristas
- [x] Sistema de navegación responsive
- [x] Efectos glassmorphism y neón

### Fase 2: Prototipo Hardware (En Progreso)
- [ ] Montaje del circuito ESP32 + RFID
- [ ] Programación del firmware en Arduino IDE
- [ ] Integración con LCD y buzzer
- [ ] Pruebas de lectura RFID

### Fase 3: Desarrollo App Móvil (Planificada)
- [ ] Diseño de interfaces en Figma
- [ ] Desarrollo en Android Studio
- [ ] Implementación de base de datos SQLite
- [ ] Integración Bluetooth con ESP32
- [ ] Sistema de notificaciones

### Fase 4: Integración y Pruebas
- [ ] Sincronización hardware-software
- [ ] Pruebas de usuario
- [ ] Ajustes basados en feedback
- [ ] Documentación técnica completa

### Fase 5: Despliegue
- [ ] Publicación de la web en hosting
- [ ] Subida de la app a Google Play Store
- [ ] Materiales de marketing
- [ ] Video demo profesional

---

## 📚 Recursos Adicionales

### Documentación Técnica
- [Datasheet ESP32](https://www.espressif.com/en/products/socs/esp32)
- [RFID RC522 Library](https://github.com/miguelbalboa/rfid)
- [Android Developer Guide](https://developer.android.com/)
- [Bluetooth Low Energy](https://developer.android.com/guide/topics/connectivity/bluetooth-le)

### Inspiración de Diseño
- Interfaces de salud digital (Apple Health, Google Fit)
- Diseño Material 3 de Google
- Tendencias de glassmorphism y neumorphism
- Paletas de colores médicos modernos

---

## 📄 Licencia

Este proyecto es un prototipo educativo desarrollado como parte de un proyecto académico.

---

## 🌟 Agradecimientos

Gracias a todos los que han contribuido al desarrollo de **PharmaSafe**, un proyecto que busca mejorar la calidad de vida mediante tecnología accesible y innovadora.

---

**PharmaSafe** - *Tu botiquín inteligente, siempre conectado* 💊✨

---

**Última actualización:** 2024  
**Versión:** 1.0.0 (Prototipo Web)