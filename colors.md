# Paleta de Colores — Ubora

> Valores extraídos del **Investors Deck 2026** (InDesign) y del lettering **"Passion for Energy"**. Son los colores que usa la marca hoy. Si diseño entrega valores Pantone/CMYK oficiales, se añaden aquí.

La marca vive en **oscuro**: fondo casi negro, texto blanco y acentos de color muy saturados que funcionan como "luz" sobre el negro. El crema se usa para romper el ritmo en slides de datos o comparativas.

---

## Base

| Nombre | HEX | RGB | Uso |
|---|---|---|---|
| **Ubora Black** | `#000000` | 0, 0, 0 | Fondo principal de slides, web y redes |
| **Carbón** | `#111619` | 17, 22, 25 | Fondos secundarios, tarjetas sobre negro, overlays de foto |
| **Blanco** | `#FFFFFF` | 255, 255, 255 | Titulares y texto sobre oscuro, logotipo en negativo |
| **Crema** | `#EDE7E4` | 237, 231, 228 | Fondo claro para gráficos, tablas y comparativas |

## Acentos

| Nombre | HEX | RGB | Uso |
|---|---|---|---|
| **Magenta Energy** | `#FF0075` | 255, 0, 117 | Color de impacto: dato destacado, serie principal en gráficos, CTA |
| **Ubora Blue** | `#0066FF` | 0, 102, 255 | Segundo color de marca: series de gráficos, iconos, enlaces |
| **Cian** | `#00D2FF` | 0, 210, 255 | Tercera serie en gráficos, detalles de interfaz |
| **Turquesa** | `#00FCCE` | 0, 252, 206 | Etiquetas/tags de sección (texto negro encima), indicadores |

Variante de azul para gráficos sobre crema: `#015BEE`.

## Degradado "Passion for Energy"

```
#D30989  →  #9727AB  →  #464FD9  →  #0A6DFA
magenta     morado      índigo      azul
```

- Dirección: de izquierda (magenta) a derecha (azul), ligeramente diagonal hacia arriba.
- Es el color del claim **"Passion for Energy"** y de las líneas de luz en el pie de los slides.
- Reservado para momentos de marca (portada, cierre, claim, firma). No usarlo de fondo en bloques de texto ni en gráficos.

---

## Proporciones orientativas

| Color | Peso en una pieza |
|---|---|
| Negro / Carbón | ~70% |
| Blanco (texto) | ~20% |
| Acentos (magenta, azul, cian, turquesa) | ≤10% |
| Degradado | Puntual, una vez por pieza |

Si una pieza va sobre crema: crema ~70%, negro para texto, y los mismos acentos.

---

## Gráficos y datos

Orden de series: **Ubora Blue → Magenta Energy → Cian → Turquesa**.
Cuando hay una cifra o año protagonista (ej. el salto de ingresos), va en magenta y el resto en azul.

---

## Contraste y accesibilidad

| Combinación | Ratio aprox. | Uso |
|---|---|---|
| Blanco sobre negro | 21:1 | ✅ Cualquier texto |
| Negro sobre crema | 17:1 | ✅ Cualquier texto |
| Negro sobre turquesa | 16:1 | ✅ Tags y etiquetas |
| Negro sobre cian | 12:1 | ✅ Etiquetas |
| Magenta sobre negro | 5.5:1 | ✅ Titulares y cifras grandes; evitar en texto pequeño |
| Blanco sobre magenta | 4:1 | ⚠️ Solo botones/CTA en bold y tamaño grande |
| Azul sobre negro | 4.3:1 | ⚠️ Cifras y titulares, no texto corrido |
| Blanco sobre azul | 4.7:1 | ✅ Botones y bloques |

---

## CTAs

| Botón | Fondo | Texto |
|---|---|---|
| Principal | Magenta Energy `#FF0075` | Blanco, Poppins Bold |
| Secundario | Transparente con borde blanco | Blanco |
| Sobre crema | Ubora Black | Blanco |

---

## Evitar

- ❌ El verde "eco" genérico del sector: no es color de Ubora.
- ❌ Amarillos/dorados solares como acento.
- ❌ Usar los cuatro acentos a la vez en una misma composición (máximo dos + el degradado puntual).
- ❌ Degradados propios con otros colores.
- ❌ Fondos blancos puros de gran superficie: si toca fondo claro, crema.

---

## Tokens (CSS)

```css
:root {
  --ubora-black:   #000000;
  --ubora-carbon:  #111619;
  --ubora-white:   #FFFFFF;
  --ubora-cream:   #EDE7E4;
  --ubora-magenta: #FF0075;
  --ubora-blue:    #0066FF;
  --ubora-cyan:    #00D2FF;
  --ubora-turquoise: #00FCCE;
  --ubora-gradient: linear-gradient(80deg, #D30989 0%, #9727AB 33%, #464FD9 66%, #0A6DFA 100%);
}
```
