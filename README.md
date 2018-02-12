# Git-basic

> Comándos básicos para el trabajo con Git 

## Creamos un repositorio vacío

echo "# Git-basic" >> README.md  
*Muestra texto en pantalla*

git init  
*Inicializa git en la carpeta*

git add README.md  
*Añadimos el fichero* 

git add .  
*Añade todo*

git commit -m "first commit"  
*Agregamos los cambios al repositorio local*

git remote add origin https://github.com/ICortesF/Git-basic.git  
*Conecatamos con el origen remoto*

git push -u origin master  
*Subimos los cambios al repositorio remoto*

## Clonamos un repositorio existente
git clone git://github.com/schacon/grit.git  

## Trabajo con ramas

git checkout -b feature_x  
*creamos una nueva rama feature_x*

git checkout master  
*vuelve a la rama principal*


git branch -d feature_x  
*y borra la rama*

git branch  
*nos nuestra las ramas*

### Una rama nueva no estará disponible para los demás a menos que subas (push) la rama a tu repositorio remoto
git push origin \<branch>  

## Juntar cambios

git pull  
*actualizar tu repositorio local al commit más nuevo*  

git merge \<branch>  
*fusionar otra rama a tu rama activa*  

### Si se producen conflictos.  

*Tú eres responsable de fusionar esos conflictos manualmente al editar los archivos mostrados por git. Después de modificarlos, necesitas marcarlos como fusionados con*  
git add \<filename>  

*Antes de fusionar los cambios, puedes revisarlos usando*  
git diff <source_branch> <target_branch>  

## Etiquetas

git tag 1.0.0 1b2e1d63ff  
*crear una nueva etiqueta llamada 1.0.0 ejecutando*  

git log  
*pbtener el commit id*  


## Datos útiles  

*Interfaz gráfica por defecto*  
gitk  

*Colores especiales para la consola*  
git config color.ui true  

*Mostrar sólo una línea por cada commit en la traza*  
git config format.pretty oneline  

*Agregar archivos de forma interactiva*  
git add -i  
