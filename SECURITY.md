# Signaler un problème de sécurité

Vous pensez avoir trouvé une **vulnérabilité** dans Tirelire, dans ses installateurs ou dans son mécanisme de mise à jour ? Merci de **ne pas** ouvrir d'issue publique avec les détails.

## Comment signaler

1. Si l'onglet **Security** de ce dépôt propose **Report a vulnerability**, utilisez ce formulaire : le signalement reste privé.
2. Sinon, contactez **Joseph Deffayet** par un **canal privé** (e-mail ou autre moyen qu'il vous aura communiqué).

Précisez :

- le problème et son impact ;
- les étapes pour le reproduire, si possible ;
- la version concernée (dans **Mon compte** > **Mises à jour**, ou dans le nom du fichier d'installation).

## Ce que fait Tirelire pour vos données

- Les données restent **sur votre ordinateur** : aucun serveur, aucune télémétrie. La seule connexion sert à vérifier les mises à jour.
- Le fichier de données est **chiffré** (SQLCipher). La clé est protégée par le trousseau du système (DPAPI sous Windows, Keychain sous macOS) et liée à votre session utilisateur.
- Les sauvegardes exportées peuvent être **protégées par un mot de passe**.
- Aucune mise à jour n'est téléchargée ni installée **sans votre accord** dans l'application.

## Périmètre

Ce dépôt ne contient que les installateurs et la documentation. Les signalements qui concernent le code source passent par le même canal.
