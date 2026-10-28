# Documentación del Proyecto: Innova ESPE 2026
---
## Estructura de Directorios
```text
ANDRANGO_EDWIN/
├── assets/
│   ├── imagenes/
│   └── video/
├── css/
│   └── styles.css
├── evidencias/
│   ├── escritorio.png
│   └── movil.png
├── index.html
└── README.md
````
## Decisiones de Maquetación y Distribución

La maquetación del portal se estructuró bajo el enfoque **Mobile First** para garantizar una experiencia óptima en dispositivos móviles y una escalabilidad fluida hacia pantallas más grandes:

- **Encabezado y Navegación (Flexbox):** Se utilizó Flexbox en la clase `.header-flex` para alinear horizontalmente el logotipo y la lista de navegación en escritorios, manteniendo la flexibilidad de apilarlos verticalmente en pantallas reducidas.
  
- **Sección de Bienvenida:** Diseñada mediante un contenedor de flujo flexible que distribuye el texto informativo y la imagen principal en dos columnas balanceadas a partir de dispositivos medianos.
  
- **Tarjeta de Proyectos (CSS Grid):** Se implementó CSS Grid en `.grid-proyectos` con `grid-template-columns: 1fr` en móviles y `repeat(3, 1fr)` mediante la regla `@media (min-width: 768px)`. Esto asegura que las tarjetas ocupen el ancho completo en celulares y se organicen automáticamente en tres columnas en monitores.

- **Ajuste de Imágenes y Herencia:** Se aplicó `object-fit: cover` a las imágenes de los proyectos para recortar y ajustar dinámicamente cualquier recurso multimedia dentro del cuadro designado sin deformar su relación de aspecto original.

- **Formulario de Registro:** Estructurado en bloques verticales mediante `.campo` para facilitar el llenado de datos y mantener una lectura clara de las etiquetas e inputs.

## Especificaciones Técnicas

### HTML5
- Maquetación semántica estructurada con `header`, `nav`, `main`, `section`, `article`, `table`, `form` y `footer`.

- Formulario de registro con validaciones nativas (`required`, `minlength`, `maxlength`, `pattern`, `type="email"`, `type="tel"`).

- Integración multimedia nativa con la etiqueta `video` y ubicación geográfica embebida con `iframe`.

### CSS3

- Estrategia de diseño adaptativo **Mobile First** con punto de quiebre en `768px` (`@media`).

- Distribución de elementos mediante **Flexbox** en navegación y **CSS Grid** en la tarjeta de proyectos.

- Aplicación de modelo de caja (`box-sizing: border-box`) y posicionamiento fijo (`position: fixed`) para la insignia flotante.

- Código modular optimizado por herencia de estilos.

## Instrucciones para Ejecutar desde Docker Hub
Puede descargar y probar la imagen directamente ejecutando en tu terminal:

```bash
docker pull edwinan21/innova-espe-2026
docker run -d -p 8080:80 edwinan21/innova-espe-2026
```
O buscar directamente en el respositorio de docker mediante este link:

https://hub.docker.com/r/edwinan21/innova-espe-2026

## Datos del Estudiante

- **Estudiante:** Edwin Lenin Andrango Sosapanta
   
- **Carrera:** Ingeniería de Software

- **Institución:** Universidad de las Fuerzas Armadas ESPE