# STREAMING GAMAZ 1.5 — IMAP multiproveedor y prueba Microsoft sin secreto

Lee primero **PRUEBA-HOTMAIL-SIN-SECRETO.md**: contiene los archivos para actualizar, cómo probar desde el panel con las cinco variables existentes y los límites del modo público experimental. Conserva tu mailboxes.json actual, incluyendo la carpeta Newsletter de Zoho.

La modalidad de aplicación propia y la documentación multiproveedor anterior se conservan abajo.

# STREAMING GAMAZ 1.4 — IMAP multiproveedor

Lee primero **ACTUALIZAR-PROVEEDORES.md**. Incluye los archivos que debes actualizar, la configuración Microsoft paso a paso y cómo conservar tus datos actuales.

- Proveedores: Gmail, Microsoft/Hotmail/Outlook, Zoho, Yahoo, iCloud, AOL, GMX e IMAP personalizado.
- Cifrado: SSL/TLS directo o STARTTLS obligatorio. Microsoft y Gmail usan TLS directo, puerto 993.
- Gmail existente: compatible con sus registros y claves de aplicación actuales.
- Microsoft: botón de autorización OAuth2, verificación IMAP y renovación cifrada guardada en GitHub.
- Otros: contraseña o clave de aplicación admitida por su proveedor. IMAP personalizado exige IMAP LOGIN sobre TLS y no integra automáticamente otros OAuth.
- Usuarios, correos permitidos, permisos por asunto, gestión de asuntos y buscador: conservados.
- Build: `npm run build`; salida: `dist`. No hacen falta D1 ni KV.

Mantén las cinco variables existentes. Solo para Microsoft añade MICROSOFT_CLIENT_ID, MICROSOFT_CLIENT_SECRET y MICROSOFT_REDIRECT_URI, siguiendo la guía. No cambies MAILBOX_ENCRYPTION_KEY.

Conserva tu script.js, mailboxes.json, lib/mail-rules.js, administrador, imágenes y estilos actuales al actualizar. No subas node_modules, dist ni secretos.

Las pruebas son simuladas y la compilación se valida con Wrangler; prueba tus conexiones reales después de configurar y desplegar.
