# Générateur d'identifiants utilisateurs

## Description
Ce script permet de générer automatiquement des identifiants utilisateurs basés sur un prénom et un nom à partir d'un fichier de noms.
Il propose plusieurs modes de génération avec différents niveaux de complexité.

## Fonctionnalités
- **Mode 1** : Génère des identifiants simples (ex: `jsmith`)
- **Mode 2** : Génère des variantes avec des séparateurs et inversions (ex: `john.smith`, `smithj`)
- **Mode 3** : Génère une liste exhaustive avec des numéros de 1 à 100 pour une wordlist massive (ex: `johnsmith1`, `jsmith99`)

## Prérequis
- **Python 3**

## Installation
Aucune installation nécessaire, il suffit d'avoir **Python 3** installé sur votre système.

## Utilisation
Exécutez le script avec les options suivantes :
```bash
python3 username_generator.py --mode <niveau> --userlist <fichier_entrée> --output <fichier_sortie>
```

### Arguments
- `--mode` : Niveau de génération des identifiants (1, 2 ou 3)
- `--userlist` : Fichier contenant une liste de noms (un par ligne, format "Prénom Nom")
- `--output` : Fichier où seront enregistrés les identifiants générés

### Exemples d'utilisation
- Générer une wordlist basique :
  ```bash
  python3 username_generator.py --mode 1 --userlist noms.txt --output wordlist.txt
  ```
- Générer une wordlist plus complexe avec séparateurs :
  ```bash
  python3 username_generator.py --mode 2 --userlist noms.txt --output wordlist.txt
  ```
- Générer une wordlist exhaustive avec numéros :
  ```bash
  python3 username_generator.py --mode 3 --userlist noms.txt --output wordlist.txt
  ```

## Résultats
Le fichier de sortie contiendra une liste d'identifiants générés pour chaque utilisateur du fichier d'entrée.

## Auteur
Développé par **Elliot Belt** - GitBook : [https://felix-billieres.gitbook.io/v2](https://felix-billieres.gitbook.io/v2)
