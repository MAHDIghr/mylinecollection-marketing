# Guide de production des images du site — My Line Collection

> **Objectif :** produire des visuels élégants, cohérents, fidèles aux produits et optimisés pour un site e-commerce rapide sur mobile.
>
> **Dépôt :** `MAHDIghr/mylinecollection-marketing`  
> **Dossier de référence :** `contenus/images-site/`

## 1. Le processus à suivre

**Références produit → Génération IA → Contrôle → Détourage → Optimisation → GitHub → Validation sur le site**

Ne pas déposer une image dans le dossier final tant qu’elle n’a pas été contrôlée et optimisée.

## 2. Les visuels à produire

### A. Bannière d’accueil — collection automne

- Récupérer l’URL et les photos du sac réellement acheté et destiné à être mis en avant.
- Utiliser ces photos comme références dans **Wevi avec Nano Banana Pro**.
- Créer une ambiance automnale premium : camel, chocolat, bordeaux, beige chaud et crème ; lumière douce et décor raffiné.
- Placer le sac clairement dans la composition et laisser une zone dégagée pour le titre et le bouton du site.
- **Ne pas intégrer de texte publicitaire dans l’image** : le texte sera ajouté dans le site.
- Préparer une version mobile dédiée si le recadrage desktop ne fonctionne pas.

### B. Sélection signature — un visuel par sac acheté

- Récupérer les liens et photos de **tous les sacs achetés**. Au lancement, les présenter tous, puisque la sélection est encore limitée.
- Choisir une image maîtresse qui définit l’angle : par exemple, vue trois-quarts avant.
- Réutiliser la même référence de cadrage, une lumière similaire et la même perspective générale pour chaque sac.
- Respecter le produit réel : forme, proportions, couleur, texture, coutures, poignées, bandoulière, fermetures et détails métalliques.
- Supprimer le fond et vérifier la présence d’une véritable transparence alpha.
- Centrer le sac sur une toile carrée et garder des marges régulières. Ajuster l’échelle visuelle sans déformer les proportions du produit.
- Comparer toutes les images côte à côte avant validation.

**Prompt de base à adapter pour chaque sac :**

> À partir de la photo de référence, créer une image e-commerce réaliste et haut de gamme pour My Line Collection. Respecter le produit d’origine : forme, proportions, couleur, matière, coutures, poignées, bandoulière, fermetures et détails métalliques. Ne pas inventer de logo ni modifier le design. Présenter le sac en vue trois-quarts avant, en reprenant l’angle et la perspective de l’image maîtresse de la série. Éclairage studio doux, détails nets, sac centré sur une toile carrée avec des marges régulières. Fond entièrement transparent avec canal alpha réel, sans fond blanc, sans damier intégré et sans halo sur les contours. Générer en qualité maximale disponible. Le fichier sera contrôlé, détouré si nécessaire, redimensionné et optimisé avant publication.

> **Important :** l’IA peut modifier de petits détails. Si le rendu n’est pas fidèle au sac vendu, corriger à partir de la photo source ou utiliser une photographie réelle. Ne pas publier un visuel trompeur.

### C. Images des catégories

Créer une image par catégorie, dans un style cohérent :

1. Sacs à main
2. Sacs bandoulière
3. Portefeuilles
4. Accessoires

Utiliser une lumière, une ambiance, un contraste et un niveau de qualité similaires. Chaque image doit représenter immédiatement sa catégorie.

### D. Visuel publicitaire multi-sacs

- Composer une scène avec plusieurs sacs, un produit principal et des produits secondaires.
- Montrer les matières, les coutures, les fermetures et les finitions.
- Utiliser une ambiance élégante, automnale et équilibrée.
- Si les sacs sont présentés comme disponibles à la vente, conserver leur apparence réelle.

Pinterest et les sites de mode peuvent servir à étudier la composition, la lumière et les ambiances. Utiliser ces références comme inspiration, pas comme des images à republier sans autorisation. Vérifier les droits d’utilisation des photos fournisseurs et les conditions des outils employés.

## 3. Dimensions, formats et poids cibles

Les poids sont des **objectifs indicatifs** : la qualité visuelle et la fidélité du produit restent prioritaires. Vérifier le poids réel après export.

| Visuel | Dimensions de départ | Format final conseillé | Poids cible |
|---|---:|---|---:|
| Bannière desktop | 1920 × 900 px | WebP ou AVIF | 200–350 Ko |
| Bannière mobile | env. 900 × 1200 px | WebP ou AVIF | 100–200 Ko |
| Sélection signature | 1000 × 1000 px | WebP transparent | 100–220 Ko/image |
| Catégories | 800 × 800 px | WebP ou AVIF | 80–160 Ko/image |
| Multi-sacs | 1600 × 1000 px | WebP ou AVIF | 150–300 Ko |

