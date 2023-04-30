# Cahier des Charges - Inscriptions Vacances

## État des lieux

Une association jeunesse en île de France propose à chaque période de vacance un programme d’activité à destination des jeunes de la région. Ces activités ont des places limités, dépendent de l’âge, nécessitent parfois des documents (autorisation de sortie, certificat médical, etc.) sont parfois payantes et ne sont ouvertes qu’aux adhérent·es de l’association.

Actuellement, ces inscriptions se font à la main sur des feuilles dans un classeur. Cela implique différents problèmes :

- Pour chaque période de vacance, il faut recréer une page, pour chaque activité. Au total, c’est une 40aine de documents qui sont créé toutes les 6 semaines alors qu’ils pourraient être automatisés.
- Chaque page correspondant à une activité, on voit pour cette activité qui est inscrit, les éléments nécessaires, etc. Mais il n’y a pas de visibilité sur l’ensemble des activités d’un·e jeune : où iel est inscrit·e, quels documents sont manquants pour l’ensemble des activités, etc.
- Pour inscrire une personne, il faut passer par l’ensemble des feuilles et inscrire son nom sur chaque.
- Lorsqu’un document spécial est demandé (autorisation de sortie), un document word est refait à chaque fois pour chaque sortie pour chaque membre de la famille. Il arrive donc qu’une famille avec 3 enfants participant à 2 sorties chacun·e ait 6 papiers à imprimer et signer.
- Régulièrement, les jeunes demandent à quoi iels sont inscrit·es. Hors, le système de classement par activité nécessite de passer chaque page une par une pour avoir les réponses, amenant parfois des erreurs.
- Pour des jeunes qui reviennent régulièrement, il faut tout de même refaire toute la procédure d’inscription (numéro de tel d’urgence, âge, etc.)
- Plusieurs personnes s’occupent des inscriptions, laissant parfois des notes dans un coin de page. Résultat, il peut y avoir des incompréhensions et des erreurs d’inscription commises.
- Lors de la sortie du programme, de nombreux·ses jeunes se présentent pour s’inscrire, des mails de parents arrivent, etc. Mais il n’y a qu’un classeur, une seule inscription peut se faire à la fois.

## Fonctionnalités nécessaires

- Se connecter
- créer un utilisateur permanent
- créer un utilisateur stagiaire et le lier à des vacances en particulier
- créer une période de vacance qui contient les infos suivantes :
  - Une saison
  - Un nom
  - une couleur pour l'identifier facilement
  - Des dates début / fin
  - Des groupes d'activité (8-12, collégiens, Stage, etc.) + une couleur pour chaque
  - Des anims tempo
- Créer une fiche jeune qui contient :
  - Un nom / prénom / prénom d'usage.
  - Une date d'anniv
  - Le contact tel d'un/des parent(s)
  - Le contact du jeune (opt)
  - un mail de contact
  - Un champs de remarques
  - son état d'adhésion qui reset chaque saison
- Créer une activité qui contient :
  - Un groupe d'activité
  - une date
  - des horaires
  - un nom
  - un nombre de places
  - la possibilité d'ajouter un PAF
  - la possibilité d'ajouter une autorisation de sortie avec le lieu
- Inscrire un jeune à une activité et suivre les documents
- Inscrire un jeune sur une liste d'attente
- Editer les autorisations de sorties personnalisées
- Visualiser les participations à une activité et l'imprimer
- Visualiser les activités d'un participant et l'imprimer
- Visualiser les places disponibles dans une activité, les docs manquants, etc.

## Structure

Liste des pages nécessaires :

- Accueil
  > affiche le programme
  > lien vers le site
  > infos inscriptions
  > bouton log in
- Log In

  > ID / MDP / MDP oublié

- Accueil Back

  > Boutons pour accéder aux pages de création et de visualisation

- Page création utilisateur·ice

  > Champs Nom, Prénom, MDP tempo à générer, mail.

