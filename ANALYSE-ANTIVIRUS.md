# Analyse antivirus — Optimiseur PC 1.0.0

**Résultat : aucune menace détectée par Microsoft Defender Antivirus le 4 octobre 2026 à 12 h 31 (Europe/Paris, UTC+02:00).**

Il s'agit d'un compte rendu publié par le projet, pas d'une certification délivrée par Microsoft ou Anthropic.

## Fichiers analysés

Les deux fichiers ont été téléchargés depuis la [version publique v1.0.0](https://github.com/orbite-zero/optimiseur-pc-telechargements/releases/tag/v1.0.0), sans connexion à un compte GitHub. Leurs empreintes ont été vérifiées avant et après l'analyse ; elles sont inchangées et correspondent aux fichiers de la version publiée.

| Fichier | Taille | Résultat |
| --- | ---: | --- |
| `OptimiseurPC.exe` | 513 536 octets | Aucune menace détectée |
| `OptimiseurPC-1.0.0.zip` | 244 856 octets | Aucune menace détectée |

Empreintes SHA-256 :

```text
25d85a1bcd89d564c68811395aff107e4686fbb8ca31ec90821fe76437b8bde6  OptimiseurPC.exe
49545f830f49d30527a2dbc4a36dc1cd09ebe1f7d95fe082084d182dbf5a90e7  OptimiseurPC-1.0.0.zip
```

## Méthode et résultats

- Antivirus : Microsoft Defender Antivirus, version `4.18.26080.4`.
- Moteur : `1.1.26080.3`.
- Renseignements de sécurité : `1.459.546.0`, mis à jour le 4 octobre 2026 à 04 h 08 (Europe/Paris), même version avant et après l'analyse.
- Analyse personnalisée de chaque fichier avec `MpCmdRun`, options `-Scan -ScanType 3 -File <fichier> -DisableRemediation`.
- Les protections de Windows sont restées activées. L'option `-DisableRemediation` empêche uniquement les corrections automatiques de cette analyse ; elle permet l'analyse des archives et ignore les exclusions de fichiers. [Documentation Microsoft](https://learn.microsoft.com/fr-fr/defender-endpoint/command-line-arguments-microsoft-defender-antivirus).
- Les deux analyses se sont terminées avec le code de retour `0` et un message explicite indiquant l'absence de menace détectée.

Extraits de sortie, avec les chemins locaux remplacés par les noms des fichiers :

```text
Scan starting...
Scan finished.
Scanning OptimiseurPC.exe found no threats.

Scan starting...
Scan finished.
Scanning OptimiseurPC-1.0.0.zip found no threats.
```

## Portée de ce résultat

Cette analyse concerne uniquement les fichiers et les renseignements de sécurité indiqués ci-dessus, à cette date. Elle ne garantit pas l'absence de toute menace et ne constitue pas un audit indépendant du code ou un test des modifications apportées à Windows. L'application reste une bêta non signée numériquement.

Une empreinte SHA-256 vérifie l'identité d'un fichier ; elle ne prouve pas sa sécurité. Garde ton antivirus activé. Si une menace est signalée, n'exécute pas le fichier et [signale le problème](https://github.com/orbite-zero/optimiseur-pc-telechargements/issues) sans publier de données personnelles.
