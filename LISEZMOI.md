# Bokin'ny Fivarotana : version installable (test terrain)

Ce dossier contient l'application complète. Elle fonctionne sans serveur ni base de données : les données de chaque épicier restent sur son téléphone.

| Fichier | Rôle |
| --- | --- |
| `index.html` | L'application |
| `sw.js` | Fonctionnement hors ligne et mises à jour |
| `manifest.webmanifest` | Nom, icône et couleurs à l'installation |
| `icons/`, `fonts/` | Icônes et polices, embarquées pour le hors-ligne |

## 1. Mettre en ligne (gratuit, environ 15 minutes, une seule fois)

Hébergement recommandé : **GitHub Pages**. Le code est public ; aucune donnée d'épicier n'y transite.

1. Créer un compte sur github.com.
2. Cliquer sur **New repository**. Nom : `bokin-fivarotana`. Visibilité : **Public**. Cocher « Add a README ». Créer.
3. Dans le dépôt : **Add file → Upload files**. Glisser **le contenu** du dossier (les fichiers et les dossiers `icons` et `fonts`, pas le dossier lui-même). Cliquer sur **Commit changes**.
4. **Settings → Pages**. Source : *Deploy from a branch*. Branche : `main`, dossier `/ (root)`. Enregistrer.
5. Après une à deux minutes, l'adresse apparaît en haut de la page : `https://<votre-identifiant>.github.io/bokin-fivarotana/`.

Alternative : Netlify ou Cloudflare Pages (glisser-déposer du dossier après création d'un compte).

## 2. Installer chez un épicier (jour 1 du test)

1. Ouvrir l'adresse dans **Chrome** sur le téléphone Android, avec une connexion.
2. Remplir l'inscription avec l'épicier : nom de la boutique, mode de saisie, argent en caisse et sur MVola, Orange Money, Airtel Money.
3. Appuyer sur **« Apetraho »** dans le bandeau vert, ou menu Chrome ⋮ → *Ajouter à l'écran d'accueil*.
4. Vérifier : couper les données mobiles, ouvrir l'icône « Fivarotana » ; l'application doit s'ouvrir normalement.
5. Faire faire à l'épicier une vente, un trosa et une dépense devant vous.

## 3. Récupérer les données du test

Dans **Fikirakirana → Alefaso ny tahiry**, l'épicier envoie un fichier `bokin-<boutique>-<date>.txt` par WhatsApp ou Messenger. Ce fichier contient toutes les opérations horodatées, les clôtures et les jours d'ouverture de l'application : il suffit à calculer les indicateurs du protocole de test. Recueillir l'accord de l'épicier avant l'envoi.

L'application rappelle elle-même de faire une sauvegarde si la dernière date de plus de sept jours.

## 4. Mettre à jour l'application

Remplacer les fichiers dans le dépôt GitHub par ceux de la nouvelle version (Upload files, puis Commit). Les téléphones détectent la nouvelle version à la prochaine ouverture avec connexion et affichent « Misy dikan-teny vaovao » ; les données sont conservées.

## 5. Précautions

- **Effacer les données de Chrome efface les données de l'application.** Le prévenir à l'épicier, et faire une sauvegarde avant toute manipulation du téléphone.
- Un même téléphone = une seule boutique.
- Testé pour Chrome sur Android. Sur iPhone, l'installation passe par Safari → Partager → *Sur l'écran d'accueil*, sans bandeau d'installation.
