# Répertoire national des opérations standardisées d'économies d'énergie

Base de données des opérations valorisables au titre du dispositif des Certificats d'Economies d'Energies.

## Définition des termes

**Fiche** : Fiche d'opération standardisée telle que définie par l'arrêté du 22 décembre 2014 définissant les opérations standardisées d'économies d'énergie.

**Bonus** : Bonification des opérations d'économies d'énergie hors charte d'engagement telle que définie par les articles 3-4 à 6-1 de l'arrêté du 29 décembre 2014 relatif aux modalités d'application du dispositif des certificats d'économies d'énergie.

**Bonification** : Bonification des opérations d'économies d'énergie relevant d'une charte d'engagement telle que définie par les articles 3-4 à 6-1 de l'arrêté du 29 décembre 2014 relatif aux modalités d'application du dispositif des certificats d'économies d'énergie.

## Description des fichiers

| repertoire_fiche.csv | Répertoire des fiches d'opération standardisée |
| repertoire_bonification.csv | Répertoire des bonifications |
| repertoire_bonus.csv | Répertoire des bonus |
| rapprochement_fiche_bonification.csv | Rapprochement des fiches d'opération standardisées et des bonifications |

### Répertoire des fiches d'opération standardisées

| Propriété | Type | Description |
|:---------:|:----:|:-----------:|
| **id** | string | Identifiant unique de la fiche d'opération standardisée au format code + version |
| **code** | string | Code de la fiche d'opération standardisée |
| **code_secteur** | string | Code du secteur d'application |
| **secteur** | string | Secteur d'application |
| **code_sous_secteur** | string | Code du sous secteur d'application |
| **sous_secteur** | string | Sous secteur d'application |
| **nom** | string | Nom de la fiche d'opération standardisée |
| **version** | string | Code de la version de l'arrêté applicable |
| **date_debut** | date | Date d'application de la version de la fiche d'opération standardisée |
| **date_fin** | date | Date de fin d'application de la version de la fiche d'opération standardisée |
| **metropole** | boolean | Application de la fiche d'opération standardisée en France métropolitaine |
| **outre_mer** | boolean | Application de la fiche d'opération standardisée en France d'outre-mer |

### Répertoire des bonifications

| Propriété | Type | Description |
|:---------:|:----:|:-----------:|
| **id** | string | Identifiant unique de la bonification au format code + version |
| **code** | string | Code de la bonification |
| **code_nature** | string | Code de la bonification au format de l'annexe 6 de l'arrêté du 4 septembre 2014 |
| **nom** | string | Nom de la bonification |
| **version** | string | Code de la version de l'arrêté applicable |
| **date_debut** | date | Date d'application de la version de la boninification |
| **date_fin** | date | Date de fin d'application de la version de la boninification |

### Répertoire des bonus

| Propriété | Type | Description |
|:---------:|:----:|:-----------:|
| **id** | string | Identifiant unique du bonus au format code + version |
| **code** | string | Code du bonus |
| **code_nature** | string | Code du bonus au format de l'annexe 6 de l'arrêté du 4 septembre 2014 |
| **nom** | string | Nom du bonus |
| **version** | string | Code de la version de l'arrêté applicable |
| **date_debut** | date | Date d'application de la version du bonus |
| **date_fin** | date | Date de fin d'application de la version du bonus |

### Rapprochement Fiche - Bonification

| Propriété | Type | Description |
|:---------:|:----:|:-----------:|
| **code_fiche** | string | Code de la fiche d'opération standardisée |
| **nom_fiche** | string | Nom de la fiche d'opération standardisée |
| **code_bonification** | string | Code de la bonification |
| **nom_bonification** | string | Nom de la bonification |

## Références réglementaires

- [Arrêté du 29 décembre 2014 relatif aux modalités d'application du dispositif des certificats d'économies d'énergie](https://www.legifrance.gouv.fr/loda/id/JORFTEXT000030001603/)
- [Arrêté du 22 décembre 2014 définissant les opérations standardisées d'économies d'énergie](https://www.legifrance.gouv.fr/loda/id/JORFTEXT000029953752/)
- [Arrêté du 4 septembre 2014 fixant la liste des éléments d'une demande de certificats d'économies d'énergie et les documents à archiver par le demandeur](https://www.legifrance.gouv.fr/loda/id/JORFTEXT000029460644/)
