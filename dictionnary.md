# DICTIONNAIRE DES VARIABLES UTILISES

## A. Dictionnaire des variables

| Variable | Type | Description | Valeurs | Source |
|----------|------|-------------|---------|--------|
| DR_NO | Int | Numéro de rapport unique | Unique | LAPD |
| Date Rptd | Date | Date de signalement | JJ/MM/AAAA | LAPD |
| Date Occ | Date | Date d'occurrence | JJ/MM/AAAA | LAPD |
| Time Occ | Int | Heure d'occurrence | 0-2359 | LAPD |
| Area | Int | Code zone police | 1-21 | LAPD |
| Area Name | String | Nom zone police | Central, etc. | LAPD |
| Crm Cd | Int | Code crime | 110-956 | LAPD |
| Crm Cd Desc | String | Description crime | Vol, etc. | LAPD |
| Vict Age | Int | Âge victime | 0-120 | LAPD |
| Vict Sex | Char | Sexe victime | M/F/X | LAPD |
| Vict Descent | Char | Origine victime | H/W/B/etc. | LAPD |
| Premis Cd | Int | Code lieu | 101-972 | LAPD |
| Premis Desc | String | Description lieu | Rue, résidence | LAPD |
| Weapon Used Cd | Int | Code arme | 100-516 | LAPD |
| Weapon Desc | String | Description arme | Pistolet, etc. | LAPD |
| Status | String | Statut investigation | IC/AA/etc. | LAPD |
| Location | String | Adresse approximative | Coordonnées | LAPD |
| Cross Street | String | Intersection | Nom rue | LAPD |
| LAT | Float | Latitude | Degrés | LAPD |
| LON | Float | Longitude | Degrés | LAPD |

## B. Codes crimes principaux

| Code | Description | Catégorie |
|------|-------------|-----------|
| 510 | Vol de véhicules | Propriété |
| 624 | Violence physique légère | Personne |
| 330 | Cambriolage véhicule | Propriété |
| 354 | Usurpation d'identité | Fraude |
| 740 | Vandalisme | Propriété |