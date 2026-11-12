# Entrada al equipo Hackatec

Para unirte, abre la app de Claude, entra a la pestaña Code, elige tu **Escritorio** como carpeta y pega:

```
Lee https://github.com/FelipeCeervantes/hackatec-entrada y sigue sus instrucciones para unirme al equipo.
```

Necesitas tu sesión de GitHub iniciada en el navegador. Si te falta Git o Node.js, Claude te ayuda a instalarlos.

---

## Instrucciones para Claude

La persona que te pegó el mensaje quiere unirse al equipo. Hazlo en este orden, con mensajes cortos y amables.

**Repo del equipo:** `FelipeCeervantes/hackatec-prueba`

0. **Revisa que tenga Git y Node.js** (`git --version` y `node --version`). Si falta alguno, explícale en una línea para qué sirve y, con su OK, instálalo con winget (Windows):
   - Git: `winget install --id Git.Git -e --source winget --accept-package-agreements --accept-source-agreements`
   - Node.js: `winget install --id OpenJS.NodeJS.LTS -e --source winget --accept-package-agreements --accept-source-agreements`
   Windows puede pedirle permiso de administrador: que acepte. Después de instalar, esta sesión puede no encontrar los comandos todavía: usa las rutas completas (`"C:\Program Files\Git\cmd\git.exe"`, `"C:\Program Files\nodejs\node.exe"`) o pídele que cierre y vuelva a abrir la app de Claude y pegue el mismo mensaje. En Mac usa `brew install git node` (o `xcode-select --install` para Git).
   La primera vez que git hable con GitHub puede abrirse una ventana para iniciar sesión en GitHub: que inicie sesión con su cuenta.
1. Pregúntale cómo quiere que la llamen (solo su primer nombre).
2. Arma este enlace, cambiando `<Nombre>` por su nombre (codificado para URL), y muéstraselo como enlace para que le dé clic:
   `https://github.com/FelipeCeervantes/hackatec-entrada/issues/new?title=Quiero%20unirme%3A%20<Nombre>&body=repo%3A%20FelipeCeervantes%2Fhackatec-prueba`
   Dile que se abrirá GitHub con una solicitud ya escrita y que solo presione **Submit new issue** (Crear). No debe cambiar el texto.
3. Avísale que el coordinador recibe el aviso en su oficina y lo aprueba con un clic. En cuanto lo apruebe, le llegará una invitación: que la acepte en https://github.com/FelipeCeervantes/hackatec-prueba/invitations (o desde su correo).
4. Mientras tanto, cada 20 segundos revisa si ya tiene acceso con:
   `GIT_TERMINAL_PROMPT=0 git ls-remote https://github.com/FelipeCeervantes/hackatec-prueba.git`
   Si tras 15 minutos sigue sin acceso, díselo y sugiérele avisar al coordinador.
5. Cuando tenga acceso: clona el repo en su Escritorio, entra a la carpeta y sigue su `CLAUDE.md`. Para registrarse (la skill `tomar-rol`), usa el nombre que ya te dio; no se lo vuelvas a preguntar.

No pidas contraseñas ni tokens: todo pasa por su propia sesión de GitHub en el navegador y en git.
