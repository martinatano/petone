# Catálogo Web — Guía de uso

## Estructura de archivos

```
/catalogo
  ├── index.html        ← Página de inicio
  ├── productos.html    ← Catálogo de productos
  ├── productos.csv     ← 📝 EL CLIENTE EDITA ESTE ARCHIVO
  └── /imagenes
        ├── 001_1.jpg
        ├── 001_2.jpg
        └── ...
```

---

## Cómo agregar productos (CSV)

Abrí `productos.csv` con Excel o Google Sheets y agregá una fila por producto:

| Columna      | Descripción                              | Ejemplo           |
|--------------|------------------------------------------|-------------------|
| `id`         | Código único del producto                | `042`             |
| `nombre`     | Nombre del producto                      | `Remera básica`   |
| `descripcion`| Descripción corta                        | `100% algodón`    |
| `precio`     | Precio sin símbolo (solo número)         | `4500`            |
| `categoria`  | Categoría (exactamente igual en todos)   | `Ropa`            |
| `foto1`      | Nombre del archivo de la foto principal  | `042_1.jpg`       |
| `foto2`      | Segunda foto (opcional)                  | `042_2.jpg`       |
| `foto3`      | Tercera foto (opcional)                  | `042_3.jpg`       |

> ⚠️ **Importante**: Si la descripción tiene comas, encerrala entre comillas dobles:
> `"Tela premium, 100% algodón"`

---

## Cómo agregar fotos

1. Nombrá cada foto con el formato: `{id}_{numero}.jpg`
   - Ej: `042_1.jpg`, `042_2.jpg`, `042_3.jpg`
2. Copiá todas las fotos a la carpeta `/imagenes`
3. Escribí el nombre del archivo en las columnas `foto1`, `foto2`, `foto3` del CSV

---

## Carga masiva desde Excel

### Opción 1 — Google Sheets (más simple)
1. Subí tu Excel a Google Drive
2. Abrilo con Google Sheets
3. Archivo → Descargar → CSV
4. Reemplazá `productos.csv` con el archivo descargado

### Opción 2 — Desde Excel directamente
1. Abrí el Excel
2. Archivo → Guardar como → CSV UTF-8
3. Reemplazá `productos.csv`

---

## Funcionalidades del catálogo

- ✅ Búsqueda en tiempo real por nombre o descripción
- ✅ Filtro por categoría (sidebar + dropdown mobile)
- ✅ Ordenamiento por nombre y precio
- ✅ Galería de hasta 3 fotos por producto con lightbox
- ✅ Paginación automática (24 productos por página)
- ✅ Responsive mobile
- ✅ Las categorías del inicio se generan automáticamente del CSV

---

## Hosting

Por ser archivos estáticos, podés subirlos a:
- **GitHub Pages** (gratis)
- **Netlify** (gratis, drag & drop)
- **Cualquier hosting compartido** (cPanel, FTP)

Solo necesitás subir los 3 archivos + la carpeta `/imagenes`.
# petone
