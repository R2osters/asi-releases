# Asi

Le logiciel de gestion de votre commerce. Vos ventes, votre stock, vos clients et vos comptes, sur votre ordinateur, sans connexion Internet au quotidien.

**[Télécharger la dernière version](../../releases/latest)**

---

## Quelle version choisir

| Votre ordinateur | Le fichier à prendre |
| --- | --- |
| **Windows** 10 ou 11 | celui qui finit par **`.exe`** |
| **Mac** à puce Apple (M1, M2, M3, M4 ou plus récente) | celui qui finit par **`arm64.dmg`** |
| **Mac** à processeur Intel | celui qui finit par **`x64.dmg`** |

### Vous ne savez pas quel Mac vous avez

Menu Pomme, en haut à gauche de l'écran, puis « À propos de ce Mac ». Si vous lisez le mot **puce** suivi de M1, M2, M3 ou M4, prenez le fichier `arm64`. Si vous lisez **processeur Intel**, prenez le fichier `x64`.

---

## Installer sur Windows

1. Lancez le fichier `.exe` que vous venez de télécharger.

2. Windows affichera un avertissement bleu : « Windows a protégé votre PC ». C'est attendu, et votre ordinateur n'a rien détecté d'anormal. Windows prévient simplement qu'il ne connaît pas l'éditeur du programme.

   Cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**.

3. L'installation vous laisse choisir le dossier, et ne demande pas les droits administrateur de la machine.

---

## Installer sur Mac

1. Ouvrez le fichier `.dmg` téléchargé, puis faites glisser **Asi** dans le dossier **Applications**.

2. Au premier lancement, macOS refusera d'ouvrir Asi. Il dira que l'application est endommagée, ou qu'elle provient d'un développeur non identifié.

   **Ce n'est pas une erreur, et votre Mac n'a rien détecté d'anormal.** macOS refuse par défaut toute application dont l'éditeur n'a pas payé de certificat auprès d'Apple. C'est notre cas aujourd'hui, et nous préférons vous le dire ici plutôt que vous laisser le découvrir.

3. Pour autoriser Asi, une seule fois :

   - ouvrez l'application **Terminal** (dossier Applications, puis Utilitaires) ;
   - copiez la ligne ci-dessous, collez-la dans la fenêtre, appuyez sur Entrée :

     ```
     xattr -dr com.apple.quarantine /Applications/Asi.app
     ```

   - ouvrez Asi normalement.

   Vous n'aurez à le faire qu'une seule fois. Ensuite, un double-clic suffit.

Un « Lisez-moi » reprenant ces étapes se trouve aussi dans le fichier `.dmg`, à côté de l'application.

---

## Où vont vos données

Asi écrit dans un dossier de votre compte, jamais dans le dossier du programme.

| | |
| --- | --- |
| Windows | `%APPDATA%\Asi` |
| Mac | `~/Bibliothèque/Application Support/Asi` |

Désinstaller le logiciel ne supprime donc pas votre travail, et une mise à jour ne l'écrase pas.

Pensez à régler la sauvegarde dès le premier jour. C'est le seul réglage à ne pas remettre à plus tard : Asi peut fabriquer une copie de vos données à intervalle régulier, gardez-en une sur une clé USB.

---

## Les mises à jour

**Sur Windows**, elles arrivent d'elles-mêmes. Asi télécharge la nouvelle version en arrière-plan et ne l'installe jamais pendant que vous travaillez : un bandeau vous propose de le faire quand cela vous arrange.

**Sur Mac**, Asi vous prévient qu'une version existe et vous revenez ici la télécharger. C'est la contrepartie du certificat Apple que nous ne payons pas encore.

Dans les deux cas, vos données ne bougent pas d'une version à l'autre.

---

## Ce dépôt

Vous êtes sur le dépôt des installateurs publics. Le code source d'Asi est privé.
