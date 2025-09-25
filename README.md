
# sem4
mkdir MiPortafolio
cd MiPortafolio
git init
touch index.html style.css
git add .
git commit -m "Estructura inicial del portafolio"
echo "<h1>Bienvenido a mi portafolio</h1>" >> index.html
git add index.html
git commit -m "Agregado título principal"
git checkout -b diseño
echo "body { background-color: #f0f0f0; }" >> style.css
git add style.css
git commit -m "Estilos básicos agregados"
git checkout master
git merge diseño
git remote add origin https://github.com/usuario/MiPortafolio.git
git push -u origin master

