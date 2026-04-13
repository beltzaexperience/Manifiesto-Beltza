# Beltza Experience · Manifiesto — Notas de Diseño
**Repo:** https://github.com/beltzaexperience/Manifiesto-Beltza  
**URL:** https://beltzaexperience.github.io/Manifiesto-Beltza/  
**Fecha de reconstrucción:** 13 de abril de 2026  

---

## Archivos
- `index.html` — estructura HTML completa
- `style.css` — todo el CSS (sin CDN externo, link directo)
- `hero-beltza.jpg` — foto hero (también en Flickr: https://live.staticflickr.com/65535/55205605695_a97483bcbd_h.jpg)
- `beltza-puno.png` — puño Beltza Records
- `logo-beltzarecords.jpg` — logo circular M06 Cara A
- `logo-beltzaexperience.jpg` — logo circular M06 Cara B
- `PI.jpeg` — foto frontón Salinas de Léniz (sección Credo)
- `jardines-jupiter.jpg` — foto entre credo e idiomas
- `13.png` — logo 13 transparente (fondo exterior quitado)

---

## Colores
```
--black:     #0a0a0a
--white:     #f2ede6  (crema cálido)
--red:       #b01a1a
--red-muted: #7a1212
--amber:     #c8922a
--muted:     #6b6155
--sapphire:  #0F52BA  (solo números de mandamientos y credo)
--cream:     #f0e8d8  (fondo credo y marquee inferior, mismo que Magic Bus)
```

---

## Tipografías
Cargadas desde Google Fonts:
- **Bebas Neue** — topband, brand-slash, números (01-10, 13), marquees, botones, tarjetas idiomas
- **Playfair Display** — títulos de mandamientos (.m-title), EL CREDO (.credo-title), firma Luis Beltza
- **Courier Prime** — cuerpo de texto en general

---

## Estructura general (de arriba a abajo)
1. **Topband** — BELTZA RECORDS · DONOSTIA · DONEZTEBE | idiomas + links | Azken Muga of Soul
2. **Brand-slash** — franja roja: BELTZA (negro) + EXPERIENCE (rojo sobre negro) + Puño
3. **Hero** — foto tienda pantalla completa, "Are You Experienced" arriba, subtítulo abajo
4. **Banda géneros** — marquee rojo: SOUL · JAZZ · PUNK...
5. **Mandamientos** — dos columnas: texto (flex:2, mín 800px) + fotos sidebar (flex:1)
6. **Marquee portadas** — discos de Flickr, borde rojo 3px
7. **Credo** — fondo crema #f0e8d8, texto negro, número 13 rojo, título Playfair
8. **Jardines de Júpiter** — foto ancho completo
9. **Brand-slash inferior** — BELTZA/RECORDS + logo 13
10. **Footer** — mismo que topband + "· Logos: Jon Mercero · 13: Luis Beltza ·"
11. **Marquee crema** — fondo #f0e8d8, texto negro
12. **Idiomas** — fondo negro, tarjetas flex 280-340px

---

## Mandamientos — detalles
- Números: Bebas Neue, `clamp(3rem,8vw,7rem)`, color **zafiro**
- Títulos: Playfair Display, `clamp(2.25rem,6vw,5.25rem)`
- Palabras tachadas: color rojo, raya blanca
- Citas (.m-quote): ámbar, borde izquierdo rojo
- Destacados (.m-quote--white): Bebas Neue, **rojo** (NWOBHM OR DIE, GREÑAS Y CHUPAS, etc.)
- Cara A / Cara B: Bebas Neue, **rojo**
- "Crumb cartografió...": ámbar itálica
- Jon Mercero / estrella tartésica: ámbar itálica
- Fotos sidebar: 16 fotos Álvaro Matximbarrena + discos + Anti-Credo, desde Flickr
- LOS MANDAMIENTOS label: Bebas Neue, **ámbar**, dentro de columna fotos

---

## Credo — detalles
- Fondo: #f0e8d8 con textura noise SVG sutil
- Color texto: negro (var(--black))
- 13: Bebas Neue, rojo, display:block arriba
- EL CREDO: Playfair Display, `clamp(3rem,8vw,7rem)`, negro
- π y AMOR: rojo dentro de la línea ámbar
- Frontón Salinas de Léniz: 0.85rem, ámbar
- "Ven y sentirás...": Playfair Display, 4 líneas, rojo en "AMOR revolucionario"
- EXPERIENCIA O MUERTE: Bebas Neue, rojo, enorme
- Firma Luis Beltza: Playfair Display, negro

---

## Tarjetas de idiomas — detalles
- Fondo sección: negro
- Tarjeta: `flex:1 1 280px; max-width:340px`, borde rojo 1px
- Cabecera: franja roja con idioma (ámbar sobre negro) + BELTZA negro / EXPERIENCE rojo sobre negro
- Subtítulo: ámbar itálica
- Cuerpo: blanco, 0.9rem
- 28 tarjetas: ES, EU, CA, EN, JA, FR, PT, AM, YUA, DE, RU, ZH, HI, AR, FA, IT, BN, TR, KO, VI, PL, UKR, NL, SW, WO, YO, QU, NAH
- Texto intro: Camarón + Quincy Jones + *Montreux Jazz Festival* en Playfair itálica ámbar

---

## Fonema UR
Todas las apariciones del fonema "ur" en el texto van en rojo `<span style="color:var(--red);">`.

---

## Responsive
- `<800px`: columnas mandamientos se apilan, fotos van a hamburguesa (selector TEXTO/FOTOS)
- `<600px`: topband y footer se apilan en vertical, brand-slash reduce tamaño

---

## Links topband
- DESDE (activo, blanco) · TIK · DES · DÈS · DE · SINCE · から · 1990
- beltzarecords.com · MAGIC BUS · UR-SAPIENS (inactivo, gris)

---

## Proyectos relacionados
- **Magic Bus:** https://github.com/beltzaexperience/magic-bus
- **UR-book:** pendiente de repo propio
- **Beltza Records:** https://www.beltzarecords.com