- Page création Vacances
  > Champs : Nom des vacances / date début / date fin / liste checkbox Stagiaires
- Page création Activité
  > Champs : Nom activité / Type activité (Activité, Sortie, soirée, repas, stage) / Horaires / Tranche d'âge / limite participant·es / PAF /

> si sortie en type d'activité, autres champs dispo :
> Sortie : lieu, moyen de locomotion, autorisation parentale

- Page création Jeune

> Différents champs : Nom, Prénom, Date de naissance, Adhérent·e oui/non, Contact jeune, Contact Parent1, Contact Parent2, Autre Contact d'urgence, Remarques (allergies, traitements, etc.)

- Page visualisation Vacance

  > Liste des activités, listes des jeunes inscrit·es avec docs manquants, liste des animateur·ices
  > bouton Ajouter une activité
  > Accès à ces sous pages de visualistation
  > impression liste jeune

- Page visualisation Activité

> Liste jeunes inscrit·es avec docs manquants
> Impression feuille présence
> Ajouter jeune

- Page visualisation Jeune

> Impression liste activité (par periode vacance)
> Impression autorisations de sortie
> Liste documents
> inscription à une activité

## Accès

- **_Admin_**
  - Création d'utilisateur·ices **permanents**
  - Accès complet
- **_Permanent·e_**
  - Création d'utilisateur·ices **Stagiaire** ou **invité**
  - Création de _Vacance_
  - Création de _Activité_
  - Création de _Jeune_
  - Inscriptions activité
  - Accès à toutes les infos (tous les _Jeunes_, toutes les _vacances_ et _activités_)
  - Impression des fiches activités, fiches jeunes, etc.
- **_Stagiaire_** ou **_invité_** (dépend d'une période _Vacance_)
- Accès aux infos pour une période de vacance uniquement (Activités, Jeunes, impression)
- Impression des fiches activités, fiches jeunes, etc. Pour une période de vacance
- **_Visiteur·se_** (Non log)
- Uniquement page d'accueil
  - Vu sur le programme
  - Lien vers le site
  - Infos diverses

## Contraintes

- Interface utilisateur·ice complète
- En adéquation avec la charte graphique existante
- Création d'une FAQ
- Intégration au site existant (?)
- Prévoir solution pour les deux programmes d'âge (ou plus, ou moins)

## Charte graphique

voir [Site](www.mjc-igny.org)

voir [Plaquette](https://www.mjc-igny.org/wp-content/uploads/2022/08/Plaquette-2022-2023-web.pdf)

voir affiches :

![affiche projection débat pourquoi nous détestent-ils nous les femmes](https://www.mjc-igny.org/wp-content/uploads/2023/02/pourquoi-nous-detestent-ils-nous-les-femmes-842x550.png)
![affiche expo au fil de l'eau](https://www.mjc-igny.org/wp-content/uploads/2023/02/Affiche-Au-fil-de-leau-1-1170x550.png)
![affiche stage éveil musical](https://www.mjc-igny.org/wp-content/uploads/2023/02/affiche-1170x550.jpg)

## Maquettes

### Premières maquettes mobiles (WIP)

![Accueil](https://zupimages.net/up/23/17/h94d.png)
![Connexion](https://zupimages.net/up/23/17/cvgs.png)
![Affichage activités](https://zupimages.net/up/23/17/9n4z.png)
![Affichage participant·es](https://zupimages.net/up/23/17/famu.png)
![Affichage vacances](https://zupimages.net/up/23/17/53cb.png)
![Ajoute Vacances, activité"s et jeune](https://zupimages.net/up/23/17/qz2h.png)
![Ajout et liste users](https://zupimages.net/up/23/17/whb4.png)

## Idées de fonctionnalités futures (non essentielles)

- Envoyer SMS
- Envoyer mail
- dupliquer activité
- export statistiques
- Mode planning ?
