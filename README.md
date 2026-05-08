# Pokedex Angular

Aplicacion web tipo Pokedex desarrollada con Angular. Permite explorar Pokemon, ver su informacion detallada y filtrar resultados por version, nombre y tipo.

## Que hace el proyecto

- Muestra un listado de Pokemon en formato visual tipo Pokedex.
- Permite buscar por nombre.
- Permite filtrar por tipo.
- Permite cambiar la version de la Pokedex.
- Muestra una vista de detalle para cada Pokemon con:
  - numero
  - nombre
  - tipos
  - altura
  - peso
  - estadisticas
  - descripcion por versiones

## Como esta hecho

El proyecto fue construido con **Angular 14** y sigue una estructura modular. La aplicacion usa:

- **Angular Router** para la navegacion entre vistas.
- **Apollo Angular + GraphQL** para consultar datos de PokeAPI GraphQL.
- **PokeAPI** como fuente de datos.
- **SCSS** para estilos.
- **Lazy loading** en las vistas principales para mejorar la carga.

## Estructura general

- `src/app/core`: configuracion base, servicios, guardas e integracion GraphQL.
- `src/app/shared`: componentes reutilizables, pipes, directivas, layout y animaciones.
- `src/app/views`: vistas principales como inicio, detalle, about, error y 404.
- `src/environments`: variables de entorno y endpoints.

## Tecnologias principales

- Angular
- TypeScript
- Apollo Angular
- GraphQL
- SCSS
- Jasmine y Karma
- ESLint

## Ejecucion local

1. Instala las dependencias:

```bash
npm install
```

2. Inicia el proyecto:

```bash
npm start
```

3. Abre el navegador en:

```text
http://localhost:4200
```

## Scripts disponibles

- `npm start`: inicia la aplicacion en desarrollo.
- `npm run build`: genera la compilacion de produccion.
- `npm run watch`: compila en modo desarrollo observando cambios.
- `npm test`: ejecuta pruebas con cobertura.
- `npm run test:cov`: ejecuta pruebas en modo headless.
- `npm run lint`: ejecuta el analisis estatico.

## Fuente de datos

La aplicacion consume informacion de:

- REST API: `https://pokeapi.co/api/v2`
- GraphQL API: `https://beta.pokeapi.co/graphql/v1beta`

## Despliegue

El proyecto fue desplegado en **Azure Static Web Apps**.

URL publicada:

`https://witty-pond-0d148791e.7.azurestaticapps.net`

La configuracion de seguridad fue revisada con **Security Headers** y quedo correcta.
