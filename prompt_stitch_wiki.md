# Prompt Stitch — Section "Référentiel des saillants" pour Historionomie

## Contexte

Je construis une page wiki pour un projet de recherche en histoire comparée. J'ai besoin d'une section "Référentiel des saillants" qui présente hiérarchiquement les phases, sous-phases et saillants du modèle.

## Design existant

La page utilise déjà ces fonts et couleurs :
- **Fonts** : Newsreader (serif, titres) + Public Sans (sans-serif, corps)
- **Background** : #f9f9f9
- **Couleurs des phases** :
  - Pré-féodale : #A0A0A0 (gris)
  - Féodale : #8B7355 (marron)
  - Oligarchique : #2E8B57 (vert)
  - Absolutiste : #6A0DAD (violet)
  - Révolution Nationale : #D4A017 (or)
  - Parlementaire : #1E90FF (bleu)
- **Icônes** : Material Symbols Outlined

## Structure hiérarchique souhaitée

```
PHASE (grande carte, toujours visible)
  ├─ Titre en Newsreader, gros, avec dot de couleur
  ├─ Description du mécanisme (toujours visible)
  │
  ├─ SOUS-PHASE (toujours visible, indentée, bordure gauche colorée)
  │   ├─ Titre en semi-bold
  │   ├─ Description (toujours visible)
  │   │
  │   ├─ SAILLANT 1 (collapsible, chacun son propre toggle)
  │   │   ├─ Toggle: icône Material + nom du saillant
  │   │   └─ Contenu déplié:
  │   │       ├─ Description du concept
  │   │       └─ Tableau comparatif (5 colonnes: Israël, France, Angleterre, Venise, Bavière)
  │   │
  │   ├─ SAILLANT 2 (collapsible)
  │   │   └─ ...
  │   │
  ├─ SOUS-PHASE (toujours visible)
  │   ├─ ...
```

## Contenu exact

### Phase féodale (#8B7355)
Description : "Interconnexion des réseaux claniques et lignagers. Le pouvoir repose sur des liens personnels de vassalité — il se fragmente à chaque succession difficile. Durée typique : ~200 ans (peut boucler et durer beaucoup plus)."

**Sous-phase : Percolation**
Description : "Le pouvoir est distribué entre des micro-pouvoirs locaux sans centre. Au seuil critique de percolation (au sens de la théorie des systèmes dynamiques), un chemin continu se forme : un chef émerge qui force les autres à se positionner."

Saillant (collapsible) :
- **Éveil féodal** (icône: wb_sunny)
  - "Le premier chef dont l'autorité supra-régionale est effective — pas un simple titre, mais un pouvoir réel qui structure le jeu politique."
  - Tableau: Israël → Saül (~-1080) | France → Louis VI (1108) | Angleterre → Guillaume (1066) | Venise → Orso Ipato (~726) | Bavière → Louis Ier (~1204)

**Sous-phase : Coagulation des élites**
Description : "Après l'éveil, il y a un centre. Les élites se « coagulent » autour du suzerain ou contre lui. Le processus est ponctué de pics féodaux (rois forts) et de crises féodales (effondrements post-pic). Chaque pic accélère l'homogénéisation. Chaque crise teste si le seuil du pacte est atteint."

Saillants (chacun collapsible) :
- **Pic féodal** (icône: terrain) — récurrent
  - "Roi fort au sommet de sa puissance personnelle. Il projette la puissance vers l'extérieur et cristallise l'opposition des barons. Son édifice est personnel et fragile."
  - Tableau: Israël → Salomon (~-960) | France → Phil. le Bel (~1295) | Angleterre → Édouard Ier (~1295) | Venise → Orseolo (~991) | Bavière → Louis IV (~1328)

- **Crise féodale** (icône: bolt, en rouge) — récurrent
  - "Effondrement du système personnel. Si les conditions du pacte ne sont pas réunies, le Parcours boucle — affiché en rouge sur les frises."
  - Pas de tableau

**Sous-phase : Bascule oligarchique**
Description : "Le pacte ne survient que quand deux conditions sont réunies simultanément : homogénéité des oligarques à l'échelle du royaume + moment de faiblesse du suzerain."

Saillant (collapsible) :
- **Pacte oligarchique** (icône: gavel)
  - "Pour la première fois, les oligarques codifient collectivement la structure de l'exécutif."
  - Tableau: Israël → — | France → Loi salique (1317) | Angleterre → Ordonnances (1311) | Venise → Abol. co-régence (1032) | Bavière → Primogéniture (1506)

---

### Phase oligarchique (#2E8B57)
Description : "Émergence puis victoire du pouvoir administratif sur les réseaux féodaux. L'État central se dote d'un impôt permanent, d'une armée permanente, d'une administration. Durée typique : ~200 ans."

