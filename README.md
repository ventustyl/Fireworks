# Projet Fireworks ![enter image description here](https://a57.foxnews.com/static.foxbusiness.com/foxbusiness.com/content/uploads/2021/06/0/0/Fireworks-iStock.jpg?ve=1&tl=1)

Ce projet est une animation de feux d'artifice réalisée en utilisant HTML et JavaScript pour le rendu graphique sur un navigateur web. Les feux d'artifice sont générés dynamiquement sur un canvas HTML5. 

## Pupitre d'artificier

Une seconde page, `pupitre-artificier.html`, autonome et sans dependance : une table de tir
pyrotechnique pilotable en direct.

- **Huit pieces** avec leur physique propre : pivoine, chrysantheme, saule, palmier, anneau,
  stroboscope, marron d'air et comete.
- **Console de balistique** : calibre (40 a 220 mm), gravite, vent, hauteur d'eclatement,
  densite d'etoiles, persistance des trainees, scintillement et cadence de tir. La vitesse
  initiale est calculee pour eclater exactement a la hauteur demandee (`v = sqrt(2gh)`).
- **Six palettes** : tricolore, or, aurore, braise, glacier, carnaval.
- **Decor** : reflet sur plan d'eau, halo de ville, fumee residuelle qui derive avec le vent.
- **Son** en Web Audio natif : detonation (bruit blanc filtre passe-bas), sifflement de montee,
  crepitement des chrysanthemes. Coupe par defaut.

### Pilotage

| Touche | Effet |
|---|---|
| Clic | Tir sur le point vise |
| `1` a `8` | Choix de la piece |
| `Espace` | Mise a feu |
| `B` | Bouquet final |
| `A` | Tir automatique |
| `S` | Son |
| `C` | Effacer le ciel |

Rendu en Canvas 2D, sans librairie. Reserve de particules recyclees, plafond a 9 000 etoiles,
frottement mis en cache par image pour tenir 60 images/s pendant un bouquet final.

L'animation d'origine (figure de Lissajous) reste dans `index.html` et est decrite ci-dessous.

## Comment ça marche 
Le fichier HTML (`index.html`) crée un canvas et charge les scripts CSS (`style.css`) et JavaScript (`script.js`) nécessaires pour l'animation. Le script JavaScript (`script.js`) est responsable de la génération des feux d'artifice. Il utilise la bibliothèque Canvas HTML5 pour dessiner les explosions de feux d'artifice à l'écran. 

## Utilisation
  1. Clonez ce référentiel sur votre ordinateur. 
  2.  Ouvrez le fichier `index.html` dans un navigateur web (assurez-vous d'avoir une connexion Internet active pour charger les scripts). 
  3.  Vous devriez voir une animation de feux d'artifice s'afficher à l'écran.

 ## Personnalisation 
Si vous souhaitez personnaliser cette animation de feux d'artifice, vous pouvez modifier les paramètres et les styles dans le fichier `script.js` et `style.css` selon vos besoins.

 ## Auteur
 Ce projet a été créé par Eric Venturino et est disponible sous licence MIT . Amusez-vous bien avec cette animation de feux d'artifice ! 
