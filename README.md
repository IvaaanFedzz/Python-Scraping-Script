# Python-Scraping-Script
Python Scraping Script es una herramienta ligera de recolección OSINT orientada a ciberseguridad. Introduces una URL y el script explora el dominio para localizar y descargar archivos públicos expuestos, incluyendo PDFs, imágenes y audios (y otros recursos estáticos habituales).


# Python Scraping Script (OSINT File Collector)

Herramienta en Python orientada a **ciberseguridad / OSINT** que, a partir de una URL, **recorre el dominio** y **extrae archivos públicos** (PDFs, imágenes, audios y otros recursos) para ayudarte a identificar exposición accidental de información.

> Uso típico: reconocimiento pasivo/activo controlado, inventariado de recursos públicos, auditoría rápida de contenido indexable y recopilación de evidencias.

---

## Características

- ✅ Entrada simple: **una URL** y listo.
- ✅ Descarga y organiza automáticamente:
  - **PDFs** (`.pdf`)
  - **Imágenes** (`.jpg`, `.jpeg`, `.png`, `.webp`, `.gif`, `.svg`)
  - **Audios** (`.mp3`, `.wav`, `.ogg`, `.m4a`, `.flac`)
  - (Opcional) otros estáticos: `.zip`, `.rar`, `.docx`, etc.
- ✅ Filtrado por **mismo dominio** (evita salir a terceros).
- ✅ Evita duplicados mediante hashing / control por URL.
- ✅ Estructura de salida limpia y práctica para análisis.
- ✅ Enfoque “day-to-day”: rápido, directo y sin complicaciones.

---

## Casos de uso en ciberseguridad

- OSINT: localizar **documentos públicos** y media expuesta.
- Auditorías: detectar **publicación involuntaria** de PDFs con metadatos sensibles.
- Pentesting (fase de reconocimiento): inventario de endpoints y recursos estáticos.
- Blue Team: verificación de **higiene de publicación** en dominios corporativos.

---

## Requisitos

- Python 3.10+ recomendado

Dependencias típicas (según implementación):
- `requests`
- `beautifulsoup4`
- `lxml` (opcional, recomendado)
- `tqdm` (opcional)

---

## Instalación

```bash
git clone https://github.com/tu-usuario/tu-repo.git
cd tu-repo
pip install -r requirements.txt


## USO

Ejemplo básico:

python scraper.py --url "https://example.com"
