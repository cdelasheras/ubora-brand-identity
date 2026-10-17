# Tipografía — Ubora

> Sistema extraído del **Investors Deck 2026** (fuentes embebidas y tamaños reales de uso). Las dos familias son gratuitas en Google Fonts.

---

## Familias

| Familia | Rol | Pesos en uso | Descarga |
|---|---|---|---|
| **Poppins** (sans-serif geométrica) | Titulares, cifras, etiquetas, botones, notas | ExtraLight 200 · Light 300 · Regular 400 · Medium 500 · SemiBold 600 · Bold 700 · ExtraBold 800 | [Google Fonts](https://fonts.google.com/specimen/Poppins) |
| **Merriweather** (serif) | Texto corrido, subtítulos y frases de apoyo | Light 300 · Light Italic 300 · Italic 400 | [Google Fonts](https://fonts.google.com/specimen/Merriweather) |

**La idea:** Poppins pone la fuerza y la estructura (lo que se lee primero); Merriweather pone la voz, el matiz humano. El contraste sans + serif es parte de la identidad, no un accidente.

El claim **"Passion for Energy"** es un lettering de brocha dibujado, no una tipografía. Se usa siempre como imagen (ver [logo.md](logo.md)); nunca se recrea con una fuente.

---

## Jerarquía

Tamaños de referencia para formato 1920×1080 (slides). En web, ver la columna de la derecha.

| Nivel | Fuente | Tamaño slide | Web (aprox.) | Ejemplo de uso |
|---|---|---|---|---|
| **Titular** | Poppins Bold | 40 pt | 32–40 px | "Rentabilidad demostrada sólo con recursos propios" |
| **Subtítulo / frase de apoyo** | Merriweather Light Italic | 40 pt (portadas) · 24 pt | 22–28 px | "Y no tiene quién lo orqueste." |
| **Cifra destacada** | Poppins Bold / ExtraBold | 40–60 pt | 40–56 px | +1.000 · 10M€ · +32% |
| **Subtítulo de bloque** | Poppins Bold o Medium | 18–24 pt | 18–20 px | Nombres de servicio, cabeceras de columna |
| **Cuerpo** | Merriweather Light | 18–24 pt | 16–18 px | Párrafos explicativos |
| **Etiqueta / tag** | Poppins Bold, MAYÚSCULAS | 14–15 pt | 12–13 px | "INSTALAMOS", tags turquesa de sección |
| **Nota / fuente / caption** | Poppins Light o ExtraLight | 14 pt | 12–13 px | Fuentes de datos, pies de gráfico |
| **Botón / CTA** | Poppins Bold, MAYÚSCULAS | — | 14–16 px | "CALCULA TU AHORRO" |

---

## Reglas

- **Titulares en Poppins Bold, en frase normal** (solo la primera letra en mayúscula). Las mayúsculas completas se reservan para tags y botones.
- **Itálica solo en Merriweather.** Es el recurso para la segunda línea que matiza o remata el titular. No usar Poppins Italic salvo excepción.
- **Interlineado:** titulares 1.1–1.2 · cuerpo 1.5–1.6.
- **Tracking:** normal en titulares y cuerpo; +5–10% en tags en mayúsculas.
- **Alineación:** a la izquierda por defecto. Centrado solo en portadas o frases sueltas.
- **Máximo:** una familia por nivel. No mezclar Merriweather en titulares ni Poppins en párrafos largos.
- **Mínimos:** 16 px para cuerpo en web; 12 px para notas.

---

## Sustitutos (cuando no se pueden instalar las fuentes)

| En lugar de | Usar |
|---|---|
| Poppins | Montserrat → Arial |
| Merriweather | Georgia |

En PowerPoint/Word corporativos, si se comparten con terceros: incrustar fuentes al guardar, o usar los sustitutos.

---

## CSS

```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700;800&family=Merriweather:ital,wght@0,300;1,300;1,400&display=swap');

:root {
  --font-head: 'Poppins', 'Montserrat', Arial, sans-serif;
  --font-body: 'Merriweather', Georgia, serif;
}

h1, h2, h3, .label, .btn, .stat { font-family: var(--font-head); font-weight: 700; }
body, p                          { font-family: var(--font-body); font-weight: 300; line-height: 1.55; }
.lede                            { font-family: var(--font-body); font-style: italic; font-weight: 300; }
.label, .btn                     { text-transform: uppercase; letter-spacing: .06em; }
.note                            { font-family: var(--font-head); font-weight: 300; font-size: 13px; }
```
