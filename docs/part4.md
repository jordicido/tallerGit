# Part 4: Col·laboració amb GitHub

## Col·laborar amb repositoris dels altres

No sempre serem propietaris d'un repositori del que volem participar. Github, en estos casos, ens proporciona eines per a poder col·laborar amb repositoris d'altres persones. En este apartat veurem com fer-ho.

## Fork

Un fork és una còpia d'un repositori que es crea a la nostra compte de GitHub. Això ens permet fer canvis al repositori sense afectar el repositori original. Per crear un fork, només hem de fer clic al botó "Fork" a la part superior dreta del repositori que volem copiar. Això crearà una còpia del repositori al nostre compte de GitHub.

Anem a posar per cas que voleu col·laborar amb este repositori, però que trobeu una errata o un error. En este cas, el primer que haureu de fer és crear un fork del repositori.

[Link al repositori d'este projecte](https://github.com/jordicido/tallerGit)

Accediu al repositori i feu clic al botó "Fork" a la part superior dreta. Això crearà una còpia del repositori al vostre compte de GitHub.

No canvies el nom del repositori, simplement forkeja'l en el teu compte de Github.

## Clonar un repositori de GitHub

Abans hem vist com vincular un repositori remot a un repositori local. Ara veurem com clonar un repositori remot. Clonar un repositori remot és similar a crear un fork, però en lloc de crear una còpia del repositori al nostre compte de GitHub, creem una còpia del repositori al nostre ordinador.

En realitat, el que està passant quan clonem un repositori és que estem creant una còpia del repositori remot al nostre ordinador. Això ens permet treballar amb el repositori localment i fer canvis sense afectar el repositori remot. Tingueu en compte que no només es copien els fitxers, sinó que també es copia tota la història de commits. Això vol dir que podem veure tots els canvis que s'han fet al repositori i qui els ha fet. Això és molt útil per a la col·laboració en equip i per a la gestió de projectes de codi obert.

Per clonar un repositori remot, utilitzarem la comanda `git clone`. Aquesta comanda ens permet crear una còpia del repositori remot al nostre ordinador. La sintaxi és la següent:

```bash
git clone <url_remot>
```

Quan clonem un repositori remot ja tindrem el repositori vinculat al remot, així que no caldrà fer `git remote add origin <url_remot>`. A continuació cloneu el repositori que heu forkejat al vostre compte de GitHub. Per fer-ho, aneu a la pàgina del repositori i feu clic al botó "Code" i copieu l'URL que apareix. Després, obriu una terminal i escriviu la comanda `git clone` seguida de l'URL que heu copiat.

## Suggerir canvis a un repositori remot

Ara que ja teniu el repositori clonat al vostre ordinador, podeu fer canvis i suggerir-los al repositori original. Per fer-ho, heu de crear una branca nova, fer els canvis i després fer un "pull request" al repositori original.
Un "pull request" és una sol·licitud per a que els propietaris del repositori original revisen els vostres canvis i els fusionen amb el seu repositori. Això és útil perquè permet als propietaris del repositori revisar els canvis abans d'acceptar-los i fusionar-los amb el seu repositori.

Per crear un "pull request", primer heu de fer els canvis al vostre repositori local. Després, heu de fer un commit dels canvis i pujar-los al vostre repositori remot. Finalment, heu de crear un "pull request" al repositori original.

Per fer un "pull request", aneu a la pàgina del repositori original i feu clic al botó "Pull requests". Després, feu clic al botó "New pull request". Això us portarà a una pàgina on podreu seleccionar la branca que heu creat i els canvis que heu fet. Després, feu clic al botó "Create pull request" per enviar la vostra sol·licitud.

És important que el missatge del "pull request" sigui clar i concís, i que expliqueu els canvis que heu fet i per què els heu fet. Això ajudarà als propietaris del repositori a entendre els vostres canvis i a revisar-los més ràpidament.

## Sincronització amb el repositori original

Si el repositori original ha canviat des que vau fer el vostre fork, és possible que vulgueu sincronitzar el vostre fork amb el repositori original. Això us permetrà tenir la versió més actualitzada del repositori original al vostre fork.

Per fer-ho, heu de seguir els següents passos:

1. Afegir el repositori original com a remot al vostre fork. Per fer-ho, utilitzeu la comanda `git remote add upstream <url_repositori_original>`. Això afegirà el repositori original com a remot anomenat "upstream".
2. Obtenir els canvis del repositori original. Per fer-ho, utilitzeu la comanda `git fetch upstream`. Això descarregarà els canvis del repositori original al vostre ordinador.
3. Fusionar els canvis del repositori original amb el vostre fork. Per fer-ho, utilitzeu la comanda `git merge upstream/main`. Això fusionarà els canvis del repositori original amb la vostra branca actual.
4. Pujar els canvis al vostre fork. Per fer-ho, utilitzeu la comanda `git push origin <nom_branque>`. Això pujarà els canvis al vostre fork a GitHub.
5. Ara ja podeu fer un "pull request" al repositori original amb els canvis que heu fet.
