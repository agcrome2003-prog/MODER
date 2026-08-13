# Animated Sign In / Sign Up — integración para el tema Horizon

Adaptación del componente `modern-login-signup` (React/shadcn) a **Liquid + JS vanilla + CSS**, para el tema **Horizon** de Shopify. Conserva el fondo animado WebGL (grilla de puntos con shader GLSL vía Three.js) y la tarjeta oscura con toggle Sign In ⇄ Sign Up.

## ⚠️ Léelo antes de instalar: qué SÍ y qué NO hace esto

Horizon usa el sistema nuevo de **Customer Accounts** de Shopify. El formulario real donde el cliente escribe su contraseña/código lo aloja Shopify en su propio dominio — el tema **no tiene ni puede tener** una plantilla de login editable, y Shopify no permite CSS/JS personalizado ahí (aplica incluso en Shopify Plus).

Por eso esta sección:
- **SÍ** reproduce el diseño exacto que pediste (fondo animado, tarjeta, toggle) como una página de tu tienda (por ejemplo `/pages/bienvenida`).
- **SÍ** conecta los botones de email a las rutas reales de Shopify (`/account/login`, `/account/register`) — el clic funciona de verdad.
- **NO** reemplaza la pantalla real donde Shopify pide el email/código — el cliente hace clic acá y Shopify le vuelve a pedir el email en su propia página (no hay forma de saltarse ese paso).
- **NO** incluye login con Google/GitHub/Apple funcional — Shopify no lo soporta nativamente. Los botones existen en el código pero están **ocultos por defecto** hasta que les cargues una URL real (ver más abajo).

Para que la página *real* de Shopify (`/account/login`) se vea lo más parecida posible, usa el editor nativo: **Configuración → Cuentas de clientes → Marca**, ahí puedes poner tu logo, colores y una imagen de fondo.

## Archivos de esta carpeta

```
shopify/
├── sections/animated-auth.liquid       # Sección: HTML + CSS (schema con settings editables)
├── assets/animated-auth.js             # Custom elements: fondo WebGL + toggle sign in/up
├── assets/three.min.js                 # Three.js r128 auto-alojado (evita CDN externo/CSP)
└── templates/page.animated-auth.json   # Plantilla de página lista para usar
```

No usé la librería de Three.js desde un CDN externo (como hacía el componente original) porque Shopify aplica una política de seguridad de contenido a nivel de plataforma que solo permite recursos de `cdn.shopify.com` — un `<script src="https://cdnjs...">` corre el riesgo real de quedar bloqueado. `three.min.js` va como asset propio del tema, mismo origen, sin riesgo.

## Instalación (copiar y pegar en el editor de Shopify)

Como no tengo conectado el repo de GitHub de tu tema Horizon en esta sesión, estos son los pasos manuales. Si en algún momento me das el `owner/repo` exacto de ese tema, puedo hacer el commit directamente ahí en vez de esto.

1. Entra a **Shopify Admin → Tienda online → Temas**, en tu tema Horizon (o una copia/borrador si prefieres probar primero) abre **⋮ → Editar código**.
2. En **Sections**, click **Add a new section**, nómbrala `animated-auth` y pega el contenido de `sections/animated-auth.liquid`.
3. En **Assets**, sube (**Add a new asset → Upload file**) los dos archivos tal cual:
   - `assets/animated-auth.js`
   - `assets/three.min.js`
4. En **Templates**, click **Add a new template**, elige tipo `page`, nombre `animated-auth` (JSON), y pega el contenido de `templates/page.animated-auth.json`.
5. Guarda todo.
6. Ve a **Tienda online → Páginas → Agregar página**. Ponle un título (ej. "Bienvenida" o "Acceder"), y en el panel derecho, bajo **Plantilla de la página**, elige `page.animated-auth`. Guarda y visita la página.

## Personalización sin tocar código

Desde el editor de temas (**Customize**), seleccionando la sección "Animated sign in / sign up", puedes cambiar:
- Textos (títulos, subtítulos, iniciales del logo, texto legal del pie)
- Colores (fondo, tarjeta, botón)
- Apagar la grilla animada (`Show animated dot-grid background`)
- Activar botones sociales si instalas una app de login social — actívalos y pega la URL real que te dé esa app; si dejas la URL vacía, el botón permanece oculto (para no mostrar un botón que no hace nada).

## Antes de publicarlo en producción

- [ ] Revisa que `/account/login` y `/account/register` funcionen para tu tienda (deberían, son las rutas nativas de Shopify).
- [ ] Si activas botones sociales, prueba el flujo completo con la app que elijas.
- [ ] Ajusta colores/logo desde el editor para que combine con tu marca.
- [ ] Opcional: en **Configuración → Cuentas de clientes → Marca**, alinea el logo/colores de la página de login *real* de Shopify con este diseño.
