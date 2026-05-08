# Política de Privacidad de Quick Paste History

**Fecha de última actualización: 8 de mayo de 2026**

---

## 1. Recopilación y Uso de Información

Quick Paste History es una herramienta de gestión del portapapeles cuya función principal es registrar, administrar y recuperar el contenido del portapapeles localmente en su dispositivo.

### 1.1 Información que **no** recopilamos

- Información de identificación personal (nombre, número de identificación, dirección, etc.)
- Información sensible como contraseñas de cuentas, números de tarjetas bancarias, etc.
- Identificadores de dispositivo (IDFV, IDFA, etc.)
- Historial de navegación, información de ubicación
- Contactos, álbum de fotos, micrófono, datos de la cámara
- Estadísticas de comportamiento de uso o datos analíticos

### 1.2 Información a la que **accedemos**

Quick Paste History solo accede a la siguiente información localmente en su dispositivo, según sea necesario para sus funciones principales:

| Tipo de datos | Propósito | Carga al servidor |
|---------------|-----------|:-----------------:|
| **Contenido del portapapeles** | Registra texto/enlaces copiados por el usuario, compatible con búsqueda, favoritos y llenado rápido | Solo almacenamiento local |
| **iCloud** | Sincroniza el historial entre sus dispositivos a través de NSUbiquitousKeyValueStore | Solo sincronización privada de iCloud |
| **Compra desde la App Store** | Verifica el estado de compra de las funciones Pro (solo verificación del recibo) | No se recopilan detalles de compra |

> Todo el procesamiento de datos del portapapeles se realiza localmente en el dispositivo y **no se cargará a ningún servidor externo**.

---

## 2. Almacenamiento de Datos

### 2.1 Almacenamiento Local

- Los historiales del portapapeles se almacenan en una base de datos SwiftData dentro del sandbox de la aplicación
- La base de datos no está cifrada (el mecanismo de sandbox de Apple proporciona aislamiento a nivel del sistema)
- Los usuarios pueden borrar manualmente todo el historial

### 2.2 Sincronización de iCloud (Función Opcional)

- Una vez activada, el historial se sincroniza a través de `NSUbiquitousKeyValueStore` en su propia cuenta de iCloud
- Los datos están protegidos por los mecanismos de seguridad de iCloud y el desarrollador no puede acceder a ellos
- La sincronización se puede desactivar en cualquier momento en los ajustes
- Desactivar la sincronización no eliminará los datos locales

### 2.3 Retención de Datos

- El historial se conserva por defecto; los usuarios pueden eliminar manualmente entradas individuales o borrar todo
- La eliminación surte efecto de inmediato y es irreversible

---

## 3. Compartición de Datos

Quick Paste History **no comparte datos de usuarios con terceros**, incluyendo, pero sin limitarse a:

- No vende datos de usuarios
- No utiliza datos para publicidad o elaboración de perfiles de usuario
- No envía ningún contenido del portapapeles a API de terceros
- No incorpora SDK de análisis de terceros

---

## 4. Extensión de Teclado y Permisos

Quick Paste History proporciona una extensión de teclado (Keyboard Extension) para pegar rápidamente contenido del historial en cualquier aplicación:

- **Acceso**: La extensión de teclado solo se ejecuta cuando está activada y solo lee el contenido del portapapeles
- **Red**: La extensión de teclado no tiene permisos de acceso a la red
- **Aislamiento de datos**: La extensión de teclado comparte datos del sandbox con la aplicación principal, pero no los expone externamente

---

## 5. Lectura del Portapapeles

Quick Paste History lee el portapapeles en las siguientes ocasiones:
- Cuando la aplicación se ejecuta en primer plano, detecta cambios en el portapapeles y registra contenido nuevo
- Cuando el usuario comparte activamente contenido a Quick Paste History

Según los requisitos del sistema iOS, la primera lectura del portapapeles activará un diálogo de permiso a nivel del sistema. Los usuarios pueden gestionar este permiso en cualquier momento en los Ajustes del Sistema.

---

## 6. Privacidad Infantil

Quick Paste History no recopila información personal de niños.

---

## 7. Cambios en la Política de Privacidad

Si la política de privacidad cambia, actualizaremos la fecha de "Última actualización" en la parte superior de la página y notificaremos a los usuarios a través de anuncios dentro de la aplicación o notas de actualización de versión.

---

## 8. Contáctenos

Si tiene preguntas sobre la política de privacidad, contáctenos a través de los siguientes canales:

- **Desarrollador**: 陈修
- **Correo electrónico**: chensingyou@126.com
- **App**: Quick Paste History (Desarrollador: Singyou)

---

> **Resumen: Sus datos le pertenecen.** Quick Paste History no carga ningún contenido a servidores, no rastrea el comportamiento del usuario y no incorpora SDK de terceros. Todos los datos del portapapeles se procesan solo localmente en el dispositivo y en el espacio privado de iCloud.
