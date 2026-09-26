# ReBlueOutlet + Supabase

La tienda pública lee los productos desde Supabase y el panel `/admin/` permite iniciar sesión y gestionar productos.

## Configuración
- `supabase-config.js` contiene la URL del proyecto y la Publishable key.
- No se usa localStorage para guardar productos.
- Las imágenes nuevas se guardan en Supabase Storage, bucket `product-images`.
- El JSON original `catalogo-productos.json` se conserva solo como fuente para la importación inicial.

## Panel
`/admin/`

## Importación de productos antiguos
El siguiente paso es incorporar una herramienta de importación de los 325 productos del JSON antiguo, subiendo también sus imágenes Base64 a Storage. No borrar el JSON hasta verificar la migración.
