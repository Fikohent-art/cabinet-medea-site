# Centre de Rééducation Fonctionnelle Dr Hentabli — Médéa

Site vitrine bilingue (français / arabe) du cabinet de Médecine Physique et
Réadaptation, Boulevard du 17 Octobre, Médéa.

Site statique, une seule page, sans build ni dépendance. `index.html` contient
tout (HTML, CSS, JS).

## Contenu

```
index.html          le site complet
assets/*.svg         cadres de remplacement provisoires (à remplacer par des photos)
netlify.toml         config de déploiement (aucun build, publie la racine)
```

## Déploiement Netlify

1. Netlify → Add new site → Import an existing project → GitHub → ce dépôt.
2. Build command : laisser vide. Publish directory : `.` (déjà réglé par `netlify.toml`).
3. Deploy.

Le site fonctionne aussi en ouvrant `index.html` localement dans un navigateur
(la carte Google Maps et les polices Google nécessitent une connexion).

## Photos

Aucune photo réelle n'est encore fournie : chaque emplacement affiche un cadre
de remplacement intégré. Pour ajouter les vraies photos, déposer dans `assets/`
les fichiers `boulevard.png`, `consultation.png`, `accueil.png`, `entree.png`,
`balneotherapie.png`, `plan-acces.png`. Aucune modification du code n'est nécessaire
(le `.png` est chargé en priorité, sinon le `.svg`, sinon le cadre CSS).

## À faire avant diffusion publique

- Remplacer l'URL `https://centre-reeducation-medea.dz/` dans `index.html`
  (balises `canonical` et Open Graph) par le domaine réel.
- Vérifier numéros de téléphone, adresse, horaires, lien Google Maps.
- Le texte « Le cabinet » présente la structure comme en activité : à confirmer.
- Versions FR et AR alignées (encadré paiement retiré, FAQ à 5 questions).
