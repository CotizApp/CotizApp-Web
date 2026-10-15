# CotizApp Web

Sitio institucional y documentación pública de CotizApp.

## Alcance

- sitio completamente estático;
- sin cookies, formularios, analytics ni código server-side;
- preparado para Firebase Hosting clásico en `cotizapp-production`;
- contenido legal y operativo alineado con los contratos actuales de Android y API.

## Vista local

Desde la raíz del repositorio:

```bash
python3 -m http.server 8080 --directory public
```

Luego abrir `http://localhost:8080`.

## Publicación

Antes de publicar, revisar los textos legales. El despliegue debe hacerse contra el proyecto explícito:

```bash
npx firebase-tools@15.32.1 deploy --project cotizapp-production --only hosting:public
```

