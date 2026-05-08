# Asistencia técnica de Quick Paste History

---

## 📧 Contactar al desarrollador

- **Correo electrónico**: chensingyou@126.com

Al enviar un correo electrónico, incluya lo siguiente:
1. Su versión de iOS
2. El modelo de su dispositivo
3. Una descripción detallada del problema o una captura de pantalla
4. Pasos para reproducir el problema (si corresponde)

---

## ❓ Preguntas frecuentes

### 1. ¿El portapapeles no se registra automáticamente?

Esto es una restricción de permisos de iOS. Asegúrese de:
1. Quick Paste History se ha ejecutado en primer plano al menos una vez
2. En el primer inicio, tocó "Permitir pegado" (ventana emergente de permisos del sistema)
3. Si lo rechazó anteriormente, vaya a **Configuración del sistema → Quick Paste History → Pegar desde otras apps** → cámbielo a **Permitir**
4. El historial del portapapeles solo se actualiza cuando la aplicación está activa en primer plano. Cada vez que pegue, abra la interfaz de la aplicación o su extensión de teclado.

---

### 2. ¿Cómo usar la extensión de teclado?

1. Vaya a **Configuración del sistema → General → Teclado → Teclados → Agregar nuevo teclado**
2. Seleccione **Quick Paste History**
3. Toque el nombre del teclado Quick Paste History → **Permitir acceso completo**
4. En cualquier campo de entrada de texto, mantenga presionada la tecla de cambio de teclado y deslice hacia arriba, luego cambie al teclado Quick Paste History para navegar y pegar contenido histórico

---

### 3. ¿La sincronización de iCloud no funciona?

1. Asegúrese de que todos sus dispositivos tengan la misma sesión de Apple ID iniciada
2. Asegúrese de que iCloud esté activado (Configuración del sistema → Perfil → iCloud → el estado debe mostrar "Iniciada sesión")
3. Abra Quick Paste History en diferentes dispositivos y espere unos 30 segundos: los datos se sincronizarán automáticamente
4. Si la sincronización no ocurre después de mucho tiempo, intente reiniciar la aplicación

> La sincronización se basa en `NSUbiquitousKeyValueStore`. Apple no proporciona una interfaz de actualización manual, y la sincronización generalmente se completa en decenas de segundos.

---

### 4. ¿Cómo borrar todo el historial?

En la página principal de la aplicación, toque el icono de configuración en la esquina superior derecha → en el menú de configuración, seleccione "Borrar todos los registros". Esta acción no se puede deshacer.

---

### 5. ¿Cómo comprar y usar las funciones Pro?

1. Toque el icono de configuración en la esquina superior derecha de la pantalla principal → **Actualización Pro**
2. Seleccione la versión Pro y realice una compra dentro de la aplicación
3. Las funciones se desbloquean automáticamente después de la compra
4. Los dispositivos con el mismo Apple ID pueden restaurar las compras (toque "Restaurar compra" en la página de compra)

---

### 6. ¿Qué es Quick Fill (Relleno rápido)?

Quick Paste History le permite agregar información de uso frecuente a Quick Fill con anticipación, proporcionando un acceso rápido en la extensión de teclado para pegar contenido común rápidamente.

---

### 7. ¿Cómo usar la función de búsqueda?

En la parte superior de la página principal hay una barra de búsqueda. Ingrese palabras clave para buscar contenido de texto en su historial. Los resultados se ordenan por relevancia.

---

### 8. ¿Mis datos están seguros?

- Todos los datos del portapapeles se almacenan únicamente en su dispositivo local y en su espacio privado de iCloud
- El desarrollador no puede acceder al contenido de su portapapeles
- No existe ningún servidor backend que reciba sus datos
- Consulte la política de privacidad para obtener más detalles

---

## 🐛 Reportar un error

Si encuentra un error, envíe un correo electrónico a chensingyou@126.com con **[Bug]** en el asunto.

Incluya en su correo electrónico:
- Versión de iOS
- Modelo del dispositivo
- Pasos para reproducir (cuanto más detallados, mejor)
- Capturas de pantalla o grabaciones de pantalla (si están disponibles)

---

## 💡 Sugerencias de funciones

¿Tiene nuevas ideas? No dude en enviarme un correo electrónico para discutirlas, con **[Sugerencia]** en el asunto. Leeré atentamente cada comentario.
