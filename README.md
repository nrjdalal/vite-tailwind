- Create a folder and open terminal in it.
- Type the follwing command in the terminal of that folder -

```
npm init vite .
```

- Enter any package name e.g. vite-tailwind, select framework and variant as "vanilla".
- Run the following commands -

```
npm install -D tailwindcss postcss autoprefixer prettier prettier-plugin-tailwindcss
```

```
npx tailwindcss init -p
```

- Edit the following file 'style.css' and replace all existing code with -

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

- Edit the following file 'tailwind.config.js' and replace all existing code with -

```js
module.exports = {
  content: ['./**/*.html'],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

- Edit the following file 'index.html' and replace all existing code with -

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <link rel="icon" type="image/svg+xml" href="favicon.svg" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Vite-Tailwind</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="mt-4 text-center">
      Here is
      <a class="underline" href="https://tailwindcss.com/docs/text-align">tailwindcss docs</a>
      for you.
    </div>
  </body>
</html>
```

- Now run the project via -

```
npm run dev
```
