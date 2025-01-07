
# Tailwind Starter

A quick guide to setting up a Tailwind CSS project.

---

### Source
Documentation: [Tailwind CSS Installation](https://tailwindcss.com/docs/installation)

---

### Useful Steps

1. Initialize your project:
```bash
 npm init -D
```


2. Install Tailwind CSS as a development dependency:
```bash
npm i -D tailwindcss

```

   




   

3. Generate a tailwind.config.js file:
```bash
npx tailwindcss init

```


4. Create an input.css file and add the following base directives:

```bash
@tailwind base;
@tailwind components;
@tailwind utilities;

```


Configure package.json
Add the following scripts to your package.json file for building and watching Tailwind CSS:
```bash

{
  "name": "tailwind-starter",
  "version": "1.0.0",
  "main": "index.js",
  "scripts": {
    "build": "tailwindcss -i ./input.css -o ./css/style.css",
    "watch": "tailwindcss -i ./input.css -o ./css/style.css --watch"
  },
  "author": "",
  "license": "ISC",
  "description": "",
  "devDependencies": {
    "tailwindcss": "^3.4.17"
  }
}
```


Build Your CSS
After setting up, you can build your CSS with the following command:

```bash
npm run build
```

This will create a css folder containing style.css, which you can reference in your HTML files.

Watching for Changes
To continuously build your CSS while working on your project, use the watch command:
```watch
npm run watch
```
