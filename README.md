<p align="center">
  <img src="docs/img/affiche.jpg" alt="Tirelire, votre argent enfin clair" width="820">
</p>

<p align="center">
  Budget, épargne et patrimoine au même endroit, sur votre ordinateur.<br>
  Application de bureau gratuite pour Windows et Mac.
</p>

<p align="center">
  <a href="https://github.com/Vitopya/tirelire-releases/releases/latest"><strong>Télécharger la dernière version</strong></a>
</p>

---

## Dernière version

<!-- release:start -->
**Version 1.6.5**, publiée le 16 octobre 2026. [Télécharger](https://github.com/Vitopya/tirelire-releases/releases/latest)

**Nouveautés**

- Sous Windows, les prochaines mises à jour se téléchargent seules et s'installent sans assistant, à la fermeture de Tirelire ou d'un clic.
- Le graphique des six derniers mois montre d'un coup d'œil ce que chaque mois a coûté, mis de côté et laissé.

**Ajustements**

- Le menu du compte ferme la barre latérale ; la version et les nouveautés s'y trouvent.
- Les sons de l'interface sont coupés par défaut. Ils se réactivent dans Mon compte > Apparence.
<!-- release:end -->

## Ce que fait Tirelire

| | |
|---|---|
| **Tableau de bord** | Le reste à vivre du mois, la répartition entre frais fixes, frais variables et épargne, le taux d'épargne, les six derniers mois en un graphique, la valeur de votre patrimoine et vos rappels. |
| **Suivi budgétaire** | Un tableau par mois : revenus, frais fixes, frais variables. Les lignes du mois précédent se reprennent en un clic ; la vue annuelle compare les douze mois. |
| **Investissements** | PEA, assurance-vie, livrets, actionnariat salarié, crypto, immobilier et prêts, supports personnalisés. Chaque support garde son historique d'opérations ; la synthèse donne la valeur nette, le rendement annualisé et une estimation après impôt. |
| **Import de relevés** | Collez le texte d'un relevé bancaire : Tirelire reconnaît les opérations, les classe et remplit le budget du mois. Vos corrections servent aux imports suivants. |
| **Rappels et alertes** | Vos échéances, avec une notification le jour venu, et des alertes automatiques : budget dépassé, relevé manquant, PEA de cinq ans, épargne salariale disponible. |
| **Sauvegardes** | Export et import complets, protégés par mot de passe si vous le souhaitez. Export CSV. |

Tout fonctionne hors ligne. Pas de compte, pas d'abonnement, pas de connexion bancaire.

## Aperçu

![Tableau de bord, thème sombre](docs/img/dashboard-dark.png)

![Tableau de bord, thème clair](docs/img/dashboard.png)

![Suivi budgétaire](docs/img/suivi-budgetaire.png)

![Investissements](docs/img/investissements.png)

![Import de données](docs/img/import-de-donnees.png)

Captures réalisées avec des données fictives.

## Télécharger et installer

Sur la page de la [dernière version](https://github.com/Vitopya/tirelire-releases/releases/latest), section **Assets**, prenez le fichier de votre ordinateur :

| Ordinateur | Fichier |
|---|---|
| Windows 10 ou 11, 64 bits | `Tirelire-Setup-X.Y.Z.exe` |
| Mac Apple Silicon (M1 et suivants) | `Tirelire-X.Y.Z-arm64.dmg` |

Les autres fichiers (`.yml`, `.blockmap`, `.zip`) servent aux mises à jour automatiques. Les Mac à processeur Intel ne sont pas pris en charge.

**Windows.** Ouvrez le fichier et suivez l'assistant. Si Windows affiche « Windows a protégé votre ordinateur », c'est parce que l'application n'a pas de certificat commercial : cliquez sur **Informations complémentaires**, puis **Exécuter quand même**.

**Mac.** Ouvrez le `.dmg` et glissez Tirelire dans **Applications**. Si macOS bloque la première ouverture : clic droit sur Tirelire, **Ouvrir**, puis confirmez. Ou **Réglages Système** > **Confidentialité et sécurité** > **Ouvrir quand même**. Ce n'est demandé qu'une fois.

## Premier lancement

1. Tirelire vous propose de protéger l'application par un mot de passe. C'est facultatif : **Continuer sans mot de passe** ouvre directement le tableau de bord, et vous pourrez en définir un plus tard dans **Mon compte** > **Sécurité**.
2. Les nouveautés de la version s'affichent, puis une courte visite présente les écrans.
3. Commencez par **Suivi budgétaire** pour saisir le mois en cours, ou par **Import de données** pour coller un relevé.

## Mises à jour

Tirelire vérifie au lancement si une nouvelle version est publiée ici.

- **Windows** : la mise à jour se télécharge seule, puis s'installe quand vous fermez l'application, ou tout de suite avec **Redémarrer maintenant**. Aucun assistant à suivre.
- **Mac** : un bandeau vous la propose. Si l'installation automatique n'aboutit pas, Tirelire ouvre cette page : téléchargez le `.dmg` et remplacez l'application.

Le détail de la version proposée se lit dans **Mon compte** > **Mises à jour**. Une mise à jour ne touche jamais à vos données.

## Vos données

**Où sont-elles ?** Sur votre ordinateur, dans un seul fichier :

| Système | Dossier |
|---|---|
| Windows | `%APPDATA%\finboard\data\` (ou `%APPDATA%\tirelire\data\` sur certaines installations) |
| Mac | `~/Library/Application Support/finboard/data/` |

**Sont-elles protégées ?** Le fichier est chiffré (SQLCipher, clé de 256 bits). La clé est créée au premier lancement et rangée dans le coffre du système (DPAPI sous Windows, Trousseau sur Mac), lié à votre session : copié sur une autre machine ou depuis un autre compte, le fichier reste illisible. Il ne protège pas une session laissée ouverte : verrouillez-la, et définissez un mot de passe dans Tirelire si l'ordinateur est partagé.

**Sauvegardes.** **Mon compte** > **Données**. Exportez de temps en temps, avec un mot de passe si le fichier quitte votre machine. C'est la seule façon de retrouver vos données après un changement d'ordinateur ou une réinstallation du système.

**Réseau.** Tirelire ne contacte qu'un serveur, cette page, pour savoir si une nouvelle version existe. Aucune donnée n'est envoyée.

## Questions fréquentes

**Tirelire se connecte-t-elle à ma banque ?**
Non, volontairement. Vous collez le texte d'un relevé, Tirelire fait le tri. Aucun identifiant bancaire n'est demandé.

**Puis-je l'utiliser sur deux ordinateurs ?**
Oui : export sur le premier, import sur le second. Il n'y a pas de synchronisation automatique.

**J'ai oublié mon mot de passe.**
Sur l'écran de connexion, **Mot de passe oublié ?** le réinitialise. Vos données sont conservées.

**Windows dit que l'application est dangereuse.**
C'est l'avertissement affiché pour les applications sans certificat commercial. Vérifiez que le fichier vient bien de cette page, puis **Informations complémentaires** > **Exécuter quand même**.

**L'application ne s'ouvre pas.**
Fermez toute fenêtre Tirelire déjà ouverte et relancez. Sous Windows, le journal `finboard-electron.log`, dans le dossier `%APPDATA%\finboard\` (ou `tirelire`), aide à comprendre : joignez-le à votre signalement.

**J'ai une version 3.x.**
La numérotation est repartie de 1.0.0 le 4 septembre 2026. Une version 3.x ne voit pas les nouvelles versions : téléchargez l'installateur ici et installez-le par-dessus, vos données sont conservées.

**Comment désinstaller ?**
Windows : **Paramètres** > **Applications** > Tirelire > **Désinstaller**. Mac : glissez Tirelire dans la corbeille. Le fichier de données reste en place ; supprimez son dossier pour tout effacer.

## Signaler un problème

- Bug ou suggestion : ouvrez une [issue](https://github.com/Vitopya/tirelire-releases/issues), avec votre système et la version de Tirelire (menu du compte, en bas de la barre latérale, ligne **Nouveautés**).
- Faille de sécurité : voir [SECURITY.md](SECURITY.md), sans détail en public.

## Conditions

Tirelire est une création de Joseph Deffayet, gratuite pour un usage personnel. Le logiciel, son interface et ses textes restent sa propriété : copie, redistribution, modification et usage commercial sont interdits sans accord écrit. Le code source n'est pas publié. Conditions complètes dans [LICENSE](LICENSE).

## English

Tirelire is a free personal finance desktop app for Windows and Apple Silicon Macs: monthly budget, investments, bank statement import. Everything stays on your computer in an encrypted file; no account, no cloud, no bank connection. This repository hosts the installers and the user guide only. Download the [latest version](https://github.com/Vitopya/tirelire-releases/releases/latest). Copyright Joseph Deffayet, all rights reserved, see [LICENSE](LICENSE).
