# Les Anomalies
**A1 :**<br>
je constate qu'il y a un defilement droite gauche 
en regardant le code je vois que qu'il n'y a pas de @media(min-with: )
pour le tableau et pour l'image 

je pense que c'est a cause de la taille de l'image qui n'est pas gere en version mobile

Ajout de : <br>
@media (max-width: 375px) {<br>
.conteneur {<br>
width: auto;
}<br>
}

**A2 :**<br>
Je constate qu'effectivement l'image est ecrase 

Je suppose que c'est a cause de la taille de l'image 

Correction : <br>

.bandeau__photo {<br>
width: 100%;<br>
height: 100%; /*passage de 220px de valeur a 100% */<br>
border-radius: var(--rayon);
}

**A3 :** <br>
Effectivement je constate que l'on ne vois pas ou l'on se trouve avec le tab

Je suppose qu'on doit aujouter une notion css pour l'accessibilité

Correction : <br>

j'ai retirer ces ligne de css<br>

*:focus {<br>
outline: none;<br>
}

**A4 :** <br>

Quand on clique sur code postal il ne se passe rien alors que sur date souhaiter ca nous "redirige" sur le champ pour selectionner une date

Je pense qu'il faut ajoute une notion de css a la class qui doit etre la meme que pour date souhaitez

Correction : <br>

label for="code-postal"Code postal /label  !-- modification du for de cp a code postale--

**A5 :** <br>

je constate que c'est illisible quand la luminosité est baissé

je pense qu'il faut changer la couleur du text

Correction : <br>

.note { <br>
color: var(--gris); /*suppression de la var -text*/ <br>
}

**A6 :**<br>

Effectivement je constate que tout le texte est en italique 

je pense qu'il y a soit une balise em
 dans le html en trop soit un mauvaise gestion dans le css du style

Correction : <br>

dans le html il y avais une balise em en trop je l'ai don retirer