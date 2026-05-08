# Despliegue en Azure Static Web Apps

Este documento describe el proceso para desplegar el proyecto en Azure usando el repositorio de GitHub `pokedex-angular-Juan`.

## Paso a paso

1. En el buscador de Azure, escribe **Static Web App**.
2. Abre el servicio y selecciona **Crear**.
3. Completa la configuracion principal:
   - **Nombre**: el nombre de la aplicacion
   - **Plan**: **Free**
   - **Origen**: **GitHub**
4. Inicia sesion con GitHub cuando Azure lo solicite.
5. Selecciona:
   - **Organizacion**: tu cuenta
   - **Repositorio**: `pokedex-angular-Juan`
   - **Rama**: `main`
6. Azure detecta automaticamente que el proyecto esta hecho con **Angular**.
7. Verifica la configuracion del build. La parte importante es:

```text
Output location: dist/pokedex-angular
```

8. Revisa toda la configuracion.
9. Haz clic en **Review + create**.
10. Si todo esta correcto, selecciona **Create**.

## Verificacion

Despues de crear el recurso, Azure genera y publica la aplicacion.

URL validada:

`https://witty-pond-0d148791e.7.azurestaticapps.net`

## Revision de seguridad

La URL fue revisada en **Security Headers** y la configuracion quedo correcta.

## Resultado

La aplicacion queda desplegada automaticamente desde GitHub cada vez que haya cambios en la rama `main`.
