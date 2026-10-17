# Rewrite — versions de test

Rewrite est une app macOS de barre de menus qui reformule le texte que vous écrivez,
dans n'importe quelle application, d'un raccourci clavier. Le code source n'est pas
publié dans ce dépôt ; celui-ci ne contient que les versions de test (`.dmg`) et leurs
notes.

## Installer

1. Onglet **[Releases](../../releases)** → téléchargez le `.dmg` de la dernière version.
2. Ouvrez-le, glissez **Rewrite** sur **Applications**.
3. Premier lancement : macOS affiche « Apple ne peut pas vérifier… » (l'app n'est pas
   encore notariée). Réglages Système › Confidentialité et sécurité → **Ouvrir quand même**.

## Vérifier l'intégrité (optionnel)

Chaque release inclut `checksums.txt` :

```bash
shasum -a 256 -c checksums.txt
```

## Confidentialité

Rewrite n'envoie jamais de message. Détails dans l'app : menu ✨ › Aide…
