# 🚀 TURISRAM DOMINICANA — Resumen de Progreso del Proyecto

> **Documento de Control y Estado Actual del Proyecto**  
> Creado para retomar el desarrollo sin necesidad de revisar el historial completo de la conversación.

---

## 📌 1. Información General del Proyecto

- **Cliente / Empresa**: TurisRam Dominicana (Traslados Ejecutivos, Transfers Aeropuerto y Tours Privados).
- **Eslogan Oficial**: *"Viaja cómodo. Llega seguro."*
- **Número Oficial de WhatsApp**: `+1 (849) 752-7408` (`18497527408`).
- **Enlace de Reseñas de Google**: `https://g.page/r/CQIGM1irEXmnEBM/review`
- **Ficha Oficial en Google Maps**: [TurisRam Dominicana en Google Maps](https://www.google.com/maps/place/TurisRan+Dominicana+%7C+Transporte+%26+Tours/@18.5959418,-75.4170951,6z/data=!3m1!4b1!4m9!1m2!2m1!1sServicio+de+transporte!3m5!1s0x20c2c276dca7ff65:0xa77911ab58330602!8m2!3d18.6698995!4d-70.130055!16s%2Fg%2F11yf57_w_r)
- **Desarrollador / Creador**: [Goglite](https://goglite.com/)

### 🛠️ Stack Tecnológico & Infraestructura
- **Framework**: Astro 5 (Modo Estático)
- **Estilos**: Tailwind CSS v4 + Vanilla CSS Custom Animations
- **Control de Versiones**: GitHub (`vmatos001/turisram-dominican`, rama `master`)
- **Hosting & Despliegue en Vivo**: Firebase Hosting (`turisram-dominican`)
- **URL en Producción**: **[https://turisram-dominican.web.app](https://turisram-dominican.web.app)**

---

## 🎨 2. Sistema de Diseño Corporativo

- **Estética Visual**: *Dark Mode Luxury Executive*.
- **Paleta de Colores Primaria**:
  - `Negro Fondo Principal`: `#0A0A0A` / `#050505` / `#030303`
  - `Dorado Corporativo / Cápsulas`: `#D4AF37`
  - `Azul Accent`: `#3B6998`
  - `Blanco Texto`: `#F7F5F0` / `#FFFFFF`
  - `Verde WhatsApp`: `#25D366`
- **Insignia Corporativa "Cápsula Dorada"**:
  - `bg-[#D4AF37] text-[#0A0A0A] text-xs font-extrabold px-5 py-1.5 rounded-full uppercase tracking-widest font-['Barlow_Condensed'] shadow-md`
- **Tipografías Google Fonts**:
  - Titulares & Insignias: `Barlow Condensed` (300, 400, 500, 600, 700, 900)
  - Parrafos & Detalles: `Barlow Semi Condensed`
  - Acentos Itálicos / Eslogan: `Lora`

---

## 🧱 3. Estructura y Módulos Desarrollados en la Landing Page (`index.astro`)

### 📍 Módulo 1: Header / Navbar (`src/components/Header.astro`)
- Barra de navegación flotante semi-transparente con logo HD de TurisRam Dominicana.
- Menú responsive mobile/desktop.
- Botón principal de cotización inmediata por WhatsApp.

### 📍 Módulo 2: Hero Section & Carrusel Inclinado a 6°
- Imagen de fondo nítida `santo-domingo-noche.webp` con opacidad y resplandor radial.
- Copys oficiales de TurisRam Dominicana con estado "Choferes VIP Disponibles en Tiempo Real".
- **Carrusel Inclinado 6°**: 3 columnas verticales de imágenes con scroll infinito continuo.
- **Marquesina Ticker**: Cinta deslizante continua con servicios VIP principales.

### 📍 Módulo 3: Live Quote Engine Widget (`src/components/QuoteModal.astro`)
- Formulario modal de cotización rápida en tiempo real.

### 📍 Módulo 4: Catálogo Executive VIP
- Bento Grid con tarjetas de servicios destacados (*Isla Saona VIP, Traslado Aeropuerto PUJ/SDQ, Van Ejecutiva VIP, Samaná & Salto del Limón*).
- **Botón Giratorio SVG 1**: Texto circular rotatorio con animación smooth scroll dirigida hacia el formulario final (`#booking-final`).
- Efecto hover con sombra de luz dorada trasera (`hover:shadow-[0_20px_50px_rgba(212,175,55,0.28)]`).

### 📍 Módulo 5: Banner Panorámico & Garantía de Servicio
- Marco contenedor de imagen panorámica ampliado (`max-w-[94rem]`).
- Cápsula Dorada `GARANTÍA DE SERVICIO` y Titular H2 `¿POR QUÉ ELEGIR TURISRAM DOMINICANA?`.
- **Botón Giratorio SVG 2 Magnético**: Sigue suavemente la posición del cursor con animación LERP en JavaScript.
- **Scroll Scrub Paralelo**: 4 tarjetas de pilares que ingresan en diagonal en paralelo sin cruzarse al hacer scroll.
- Marquesina horizontal ultra-lenta continua de derecha a izquierda.

### 📍 Módulo 6: Sección de Testimonios Sticky Card Stacking (`src/components/TestimonialsSection.astro`)
- Cápsula Dorada `EXPERIENCIAS REALES DE CLIENTES`.
- **Reseñas Verificadas de Google Maps**: Opiniones 5.0★ reales copiadas directamente de la ficha oficial de negocio (*Kimberlin Montero, Familia Isasi, Rafalis Montero, Mercedes Méndez, Acelis Montero*).
- Botón directo **"Escribe una reseña"** enlazado a la ficha de Google.
- Tarjetas apilables con efecto CSS `sticky top-[100px + index * 28px]`.

### 📍 Módulo 7: Sección Sobre Nosotros Preview (`src/components/AboutPreviewSection.astro`)
- Marco de corte SVG invertido personalizado (`clip-inverted-turisram`).
- Tagline Insignia `✱ SOBRE NOSOTROS` e iconos de redes sociales dorados reubicados.
- Métrica `100% COBERTURA NACIONAL | 5.0 ★` ajustada dentro de la muesca inferior.
- Firma corporativa `TURISRAM DOMINICANA` y botón **`CONOCE MÁS SOBRE NOSOTROS →`** hacia `/nosotros`.

### 📍 Módulo 8: Acordeón Preguntas Frecuentes (FAQs)
- Cápsula Dorada `PREGUNTAS FRECUENTES`.
- Preguntas y respuestas desplegables sobre traslados, peajes, vehículos y reservas.

### 📍 Módulo 9: Bloque Final — Formulario de Cotización / Reserva VIP (`src/components/FinalBookingSection.astro`)
- Cápsula Dorada `COTIZACIÓN RÁPIDA & RESERVA VIP`.
- Titular H2: **"Reserva tu transporte seguro en menos de 2 minutos"**.
- Formulario de alta conversión con 8 campos clave: *Origen, Destino, Fecha, Hora, Pasajeros, Equipaje, Nombre y WhatsApp/Email*.
- Botón principal que envía automáticamente la cotización formateada a WhatsApp.
- Avisos legales y políticas de privacidad.

### 📍 Módulo 10: Footer Corporativo (`src/components/Footer.astro`)
- Logotipo de gran tamaño `logo-turisram.webp`.
- Fila de iconos de redes sociales dorados (*Google Maps, WhatsApp, Instagram, Facebook*).
- Enlaces de navegación rápida y cobertura de los 5 aeropuertos principales del país.
- Crédito de autor oficial: **`Creada por Goglite`** enlazado a [goglite.com](https://goglite.com/).
- Marca de agua gigante `TURISRAM` en el fondo (`z-0`) alineada a la base inferior en versión PC (`hidden md:block absolute bottom-0`) sin espacio vacio por debajo.

### 📍 Elementos Globales:
- **Botón Flotante de WhatsApp** (`src/components/WhatsAppButton.astro`): Botón permanente en la esquina inferior derecha con icono oficial SVG y z-index máximo.
- **Preloader VIP de Carga** (`src/components/Preloader.astro`): Pantalla de carga con fondo negro (`#000000`), logo oficial con movimiento de flotación suave y texto `"CARGANDO..."` con animación de recorrido de brillo horizontal en gradiente. Desaparición fluida tras la carga del DOM.
- **Puntero Custom VIP en Negativo** (`src/components/CustomCursor.astro`): Cursor personalizado de dos elementos (punto central y anillo seguidor) con desplazamiento elegante por animación LERP en JavaScript y efecto en negativo (`mix-blend-difference`), con expansión interactiva al hacer hover sobre botones y enlaces.

---

## 🚦 4. Estado de los Comandos de Despliegue

Cada cambio realizado se prueba localmente y se despliega con:

```powershell
# 1. Compilación Limpia
npx astro build

# 2. Commit & Push a GitHub
git add .
git commit -m "Descripción del cambio"
git push origin master

# 3. Despliegue a Producción Firebase
npx -y firebase-tools@latest deploy --only hosting
```

---

## 📌 5. Pasos Sugeridos para la Próxima Sesión

1. **Páginas Secundarias**:
   - Refinar y adaptar los diseños completos de `/nosotros`, `/servicios` y `/contacto` manteniendo la línea estética de la página de inicio.
2. **Enlaces Definitivos de Redes Sociales**:
   - Actualizar los enlaces finales de Instagram, Facebook y TikTok cuando el cliente los suministre.
3. **Imágenes Definitivas de Flota**:
   - Sustituir las imágenes temporales por la galería fotográfica oficial de los vehículos definitivos.

---
*Archivo generado automáticamente por Antigravity AI — 2026.*
