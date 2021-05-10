# TP Désobfuscation

> AURIOL Thomas

---
## Procédure
Repérer chaque ligne qui pourrait être changer par exemple :

- Pour transformer le nom d'une variable:
> Entrée :
> `sWQL = FLQZEsG("gq14V+IwdBHohEVdaK7yS...")`
>
> Sortie :
> `query = FLQZEsG("gq14V+IwdBHohEVdaK7yS...")`

- Pour transformer un string:
> On récupère la ligne que l'on veut modifier et on l'affiche avec de `Debug.Print`
>
> Entrée :
> `Debug.Print FLQZEsG("gq14V+IwdBHohEVdaK7ySOp3F0yC71Zdqra7UKDjUFxotvVUoqbfVaDy8Vb46X9V")`
>
> Sortie :
> `Select * From Win32_NetworkAdapterConfiguration`

On continue de faire ça pour la suite du code en continuant à remplacer chaque chaque ligne.

Après avoir terminé on peut supprimer les 4 fonctions après les différents Sub qui permettent de déobfusquer le texte.

---
## Que fait le code ?
Le code affiche les propriétés des éléments root de windows.

On peut trouver un Url qui permet de télécharger un document nous disant de faire une documentation : La voici.