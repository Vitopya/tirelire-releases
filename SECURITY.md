# Signalement d'un probleme de securite

Si vous pensez avoir identifie une **vulnerabilite** dans l'application Tirelire, ses installateurs ou son mecanisme de mise a jour, merci de **ne pas** ouvrir une issue publique avec les details.

## Comment signaler

1. Si l'onglet **Security** de ce depot propose **Report a vulnerability** (signalement prive), utilisez ce formulaire.
2. Sinon, contactez **Joseph Deffayet** par un **canal prive** (e-mail ou autre moyen qu'il vous aura communique).

Indiquez :

- une description claire du probleme et de son impact ;
- les etapes de reproduction si possible ;
- la version concernee (visible dans **Mon compte** > **Mises a jour**, ou dans le nom du fichier installateur).

## Ce que fait Tirelire pour vos donnees

- Les donnees restent **sur votre machine** : aucun serveur, aucune telemetrie, aucun appel reseau hors verification des mises a jour.
- Le fichier de donnees est **chiffre au repos** (SQLCipher). La cle est protegee par le trousseau du systeme (DPAPI sous Windows, Keychain sous macOS) et liee a votre session utilisateur.
- Les sauvegardes exportees peuvent etre **protegees par un mot de passe**.
- Aucune mise a jour n'est telechargee ni installee **sans votre accord** explicite dans l'application.

## Perimetre

Ce depot ne contient que des binaires et de la documentation. Les signalements concernant le code source sont traites par le meme canal.
