# CinnamonEQ
# 🎛️ Cinnamon EQ (Cinnamon Audio DSP Lab)

![License](https://shields.io)
![Platform](https://shields.io)
![Audio Engine](https://shields.io)

**Cinnamon EQ** es un rack analítico de ecualización paramétrica y gráfica profesional de 15 bandas desarrollado como una aplicación web móvil de alto rendimiento (PWA). Inspirado en la densidad de datos de *Bitchord/Archivetune* y la icónica nostalgia de personalización de *Winamp*, este entorno procesa audio a 60 FPS con aceleración por hardware, ofreciendo herramientas premium de audio de forma 100% gratuita y abierta para toda la comunidad audiófila.

---

## 🕯️ Dedicatoria Especial

> *Este software no tiene precio, no tiene anuncios y nunca tendrá costo alguno. Es un regalo puro para la comunidad y para los amantes de la música.*
>
> **Cinnamon EQ** fue creado con profundo amor, respeto y nostalgia **en memoria de mi perrita y hermanita, Canela (Cinnamon)**, quien partió de este mundo hace 2 años. Ella fue mi compañera de vida fidelísima, mi alegría en los días oscuros y mi sombra silenciosa mientras escuchaba música. 
> 
> Aunque sus patitas ya no caminen a mi lado, su nombre y su luz quedan inmortalizados en este código. Dondequiera que estés, Canela, este monumento digital es para ti. Que la música siga sonando fuerte, limpia y eterna, directo hasta el cielo. 🐾✨

---

## 🛠️ Especificaciones Técnicas y Características Premium

### 1. Procesamiento DSP de Alta Precisión
*   **15 Bandas ISO en Cascada:** Filtros en serie `BiquadFilterNode` configurados en las frecuencias audiófilas de precisión: 25Hz, 40Hz, 63Hz, 100Hz, 160Hz, 250Hz, 400Hz, 630Hz, 1kHz, 1.6kHz, 2.5kHz, 4kHz, 6.3kHz, 10kHz y 16kHz.
*   **Fase Optimizada:** Bandas extremas en `lowshelf`/`highshelf` e intermedias en `peaking` calibradas con un factor Q estricto de `0.707` para evitar valles de fase o sonido hueco.
*   **Limitador Brickwall:** Nodo de compresión dinámico final (`threshold: -0.5`, `ratio: 20`) que actúa como escudo contra el clipping digital si saturas los decibelios.
*   **Módulos de Expansión:** Incluye perillas (*knobs*) dedicadas para **Bass Boost** (refuerzo de transitorios a 45Hz) y **Spatializer** (expansión de escena sonora *Soundstage* mediante desfase por Efecto Haas).

### 📊 2. Pantalla LCD Analítica (Canvas 60 FPS)
Fondo con rejilla técnica logarítmica (20Hz - 20kHz) interactiva al tacto que conmuta entre 5 modos visuales avanzados:
*   **Lámpara de Lava Procedural:** Burbujas orgánicas reactivas en tamaño y velocidad a los subgraves.
*   **Barras Winamp Pro:** Espectrómetro logarítmico de caída lenta de picos (*peak drop*).
*   **Osciloscopio Líquido:** Onda senoidal continua con persistencia de fósforo CRT simulada.
*   **Túnel Estelar 3D:** Campo de 250 partículas con efecto de hipervelocidad *Warp* activado por los golpes de graves.
*   **Espectrograma Circular:** Anillo simétrico de 64 vectores radiales en 360°.

### 🎭 3. Motor de Skins Mutables & Tuner
Inyección radical de variables CSS nativas para mutar el chasis físico del ecualizador:
*   `Classic Winamp` (Gris industrial texturizado retro)
*   `Cyberpunk Neón` (Fluorescente fosforescente con glitch sutil)
*   `Aero Y2K Gel` (Cápsulas de gel translúcidas con brillos 3D esmerilados)
*   `Pixel 8-Bit` (Bordes rígidos de 4px y tipografía arcade)
*   `Sunset / Deep Ocean` (Degradados fluidos orgánicos y minimalistas)
*   *Tuner Integrado:* 3 Selectores de color nativos para personalizar las variables de la skin activa en tiempo real.

### 🧠 4. Asistente Acústico por IA Local
Barra de comandos por lenguaje natural que analiza semánticamente las peticiones del usuario (ej: *"quiero bajos profundos de concierto y voces claras"*) y calcula algebraicamente la curva de ecualización óptima, moviendo los sliders físicos de forma animada automáticamente y **100% libre de APIs de pago**.

---

## 📥 Clonación e Instalación PWA

Al estar construido sobre la capa cliente del navegador, puedes ejecutar este entorno sin necesidad de instalar servidores locales.

1. Clona el repositorio:
   ```bash
   git clone https://github.com
   ```
2. Abre el archivo `index.html` en cualquier navegador moderno.
3. Para dispositivos móviles, accede a través de tu servidor de despliegue (ej. GitHub Pages), abre el menú del navegador y selecciona **"Añadir a la pantalla de inicio"** para correr la app a pantalla completa y de manera offline gracias al Service Worker integrado.

---

## 📜 Licencia

Este proyecto está bajo la Licencia **MIT** - Siéntete libre de usarlo, modificarlo y compartirlo. Mantengamos el audio profesional abierto, transparente y accesible para todos en memoria de Canela.
