# security-perf
Analyse du site d'autoécole "ornikar" avec rapport d'analyse

#### Site : https://www.ornikar.com

#### Performances : 61%
- Les images non affichées à l'écran ne devraient pas être chargées
- Retirer le css inutilisé de la page de style
- Charger les scripts js bloquant le chargement de l'app depuis un fichier physiquement présent et non un cdn
- Mettre en place une gestion du cache pour certaines ressources
- Le js met trop de temps à être évalué (rajouter service workers etc ...)

#### WebApp Progressive : 54%
 - Charger en offline en renvoyant un statut http 200
 - Annoncer à l'utilisateur qu'il peut ajouter l'application à l'écran d'accueil
 - Mettre en place les services workers
 - Ajouter un splash screen pendant le chargement de la webapp progressive
 - Ajouter une couleur de thème pour que les éléments chromes soient accordés au niveau de la couleur de l'app
 - La taille de l'écran de l'application n'est pas optimisé pour un usage sur mobile/tablette
 
 #### Accessibilité : 42%
 - Ajouter des attributs "alt" et des "names" compréhensibles sur les inputs
 - Il faut ajouter du contraste entre le premier plan et la couleur de background-color
 
 #### Bonnes pratiques : 93%
 - Inclure les documents via document.write() en js pour optimiser de dizaine de seconde le chargement de la page pour les utilisateurs ayant une faible connexion
 
 #### SEO : 100%
 - Rien a modifier pour l'instant
