# Part 0: Instal·lació i configuració de Git

## Què és Git?

Git és un sistema de control de versions distribuït. Això vol dir que ens permet portar un registre de tots els canvis que fem en els nostres projectes, així com treballar en equip de manera eficient. Git ens ajuda a gestionar el codi font i a col·laborar amb altres persones sense perdre la feina feta.

## Instal·lar Git

Per instal·lar Git, podeu seguir les instruccions de la [pàgina oficial de Git](https://git-scm.com/downloads). Un cop instal·lat, podeu comprovar que tot funciona correctament executant la comanda següent en el terminal:

```bash
git --version
```

Si tot ha anat bé, haureu de veure la versió de Git que teniu instal·lada.

## Configurar Git

Abans de començar a utilitzar Git, és important configurar el vostre nom d'usuari i correu electrònic. Això és necessari perquè Git pugui identificar qui ha fet cada canvi. Podeu fer-ho executant les següents comandes:

```bash
git config --global user.name "El vostre nom"
git config --global user.email "el vostre correu electrònic"
```

Això només cal fer-ho una vegada, i després Git recordarà la vostra configuració.
