# 🎵 FRED · Adivina la canción

Juego de memoria tipo *Simon* de **9 botones** que revela una canción por pedazos: entre más avanza la secuencia, más clara queda cuál es. Quien la reconoce, la adivina y gana el punto. Para 2–6 jugadores por turnos, con efectos (explosión/abucheo al fallar, celebración al ganar).

## Páginas

- **`index.html`** — el juego. Lee la biblioteca desde `canciones.json` y reproduce los MP3 de la carpeta `canciones/`.
- **`admin.html`** — administrador. Sube cada archivo de audio y lo etiqueta con **canción, artista y año**, guardándolo en este repositorio vía la API de GitHub.

Servidas con **GitHub Pages**:

- Juego: `https://soytorresllamas.github.io/fred-adivina-la-cancion/`
- Admin: `https://soytorresllamas.github.io/fred-adivina-la-cancion/admin.html`

## Cómo agregar canciones

1. Abre **`admin.html`**.
2. Pega tu **token personal de GitHub** con permiso *Contents: read/write* sobre este repo. Se guarda solo en tu navegador.
3. Elige el archivo MP3 (clips cortos de ~20–40 s funcionan mejor), escribe canción / artista / año y pulsa **Guardar en el repo**.
4. El admin sube el audio a `canciones/` y actualiza `canciones.json`. El juego lo toma en ~1 minuto (al republicar Pages).

## Estructura de datos

`canciones.json` es un arreglo:

```json
[
  { "file": "dancing-queen-abba.mp3", "song": "Dancing Queen", "artist": "ABBA", "year": "1976" }
]
```

El juego construye el título visible como `Canción — Artista (Año)`.

## ⚠️ Derechos de autor

Este repo es **público**. Subir música con copyright a un repo público puede infringir derechos de autor (riesgo de DMCA). Usa fragmentos cortos, música propia/libre, o cambia el repo a **privado** si necesitas más resguardo.
