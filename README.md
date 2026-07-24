# Proyectos Portfolio — Micaela García

Sitio 100% dinámico: `index.html` le pregunta a GitHub en vivo qué carpetas de proyecto existen y qué contenido tiene cada una. No hay ningún archivo central que editar — cada proyecto vive solo en su propia carpeta.

## Estructura por proyecto

```
nombre-del-proyecto/
├── texto.json          ← obligatorio, la info del proyecto
├── imagenes/            ← poné acá tus fotos (cualquier nombre, cualquier formato)
├── videos/              ← tus videos (mp4)
└── documentos/          ← PDFs sueltos (cualquier nombre)
```

**Regla única:** el nombre de la carpeta del proyecto (ej: `paracaidismo-chascomus`) es libre, pero no puede tener espacios ni tildes — usá guiones.

## texto.json — plantilla para copiar

```json
{
  "title": "Nombre del proyecto",
  "role": "Tu rol en el proyecto",
  "category": "grid1",
  "context": "Una línea de contexto sobre el cliente/proyecto.",
  "bullets": [
    "Qué hiciste, punto 1",
    "Qué hiciste, punto 2"
  ],
  "narrative": "Párrafo narrativo opcional, en primera persona.",
  "result": "Resultado medible del proyecto.",
  "docLabels": {
    "nombre-real-del-archivo.pdf": "Nombre lindo que se va a ver en el sitio"
  }
}
```

`docLabels` es opcional — si no lo completás, el sitio usa el nombre del archivo tal cual.

## Categorías (van en "category")
- `grid1` — Identidad y diseño editorial
- `grid2` — Producción y experiencias creativas
- `grid3` — Contenido digital
- `grid4` — Marketing estratégico

## Para sumar un proyecto nuevo
1. Creá una carpeta nueva en la raíz del repositorio, con el nombre del proyecto.
2. Adentro, creá `texto.json` con la plantilla de arriba, completa.
3. Subí tus fotos a `imagenes/`, videos a `videos/`, PDFs a `documentos/` — con cualquier nombre.
4. Listo. No hay paso 5. El sitio lo va a mostrar solo la próxima vez que alguien lo abra.

## Ejemplo real ya armado
La carpeta `paracaidismo-chascomus/` tiene el `texto.json` completo como ejemplo — copiá esa estructura para los demás proyectos.

## Ya no existen (de la versión anterior)
- `data/proyectos.json` — ya no se usa.
- Nombres de archivo obligatorios (`slug-1.jpg`) — ya no hace falta, cualquier nombre funciona.
- Declarar cuántas fotos/videos tiene un proyecto — el sitio las cuenta solo.
