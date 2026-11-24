# Journal des modifications

## 2026.11.24
- Nouvelle page Wishlist (Plus > Wishlist) : jeux que tu veux faire, avec nom, console, durées HowLongToBeat, tags, date de sortie et note.
- Date de sortie complète (jj.mm.aaaa), partielle (mm.aaaa ou aaaa) ou « À annoncer ». Le jeu passe tout seul à « Déjà disponible » à la date indiquée (à la fin du mois ou de l'année pour une date partielle).
- Durée personnalisée pour chaque jeu (heures et jours), calculée avec le même modèle que « Simuler un jeu ».
- Tri par date de sortie, nom, console, durée pour toi, tag ou date d'ajout ; filtres par état, console et tags (tous ces tags ou au moins un) ; recherche.
- Bouton « Commencer ce jeu » : crée le jeu dans Solo avec console, durées et prévision initiale, puis le retire de la wishlist.
- La wishlist est incluse dans la sauvegarde totale. Format de sauvegarde passé à la version 5.
- Correctif : le cache du modèle de prévision se met maintenant à jour aussi quand tu modifies un jeu ou une durée sans changer le nombre de jeux ni de sessions.

## 2026.11.22
- Sauvegarde par année : Plus, Sauvegarde et restauration, section « Années ». Chaque année s'enregistre dans son fichier `suivi-jeux-annee-AAAA.json` (sessions, parties, jeux concernés, partenaires, historiques mensuels).
- Chargement d'une année depuis son fichier, avec aperçu : une année déchargée est rechargée, une année présente reçoit seulement les sessions manquantes (rien n'est écrasé ni dupliqué).
- Décharger une année pour alléger l'app : possible seulement si son fichier est enregistré et à jour, jamais pour l'année en cours. L'app garde les totaux par jeu, donc les prévisions ne changent pas.
- Restauration d'une sauvegarde totale : cases à cocher pour ne charger que certaines années.
- Format de sauvegarde passé à la version 4 (une app plus ancienne refuse ces fichiers).

## 2026.11.20
- Nouveau style « Les quatre éléments » : chaque page a son élément et sa couleur (Chrono = terre, Combat = feu, Bilan = air, Plus = eau), avec bannière, décor et sceau en kanji (土 火 風 水).
- Deux nouvelles polices : Zen Antique (Chrono, Combat) et Shippori Mincho (Bilan, Plus), pour les titres et le texte de ce style.

## 2026.11.19
- DLC et démos pour les jeux solo : deux cases dans la fiche (exclusives). Un DLC se rattache à un jeu solo de base (nom à saisir, rattachement par identifiant) et s'affiche sous lui, avec un bloc « jeu de base, DLC, total ».
- DLC et démos comptent dans les totaux et les sessions des bilans, mais sont exclus des moyennes par jeu, des classements (plus long, plus court, plus joué), des jeux finis, des distances et de la complétion moyenne.
- Un DLC garde sa propre estimation HowLongToBeat. DLC et démos n'entrent pas dans le calibrage des prévisions.
- Suppression du jeu de base : ses DLC redeviennent des jeux normaux.

## 2026.11.17.3
- Styles Allons-y !, Dinosaures, High noon et Yggdrasil : l'encadré passe derrière le contenu et n'a plus de bord supérieur, donc il ne cache plus rien au défilement.

## 2026.11.17.2
- Ouverture hors ligne : `sw.js` garde une copie de l'app (réseau d'abord, copie en secours).

## 2026.11.17
- Écran d'accueil (feu de camp, cadran à l'heure réelle, nuit étoilée), nouvelle icône.
- Garde-fous : échec d'enregistrement signalé, suppression d'un jeu en deux temps, restauration avec comparaison des totaux, chrono de plus de 12 h à confirmer, sessions trop courtes signalées.
- Version et date de dernière sauvegarde affichées dans Plus.
- Clé de stockage `save-point-v1` (reprise automatique de `suivi-solo-v1`).
