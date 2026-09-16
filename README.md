# PLO FARMA — Landing V2

Rediseño de la landing B2B de PLO Droguería.

## Imágenes

- `assets/plo-farma-logo.png` — logo oficial recortado y optimizado para el encabezado.
- `assets/bodega-farmaceutica-hero.jpg` — imagen alternativa de la bodega farmacéutica.
- `assets/control-inventario-plo.jpg` — sección de control de inventario.

Las versiones JPG están optimizadas para web; los PNG originales se conservan en `assets/`.

## Preinscripción

La landing incluye un formulario de preinscripción y una cuenta regresiva al 1 de octubre de 2026. Los registros se guardan en el proyecto Supabase `PLO Farma` (`bjdzivfwjxplbufqedko`), tabla `public.preinscripciones`.

La tabla tiene RLS activo. El rol público solo puede insertar registros que incluyan consentimiento; no puede leer, modificar ni eliminar datos. La landing utiliza únicamente la clave publicable de Supabase, nunca una clave secreta o `service_role`.

## Desarrollo local

```bash
python3 -m http.server 4173
```

Abrir `http://localhost:4173`.
