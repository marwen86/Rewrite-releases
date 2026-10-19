<p align="center">
  <img src="icon.png" width="128" height="128" alt="Icône de Rewrite">
</p>

<h1 align="center">Rewrite</h1>
<p align="center"><em>Reformulez votre texte, où que vous écriviez, d'un raccourci clavier.</em></p>

Rewrite est une petite app macOS de barre de menus. Placez le curseur dans n'importe
quel champ de texte — Slack, Mail, Notes, un formulaire web — appuyez sur le raccourci,
et le texte sélectionné (ou tout le champ) est reformulé sur place : orthographe et
grammaire corrigées, style adapté à l'application (message d'équipe, e-mail
professionnel, note). La mise en page d'origine (listes, paragraphes, retours à la
ligne) est toujours conservée.

Le code source n'est pas publié dans ce dépôt ; celui-ci ne contient que les versions
de test (`.dmg`) et leurs notes.

## Fonctionnalités

- **Raccourci global personnalisable**, actif dans toutes les applications.
- **Ton adapté automatiquement** : messagerie d'équipe, e-mail professionnel, ou neutre selon le contexte.
- **Mise en page préservée** : puces, numéros, paragraphes, lignes vides.
- **Plusieurs moteurs au choix** : Apple Intelligence (sur l'appareil, sans clé ni frais), un compte Claude ou OpenAI (clé API), ou un modèle local compatible OpenAI (Ollama, LM Studio).
- **Mises à jour intégrées** : l'app vérifie elle-même les nouvelles versions publiées ici, et vérifie l'intégrité du fichier téléchargé avant de l'ouvrir.
- **Confidentialité** : aucun message n'est jamais envoyé ailleurs qu'au moteur de reformulation choisi ; rien n'est stocké.

## Installer

1. Onglet **[Releases](../../releases)** → téléchargez le `.dmg` de la dernière version.
2. Ouvrez-le, glissez **Rewrite** sur **Applications**.
3. Premier lancement : macOS affiche « Apple ne peut pas vérifier… » (l'app n'est pas
   encore notariée). Réglages Système › Confidentialité et sécurité → **Ouvrir quand même**.

Les mises à jour suivantes se font depuis l'app (menu ✨ › **Vérifier les mises à
jour…**, ou automatiquement une fois par jour) : le fichier est téléchargé, son
empreinte vérifiée, puis il ne reste qu'à l'ouvrir et glisser la nouvelle version sur
Applications.

## Vérifier l'intégrité (optionnel)

Chaque release inclut `checksums.txt` :

```bash
shasum -a 256 -c checksums.txt
```

## Confidentialité

Rewrite n'envoie jamais de message. Détails dans l'app : menu ✨ › Aide…
