# Major-Project-using-Tailwind
```
npm init
```
then press `Enter` until process ends which leads to creation of `package.json`
[Tailwind Docs](https://tailwindcss.com/docs/installation)
```
npm install -D tailwindcss
```
inside `tailwindcss.config.js` in content add below one:-
```
content: ["./dist/index.html"],
```
then create `src folder` and create file with desired name here i used `style.css` and add this in it:-
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
then run this command:-
```
npx tailwindcss -i ./src/style.css -o ./dist/output.css --watch
```
and inside the `package.json` add this line in `scripts` below `test`:-
```
"dev": "tailwindcss -i ./src/style.css -o ./dist/output.css --watch"
```
just connect the `output.css` with html:-
```
<link rel="stylesheet" href="./output.css">
```
and continue with your app.
