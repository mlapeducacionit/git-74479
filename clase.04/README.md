# Clase 04 - Git Desarrollo Colaborativo

# Git Pages
Me permite alojar un sitio. Sitios Estaticos. JavaScript, html, css. React, Vue, Angular. Hosting gratuito.

Tengo que crear un repositorio especial. 

<nombre-cuenta-github>.github.io

Y si ya tengo ocupado. Puedo a partir de cualquier repositorio hacer un GitPages.

Settings > Pages

![Github](_ref/gitpages.png)

## PDF con comandos (Machete)

<https://training.github.com/downloads/github-git-cheat-sheet.pdf>
<https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet>

## Cherry Pick
Permite seleccionar un commit  o varios de manera independiente y colocarlos en otra rama.

### Selecioando un unico commit

```sh
git cherry-pick <hash>
```

### Seleciono varios commit con extremos

```sh
git cherry-pick <hash>^..<hash>
```

### Seleciono varios commit sin extremos

```sh
git cherry-pick <hash>..<hash>
```

