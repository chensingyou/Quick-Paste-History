# Politique de Confidentialité de Quick Paste History

**Dernière mise à jour : 8 mai 2026**

---

## 1. Collecte et Utilisation des Informations

Quick Paste History est un outil de gestion du presse-papiers dont la fonction principale est d'enregistrer, gérer et retrouver le contenu du presse-papiers localement sur votre appareil.

### 1.1 Informations que nous **ne collectons pas**

- Informations d'identification personnelle (nom, numéro de carte d'identité, adresse, etc.)
- Informations sensibles telles que mots de passe de compte, numéros de carte bancaire, etc.
- Identifiants d'appareil (IDFV, IDFA, etc.)
- Historique de navigation, informations de localisation
- Contacts, album photo, microphone, données de la caméra
- Statistiques de comportement d'utilisation ou données d'analyse

### 1.2 Informations auxquelles nous **accédons**

Quick Paste History accède uniquement aux informations suivantes localement sur votre appareil, nécessaires à ses fonctions essentielles :

| Type de données | Objectif | Téléversement sur serveur |
|-----------------|----------|:------------------------:|
| **Contenu du presse-papiers** | Enregistre le texte/les liens copiés par l'utilisateur, prend en charge la recherche, les favoris et le remplissage rapide | Stockage local uniquement |
| **iCloud** | Synchronise l'historique entre vos appareils via NSUbiquitousKeyValueStore | Synchronisation iCloud privée uniquement |
| **Achat intégré App Store** | Vérifie le statut d'achat des fonctionnalités Pro (vérification du reçu uniquement) | Aucun détail d'achat collecté |

> Tout le traitement des données du presse-papiers est effectué localement sur l'appareil et **ne sera pas téléversé vers un serveur externe**.

---

## 2. Stockage des Données

### 2.1 Stockage Local

- Les historiques du presse-papiers sont stockés dans une base de données SwiftData dans le bac à sable de l'application
- La base de données n'est pas chiffrée (le mécanisme de bac à sable d'Apple assure une isolation au niveau système)
- Les utilisateurs peuvent effacer manuellement tout l'historique

### 2.2 Synchronisation iCloud (Fonctionnalité Optionnelle)

- Une fois activée, l'historique est synchronisé via `NSUbiquitousKeyValueStore` sur votre propre compte iCloud
- Les données sont protégées par les mécanismes de sécurité d'iCloud et ne sont pas accessibles au développeur
- La synchronisation peut être désactivée à tout moment dans les paramètres
- La désactivation de la synchronisation ne supprime pas les données locales

### 2.3 Conservation des Données

- L'historique est conservé par défaut ; les utilisateurs peuvent supprimer manuellement des entrées individuelles ou tout effacer
- La suppression prend effet immédiatement et est irréversible

---

## 3. Partage des Données

Quick Paste History **ne partage pas les données des utilisateurs avec des tiers**, y compris, mais sans s'y limiter :

- Ne vend pas les données des utilisateurs
- N'utilise pas les données pour la publicité ou le profilage des utilisateurs
- N'envoie aucun contenu du presse-papiers à des API tierces
- N'intègre aucun SDK d'analyse tiers

---

## 4. Extension de Clavier et Autorisations

Quick Paste History fournit une extension de clavier (Keyboard Extension) pour coller rapidement du contenu historique dans n'importe quelle application :

- **Accès** : L'extension de clavier ne s'exécute que lorsqu'elle est activée et ne lit que le contenu du presse-papiers
- **Réseau** : L'extension de clavier n'a pas d'autorisation d'accès réseau
- **Isolation des données** : L'extension de clavier partage les données du bac à sable avec l'application principale mais ne les expose pas à l'extérieur

---

## 5. Lecture du Presse-papiers

Quick Paste History lit le presse-papiers dans les cas suivants :
- Lorsque l'application est active au premier plan, elle détecte les changements du presse-papiers et enregistre le nouveau contenu
- Lorsque l'utilisateur partage activement du contenu vers Quick Paste History

Conformément aux exigences d'iOS, la première lecture du presse-papiers déclenchera une fenêtre d'autorisation au niveau système. Les utilisateurs peuvent gérer cette autorisation à tout moment dans les Réglages Système.

---

## 6. Confidentialité des Enfants

Quick Paste History ne collecte pas d'informations personnelles auprès des enfants.

---

## 7. Modifications de la Politique de Confidentialité

Si la politique de confidentialité change, nous mettrons à jour la date de « Dernière mise à jour » en haut de la page et informerons les utilisateurs via des annonces dans l'application ou des notes de mise à jour.

---

## 8. Nous Contacter

Si vous avez des questions concernant la politique de confidentialité, veuillez nous contacter via les canaux suivants :

- **Développeur** : 陈修
- **E-mail** : chensingyou@126.com
- **App** : Quick Paste History (Développeur : Singyou)

---

> **Résumé : Vos données vous appartiennent.** Quick Paste History ne téléverse aucun contenu sur des serveurs, ne suit pas le comportement des utilisateurs et n'intègre aucun SDK tiers. Toutes les données du presse-papiers sont traitées uniquement localement sur l'appareil et dans l'espace privé iCloud.
