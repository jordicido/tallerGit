# Part 5: Desfer canvis

## Context

A voltes, als projectes, ens adonem que hem comès un error i volem desfer els canvis que hem fet. En este apartat veurem com fer-ho.

## Desfer canvis en fitxers

Si heu modificat un fitxer i voleu desfer els canvis, podeu utilitzar la comanda `git checkout`. Aquesta comanda us permetrà desfer els canvis en un fitxer concret i tornar a la versió anterior. La sintaxi és la següent:

```bash
git checkout <nom_fitxer>
```

Això desferà els canvis en el fitxer especificat i tornarà a la versió que tenia l'arxiu en l'últim commit.

## Desfer un commit

Si heu fet un commit i voleu desfer-lo, podeu utilitzar la comanda `git reset`. Aquesta comanda us permetrà desfer un commit i tornar a l'estat anterior. La sintaxi és la següent:

```bash
git reset <hash_commit>
```

Hi ha dues opcions del reset, `--soft` i `--hard`. La diferència és que `--soft` manté els canvis en l'índex, mentre que `--hard` els elimina completament. Si voleu desfer un commit i mantenir els canvis, utilitzeu `--soft`. Si voleu desfer un commit i eliminar els canvis, utilitzeu `--hard`.

Tingueu en compte que `git reset` és una comanda perillosa, ja que pot eliminar canvis que no es poden recuperar. Assegureu-vos de fer una còpia de seguretat dels fitxers abans d'utilitzar-la.

## Desfer un canvi sense desfer l'historial de commits

Si voleu desfer un canvi en un fitxer sense desfer l'historial de commits, podeu utilitzar la comanda `git revert`. Aquesta comanda crea un nou commit que desfà els canvis del commit especificat. La sintaxi és la següent:

```bash
git revert <hash_commit>
```

El que fa `git revert` és crear un nou commit que desfà els canvis del commit especificat. Això és útil si voleu desfer un canvi sense eliminar l'historial de commits. A més, `git revert` és una comanda segura, ja que no elimina cap canvi i manté l'historial de commits intacte.
