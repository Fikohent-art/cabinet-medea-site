# Centre de Rééducation Fonctionnelle Dr Hentabli — Médéa

Site vitrine bilingue (français / arabe) du cabinet de Médecine Physique et
Réadaptation, Boulevard du 17 Octobre, Médéa.

En ligne : **https://cabinet-reeducation-medea.netlify.app/**

Site statique, une seule page, sans build ni dépendance. `index.html` contient
tout (HTML, CSS, JS). Netlify redéploie à chaque push sur `main`.

## Contenu

```
index.html          le site complet
assets/*.jpg         les 6 photos réelles du cabinet (~740 Ko au total)
assets/*.svg         cadres de remplacement, filet de sécurité si une photo manque
netlify.toml         config de déploiement (aucun build, publie la racine)
```

Chaque emplacement charge `assets/<nom>.jpg`, sinon `.png`, sinon `.svg`, sinon un
cadre CSS. Pour changer une photo : remplacer `assets/<nom>.jpg` (noms : boulevard,
consultation, accueil, entree, balneotherapie, plan-acces), aucun changement de code.

## À faire

- Si un domaine propre est pris (ex. `.dz`), mettre à jour `canonical` et `og:url`
  dans `index.html`.
- Vérifier numéros de téléphone, adresse, horaires, lien Google Maps.
- Le texte « Le cabinet » présente la structure comme en activité : à confirmer.
