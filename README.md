# Hub Innova Crayons

Hub digital de **Startup School 2026 · Aprende y Emprende**, del Centro de Emprendimiento **Innova Crayons**. Reúne en un solo lugar las guías, plantillas y el calendario del programa, los proyectos de los equipos y el avance de cada uno hacia el pitch final.

Sitio publicado: https://innovarayonshub.netlify.app/

## Qué incluye

- **Recursos:** guías, plantillas y un caso de estudio, con filtro por etapa de Design Thinking y botón de descarga.
- **Calendario del programa:** las 6 sesiones de Design Thinking (2 al 18 de noviembre) y la presentación final (21 de noviembre).
- **Proyectos:** los proyectos de los equipos y la etapa en la que está cada uno.
- **Mi progreso:** una ruta de 9 etapas que cada equipo marca al completarlas. El avance se guarda solo en el navegador de cada persona.

## Estructura del repositorio

```
hub-innova-rayons/
├── index.html          Todo el sitio (diseño, datos y código)
├── logo-innova.png     Logo de Innova Crayons
├── logo-startup.jpg    Logo de Startup School 2026
├── README.md           Este archivo
└── recursos/           PDFs y plantillas que se descargan desde el sitio
```

## Cómo editar el contenido

Todo vive en `index.html`. Los datos se editan en el bloque `<script>` del final, en cuatro listas:

| Lista | Qué controla |
|---|---|
| `SESSIONS` | El calendario del programa (fecha, sesión y mentor). |
| `RES` | Las tarjetas de la sección Recursos. |
| `PROJ` | Las tarjetas de la sección Proyectos. |
| `STEPS` | Las etapas de Mi progreso. |

Cada recurso de `RES` se escribe así:

```js
{k:"Plantilla", st:"Empatizar", t:"Mapa de empatía", p:"Qué piensa, siente, dice y hace tu usuario.", f:"Plantilla editable", u:"recursos/mapa-de-empatia.docx"},
```

| Campo | Significado |
|---|---|
| `k` | Tipo de recurso: Guía, Plantilla, Caso o Documento. |
| `st` | Etapa a la que pertenece (Empatizar, Definir, Idear, Prototipar, Modelo de Negocio, Pitch o Concurso). Es lo que usa el filtro. |
| `t` | Título de la tarjeta. |
| `p` | Descripción corta. |
| `f` | Formato y extensión, por ejemplo "PDF · 3 págs". |
| `u` | Ruta del archivo que se descarga. Si no se pone, la tarjeta muestra "Próximamente". |

Cada línea termina en coma. Una coma o comilla de menos puede hacer que el sitio deje de cargar, así que conviene revisar la página después de guardar.

## Cómo subir un recurso nuevo

1. Sube el archivo a la carpeta `recursos/` (en GitHub: **Add file → Upload files**).
2. Usa un nombre en minúsculas, sin espacios ni tildes (`mapa-de-empatia.docx`, no `Mapa Empatía.docx`).
3. En `index.html`, agrega o edita la línea del recurso en `RES` y escribe su ruta en `u:"recursos/nombre-del-archivo.ext"`. La ruta debe coincidir exactamente con el nombre del archivo.
4. Guarda los cambios (**Commit changes**) y revisa que el botón **Descargar** funcione en el sitio.

Funciona con PDF, Word, Excel y PowerPoint. GitHub acepta archivos de hasta 25 MB desde el navegador.

## Recursos del programa

| Recurso | Tipo | Etapa | Archivo en `recursos/` |
|---|---|---|---|
| Cómo entrevistar a tus usuarios | Guía | Empatizar | `guia-como-entrevistar-a-tus-usuarios.pdf` |
| Mapa de empatía | Plantilla | Empatizar | `mapa-de-empatia.docx` |
| Enunciado del problema | Plantilla | Definir | `enunciado-del-problema.docx` |
| Lluvia de ideas en 15 minutos | Guía | Idear | `guia-lluvia-de-ideas-en-15-minutos.pdf` |
| Lienzo de MVP | Plantilla | Prototipar | `lienzo-de-mvp.docx` |
| Prototipos con S/ 0 | Caso | Prototipar | `caso-prototipos-con-s-0.pdf` |
| Lean Canvas escolar | Plantilla | Modelo de Negocio | `lean-canvas-escolar.docx` |
| No es lo que dices, sino cómo lo dices | Guía | Pitch | Pendiente (material del taller de comunicación) |
| Estructura de pitch de 3 minutos | Plantilla | Pitch | `pitch-de-3-minutos.docx` |
| Bases oficiales Startup School 2026 | Documento | Concurso | Pendiente (las entrega la organización) |
| Ficha de proyecto final | Plantilla | Concurso | `ficha-de-proyecto-final.docx` |

Los recursos pendientes se muestran como "Próximamente" hasta que se suba su archivo.

## Calendario del programa

| Fecha | Sesión | Mentor |
|---|---|---|
| 2 de noviembre | Empatizar | Karol Boza Salas |
| 4 de noviembre | Definir | Luz A. Herrera |
| 9 de noviembre | Idear | Mate Valencia |
| 11 de noviembre | Prototipar | Cristhian Valle |
| 16 de noviembre | Modelo de Negocio | Diego Rodríguez |
| 18 de noviembre | Pitch | Por confirmar |
| 21 de noviembre | Presentación final ante el jurado | Jurado del concurso |

La meta mínima para la presentación final es tener un **MVP** y la **ficha de proyecto**.

## Notas

- Los proyectos que aparecen en la sección Proyectos son **de demostración**. Deben reemplazarse por los proyectos reales de los 10 equipos del concurso.
- El avance de Mi progreso se guarda en el navegador de cada persona y no se comparte entre dispositivos.
- Este repositorio es público: no subas datos personales de estudiantes ni documentos que no deban ser vistos por cualquiera.

---

Innova Crayons · Centro de Emprendimiento · Startup School 2026, primera edición.
