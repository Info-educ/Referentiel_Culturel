# Référentiel culturel

Banque personnelle de références culturelles, organisée par thèmes et supports.
Site 100 % statique (HTML/CSS/JS), hébergé sur GitHub Pages, synchronisé entre
appareils via le fichier `data.json` de ce dépôt.

## Fichiers

| Fichier      | Rôle                                                            |
|--------------|-----------------------------------------------------------------|
| `index.html` | Le site complet (interface + moteur). Ne pas renommer.          |
| `data.json`  | Les données (thèmes, supports, références). Mis à jour automatiquement par le site. |
| `README.md`  | Ce mode d'emploi.                                               |

## Installation (une seule fois)

1. Créer un dépôt **public** sur GitHub (ex. `referentiel-culturel`).
2. Y déposer `index.html`, `data.json` et `README.md` (bouton *Add file → Upload files*).
3. Dans le dépôt : **Settings → Pages** → Source : *Deploy from a branch* →
   Branch : `main`, dossier `/ (root)` → **Save**.
4. Après 1 à 2 minutes, le site est en ligne à l'adresse :
   `https://VOTRE-PSEUDO.github.io/NOM-DU-DEPOT/`

## Activer la synchronisation (une fois par appareil)

1. Sur GitHub : avatar → **Settings → Developer settings →
   Personal access tokens → Fine-grained tokens → Generate new token**.
   - *Repository access* : **Only select repositories** → ce dépôt uniquement.
   - *Permissions → Repository permissions → Contents* : **Read and write**.
   - Choisir une expiration longue, générer, **copier le token** (`github_pat_…`).
2. Sur le site : bouton **⇅** dans l'entête → renseigner pseudo, dépôt,
   branche (`main`) et token → **Activer la synchronisation**.
3. Le bouton ⇅ devient vert : chaque modification est enregistrée dans
   `data.json`, et chaque appareil récupère la dernière version à l'ouverture.

⚠️ Le token est un mot de passe : ne pas le partager, le révoquer en cas de doute.
⚠️ Le dépôt étant public, le contenu de `data.json` est lisible par tous :
ne pas y mettre d'informations personnelles ou professionnelles sensibles.

## Utilisation quotidienne

- **✎ Modifier** : ajouter/supprimer/modifier références, thèmes, supports ;
  classer avec ▲▼ (références) et ◀▶ (thèmes).
- **🎨** : mode clair/sombre, couleur du fond et de l'entête (réglages propres
  à chaque appareil).
- **Exporter / Importer (JSON)** : sauvegarde de secours manuelle.

## Sur téléphone

Ouvrir l'adresse du site puis « Ajouter à l'écran d'accueil » : le référentiel
se lance alors comme une application.
