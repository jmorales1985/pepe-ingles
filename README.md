# 🦜 Pepe habla inglés

Juego web gratuito para que niños aprendan **inglés** jugando, con la mascota **Pepe el loro**. Estilo Lingokids: colorido, con pronunciación en voz, animaciones y estrellitas de recompensa.

## ✨ Características

- **6 temas:** Animales, Colores, Números, Comida, Familia y Cuerpo.
- **Modo Aprender** 📖 — tarjetas con imagen, palabra en inglés y en español. El juego *pronuncia* cada palabra en voz alta.
- **Modo Jugar** 🎮 — escucha la palabra en inglés y toca la imagen correcta. Da estrellas, sonidos, confeti y ánimo en español.
- **Instalable (PWA):** se agrega a la pantalla de inicio del celular y **funciona sin conexión** tras la primera carga.
- Diseño pensado para niños: botones grandes, colores tropicales y respeto por *reducir movimiento*.

## 🚀 Publicar en Vercel (recomendado)

Es un sitio **estático de un solo archivo**, no requiere build.

1. Subí este contenido a un repositorio de GitHub (con `index.html` en la raíz).
2. En [vercel.com/new](https://vercel.com/new) importá el repo.
3. Deploy sin configurar nada. Queda en `https://<tu-proyecto>.vercel.app`.

Cada `git push` redespliega automáticamente.

### Alternativa: GitHub Pages

Settings → Pages → Source: `main` / `root`. Queda en `https://<usuario>.github.io/<repo>`.

## 💻 Correr localmente

El service worker necesita un servidor (no abrir el archivo con `file://`):

```bash
python3 -m http.server 8000
# abrir http://localhost:8000
```

## 🛠️ Tecnología

- HTML, CSS y JavaScript puro (sin frameworks ni dependencias).
- Voz con la **Web Speech API** del navegador (suena mejor en Chrome/Safari con voces en inglés instaladas).
- Efectos de sonido con **Web Audio API** (generados, sin archivos).
- Tipografías: Fredoka + Nunito (Google Fonts).

## 📁 Estructura

```
index.html        # el juego completo
manifest.json     # configuración PWA
sw.js             # service worker (offline)
icons/            # íconos de la app
```

## 📄 Licencia

Uso libre educativo. Los emojis son del sistema operativo de cada dispositivo.
