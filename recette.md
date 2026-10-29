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