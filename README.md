# Optimiseur PC — téléchargements

Une application Windows pour centraliser le nettoyage, le stockage, les applications, les programmes au démarrage et les réglages de performances.

**Version actuelle : 1.1.0 bêta.**

## Télécharger

**[Télécharger Optimiseur PC 1.1.0 — pack ZIP](https://github.com/orbite-zero/optimiseur-pc-telechargements/releases/download/v1.1.0/OptimiseurPC-1.1.0.zip)**

Le pack contient l'application, un guide rapide et les notices de licence.

[Fichier EXE seul](https://github.com/orbite-zero/optimiseur-pc-telechargements/releases/download/v1.1.0/OptimiseurPC.exe) · [Notes de version et licences](https://github.com/orbite-zero/optimiseur-pc-telechargements/releases/tag/v1.1.0) · [Signaler un problème](https://github.com/orbite-zero/optimiseur-pc-telechargements/issues)

![Aperçu du tableau de bord avec des données fictives](apercu.png)

## Développement et sécurité

Optimiseur PC est un projet indépendant publié par **orbite-zero**, développé avec l'aide de **Claude Code, l'outil de développement d'Anthropic**. Ce projet n'est ni édité ni certifié par Anthropic.

**Analyse du 4 octobre 2026 de la version 1.0.0 : Microsoft Defender n'a détecté aucune menace** dans `OptimiseurPC.exe` et `OptimiseurPC-1.0.0.zip`. La version 1.1.0 n'a pas encore été analysée de la même façon. [Consulter le compte rendu et les empreintes des fichiers analysés](ANALYSE-ANTIVIRUS.md).

Ce résultat concerne ces fichiers à cette date. Il ne constitue pas une certification ni une garantie d'absence de toute menace, et ne remplace pas les tests des fonctions de l'application.

La version 1.1.0 est une **bêta non signée numériquement**. Windows SmartScreen peut afficher un avertissement de réputation pour une application récente ou peu connue. Cet avertissement ne signifie pas, à lui seul, qu'un virus a été détecté. [En savoir plus auprès de Microsoft](https://learn.microsoft.com/fr-fr/windows/apps/package-and-deploy/smartscreen-reputation).

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

Avant chaque nettoyage, **Voir les fichiers** montre ce qui sera supprimé, puis une confirmation séparée est demandée. Choisir « Annuler » ne modifie rien.

**Maintenance > Tout annuler** restaure les réglages sauvegardés et, pendant 7 jours, les fichiers nettoyés : ils sont mis de côté au lieu d'être effacés. **Libérer l'espace maintenant** les supprime définitivement. Le vidage de la corbeille, le nettoyage des composants Windows et les désinstallations ne sont pas annulés par ce bouton.

## Vérifier le téléchargement

Les empreintes SHA-256 du pack et de l'exécutable figurent dans [SHA256SUMS.txt](SHA256SUMS.txt).

Une empreinte permet de vérifier que le fichier correspond à celui publié ; elle ne constitue pas une analyse antivirus.

```powershell
Get-FileHash .\OptimiseurPC.exe -Algorithm SHA256
```

## Licence

Les versions 1.0.0 et 1.1.0 sont publiées sous [licence MIT](LICENSE). La police Orbitron intégrée est fournie sous [licence SIL Open Font License 1.1](Orbitron-OFL.txt). Les deux notices sont incluses dans le pack ZIP et proposées avec la version téléchargeable.
