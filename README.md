******Pour l'installation*****


1--- Commandes

Run: npm init
Run: npm install -D tailwindcss postcss-cli autoprefixer


2--- Créer dociers/fichier 

public =>index.html
scr =>tailwind.css


3-- Dans tailwind.css
ajouter

@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base{

}


@layer components {
 
}



3-- Build

Ajouter dans le package.json: script =>"build:dev": "postcss -w scr/tailwind.css -o public/style.css

Run: npm run build:dev


4--Extension
installer: tailwind CSS IntelliSence

5--Purge
Ajouter dans tailwind.config.js : purge => ./public/index.html
Run : $env: NODE_ENV="production"
Run : npm run build 