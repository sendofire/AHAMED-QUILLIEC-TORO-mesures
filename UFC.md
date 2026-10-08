# Exercice 8

**Réponse $UFC$ de la leçon**

$$
    \begin{align}
    UFC &= \sum_{i=1}^{5}\sum_{j=1}^{3} w_{ij} \times x_{ij}\\ 
    &= 12 \times 2 + 6 + 10 + 7 + 21 \times 2 + 35 + 20 \\
    UFC &= 144
    \end{align}
$$

### Comment établir les valeurs de poids, qui rendent comptent des importances relatives ?
Pour établir les poids il faut identifier des indicateurs objectifs et quantifiables (champs traités, données accédées), ensuite calquer leur pondération sur l'effort moyen historique mesuré sur des projets similaires, puis formaliser cette relation dans un tableau.

### Pour évaluer la complexité d'un projet client, on s'appuie sur ces éléments :
- Les standards et abaques historiques
- Historique de l'équipe
- Le découpage fonctionnel
- L'estimation collective

### En admettant qu’on sache prédire, en gros, combien de modules de haut niveau seront nécessaires, comment évaluer leurs importances relatives ?

- Le périmètre fonctionnel
- La compléxité algorithmique et technique
- Le niveau de risque et d'inconnu
- La valeur métier

### Et commment rendre compte de ces importances relatives à travers un système de poids ?

On établit ce système en choisissant un module de référence comme étalon (poids 1), puis en attribuant aux autres un coefficient multiplicateur selon leur taille, leur difficulté technique et leur niveau de risque.

### Par exemple, dans le développement d’un site web marchand, si on compte en écrans, tous se valent-ils en complexité ?

Non, tous les écrans ne se valent pas, car l'effort dépend de ce qui se passe en coulisses (la logique métier, les données et la sécurité).

###  Un écran d’alerte “saisie incorrecte” demande-t-il autant de travail à développer qu’un formulaire de saisie ?

Non, un modale "saisi incorrecte" demandera moins de travaille qu'un formulaire, car le modale c'est juste un affichage avec un boutton pour fermer. Et un formulaire va demandé une organisation pour récupérer chaque information et la traiter.

### Comment établir des intuitions de difficultés relatives ?

- Les volumes de données
- La logiques technique
- Les contraintes nonn fonctionnelle (niveau de sécurité, tolérence aux panne, ...)
- L'historique et l'expertise

### Comment chiffrer ces difficultés relatives à travers l’établissement de valeurs de pondération ?

- Fixer un étalon (poids 1) : on choisit l'élément le plus simple, le mieux maîtrisé et sans risque du projet (par exemple : un modale).
- Classer par palier relatif: on compare les autres composant avec cette étalon.
- Appliquer la pondération : en multipliant le nombre d'éléments de chaque catégorie par leur poids respectif, on obtient une charge globale représentative de la réalité technique, prête à être convertie en temps ou en budget.