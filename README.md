# Equa

Aplicación de citas que empiezan en una mesa, no en un chat.

Esto es la versión web, para poder enseñarla desde cualquier dispositivo sin
instalar nada: **https://srinsolente.github.io/equa/**

Desde el móvil se puede añadir a la pantalla de inicio y se abre como una
aplicación, sin barra de navegador.

## Qué es y qué no es

Es la aplicación de verdad compilada para navegador: las mismas pantallas,
las mismas reglas y el mismo recorrido que la versión de móvil. Los perfiles
y los eventos son de ejemplo, y todo lo que hagas se guarda únicamente en tu
propio navegador: no hay servidor detrás todavía.

Lo único que no existe aquí es la biometría, que es del teléfono.

## Cómo está hecho

`index.html` es un único archivo con todo dentro: el código de cada pantalla,
las tipografías y los iconos. No pide nada por red. Se genera desde el
proyecto con:

```
npx expo export --platform web --output-dir dist-web
node scripts/pagina-web.mjs
```

El código fuente vive aparte.
