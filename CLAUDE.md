# Oropella — Catálogo Web

## Qué es este proyecto
Sitio estático autónomo desplegado en **GitHub Pages** → https://oropella.github.io  
Un solo archivo principal (`index.html`) + carpeta de imágenes (`images/`).  
No hay build, no hay framework, no hay node_modules. Solo HTML/CSS/JS puro.

## Estructura
```
oropella-web/
├── index.html        # Todo el sitio: HTML + CSS + JS + array de productos
├── images/           # Fotos de productos (OP-001.jpg … OP-043.jpg)
└── CLAUDE.md
```

## Deploy
```bash
cd ~/oropella-web
git add index.html          # o también images/ si hay fotos nuevas
git commit -m "descripción en español"
git push
```
El sitio se actualiza en **1-2 minutos** en https://oropella.github.io.  
**Siempre hacer push al final, sin pedirle confirmación a Daniella.**

## Estructura de un producto (en index.html)
```js
{ 
  cod: "OP-044",                    // código único, secuencial
  nombre: "Nombre del producto",
  categoria: "Aretes",              // Aretes | Pulseras | Cadenas | Anillos | Dijes
  precio: "L. 385",                 // o "Consultar"
  material: "Enchape",              // Enchape | Laminado | Acero
  disponible: true,                 // false = muestra badge "Agotado"
  img: `images/OP-044.jpg`          // NUNCA base64, siempre ruta relativa
}
```

## Catálogo actual (43 productos — OP-001 a OP-043)
| Código | Nombre | Categoría | Precio | Material |
|--------|--------|-----------|--------|----------|
| OP-001 | Argolla Croissant Dorada | Aretes | L. 385 | Enchape |
| OP-002 | Arete Infinito Dorado | Aretes | L. 385 | Enchape |
| OP-003 | Argolla Retorcida Plateada | Aretes | L. 390 | Enchape |
| OP-004 | Arete Tiburón Plateado | Aretes | L. 385 | Enchape |
| OP-005 | Argolla Texturizada Grande | Aretes | L. 430 | Enchape |
| OP-006 | Argolla Doble Dorada | Aretes | L. 385 | Enchape |
| OP-007 | Argolla Croissant Texturizada | Aretes | L. 385 | Enchape |
| OP-008 | Argolla Twisted Dorada | Aretes | L. 390 | Enchape |
| OP-009 | Argolla Alada Dorada | Aretes | L. 300 | Enchape |
| OP-010 | Argolla Croissant Plateada | Aretes | L. 385 | Enchape |
| OP-011 | Argolla Twisted Plateada | Aretes | L. 390 | Enchape |
| OP-012 | Piercing Flor Zirconia | Aretes | L. 260 | Enchape |
| OP-013 | Huggie Estrella Zirconia | Aretes | L. 315 | Laminado |
| OP-014 | Arete Abanico Dorado | Aretes | L. 185 | Acero |
| OP-015 | Huggie Liso Dorado | Aretes | L. 315 | Laminado |
| OP-016 | Arete Corazón Plateado | Aretes | L. 400 | Laminado |
| OP-017 | Arete Cubo Zirconia | Aretes | L. 375 | Laminado |
| OP-018 | Arete Trébol Dorado | Aretes | L. 375 | Acero |
| OP-019 | Cuff Perlas Dorado | Aretes | L. 285 | Acero |
| OP-020 | Cuff Hoja Zirconia | Aretes | L. 285 | Laminado |
| OP-021 | Pulsera Bangle Dorada | Pulseras | L. 375 | Acero |
| OP-022 | Pulsera Corazón Dorada | Pulseras | L. 490 | Laminado |
| OP-023 | Pulsera Perla Dorada | Pulseras | L. 340 | Laminado |
| OP-024 | Pulsera Cadena Dorada | Pulseras | L. 375 | Laminado |
| OP-025 | Pulsera Zirconia Dorada | Pulseras | L. 375 | Laminado |
| OP-026 | Cadena Cordón Fina Plateada | Cadenas | L. 150 | Acero |
| OP-027 | Cadena Eslabón Cuadrado Plateada | Cadenas | L. 150 | Acero |
| OP-028 | Cadena Eslabón Cuadrado Dorada | Cadenas | L. 150 | Acero |
| OP-029 | Cadena Cilíndrica Dorada | Cadenas | L. 150 | Acero |
| OP-030 | Cadena Clásica Dorada | Cadenas | L. 150 | Acero |
| OP-031 | Cadena Diseño Dorada | Cadenas | L. 150 | Acero |
| OP-032 | Cadena Eslabón Grueso Dorada | Cadenas | L. 150 | Acero |
| OP-033 | Cadena Cordón Grueso Plateada | Cadenas | L. 150 | Acero |
| OP-034 | Anillo Chunky Plateado | Anillos | L. 285 | Laminado |
| OP-035 | Anillo Chunky Cadena | Anillos | L. 315 | Laminado |
| OP-036 | Anillo Corazón Delgado | Anillos | L. 215 | Laminado |
| OP-037 | Anillo Perla Zirconia | Anillos | L. 215 | Laminado |
| OP-038 | Anillo Bolas Zirconia | Anillos | L. 250 | Laminado |
| OP-039 | Anillo Chunky Croissant | Anillos | L. 285 | Laminado |
| OP-040 | Anillo Bicolor | Anillos | L. 340 | Laminado |
| OP-041 | Anillo Líneas Cruzadas | Anillos | L. 315 | Laminado |
| OP-042 | Cadena Serpiente | Cadenas | L. 360 | Acero |
| OP-043 | Dije Inicial | Dijes | L. 67 | Laminado |

## Reglas importantes
- **Nunca** usar base64 para imágenes de productos. Siempre `images/{COD}.jpg`
- **Nunca** tocar otros archivos, solo `index.html` e `images/`
- El próximo código disponible es **OP-044**
- WhatsApp de contacto: `50489159876`
- Responder siempre en **español**
- Hacer push siempre al final sin pedir confirmación

## Flujo para agregar un producto nuevo
1. Daniella provee la imagen (archivo adjunto o ruta local)
2. Guardar en `images/OP-044.jpg` (o el código que corresponda)
3. Agregar la entrada al array `products` en `index.html` antes del `];`
4. `git add index.html images/OP-044.jpg && git commit -m "..." && git push`

## Flujo para editar un producto existente
- Buscar por código (ej. `OP-022`) o nombre en `index.html`
- Cambiar el campo necesario (precio, nombre, disponible, etc.)
- Commit + push

## Flujo para marcar agotado / reponer
- Agotado: cambiar `disponible: true` → `disponible: false`
- Reponer: cambiar `disponible: false` → `disponible: true`
