# Clase 02 - Git desarrollo colaborativo

## Archivo .gitignore
Existe un archivo que nos permite ignorar ciertos archivos que queremos que no sean parte de los commits. Se crea generalmente en el carpeta raiz del proyecto.

```sh
touch .gitignore
```

## Archivo .gitkeep
Existe un archivo que nos permite agregar a los commit, las carpetas vacias que git por defecto ignora.

```sh
touch .gitkeep
```

# Subir nuestro repositorio a la nube
No logueamos en GitHub y creamos un repositorio de GitHub. Dejo todo por defecto y si quiero cambio la visibilidad, publico todos pueden acceder y solo yo modifico. Privado. Nadie puede ver a menos que lo agregue al repositorio para que lo vea.

## Agregar la url del repositorio remoto al repo local

```sh
git remote add <alias> <url>
git remote add origin https://github.com/mlapeducacionit/git-74479.git
```

## Confirmar si tengo un remoto en el repositorio local

```sh
git remote
git remote -v # mas detalle -v:verbose
```

## Subir la copia completa o parcial de commits del local al remoto

```sh
git push -u <repositorio-remoto> <rama/branch>
git push -u origin main # -u -> sincronizar la rama local con la remota. Solo la primera vez se agrega el flag/bandera -u
```




# RAMAS (Branches)

