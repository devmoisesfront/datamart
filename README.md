# Datamart Dashboard (HTML)

Página de login + dashboard que incrusta un reporte de Power BI.

## Requisitos
- Navegador moderno (Chrome, Edge, Firefox, Safari).
- Conexión a internet para cargar la CDN de estilos y el iframe de Power BI.

## Uso
1) Abre `Index.html` en el navegador.
2) Ingresa las credenciales:
   - Usuario: `admin@acme.com`
   - Contraseña: `admin123`
3) Presiona **Entrar** o usa **Enter** en la contraseña.
4) Dentro del dashboard puedes ver el reporte y cerrar sesión con **Cerrar sesión**.

## Características
- Estilo glass, responsive (una columna en móvil, botones de ancho completo).
- Incrustación de Power BI con iframe.
- Botón de cierre de sesión que limpia credenciales de la vista.
- Validación simple en el cliente (sin backend).

## Notas de seguridad
- Las credenciales están embebidas solo para demo; en producción usa autenticación real (backend + tokens) y nunca expongas claves en el front.
- Considera servir sobre HTTPS si se usa en red.

## Personalización rápida
- Cambia el título en `<title>` dentro de `Index.html`.
- Ajusta el iframe de Power BI reemplazando la URL en el atributo `src`.
- Paleta: edita variables en `:root` (colores `--accent`, `--accent-2`, etc.).
