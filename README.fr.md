> [!NOTE]
> Nous utilisons GitHub pour suivre les bugs, discuter des demandes de fonctionnalités et publier les exécutables.
> SafeFanControl **n'est pas** un logiciel open source.

<div align="center">

[English](README.md) | [简体中文](README.zh-Hans.md) | [繁體中文](README.zh-Hant.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Español](README.es.md) | **Français** | [Русский](README.ru.md)

</div>

---

# SafeFanControl

**Prenez le contrôle des ventilateurs de votre Mac**

SafeFanControl est une **app macOS native** qui vous permet de surveiller les températures et de gérer la vitesse des ventilateurs sur les Mac Apple Silicon et Intel. Téléchargement gratuit — vos ventilateurs, vos règles, et le système reprend toujours la main si quelque chose tourne mal.

[Télécharger pour macOS](https://github.com/SafeFanControl/SafeFanControl/releases)

---

## Fonctionnalités

### Tous les modes de contrôle des ventilateurs dont vous pourriez avoir besoin

SafeFanControl vous donne un contrôle total sur la façon dont votre Mac réagit à la chaleur, avec trois modes de fonctionnement distincts adaptés à votre flux de travail.

- **Monitor** — lisez les températures et les vitesses des ventilateurs en temps réel sans toucher au contrôle système
- **Safe Max** — passe automatiquement à la vitesse maximale lorsqu'un seuil de température est atteint, puis rend le contrôle à macOS une fois la chaleur dissipée
- **Curve** — définissez votre propre courbe température/vitesse pour un contrôle continu et proportionnel
- Changez de mode instantanément depuis la barre des menus, sans ouvrir aucune fenêtre

### Conçu avant tout pour la sécurité

Une architecture à trois processus garantit qu'en cas de problème, macOS reprend toujours automatiquement le contrôle des ventilateurs, sans aucune intervention manuelle.

- Un **processus de surveillance (watchdog)** surveille l'assistant en arrière-plan ; s'il plante alors que les ventilateurs sont en mode manuel, macOS reprend la main instantanément
- Les **transitions en fondu douces** évitent les sauts brusques de vitesse qui pourraient être audibles ou gênants
- Le **verrouillage par seuil** maintient Safe Max stable lors de brèves fluctuations de température
- La fenêtre d'authentification administrateur standard de macOS installe l'assistant en arrière-plan — sans Terminal, sans étapes manuelles

### Toujours dans la barre des menus

Une app légère dans la barre des menus met les données des capteurs en direct et le changement de mode à portée de clic — toujours visible, jamais encombrante.

- Températures CPU et GPU mises à jour en temps réel
- Vitesse actuelle du ventilateur et mode de contrôle actif toujours visibles
- Basculez entre Monitor, Safe Max et Curve directement depuis le menu déroulant
- Compatible avec Apple Silicon M1 à M5 et les Mac Intel équipés d'une puce T2 ; disponible en 8 langues

---

## Tarif

SafeFanControl suit un modèle de **téléchargement gratuit, achat unique**. Pas d'abonnement. Pas de frais récurrents. Payez une fois, c'est à vous pour toujours.

| | Gratuit | Licence complète |
|---|---|---|
| **Prix** | $0 — pour toujours | $8.99 — paiement unique |
| Mode Monitor (lecture seule) | ✅ | ✅ |
| Affichage de la température en direct | ✅ | ✅ |
| Affichage de la vitesse des ventilateurs | ✅ | ✅ |
| Capteurs CPU, GPU, SoC | ✅ | ✅ |
| Prise en charge par génération M1–M5 | ✅ | ✅ |
| **Mode Safe Max** | ❌ | ✅ |
| **Mode Curve** | ❌ | ✅ |
| Transitions en fondu douces | ❌ | ✅ |
| Logique de verrouillage / anti-rebond | ❌ | ✅ |
| Safe Max multi-règles | ❌ | ✅ |
| **Assistant de test des ventilateurs** | ❌ | ✅ |
| Page de débogage et de diagnostic | ❌ | ✅ |

---

## Téléchargement et installation

### Configuration requise

| Exigence | Détails |
|---|---|
| **macOS** | 15 (Sequoia) ou ultérieur |
| **Matériel Mac** | Apple Silicon (M1, M2, M3, M4, M5) ou Mac Intel avec puce T2 |
| **Autorisations** | Une demande de mot de passe administrateur pour installer le démon assistant en arrière-plan |
| **Espace disque** | ~5 Mo |

### Installation

1. **Ouvrez le `.dmg` téléchargé** et faites glisser SafeFanControl dans votre dossier Applications.
2. **Lancez l'app.** Au premier lancement, une fenêtre d'administrateur installe l'assistant en arrière-plan et le démon de surveillance.
3. **C'est fait.** Pas de Terminal. Pas d'approbations manuelles. L'Assistant de test des ventilateurs vous guidera pour confirmer que tout fonctionne sur votre matériel.

> macOS peut afficher une alerte Gatekeeper au premier lancement, car l'app n'est pas distribuée via l'App Store. Faites un **clic droit → Ouvrir** pour continuer.

### Désinstallation

SafeFanControl inclut une procédure de désinstallation complète dans **Réglages → Désinstaller**. Elle supprime le démon assistant, le démon de surveillance et tous les fichiers associés en une seule étape.

---

## FAQ

**Existe-t-il un essai gratuit des fonctionnalités complètes ?**
Oui — les modes Safe Max et Curve sont déverrouillés pour un **essai de 14 jours** dès le premier lancement. Aucun paiement requis.

**Que couvre la licence ?**
Une licence couvre tous vos Mac **personnels**. Elle n'est pas destinée à la redistribution ni à un usage commercial sur un parc de machines.

**Dois-je racheter après une mise à niveau de macOS ?**
Non. Votre licence est permanente.

**Dois-je racheter si je change de Mac ?**
Non — votre licence vous appartient. Utilisez votre clé de licence existante pour enregistrer votre nouveau Mac.

**Quelle est votre politique de remboursement ?**
Comme nous respectons votre vie privée, l'app utilise un système d'enregistrement hors ligne. Une fois émise, une clé de licence ne peut pas être désactivée à distance — par conséquent, toutes les ventes sont définitives et aucun remboursement standard ne peut être accordé. Nous vous encourageons vivement à utiliser l'essai de 14 jours avant d'acheter. Exception : si une mise à jour de macOS d'Apple désactive de façon permanente les méthodes de contrôle des ventilateurs sous-jacentes, nous rembourserons intégralement les licences achetées au cours des 30 derniers jours.

**Pourquoi l'app n'est-elle pas sur le Mac App Store ?**
SafeFanControl installe un démon assistant privilégié en arrière-plan, ce qui est incompatible avec les règles strictes de bac à sable (sandbox) de l'App Store. La distribution est directe — mais le programme d'installation est analysé, notarisé et signé via le système de signature d'Apple.

**Puis-je l'utiliser sans payer ?**
Oui — le mode Monitor est entièrement gratuit et le restera toujours.

**Que se passe-t-il si le serveur de licences est mis hors ligne à l'avenir ?**
La clé de licence fonctionne hors ligne et ne nécessite aucune vérification par Internet. Vous pouvez vous enregistrer à tout moment, tant que vous disposez de votre clé de licence.

**Que se passe-t-il si vous abandonnez ce projet ?**
Tout produit a une durée de vie. Cependant, tant que je peux coder et que les revenus du produit couvrent ses frais de base (comme la cotisation annuelle au Apple Developer Program), je continuerai à le maintenir. Si vous aimez ce produit, partagez-le avec vos amis. Si (et seulement si) le jour vient où je dois abandonner ce projet, je partagerai le code source avec tous les utilisateurs payants sous licence AGPL v3.

**Que faire si je perds ma clé de licence ?**
Veuillez contacter la plateforme de vente ou nous écrire directement.

---

## Confidentialité

SafeFanControl ne collecte **aucune** donnée de télémétrie, d'analyse ou de rapport de plantage. Les données de votre matériel restent sur votre appareil.
