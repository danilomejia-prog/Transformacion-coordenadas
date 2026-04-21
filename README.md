# Transformador UTM WGS84 → PSAD56

Aplicación web estática para publicar en **GitHub Pages**.

## Funciones
- Importa un archivo `.csv`
- Permite seleccionar la columna de **Este** y **Norte**
- Transforma coordenadas **UTM WGS84 → UTM PSAD56**
- Descarga un nuevo `.csv` con los resultados

## Publicación en GitHub Pages
1. Crear un repositorio en GitHub.
2. Subir el archivo `index.html`.
3. Ir a **Settings > Pages**.
4. En **Build and deployment**, seleccionar la rama principal y carpeta raíz `/root`.
5. Guardar.
6. GitHub publicará la app con un enlace web.

## Columnas agregadas al CSV de salida
- `Este_PSAD56`
- `Norte_PSAD56`
- `EPSG_Origen`
- `EPSG_Destino`
- `Estado_Transformacion`

## Zonas soportadas
- WGS84 / UTM 17S → PSAD56 / UTM 17S
- WGS84 / UTM 18S → PSAD56 / UTM 18S
- WGS84 / UTM 17N → PSAD56 / UTM 17N
- WGS84 / UTM 18N → PSAD56 / UTM 18N

## Nota
La app usa `proj4js` y `PapaParse` desde CDN, por lo que funciona bien en GitHub Pages.
