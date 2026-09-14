# Dylan Mazzei Site

Breve guía para subir este repositorio a GitHub y desplegar en Coolify.

Pasos rápidos:

1. Crea un repo en GitHub (p. ej. `dylanmazzei-site`).
2. Desde este directorio local, inicializa Git y sube:

```
cd "c:\\Users\\Andres\\Documents\\DYLANN\\horizons"
git init
git checkout -b main
git add .
git commit -m "Initial commit"
git remote add origin <URL_DEL_REPO>
git push -u origin main
```

3. En Coolify: crea un recurso tipo Application, conecta con GitHub y selecciona la rama `main`.
4. Elige método de build (Nixpacks o Static/Docker según el proyecto) y agrega las variables de producción en la interfaz de Coolify.

Notas de seguridad:

- No subas archivos con secretos. Usa `.env` local y guarda variables en Coolify.
- Rellena `.env.example` con las claves que tu despliegue necesita (sin valores reales).

Si quieres, puedo crear el repositorio en GitHub por ti si instalas y autorizas la GitHub CLI (`gh`) o me das el URL remoto para empujar.