### Règles techniques

- Générer en qualité maximale disponible, idéalement en 4K si l’outil le permet, puis **redimensionner selon l’usage réel**.
- **WebP** est le format par défaut conseillé. Comparer avec **AVIF** si l’outil de conversion et l’intégration le permettent.
- Pour les sacs détourés, vérifier que le format final conserve la transparence. Le JPEG ne la conserve pas.
- Le PNG peut servir de source intermédiaire, mais il est souvent trop lourd pour la livraison web.
- Ajuster la compression image par image : contrôler les contours, les textures, les coutures, les détails métalliques et les couleurs.
- Conserver les sources haute résolution dans un espace de travail séparé ; ne pas les mélanger aux fichiers finaux servis par le site.
- Outil possible pour comparer les formats et la compression : [Squoosh](https://squoosh.app/).

## 4. Contrôle qualité avant livraison

Pour chaque fichier, vérifier :

- [ ] Le produit reste fidèle à sa photo source.
- [ ] Aucun détail important n’est déformé ou inventé.
- [ ] Le cadrage et les marges sont cohérents avec les autres images de la même série.
- [ ] Pour la sélection signature, le fond est réellement transparent et les contours sont propres.
- [ ] Les dimensions correspondent au tableau.
- [ ] Le format final est adapté et le poids a été vérifié.
- [ ] La compression ne dégrade pas visiblement les détails.
- [ ] Le nom du fichier est descriptif et compréhensible.

## 5. Déposer les fichiers dans ce dossier

Utiliser cette organisation simple :

```text
contenus/
└── images-site/
    ├── README.md
    ├── accueil/
    │   ├── hero-automne-desktop.webp
    │   └── hero-automne-mobile.webp
    ├── selection-signature/
    │   ├── sac-main-modele-descriptif.webp
    │   └── ...
    ├── categories/
    │   ├── sacs-a-main.webp
    │   ├── sacs-bandouliere.webp
    │   ├── portefeuilles.webp
    │   └── accessoires.webp
    └── campagne/
        └── collection-multi-sacs-automne.webp
```

Adapter les noms des fichiers aux modèles réellement retenus. Éviter les noms vagues tels que `image1-final-v2.webp`.

Pour chaque série, noter dans ce README ou dans un petit tableau de suivi : **nom du fichier, section, dimensions, format, poids, source produit et statut de validation**. Mettre à jour la liste de livraison lorsque les images sont ajoutées.

## 6. Intégration et performance du site

- Tester les images sur ordinateur et sur mobile, notamment les recadrages et la lisibilité.
- Prévoir une composition mobile dédiée si le format horizontal ne convient pas.
- Donner la priorité au chargement de la bannière principale lorsqu’elle est visible dès l’arrivée sur la page.
- Utiliser le chargement différé pour les images situées plus bas dans la page lorsque pertinent.
- Préserver le ratio des images afin d’éviter les déformations et les déplacements de contenu.
- Vérifier le rendu et les performances avec les outils de développement ou Lighthouse/PageSpeed Insights.
- Le dépôt GitHub sert à conserver les livrables. Ne pas supposer que les liens de prévisualisation GitHub constituent l’hébergement final des images de la boutique : l’intégration doit utiliser l’emplacement de production prévu.

Références utiles : [Optimisation des images web — web.dev](https://web.dev/learn/performance/image-performance/) · [Images responsives — web.dev](https://web.dev/learn/design/responsive-images/).

## 7. Checklist finale de livraison

- [ ] Bannière automne desktop validée ; version mobile créée si nécessaire.
- [ ] Un visuel validé pour chaque sac acheté dans la sélection signature.
- [ ] Angles, perspectives et échelles visuelles cohérents dans la sélection signature.
- [ ] Quatre images de catégories livrées.
- [ ] Visuel publicitaire multi-sacs livré.
- [ ] Détourage, transparence, dimensions et poids vérifiés.
- [ ] Fichiers finaux déposés dans les bons sous-dossiers.
- [ ] Liste des fichiers et métadonnées mise à jour.
- [ ] Rendu desktop et mobile contrôlé avant intégration définitive.

**Critère d’acceptation :** les visuels sont esthétiques, cohérents, fidèles aux produits réellement vendus, correctement optimisés et prêts à être intégrés au site.
