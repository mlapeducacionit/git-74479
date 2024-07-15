# Clase 03 - Git Desarrollo Colaborativo

## Repasando las fusiones en GIT
Estando en al rama que me quiero traer los cambios. Por ejemplo si me quiero traer la rama repaso-branches a main. Tengo que estar parado en la rama main y luego ejecutar el comando siguiente...

```sh
git merge <nombre-rama-que-me-quiero-traer>
git merge repaso-branches
```

## Comparando ramas con git diff (tambien puedo ver la diferencia entre ramas)

```sh
git diff <nombre-rama>
git diff main
```

# Tipos de fusiones y su resolucion

* Fast-forward: Cuando no hay conflictos. Git soluciona automaticamente la fusion
* Conflicto: Git no puede resolver por si solo la fusion por ende necesita la ayuda del desarrollor o los desarrolladores involucrados en el codigo que se esta fusionando.