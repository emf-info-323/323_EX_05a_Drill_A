<h1><code>Module 323</code> - Programmer de manière fonctionnelle</h1>

# 😅 Exercice 05 - Entraînement à map().filter().reduce()

## Objectifs

- S'entraîner à l'utilisation de ces méthodes incontournables de programmation fonctionnelle que sont `map()`, `filter()` et `reduce()` et autres.

## Rapports à produire

Les rapports à produire :

**Entraînement à `filter()`**

- [F1 - Les villes du canton de Fribourg (FR)](#f1---les-villes-du-canton-de-fribourg-fr)
- [F2 - Les évaluations de Maths avec une note 6.0](#f2---les-évaluations-de-maths-avec-une-note-60)
- [F3 - Les villes ayant de 500 à 1000 habitants](#f3---les-villes-ayant-de-500-à-1000-habitants)

**Entraînement à `map()`**

- [M1 - La liste des marques de moto](#m1---la-liste-des-marques-de-moto)
- [M2 - La liste des Prénom NOM des évalutions (avec doublons)](#m2---la-liste-des-prénom-nom-des-évalutions-avec-doublons)
- [M3 - Toutes les villes et cantons (sans les habitants)](#m3---toutes-les-villes-et-cantons-sans-les-habitants)

**Entraînement à `reduce()`**

- [R1 - La plus petite date d'évaluation](#r1---la-plus-petite-date-dévaluation)
- [R2 - Pour chaque branche, le nombre d'évaluations réalisées](#r2---pour-chaque-branche-le-nombre-dévaluations-réalisées)
- [R3 - Pour chaque branche, le nombre de notes, leur moyenne à 2 décimales, la min et max](#r3---pour-chaque-branche-le-nombre-de-notes-leur-moyenne-à-2-décimales-la-min-et-max)

**Entraînement au chaînage**

- [C1 - La liste des MARQUE / Modèle de motos](#c1---la-liste-des-marque--modèle-de-motos)
- [C2 - La liste des "NOM Prénom" des évalutions (sans doublons et triée)](#c2---la-liste-des-nom-prénom-des-évalutions-sans-doublons-et-triée)
- [C3 - Le prix moyen des motos de chaque marque](#c3---le-prix-moyen-des-motos-de-chaque-marque)
- [C4 - Pour chaque marque, la plus chère et la moins chère des motos](#c4---pour-chaque-marque-la-plus-chère-et-la-moins-chère-des-motos)
- [C5 - Pour CLAIRE Voyante, les branches et ses moyennes](#c5---pour-claire-voyante-les-branches-et-ses-moyennes)
- [C6 - { canton: population }, triée](#c6----canton-population--triée)
- [C7 - \[ { canton, population } \], triée](#c7-----canton-population---triée)
- [C8 - \[ \[ canton, population \] \], triée](#c8-----canton-population---triée)

### F1 - Les villes du canton de Fribourg (FR)

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   {
      "ville": "Fribourg",
      "canton": "FR",
      "habitants": 39000
   },
   {
      "ville": "Bulle",
      "canton": "FR",
      "habitants": 24400
   },
   {
      "ville": "Villars-sur-Glâne",
      "canton": "FR",
      "habitants": 12500
   },
   {
      "ville": "Riaz",
      "canton": "FR",
      "habitants": 2500
   },
   {
      "ville": "Lessoc",
      "canton": "FR",
      "habitants": 150
   },
   {
      "ville": "Lully",
      "canton": "FR",
      "habitants": 900
   },
   {
      "ville": "Villars",
      "canton": "FR",
      "habitants": 450
   }
]
```

### F2 - Les évaluations de Maths avec une note 6.0

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   {
      "date": "02.12.2024",
      "nom": "NISSENS",
      "prenom": "Remy",
      "branche": "Maths",
      "note": 6
   },
   {
      "date": "20.03.2025",
      "nom": "TERRIEUR",
      "prenom": "Alex",
      "branche": "Maths",
      "note": 6
   },
   {
      "date": "05.05.2025",
      "nom": "TARISTE",
      "prenom": "Guy",
      "branche": "Maths",
      "note": 6
   },
   {
      "date": "30.05.2025",
      "nom": "FICE",
      "prenom": "Eddy",
      "branche": "Maths",
      "note": 6
   },
   {
      "date": "03.10.2024",
      "nom": "HARONI",
      "prenom": "Mac",
      "branche": "Maths",
      "note": 6
   }
]
```

### F3 - Les villes ayant de 500 à 1000 habitants

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   {
      "ville": "Lully",
      "canton": "FR",
      "habitants": 900
   },
   {
      "ville": "Lully",
      "canton": "VD",
      "habitants": 700
   },
   {
      "ville": "Villars",
      "canton": "VD",
      "habitants": 620
   }
]
```

### M1 - La liste des marques de moto

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   "Honda",
   "Yamaha",
   "Ducati",
   "BMW",
   "Harley-Davidson"
]
```

### M2 - La liste des Prénom NOM des évalutions (avec doublons)

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   "Claire VOYANTE",
   "Alain TERNET",
   "Guy TARISTE",
   "Claire VOYANTE",
   "John D'ŒUF",
   "Alain TERRIEUR",
   "Alain TERRIEUR",
   "Eddy FICE",
   "Remy NISSENS",
   "Alex TERRIEUR",
   "Alain TERNET",
  ...
  ...
  ...
   "Remy NISSENS",
   "Eddy FICE",
   "Alain TERNET",
   "Claire VOYANTE",
   "Mac HARONI",
   "Alex TERRIEUR",
   "Théo RIQUE",
   "John D'ŒUF",
   "Alex TERRIEUR",
   "Claire VOYANTE",
   "Alain TERRIEUR"
]
```

### M3 - Toutes les villes et cantons (sans les habitants)

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   {
      "ville": "Fribourg",
      "canton": "FR"
   },
   {
      "ville": "Bulle",
      "canton": "FR"
   },
   {
      "ville": "Villars-sur-Glâne",
      "canton": "FR"
   },
   {
      "ville": "Riaz",
      "canton": "FR"
   },
   {
      "ville": "Lessoc",
      "canton": "FR"
   },
   {
      "ville": "Lausanne",
      "canton": "VD"
   },
   {
      "ville": "Yverdon-les-Bains",
      "canton": "VD"
   },
   {
      "ville": "Montreux",
      "canton": "VD"
   },
   {
      "ville": "Olten",
      "canton": "SO"
   },
   {
      "ville": "Solothurn",
      "canton": "SO"
   },
   {
      "ville": "Grenchen",
      "canton": "SO"
   },
   {
      "ville": "Sion",
      "canton": "VS"
   },
   {
      "ville": "Martigny",
      "canton": "VS"
   },
   {
      "ville": "Brig-Glis",
      "canton": "VS"
   },
   {
      "ville": "Zermatt",
      "canton": "VS"
   },
   {
      "ville": "Bern",
      "canton": "BE"
   },
   {
      "ville": "Biel/Bienne",
      "canton": "BE"
   },
   {
      "ville": "Thun",
      "canton": "BE"
   },
   {
      "ville": "Lully",
      "canton": "FR"
   },
   {
      "ville": "Lully",
      "canton": "VD"
   },
   {
      "ville": "Lully",
      "canton": "GE"
   },
   {
      "ville": "Villars",
      "canton": "VD"
   },
   {
      "ville": "Villars",
      "canton": "FR"
   }
]
```

### R1 - La plus petite date d'évaluation

À partir des données disponibles, vous devez obtenir ceci :

```json
"01.01.2025"
```

### R2 - Pour chaque branche, le nombre d'évaluations réalisées

À partir des données disponibles, vous devez obtenir ceci :

```json
{
   "Physique": 84,
   "Français": 86,
   "Allemand": 78,
   "Maths": 84,
   "Anglais": 83,
   "Histoire": 82,
   "Géographie": 85,
   "Chimie": 84
}
```

### R3 - Pour chaque branche, le nombre de notes, leur moyenne (à 2 décimales), la min et max

À partir des données disponibles, vous devez obtenir ceci :

```json
{
   "Physique": {
      "nbre": 84,
      "total": 362.1,
      "min": 2.7,
      "max": 6,
      "moyenne": "4.31"
   },
   "Français": {
      "nbre": 86,
      "total": 362.69999999999993,
      "min": 2.7,
      "max": 6,
      "moyenne": "4.22"
   },
   "Allemand": {
      "nbre": 78,
      "total": 333.80000000000007,
      "min": 2.8,
      "max": 6,
      "moyenne": "4.28"
   },
   "Maths": {
      "nbre": 84,
      "total": 378.2,
      "min": 2.7,
      "max": 6,
      "moyenne": "4.50"
   },
   "Anglais": {
      "nbre": 83,
      "total": 364.0999999999999,
      "min": 2.7,
      "max": 6,
      "moyenne": "4.39"
   },
   "Histoire": {
      "nbre": 82,
      "total": 354.80000000000007,
      "min": 2.7,
      "max": 6,
      "moyenne": "4.33"
   },
   "Géographie": {
      "nbre": 85,
      "total": 368.1000000000001,
      "min": 2.7,
      "max": 6,
      "moyenne": "4.33"
   },
   "Chimie": {
      "nbre": 84,
      "total": 358,
      "min": 2.7,
      "max": 6,
      "moyenne": "4.26"
   }
}
```

### C1 - La liste des MARQUE / Modèle de motos

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   "BMW / K1600GTL",
   "BMW / R nineT",
   "BMW / R1250GS",
   "BMW / S1000RR",
   "DUCATI / 916",
   "DUCATI / Monster 1200",
   "DUCATI / Panigale V4",
   "DUCATI / Scrambler Icon",
   "HARLEY-DAVIDSON / Electra Glide",
   "HARLEY-DAVIDSON / Fat Boy 114",
   "HARLEY-DAVIDSON / Sportster 883",
   "HARLEY-DAVIDSON / Street Glide Special",
   "HONDA / Africa Twin CRF1100L",
   "HONDA / CB750 Four",
   "HONDA / CBR1000RR Fireblade",
   "HONDA / Gold Wing",
   "YAMAHA / MT-09",
   "YAMAHA / Ténéré 700",
   "YAMAHA / XT500",
   "YAMAHA / YZF-R1"
]
```

### C2 - La liste des "NOM Prénom" des évalutions (sans doublons et triée)

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   "D'ŒUF John",
   "FICE Eddy",
   "HARONI Mac",
   "NISSENS Remy",
   "RIQUE Théo",
   "TARISTE Guy",
   "TERNET Alain",
   "TERRIEUR Alain",
   "TERRIEUR Alex",
   "VOYANTE Claire"
]
```

### C3 - Le prix moyen des motos de chaque marque

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   {
      "marque": "Honda",
      "prixMoyen": "20750.00"
   },
   {
      "marque": "Yamaha",
      "prixMoyen": "12875.00"
   },
   {
      "marque": "Ducati",
      "prixMoyen": "19125.00"
   },
   {
      "marque": "BMW",
      "prixMoyen": "21625.00"
   },
   {
      "marque": "Harley-Davidson",
      "prixMoyen": "24125.00"
   }
]
```

### C4 - Pour chaque marque, la plus chère et la moins chère des motos

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   {
      "marque": "Honda",
      "moinsChere": {
         "nom": "CB750 Four",
         "prix": 12000
      },
      "plusChere": {
         "nom": "Gold Wing",
         "prix": 33000
      }
   },
   {
      "marque": "Yamaha",
      "moinsChere": {
         "nom": "XT500",
         "prix": 9000
      },
      "plusChere": {
         "nom": "YZF-R1",
         "prix": 21000
      }
   },
   {
      "marque": "Ducati",
      "moinsChere": {
         "nom": "Scrambler Icon",
         "prix": 10000
      },
      "plusChere": {
         "nom": "Panigale V4",
         "prix": 26000
      }
   },
   {
      "marque": "BMW",
      "moinsChere": {
         "nom": "R nineT",
         "prix": 17000
      },
      "plusChere": {
         "nom": "K1600GTL",
         "prix": 28000
      }
   },
   {
      "marque": "Harley-Davidson",
      "moinsChere": {
         "nom": "Sportster 883",
         "prix": 11000
      },
      "plusChere": {
         "nom": "Electra Glide",
         "prix": 31000
      }
   }
]
```

### C5 - Pour CLAIRE Voyante, les branches et ses moyennes

À partir des données disponibles, vous devez obtenir ceci :

```json
{
   "Physique": 4.53,
   "Maths": 4.69,
   "Géographie": 3.37,
   "Chimie": 4.03,
   "Allemand": 4.55,
   "Anglais": 3.65,
   "Français": 3.94,
   "Histoire": 4.32
}
```

### C6 - { canton: population }, triée

À partir des données disponibles, vous devez obtenir ceci :

```json
{
   "FR": 79900,
   "VD": 206120,
   "SO": 53800,
   "VS": 74400,
   "BE": 234600,
   "GE": 350
}
```

### C7 - [ { canton, population } ], triée

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   {
      "canton": "BE",
      "population": 234600
   },
   {
      "canton": "FR",
      "population": 79900
   },
   {
      "canton": "GE",
      "population": 350
   },
   {
      "canton": "SO",
      "population": 53800
   },
   {
      "canton": "VD",
      "population": 206120
   },
   {
      "canton": "VS",
      "population": 74400
   }
]
```

### C8 - [ [ canton, population ] ], triée

À partir des données disponibles, vous devez obtenir ceci :

```json
[
   [
      "BE",
      234600
   ],
   [
      "FR",
      79900
   ],
   [
      "GE",
      350
   ],
   [
      "SO",
      53800
   ],
   [
      "VD",
      206120
   ],
   [
      "VS",
      74400
   ]
]
```

---

<img src="res/EMF_logo_RVB_Info_long.png" width="25%" style="margin-left:-20px;">
