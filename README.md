# Python-Scraping-Script
Python Scraping Script es una herramienta ligera de recolección OSINT orientada a ciberseguridad. Introduces una URL y el script explora el dominio para localizar y descargar archivos públicos expuestos, incluyendo PDFs, imágenes y audios (y otros recursos estáticos habituales).


# Python Scraping Script — Document Collector (OSINT / Ciberseguridad)

Script en Python orientado a **ciberseguridad/OSINT**: introduces una URL y el script **rastrea el dominio** para localizar y descargar **todos los documentos públicos** que encuentre, incluyendo:

- **PDF** (`.pdf`)
- **Word** (`.doc`, `.docx`)
- **Documentos** (otros formatos configurables: `.txt`, `.rtf`, `.odt`, etc.)

El objetivo es facilitar el reconocimiento y la auditoría de exposición: recopilar evidencias, revisar metadatos y detectar publicación accidental de información.

---

## Qué hace exactamente

1. Recibe una URL inicial (seed).
2. Rastrea enlaces internos (mismo dominio) hasta agotar el alcance definido.
3. Identifica recursos descargables por extensión o por cabeceras HTTP.
4. Descarga y organiza todos los archivos detectados.
5. Genera un log y, si lo implementas, un reporte (CSV/JSON) para evidencias.

> El rango temporal (por ejemplo “del 2000 hasta hoy”) no es un filtro: el script descarga cualquier recurso público accesible, independientemente de su antigüedad.

---

## Salida en el Escritorio (automática)

Por defecto, el script crea una carpeta en tu Escritorio:

- Windows: `C:\Users\<usuario>\Desktop\scrape_<dominio>_<fecha>`
- Linux: `~/Desktop/scrape_<dominio>_<fecha>`
- macOS: `~/Desktop/scrape_<dominio>_<fecha>`

Dentro, separa por tipo:

# Python Scraping Script — Document Collector (OSINT / Ciberseguridad)

Script en Python orientado a **ciberseguridad/OSINT**: introduces una URL y el script **rastrea el dominio** para localizar y descargar **todos los documentos públicos** que encuentre, incluyendo:

- **PDF** (`.pdf`)
- **Word** (`.doc`, `.docx`)
- **Documentos** (otros formatos configurables: `.txt`, `.rtf`, `.odt`, etc.)

El objetivo es facilitar el reconocimiento y la auditoría de exposición: recopilar evidencias, revisar metadatos y detectar publicación accidental de información.

---

## Qué hace exactamente

1. Recibe una URL inicial (seed).
2. Rastrea enlaces internos (mismo dominio) hasta agotar el alcance definido.
3. Identifica recursos descargables por extensión o por cabeceras HTTP.
4. Descarga y organiza todos los archivos detectados.
5. Genera un log y, si lo implementas, un reporte (CSV/JSON) para evidencias.

> El rango temporal (por ejemplo “del 2000 hasta hoy”) no es un filtro: el script descarga cualquier recurso público accesible, independientemente de su antigüedad.

---

## Salida en el Escritorio (automática)

Por defecto, el script crea una carpeta en tu Escritorio:

- Windows: `C:\Users\<usuario>\Desktop\scrape_<dominio>_<fecha>`
- Linux: `~/Desktop/scrape_<dominio>_<fecha>`
- macOS: `~/Desktop/scrape_<dominio>_<fecha>`

Dentro, separa por tipo:

# Python Scraping Script — Document Collector (OSINT / Ciberseguridad)

Script en Python orientado a **ciberseguridad/OSINT**: introduces una URL y el script **rastrea el dominio** para localizar y descargar **todos los documentos públicos** que encuentre, incluyendo:

- **PDF** (`.pdf`)
- **Word** (`.doc`, `.docx`)
- **Documentos** (otros formatos configurables: `.txt`, `.rtf`, `.odt`, etc.)

El objetivo es facilitar el reconocimiento y la auditoría de exposición: recopilar evidencias, revisar metadatos y detectar publicación accidental de información.

---

## Qué hace exactamente

1. Recibe una URL inicial (seed).
2. Rastrea enlaces internos (mismo dominio) hasta agotar el alcance definido.
3. Identifica recursos descargables por extensión o por cabeceras HTTP.
4. Descarga y organiza todos los archivos detectados.
5. Genera un log y, si lo implementas, un reporte (CSV/JSON) para evidencias.

> El rango temporal (por ejemplo “del 2000 hasta hoy”) no es un filtro: el script descarga cualquier recurso público accesible, independientemente de su antigüedad.

---

## Salida en el Escritorio (automática)

Por defecto, el script crea una carpeta en tu Escritorio:

- Windows: `C:\Users\<usuario>\Desktop\scrape_<dominio>_<fecha>`
- Linux: `~/Desktop/scrape_<dominio>_<fecha>`
- macOS: `~/Desktop/scrape_<dominio>_<fecha>`

Dentro, separa por tipo:

# Python Scraping Script — Document Collector (OSINT / Ciberseguridad)

Script en Python orientado a **ciberseguridad/OSINT**: introduces una URL y el script **rastrea el dominio** para localizar y descargar **todos los documentos públicos** que encuentre, incluyendo:

- **PDF** (`.pdf`)
- **Word** (`.doc`, `.docx`)
- **Documentos** (otros formatos configurables: `.txt`, `.rtf`, `.odt`, etc.)

El objetivo es facilitar el reconocimiento y la auditoría de exposición: recopilar evidencias, revisar metadatos y detectar publicación accidental de información.

---

## Qué hace exactamente

1. Recibe una URL inicial (seed).
2. Rastrea enlaces internos (mismo dominio) hasta agotar el alcance definido.
3. Identifica recursos descargables por extensión o por cabeceras HTTP.
4. Descarga y organiza todos los archivos detectados.
5. Genera un log y, si lo implementas, un reporte (CSV/JSON) para evidencias.

> El rango temporal (por ejemplo “del 2000 hasta hoy”) no es un filtro: el script descarga cualquier recurso público accesible, independientemente de su antigüedad.

---

## Salida en el Escritorio (automática)

Por defecto, el script crea una carpeta en tu Escritorio:

- Windows: `C:\Users\<usuario>\Desktop\scrape_<dominio>_<fecha>`
- Linux: `~/Desktop/scrape_<dominio>_<fecha>`
- macOS: `~/Desktop/scrape_<dominio>_<fecha>`

Dentro, separa por tipo:

Uso

Básico:

python scraper.py --url "https://example.com"


“Scrapear todo”: limitaciones reales (importante)

El script puede descargar todo lo que sea públicamente accesible, pero existen límites inevitables:

No puede acceder a contenido que requiera login, tokens o APIs privadas.

No puede descubrir archivos no enlazados (a menos que añadas enumeración de rutas/wordlists).

Puede haber bloqueos por WAF, rate-limit, CAPTCHA, o permisos del servidor.

En sitios grandes, “todo” puede ser enorme: usa límites si es necesario.
