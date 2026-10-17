# Lemonade

Application Android simple et interactive réalisée avec Kotlin et Jetpack Compose. L'utilisateur prépare une citronnade en appuyant sur l'image affichée à l'écran.

## Fonctionnement

1. Appuyer sur le citronnier pour cueillir un citron.
2. Appuyer sur le citron pour le presser. Le nombre de pressions nécessaires est aléatoire, entre 2 et 4.
3. Appuyer sur le verre de citronnade pour le boire.
4. Appuyer sur le verre vide pour recommencer.

## Informations techniques

- Langage : Kotlin
- Interface : Jetpack Compose (Material 3)
- Nom du package : com.example.lemonade
- SDK minimum : 24
- Modèle de projet : Empty Activity

## Structure du projet

```
app/src/main/
  java/com/example/lemonade/MainActivity.kt
  res/drawable/
    lemon_tree.xml
    lemon_squeeze.xml
    lemon_drink.xml
    lemon_restart.xml
  res/values/strings.xml
```

## Points clés du code

- Les étapes de la préparation sont représentées par quatre constantes (SELECT, SQUEEZE, DRINK, RESTART).
- Le nombre de pressions est tiré avec `(2..4).random()`.
- `rememberSaveable` conserve l'étape en cours lors de la rotation de l'écran.
- Le composable `LemonTextAndImage` affiche le libellé et l'image cliquable de chaque étape.

## Installation et lancement

1. Ouvrir le projet dans Android Studio.
2. Attendre la fin de la synchronisation Gradle.
3. Sélectionner un émulateur ou un appareil Android.
4. Cliquer sur le bouton Run.

