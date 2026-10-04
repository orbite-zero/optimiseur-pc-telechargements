# Optimiseur PC — téléchargements

Une application Windows pour centraliser le nettoyage, le stockage, les applications, les programmes au démarrage et les réglages de performances.

**Version actuelle : 1.1.0 bêta.**

## Télécharger

**[Télécharger Optimiseur PC 1.1.0 — pack ZIP](https://github.com/orbite-zero/optimiseur-pc-telechargements/releases/download/v1.1.0/OptimiseurPC-1.1.0.zip)**

Le pack contient l'application, un guide rapide et les notices de licence.

[Fichier EXE seul](https://github.com/orbite-zero/optimiseur-pc-telechargements/releases/download/v1.1.0/OptimiseurPC.exe) · [Notes de version et licences](https://github.com/orbite-zero/optimiseur-pc-telechargements/releases/tag/v1.1.0) · [Signaler un problème](https://github.com/orbite-zero/optimiseur-pc-telechargements/issues)

![Aperçu du tableau de bord avec des données fictives](apercu.png)

## Nouveautés de la version 1.1.0

- **Voir les fichiers** permet de consulter les fichiers concernés avant chaque nettoyage. Une confirmation séparée est demandée ; **Annuler** ne touche à rien.
- Les fichiers nettoyés sont mis de côté pendant **7 jours** et peuvent être restaurés avec **Maintenance > Tout annuler**.

## Développement et sécurité

Optimiseur PC est un projet indépendant publié par **orbite-zero**, développé avec l'aide de **Claude Code, l'outil de développement d'Anthropic**. Ce projet n'est ni édité ni certifié par Anthropic.

**Analyse historique de la version 1.0.0, du 4 octobre 2026 : Microsoft Defender n'a détecté aucune menace** dans les fichiers `OptimiseurPC.exe` et `OptimiseurPC-1.0.0.zip` de cette ancienne version. [Consulter le compte rendu et les empreintes des fichiers analysés](ANALYSE-ANTIVIRUS.md).

Ce résultat concerne uniquement les fichiers de la version 1.0.0 à cette date et **ne s'applique pas à la version 1.1.0**. Aucune nouvelle analyse antivirus de la version 1.1.0 n'a été effectuée dans le cadre de cette publication. Ce résultat historique ne constitue pas une certification ni une garantie d'absence de toute menace, et ne remplace pas les tests des fonctions de l'application.

La version 1.1.0 est une **bêta non signée numériquement**, testée sur peu de PC. Windows SmartScreen peut afficher un avertissement de réputation pour une application récente ou peu connue. Cet avertissement ne signifie pas, à lui seul, qu'un virus a été détecté. [En savoir plus auprès de Microsoft](https://learn.microsoft.com/fr-fr/windows/apps/package-and-deploy/smartscreen-reputation).

Télécharge l'application uniquement depuis les liens de cette page et garde les protections de Windows activées. Si ton antivirus signale une menace, n'exécute pas le fichier et [signale la détection](https://github.com/orbite-zero/optimiseur-pc-telechargements/issues), en masquant toute donnée personnelle dans les captures.

## Utilisation

1. Télécharge le pack ZIP et extrais son contenu.
2. Ouvre `OptimiseurPC.exe`. Les modifications des réglages Windows nécessitent les droits administrateur.
3. Crée le point de restauration proposé avant la première modification.

**Configuration prévue :** Windows 11 64 bits avec .NET Framework 4.8. Windows 10 n'a pas été testé.

Pour découvrir l'interface sans modifier le PC, ouvre PowerShell dans le dossier de l'application et lance :

```powershell
.\OptimiseurPC.exe --demo
```

**Maintenance > Tout annuler** restaure les réglages sauvegardés et, pendant 7 jours, les fichiers nettoyés mis de côté. **Libérer l'espace maintenant** supprime définitivement ces fichiers et rend leur restauration impossible avec ce bouton. Le vidage de la corbeille, le nettoyage des composants Windows et les désinstallations ne sont pas annulés par ce bouton.

## Vérifier le téléchargement

Les empreintes SHA-256 du pack et de l'exécutable figurent dans [SHA256SUMS.txt](SHA256SUMS.txt).

Une empreinte permet de vérifier que le fichier correspond à celui publié ; elle ne constitue pas une analyse antivirus.

```powershell
Get-FileHash .\OptimiseurPC.exe -Algorithm SHA256
```

## Licence de la version 1.1.0

La version 1.1.0 est distribuée sous [licence MIT](LICENSE). La version 1.0.0 conserve également sa licence MIT. La police Orbitron intégrée est fournie sous [licence SIL Open Font License 1.1](Orbitron-OFL.txt). Les deux notices sont incluses dans le pack ZIP et proposées avec la version téléchargeable.
