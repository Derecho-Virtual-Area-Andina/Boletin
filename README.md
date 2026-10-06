# Boletín Derecho Virtual

Boletín quincenal de la Facultad de Derecho, modalidad virtual, de la Fundación Universitaria del Área Andina. El sitio se publica con GitHub Pages desde este repositorio y su dirección pública es `https://derecho-virtual-area-andina.github.io/Boletin/`.

## Contenido del repositorio

| Archivo | Para qué sirve | ¿Se modifica cada quincena? |
|---|---|---|
| `index.html` | Diseño y funcionamiento del boletín. Incluye el logotipo oficial y las tipografías Brown y Areandina Voz, con aval institucional para uso web. | No |
| `contenidos.csv` | Todas las entregas, una fila por ítem. La página lo lee en cada visita. | Sí, se reemplaza completo |
| `recursos/plantilla-contenidos.xlsx` | Hoja que diligencian los responsables de cada sección, con instrucciones por columna. | No |
| `recursos/plantilla-correo.html` | Correo que invita a abrir el boletín. | Se copia y ajusta en cada envío |
| `recursos/banner-correo.jpg`, `logo-blanco.png`, `logo-verde.png` | Imágenes que el correo carga desde este sitio. | No |
| `imagenes/AAAA-NN/` | Imágenes de cada entrega, una carpeta por número (ej. `imagenes/2026-02/`). | Se agrega una carpeta por entrega |
| `.nojekyll` | Indica a GitHub que publique los archivos tal cual. | No |

## Ciclo de cada entrega

El ciclo dura quince días. Durante los primeros ocho, cada responsable agrega sus filas a la hoja de contenidos con estado «Borrador», usando el número de la nueva entrega (02, 03, etc.) y conservando las filas de entregas anteriores, que forman el archivo del boletín. Los tres o cuatro días siguientes corresponden a revisión y armado, y los últimos al envío.

1. Al cierre de la recolección se revisa la hoja y se cambia a «Aprobado» el estado de las filas que saldrán publicadas.
2. Se exporta la pestaña «Contenidos» como CSV con codificación UTF-8 y se nombra `contenidos.csv`.
3. Antes de subirlo, se abre el boletín con `?editor=1` al final de la dirección, se pulsa «Cargar contenido» y se elige el CSV. La página muestra cómo quedará la entrega y advierte errores (fechas vencidas, notas jurídicas sin fuente, síntesis demasiado largas, nodos inexistentes). Esta vista previa ocurre solo en el navegador de quien la hace y no publica nada.
4. En el repositorio se usa «Add file», luego «Upload files», se arrastra el nuevo `contenidos.csv` y se confirma con «Commit changes». El archivo anterior queda guardado en el historial.
5. En pocos minutos el sitio muestra la nueva entrega como la más reciente.
6. Si la entrega trae imágenes, se suben antes a su carpeta en `imagenes/` (ver la sección Imágenes).
7. Se prepara el correo a partir de `recursos/plantilla-correo.html` con los tres destacados de la entrega y el enlace terminado en `?n=` más el número de la entrega.

## Imágenes

Durante la recolección, los responsables suben sus imágenes a la carpeta compartida de Drive y pegan el enlace del archivo en la columna `imagen` de la hoja, junto con una descripción breve (`imagen_alt`) y el crédito (`imagen_credito`). Al armar la entrega, el editor descarga esas imágenes, las reduce a 1200 píxeles de ancho en JPG o WEBP (menos de 250 KB cada una), las sube a `imagenes/AAAA-NN/` y reemplaza en la hoja el enlace de Drive por la ruta del repositorio, por ejemplo `imagenes/2026-02/lunes-juridico.jpg`. Los nombres de archivo van en minúsculas, sin tildes ni espacios.

La página acepta enlaces de Drive si la imagen está compartida con cualquier persona que tenga el enlace, pero Google limita ese uso y la imagen puede dejar de verse sin aviso; la vista previa editorial lo señala. Si una imagen no carga, la página la oculta y la nota se muestra completa.

Solo se publican fotos propias, del banco institucional de Mercadeo o con licencia que permita su uso, y las fotos de personas identificables requieren su autorización. Las imágenes tomadas de medios de prensa no se usan; para una noticia jurídica basta el enlace a la fuente.

## Recuperar una versión anterior

Si un `contenidos.csv` sale con errores, en el repositorio se abre el archivo, se pulsa «History», se elige la versión correcta, se descarga y se vuelve a subir.

## Reglas de marca

Los colores provienen del Manual de Identidad Visual de Areandina. Gestión académica usa verde (#7FB536), Actualidad jurídica magenta (#E6007E), Comunidad Areandina naranja (#F59C2F) y Para repasar gris (#606060), con los tonos oscuros de la paleta tonal del manual donde hay texto sobre color. El logotipo no se modifica ni se recompone; ante cualquier duda de uso se consulta a disenomercadeo@areandina.edu.co.

## Administración

La organización en GitHub tiene como propietario al docente que la creó. Cuando el programa designe otra cuenta administradora, se agrega en «People» con el rol Owner antes de cualquier cambio de responsable, de modo que el boletín nunca quede sin administración.

## Datos del sitio

Organización en GitHub: `Derecho-Virtual-Area-Andina`. Repositorio: `Boletin` (con B mayúscula; la dirección distingue mayúsculas). Dirección pública: https://derecho-virtual-area-andina.github.io/Boletin/
