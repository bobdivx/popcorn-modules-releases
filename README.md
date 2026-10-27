# Popcornn — modules officiels (artefacts signés)

Ce dépôt **ne contient aucune source** : uniquement les **releases** des modules officiels
Popcornn (binaires, archives de données) et le catalogue signé du store.

- Catalogue : https://github.com/bobdivx/popcorn-modules-releases/releases/download/catalog/catalog.json
  (+ `catalog.json.minisig`).
- Une release par module et par version : `<id>-v<version>` (`release.json` + `.minisig`,
  binaires par plateforme et leur `.minisig`, `SHA256SUMS`).
- Tout est signé avec la clé officielle Popcornn (minisign) :

```
RWRoYJglb7zUH+1VkYMEPEykRUjYVhpVX9PEbrhSKJNSt5+TP4oejxFX
```

Vérification : `minisign -Vm catalog.json -P RWRoYJglb7zUH+1VkYMEPEykRUjYVhpVX9PEbrhSKJNSt5+TP4oejxFX`

Les modules s'installent depuis **Paramètres → Modules** du serveur Popcornn, qui vérifie la
signature et les empreintes avant installation. Releases publiées automatiquement ; ne pas ouvrir
de PR ici.