**Sous-phase : Essor oligarchique**
Description : "Les oligarques dotent l'exécutif central d'un pouvoir suffisant pour arbitrer leurs conflits. Codification du droit, protection de la propriété privée, croissance économique."

Saillants :
- **1er monarque oligarchique** (icône: stars)
  - "Le premier souverain disposant d'un État central — impôt permanent, armée permanente, administration."
  - Tableau: Israël → Omri (-885) | France → Philippe VI (1328) | Angleterre → Édouard III (1327) | Venise → Contarini (~1043) | Bavière → Guillaume IV (~1508)

- **Pic oligarchique** (icône: terrain)
  - "Le pic de puissance et de prestige pendant la phase."
  - Tableau: Israël → Jéroboam II (~-770) | France → François Ier (~1515) | Angleterre → Édouard III (~1350) | Venise → Foscari (~1440) | Bavière → Albert V (~1555)

- **Fin de l'expansion** (icône: block)
  - "Le moment où l'expansion extérieure cesse et les tensions internes prennent le relais."
  - Tableau: Israël → ~-746 | France → Cateau-Cambrésis (1559) | Angleterre → — | Venise → Agnadello (1509) | Bavière → —

**Sous-phase : Polarisation des élites**
Description : "La classe prébendière et la classe patrimoniale se polarisent. Les élites patrimoniales se rallient à l'administration, abandonnant leurs clientèles rurales."
(Pas de saillant propre)

**Sous-phase : Guerre sociale**
Description : "Le conflit nécessaire entre factions. Ne se résout pas par la victoire d'une faction mais par le triomphe de l'État central. Une figure « tiers » émerge."

Saillant :
- **Guerre sociale** (icône: local_fire_department)
  - "Le conflit factieux qui conclut la phase. Peut prendre la forme d'une guerre conventionnelle ou de tensions institutionnelles."
  - Tableau: Israël → -700 à -641 | France → G. de Religion (~1562-98) | Angleterre → Deux-Roses (~1455-85) | Venise → ~1628-1669 | Bavière → ~1564-1597

---

### Phase absolutiste (#6A0DAD)
Description : "Achèvement de l'élimination des réseaux féodaux et oligarchiques par le pouvoir central. L'administration acquiert une supériorité incontestée. Durée typique : ~200 ans."

**Sous-phase : Absolutisation (~50-100 ans)**
Description : "Le pouvoir central met au pas les grands féodaux et oligarques. L'ancienne aristocratie est intégrée dans l'administration (domestication) ou écartée du pouvoir (exclusion)."

Saillants :
- **1er monarque absolu** (icône: crown, filled)
  - "La figure qui résout la guerre sociale et inaugure la concentration du pouvoir."
  - Tableau: Israël (prol.) → Simon Thassi (-140) | France → Henri IV (1598) | Angleterre → Henri VII (1485) | Venise → Inquisiteurs (~1669) | Bavière → Maximilien Ier (1597)

- **DGRO** (icône: whatshot)
  - "Dernière grande révolte oligarchique. Absente quand les oligarques n'ont pas de base territoriale."
  - Tableau: Israël → Jannée (-94) | France → La Fronde (1648-53) | Angleterre → Henri VIII (~1534-40) | Venise → — | Bavière → —

**Sous-phase : Impérialisme absolutiste**
Description : "Le pouvoir central dispose de moyens sans précédent. Politique expansionniste, multiplication des guerres, domestication de la noblesse par la cour."

Saillants :
- **Pic absolutiste** (icône: terrain)
  - "Le sommet de la puissance absolutiste — expansion maximale, prestige maximal."
  - Tableau: Israël → Hérode (~-20) | France → Louis XIV (~1682) | Angleterre → Élisabeth Ière (~1580) | Venise → Morosini (~1688) | Bavière → Max. III Joseph (~1756)

- **Fin de l'expansion** (icône: block)
  - "Le pouvoir central atteint les limites de son expansion."
  - Tableau: Israël → Mort d'Hérode (-4) | France → Utrecht (1713) | Angleterre → — | Venise → Passarowitz (1718) | Bavière → Blenheim (1704)

- **Remontrance** (icône: record_voice_over)
  - "Dernière tentative institutionnelle de reprendre des prérogatives au pouvoir absolu. Échoue et ouvre l'AR."
  - Tableau: Israël → — | France → Polysynodie (1715) | Angleterre → Apology (1604) | Venise → Correzione (1761) | Bavière → Landtag (1848)

**Sous-phase : Ancien Régime (~35-100 ans)**
Description : "Le système absolutiste à maturité. Les élites se sédimentent, la mobilité sociale se fige. Le clivage gauche-droite saute : ED + EG convergent en bloc contestataire."

