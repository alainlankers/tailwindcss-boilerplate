# Tailwind CSS boilerplate  
## Steps to setup
Create your project folder
```
npm init -y
npm install tailwindcss postcss postcss-cli autoprefixer
npx tailwindcss init -p
```
Create **tailwind.css** file in project root.  
Create **/dist** folder and add **/css** folder  
Go to dist/css and add file **styles.css**  
Go to dist/ and add file **index.html**  

Add to tailwind.css:  
```css
@tailwind base; 
@tailwind components; 
@tailwind utilities;
```
Add to index.html:  
```html
<link rel="stylesheet" href="css/styles.css">
```
Add to package.json:
```json
"scripts": {
"build": "​postcss​ tailwind.css -o dist/css/styles.css", 
"watch": "postcss tailwind.css -o dist/css/styles.css --watch"
},
```
```
npm run watch
npm run build
```