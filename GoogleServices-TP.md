# TP Google services
Dans ce TP vous allez apprendre à utiliser plusieurs services google, les plus utiles pour composer une application mobile. 

## Notions
- Récuperer une clé d'API pour un service Google
- Utiliser l'assistant Android Studio pour Firebase
- Implémenter une Carte Google Maps dans votre application 
- Detecter la localisation GPS du téléphone et l'afficher
- Parcourir une documentation et s'en servir dans votre projet
- Utiliser les notifications via FCM (GCM est déprécié) 
- Construire une notification dans votre application

## Exercice 1 - Créer le projet
Créer un nouveau projet Android Studio avec une Activité Vide. 

Dans le manifest du projet ajouter les permissions d'accès à la localisation précise `FINE_LOCATION`
```xml
 <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
```

### Ajouter les services Google play `googlePlayServices`

- Dans votre fichier `build.gradle` ajouter les dépendances nécessaire pour accéder aux services Google Play : 
Il faut s'assurer que vous trouviez bien la ligne suivant dans `repositories`
    ```groovy
    google() ou maven { url "https://maven.google.com" }
    ```

- Ensuite il faut importer les bibliothèques qui vont nous être utiles. Puisque nous allons avoir besoin de la localisation, il faut que vous ajoutiez la **bonne bibliothèque** depuis cette liste :

    | Google+                                  | com.google.android.gms:play-services-plus:16.0.0      |
    |------------------------------------------|-------------------------------------------------------|
    | Google Account Login                     | com.google.android.gms:play-services-auth:16.0.1      |
    | Google Actions, Base Client Library      | com.google.android.gms:play-services-base:16.1.0      |
    | Google Sign In                           | com.google.android.gms:play-services-identity:16.0.0  |
    | Google Analytics                         | com.google.android.gms:play-services-analytics:16.0.6 |
    | Google Awareness                         | com.google.android.gms:play-services-awareness:16.0.0 |
    | Google Cast                              | com.google.android.gms:play-services-cast:16.1.2      |
    | Google Cloud Messaging                   | com.google.android.gms:play-services-gcm:16.0.0       |
    | Google Drive                             | com.google.android.gms:play-services-drive:16.0.0     |
    | Google Fit                               | com.google.android.gms:play-services-fitness:16.0.1   |
    | Google Location and Activity Recognition | com.google.android.gms:play-services-location:16.0.0  |
    | Google Mobile Ads                        | com.google.android.gms:play-services-ads:17.1.2       |
    | Mobile Vision                            | com.google.android.gms:play-services-vision:17.0.2    |
    | Google Nearby                            | com.google.android.gms:play-services-nearby:16.0.0    |
    | Google Panorama Viewer                   | com.google.android.gms:play-services-panorama:16.0.0  |
    | Google Play Game services                | com.google.android.gms:play-services-games:16.0.0     |
    | SafetyNet                                | com.google.android.gms:play-services-safetynet:16.0.0 |
    | Google Pay                               | com.google.android.gms:play-services-wallet:16.0.1    |
    | Wear OS by Google                        | com.google.android.gms:play-services-wearable:16.0.1  |



## Exercice 2 - Clé d'API pour Maps

## Exercice 3 - Lire la documentation de Google Maps API

## Exercice 4 - Les notifications

## Exercice 5 - FCM et Firebase
