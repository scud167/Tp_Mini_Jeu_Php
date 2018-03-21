# Tp_Mini_Jeu_Php
## Juste pour l'entrainement (OpenClassRooms)

### Amelioration a faire
    
#### Un système de niveau. Vous pourriez très bien assigner à chaque personnage un niveau de 1 à 100. Le personnage bénéficierait aussi d'une expérience allant de 0 à 100. Lorsque l'expérience atteint 100, le personnage passe au niveau suivant.

- le niveau et l'expérience deviendraient des caractéristiques du personnage, donc... Pas besoin de vous le dire, je suis sûr que vous savez ce que ça signifie !

#### Un système de force. La force du personnage pourrait augmenter en fonction de son niveau, et les dégâts infligés à la victime seront donc plus importants.

- de même, la force du personnage serait aussi une caractéristique du personnage.

#### Un système de limitation. En effet, un personnage peut en frapper autant qu'il veut dans un laps de temps indéfini. Pourquoi ne pas le limiter à 3 coups par jour ?

- il faudrait que vous stockiez le nombre de coups portés par le personnage, ainsi que la date du dernier coup porté. Cela ferait donc deux nouveaux champs en BDD, donc deux nouvelles caractéristiques pour le personnage !

#### Un système de retrait de dégâts. Chaque jour, si l'utilisateur se connecte, il pourrait voir ses dégâts se soustraire de 10 par exemple.

- il faudrait stocker la date de dernière connexion. À chaque connexion, vous regarderiez cette date. Si elle est inférieure à 24h, alors vous ne feriez rien. Sinon, vous retireriez 10 de dégâts au personnage puis mettriez à jour cette date de dernière connexion.
