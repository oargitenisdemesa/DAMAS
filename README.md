# Damas

Juego de damas españolas: contra la máquina (3 niveles, elegir color), dos jugadores en el mismo móvil, online y ranking. Con reloj por jugada y deshacer.

## Publicar en GitHub Pages
1. Sube estos archivos a la raíz de un repositorio: `index.html`, `firebase-config.js` (y opcionalmente `firestore.rules` y este README).
2. En el repositorio: Settings → Pages → Branch `main` / carpeta `/ (root)` → Save.
3. La web quedará en `https://TU-USUARIO.github.io/NOMBRE-REPO/`.

Con solo esto ya funcionan **máquina** y **mismo móvil**.

## Activar online y ranking (Firebase, gratis)
1. Entra en https://console.firebase.google.com y crea un proyecto.
2. Build → Authentication → Get started → activa el proveedor **Anónimo**.
3. Build → Firestore Database → Create database (modo producción).
4. Pestaña Reglas de Firestore: pega el contenido de `firestore.rules` y publica.
5. Project settings → Tus apps → añade una app web (`</>`) y copia el objeto `firebaseConfig`.
6. Pega esos valores en `firebase-config.js` y súbelo al repositorio.
7. En Authentication → Settings → Authorized domains, añade `TU-USUARIO.github.io`.

Nota: el ranking lo escribe cada cliente, así que alguien con conocimientos podría falsear puntos.
