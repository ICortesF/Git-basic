# Git-basic

> Comándos básicos para el trabajo con Git 

## Creamos un repositorio vacío

echo "# Git-basic" >> README.md  
Muestra texto en pantalla

git init  
Inicializa git en la carpeta

git add README.md  
Añadimos el fichero 

git add .  
Añade todo

git commit -m "first commit"  
Agregamos los cambios al repositorio local

git remote add origin https://github.com/ICortesF/Git-basic.git  
conecatamos con el origen remoto

git push -u origin master  
Subimos los cambios al repositorio remoto

## Clonamos un repositorio existente
git clone git://github.com/schacon/grit.git  

## Trabajo con ramas

git checkout -b feature_x  
creamos una nueva rama feature_x

git checkout master  
vuelve a la rama principal


git branch -d feature_x  
y borra la rama

### Una rama nueva no estará disponible para los demás a menos que subas (push) la rama a tu repositorio remoto
git push origin <branch>  
