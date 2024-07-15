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

* Fast-forward: Cuando no hay conflictos. Git soluciona automaticamente la fusion.

* Conflicto: Git no puede resolver por si solo la fusion por ende necesita la ayuda del desarrollor o los desarrolladores involucrados en el codigo que se esta fusionando.

* Algoritmo (fusion de 3 vias): Cuando git detecta cierto grado de modificacion, no utiliza el fast-forward. Utiliza diferentes tipos de algoritmos. Tambien soluciona por si mismo los posible inconvenientes en la fusion. Pero crea un nuevo commit intermedio, usando el ultimo commit de cada rama.


# Herramientas con GUI para la gestion de un repositorio de GIT ///

* GitHub Desktop: <https://github.com/apps/desktop>
* GitKraken: <https://www.gitkraken.com/>

# Stashes
Es una estructura de datos tipo pila.

## Crear un stash

```sh
git stash
```

## Listar todos los stashes

```sh 
git stash list
```

## Recuperar un stash 
No solo recupera el ultimo stash hecho y lo borra

```sh 
git stash pop
```

# Stash con nombre personalizado

```sh
git stash -m "mensaje personalizado"
```

# Aplicar un stash en particular

```sh
git stash apply <numero-de-stash>
git stash apply 1
```

## Borrar un stash 

```sh
git stash drop # Borra el ultimo stash
git stash drop 2 # Borra el stash elegido, en este caso el 2
```