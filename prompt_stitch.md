# Prompt pour Google Stitch — Historionomie Viewer

## Contexte

Je travaille sur un projet de recherche en histoire comparée appelé "historionomie" (cadre de Philippe Fabry). Le principe : toute nation traverse une succession de phases obligées dans sa construction nationale. Chaque phase a des sous-phases et des "saillants" (événements ponctuels identifiables). J'ai déjà analysé 5 nations et je veux un outil de visualisation interactif.

## Les données

### Les phases (dans l'ordre, couleur associée)
1. **Phase féodale** (#8B7355, marron) — ~200 ans. Réseaux de vassalité, pouvoir personnel fragile.
2. **Phase oligarchique** (#2E86C1, bleu) — ~200 ans. Émergence de l'État central, conflit entre élites.
3. **Phase absolutiste** (#7D3C98, violet) — ~200 ans. L'administration centrale domine tout.
4. **Révolution Nationale** (#C0392B, rouge) — ~25-80 ans. Renversement de l'ordre absolutiste.
5. **Phase parlementaire** (#27AE60, vert) — Très longue. Démocratie parlementaire.

### Les sous-phases de chaque phase
- Féodale : Percolation → Coagulation des élites → Bascule oligarchique
- Oligarchique : Essor oligarchique → Polarisation des élites → Guerre sociale
- Absolutiste : Absolutisation → Impérialisme absolutiste → Ancien Régime
- RN : Révolution initiale (explosion → expérience parlementaire → phase aiguë → moment thermidorien) → Impérialiste Revanchard → Restauration → Glorieuse Révolution

### Les saillants (événements marqueurs)
Chaque saillant a : un titre, une date (année), une figure associée (personne ou événement), un résumé, une description longue, un niveau de confiance (high/medium/low).

Saillants de la phase féodale :
- Éveil féodal (icône soleil) — premier chef supra-régional effectif
- Pic féodal (icône montagne) — roi fort, pouvoir personnel au sommet
- Crise féodale (icône éclair, ROUGE si avortement) — effondrement post-pic
- Pacte oligarchique (icône marteau de juge) — les oligarques codifient les règles

Saillants de la phase oligarchique :
- 1er monarque oligarchique (icône étoiles) — premier souverain avec État central
- Pic oligarchique (icône montagne) — pic de puissance/prestige oligarchique
- Fin de l'expansion (icône blocage) — fin de l'expansion extérieure
- Guerre sociale (icône feu) — conflit factieux résolu par un "tiers"

Saillants de la phase absolutiste :
- 1er monarque absolu (icône couronne) — figure qui résout la guerre sociale
- DGRO (icône flamme) — dernière révolte oligarchique
- Pic absolutiste (icône montagne) — sommet de puissance absolutiste
- Fin de l'expansion absolutiste (icône blocage)
- Remontrance (icône orateur) — tentative institutionnelle échouée, ouvre l'AR
- Ancien Régime — sédimentation, sclérose

Saillants de la RN :
- Explosion de l'AR (icône flash) — basculement des élites
- Expérience parlementaire (icône parlement) — on essaie la démocratie
- Phase aiguë (icône crâne) — les radicaux prennent le pouvoir
- Moment thermidorien (icône balance) — le centre reprend la main
- Impérialiste Revanchard (icône militaire) — figure autoritaire
- Glorieuse Révolution (icône étoile) — parlementarisme ancré

Saillants spéciaux :
- Choc d'hétérogénéité (icône groupe, ROUGE) — expansion qui hétérogénéise la société
- Écrasement (ROUGE) — RN écrasée par force extérieure

### Les 5 nations analysées

**Israël antique** (~-1080 à 135) — Deux parcours (antique + prolongement post-exil). RN avortée en 66-70 (écrasée par Rome). Nombreux reboots (conquête babylonienne, destruction du Temple).

**France** (~1108 à 1830) — Parcours complet de référence. Phase féodale : Louis VI → Philippe le Bel → Loi salique (1317). Phase oligarchique : Philippe VI → François Ier → Guerres de Religion. Phase absolutiste : Henri IV → Louis XIV → Polysynodie (1715) → Ancien Régime. RN : 1789 → Terreur → Bonaparte → 1830.

**Angleterre** (~829 à 1688) — Phase féodale avortée (5 boucles, 500 ans) puis reboot normand (1066). Phase oligarchique : Édouard III → Guerre des Deux-Roses. Phase absolutiste : Henri VII → Élisabeth → Stuarts. RN : Guerre civile (1642) → Cromwell → 1688.

**Venise** (~726 à 1866) — Phase oligarchique la plus longue (637 ans, expansion retarde polarisation). Phase absolutiste institutionnelle (Inquisiteurs d'État, pas un monarque). RN avortée (1848, écrasée par Autriche). Absorbée dans Parcours italien.

**Bavière** (~1180 à 1919) — Phase féodale longue (326 ans, partitions). Phase oligarchique courte (91 ans, accélérée par Contre-Réforme). Phase absolutiste avec deux cycles d'impérialisme (le prolongement napoléonien de 1806 avorte le 1er AR et relance un 2e cycle). RN avortée (1918-1919, absorbée dans RN allemande).

### Tableau comparatif complet des saillants

| Saillant | Israël antique | France | Angleterre | Venise | Bavière |
|---|---|---|---|---|---|
| Éveil féodal | Saül (~-1080) | Louis VI (~1108) | Guillaume (1066) | Orso Ipato (~726) | Louis Ier (~1204) |
| Pic féodal | Salomon (~-960) | Philippe le Bel (~1295) | Édouard Ier (~1295) | Orseolo (~991) | Louis IV (~1328) |
| Pacte oligarchique | — | Loi salique (1317) | Ordonnances (1311) | Abolition co-régence (1032) | Primogéniture (1506) |
| 1er monarque oligarchique | Omri (-885) | Philippe VI (1328) | Édouard III (1327) | Contarini (~1043) | Guillaume IV (~1508) |
| Pic oligarchique | Jéroboam II (~-770) | François Ier (~1515) | Édouard III (~1350) | Foscari (~1440) | Albert V (~1555) |
| Guerre sociale | -700 à -641 | Guerres de Religion (~1562-98) | Guerre des Deux-Roses (~1455-85) | Tensions inst. (~1628-69) | ~1564-1597 |
| 1er monarque absolu | Josias (-640) | Henri IV (1598) | Henri VII (1485) | Inquisiteurs d'État (~1669) | Maximilien Ier (1597) |
| Pic absolutiste | — (interrompu) | Louis XIV (~1682) | Élisabeth Ière (~1580) | Morosini (~1688) | Max. III Joseph (~1756) |
| Remontrance | — | Polysynodie (1715) | Apology of Commons (1604) | Correzione (1761) | Landtag (1848) |
| Ancien Régime | — | ~1715-1789 | ~1603-1642 | ~1718-1848 | ~1848-1918 |
| Explosion de l'AR | — | 1789 | 1642 | 1848 | 1918 |
| Exp. parlementaire | — | Assemblée nat. (1789-91) | Long Parliament (1640-48) | Rép. de Manin (1848-49) | État libre (1918-19) |
| Phase aiguë | — | Terreur (1792-94) | Exéc. Charles Ier (1649) | Pouvoirs illimités (1849) | Rép. des Conseils (1919) |
| IR | — | Bonaparte (1799) | Cromwell (1653) | — (avortée) | — (absorbée) |
| Glorieuse Révolution | — | 1830 | 1688 | — (absorbée 1866) | — (absorbée 1919) |

## L'interface souhaitée

### Page d'accueil
- Titre "Historionomie — Parcours de construction nationale"
- Grille de cartes cliquables pour chaque nation (nom, dates, statut)
- Bouton "Comparer" qui ouvre le mode comparaison

### Vue individuelle (frise d'une nation)
- Frise chronologique horizontale interactive
- Bandes colorées pour les phases (pleine hauteur)
- Bandes plus fines pour les sous-phases (sous les phases)
- Losanges/diamants pour les saillants, positionnés sur la frise avec des labels
  - Couleur du losange = couleur de la phase
  - Rouge pour les avortements/écrasements
  - Icône dans le losange
- Zone de perturbations (hachures diagonales rouges semi-transparentes)
- Tooltip au survol de chaque élément (titre + résumé)
- Panneau de détail à droite ou en bas au clic (description complète, confiance, alternatives)
- Zoom/pan sur la frise (molette, drag)

### Mode comparaison (feature principale)
- Sélection de 2 à 5 nations via des checkboxes
- Frises parallèles empilées verticalement, une par nation
- **Alignement au choix** :
  - Par date absolue (toutes les frises sur le même axe chronologique)
  - Par saillant (aligner les "1er monarque absolu" de toutes les nations, les "pic absolutiste", etc.) — pour voir les parallèles structurels indépendamment de la chronologie
- Lignes de connexion en pointillé entre les saillants équivalents des différentes nations
- Highlight : quand on survole un saillant sur une frise, le saillant équivalent s'illumine sur les autres frises

### Page de référence / wiki
- Présentation hiérarchique du cadre théorique :
  - Phase > sous-phase > saillants (collapsible)
  - Chaque saillant a sa définition + tableau des exemples par nation
- Les deux moteurs du Parcours (construction de l'État central + homogénéisation culturelle)
- Les perturbations (reboot, prolongement, choc d'hétérogénéité)

### Design
- Clean, sobre, académique mais moderne
- Police sans-serif (Segoe UI, system-ui)
- Fond clair (#fafafa), cartes blanches avec bordures légères
- Les couleurs des phases sont le fil conducteur visuel
- Responsive (desktop-first, mais utilisable sur tablette)
- Animations subtiles (hover, transitions)

### Stack technique
- Single Page Application
- Les données sont en dur dans le code (JSON) — pas de backend
- Utiliser une librairie de timeline si pertinent (vis.js, D3.js, ou custom SVG)
- Material Icons pour les icônes des saillants