Saillant :
- **Ancien Régime** (icône: hourglass_top)
  - "Sédimentation des élites, surproduction élitaire. La rupture est inévitable."
  - Tableau: Israël → 4 à 66 | France → ~1715-1789 | Angleterre → ~1603-1642 | Venise → ~1718-1848 | Bavière → ~1848-1918

---

### Révolution Nationale (#D4A017)
Description : "Renversement de l'ordre absolutiste. Le bloc contestataire (ED + EG) fait tomber le bloc élitaire. Durée typique : ~25-80 ans."

**Sous-phase : Révolution initiale**
Description : "Explosion, expérience parlementaire, phase aiguë, moment thermidorien. La période la plus turbulente."

Saillants :
- **Explosion de l'AR** (icône: flash_on)
  - "L'AR perd sa légitimité et sa capacité financière. Les élites basculent."
  - Tableau: Israël → Grande Révolte (66) | France → 1789 | Angleterre → Guerre civile (1642) | Venise → Insurrection (1848) | Bavière → Eisner (1918)

- **Expérience parlementaire** (icône: account_balance)
  - "On expérimente le parlementarisme après le renversement."
  - Tableau: Israël → Gouv. coalition (66-67) | France → Ass. nat. (1789-91) | Angleterre → Long Parl. (1640-48) | Venise → Rép. Manin (1848-49) | Bavière → État libre (1918-19)

- **Phase aiguë** (icône: skull, filled)
  - "L'extrême-gauche prend le contrôle et élimine les modérés."
  - Tableau: Israël → Zélotes (67-70) | France → Terreur (1792-94) | Angleterre → Exéc. Charles Ier (1649) | Venise → Pouvoirs ill. (1849) | Bavière → Rép. Conseils (1919)

- **Moment thermidorien** (icône: balance)
  - "Le centre reprend le pouvoir et purge l'EG."
  - Tableau: Israël → — (écrasée) | France → Directoire (1794-99) | Angleterre → Rump Parl. (1649-53) | Venise → — (écrasée) | Bavière → — (absorbée)

**Sous-phase : Impérialiste Revanchard**
Description : "Figure autoritaire qui renoue avec la verticalité du pouvoir. Ventilation des élites, méritocratie, impérialisme militaire."

Saillant :
- **Émergence de l'IR** (icône: military_tech)
  - "Le moment où la figure autoritaire prend le pouvoir."
  - Tableau: Israël → — | France → Bonaparte (1799) | Angleterre → Cromwell (1653) | Venise → — (avortée) | Bavière → — (absorbée)

**Sous-phase : Restauration → Glorieuse Révolution**
Description : "L'IR tombe. Régime à base élargie, pas encore pleinement parlementaire. Une réplique ancre définitivement le parlementarisme."

Saillant :
- **Glorieuse Révolution** (icône: star)
  - "Transition définitive vers l'État-nation parlementaire."
  - Tableau: Israël → — | France → 1830 | Angleterre → 1688 | Venise → — (abs. 1866) | Bavière → — (abs. 1919)

---

### Perturbations (#ba1a1a)
Description : "Le Parcours peut être perturbé par des chocs externes. L'effet dépend de ce qu'ils font aux deux moteurs."

Saillants :
- **Reboot** (icône: restart_alt) — "Destruction des institutions. Le Parcours régresse."
- **Prolongement** (icône: pause) — "Hétérogénéisation sans destruction. Le Parcours stagne."
- **Choc d'hétérogénéité** (icône: group_add, rouge) — "Expansion territoriale qui hétérogénéise brutalement. Peut avorter une sous-phase."

## Spécifications de design

- **Hiérarchie visuelle claire** : les phases doivent être immédiatement distinguables des sous-phases, et les sous-phases des saillants
- Chaque **phase** a une bordure gauche épaisse (4px) dans sa couleur + titre en Newsreader 1.3rem
- Chaque **sous-phase** a une bordure gauche fine (2px) dans la couleur de la phase, indentée, titre en Public Sans 0.95rem semi-bold
- Chaque **saillant** est son propre collapsible (toggle individuel), avec :
  - L'icône Material du saillant (dans la couleur de la phase)
  - Le nom du saillant en Public Sans bold
  - Au clic, s'ouvre pour montrer la description + le tableau comparatif
- **Pas de fond coloré agressif** — rester sur les blancs/gris très légers (#fff, #faf8f4, #f3f3f3)
- Les tableaux doivent être compacts (font-size ~0.78rem), avec header grisé
- Animations douces sur les toggles (rotate de la flèche, slide-down du contenu)
- Responsive : les tableaux passent en scroll horizontal sur mobile
