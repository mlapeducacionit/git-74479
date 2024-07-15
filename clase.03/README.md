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

# Para obtener ayuda 

```sh 
git merge --help
```

# Tipos de fusiones y su resolucion

* Fast-forward: Cuando no hay conflictos. Git soluciona automaticamente la fusion.

* Conflicto: Git no puede resolver por si solo la fusion por ende necesita la ayuda del desarrollor o los desarrolladores involucrados en el codigo que se esta fusionando.

* Algoritmo (fusion de 3 vias): Cuando git detecta cierto grado de modificacion, no utiliza el fast-forward. Utiliza diferentes tipos de algoritmos. Tambien soluciona por si mismo los posible inconvenientes en la fusion. Pero crea un nuevo commit intermedio, usando el ultimo commit de cada rama.