<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://ai.google.dev/static/site-assets/images/share-ais-513315318.png" />
</div>

# Exécuter et déployer votre application AI Studio

Ceci contient tout ce dont vous avez besoin pour exécuter votre application en local.

## Exécution en local

**Prérequis :**  [Android Studio](https://developer.android.com/studio)


1. Ouvrez Android Studio
2. Sélectionnez **Open** et choisissez le dossier contenant ce projet
3. Laissez Android Studio corriger les éventuelles incompatibilités lors de l'importation du projet
4. Exécutez l'application sur un émulateur ou un appareil physique
# Hydratation Tracker 💧
 
Application Android de suivi de consommation d'eau quotidienne, développée avec **Jetpack Compose** et **Material 3**.
 
## 📱 Aperçu
 
Cette application permet à l'utilisateur de suivre son hydratation au quotidien : enregistrement des prises d'eau, suivi de l'objectif journalier, et visualisation de la progression via une interface moderne construite entièrement en Compose.
 
> l'application permet l'ajout rapide de verres d'eau (100ml, 250ml, 500ml), retrace l'historique de consommation, precise l'heure de la dernière prise;et enregistre la serie de jour ou l'objectif quotidien de 2L a été atteint.
 
## 🛠️ Stack technique
 
| Élément | Détail |
|---|---|
| Langage | Kotlin |
| UI | Jetpack Compose + Material 3 |
| Architecture | MVVM (`data`, `ui`, `viewmodel`) |
| Build system | Gradle (Kotlin DSL) |
| AGP | 8.10.1 |
| Kotlin | 2.0.21 |
| compileSdk / targetSdk | 36 |
| minSdk | 24 |
| Namespace | `com.example` |
| Application ID | `com.aistudio.hydratation.track` |
 
## 📂 Structure du projet
 
```
app/
 └── src/main/java/com/example/
      ├── data/         # Sources de données (Room, repositories)
      ├── ui/           # Écrans et composants Compose
      ├── viewmodel/    # ViewModels (état et logique de présentation)
      └── MainActivity.kt
```
 
## 🚀 Installation et exécution
 
### Prérequis
- Android Studio (version récente, compatible AGP 8.10.1)
- JDK fourni avec Android Studio
- Un appareil Android physique (API 24+) ou un émulateur, avec le débogage USB activé pour un appareil physique
### Étapes
 
1. Cloner le dépôt :
```
   git clone <url-du-depot>
```
2. Ouvrir le projet dans Android Studio.
3. Laisser Gradle synchroniser le projet (première synchronisation).
4. Générer un keystore de debug si nécessaire (voir `DOCUMENTATION_ERREURS.md`, section keystore).
5. Sélectionner un appareil dans le menu déroulant en haut de l'IDE.
6. Cliquer sur ▶️ **Run** pour compiler et installer l'application.
### Configuration Gradle importante
 
Le fichier `gradle.properties` doit contenir :
```properties
android.useAndroidX=true
android.enableJetifier=true
```
 
## 🐞 Problèmes connus / Historique de débogage
 
L'ensemble des erreurs rencontrées lors de la mise en place du projet (configuration Gradle, signature, compilation Kotlin, dépendances) ainsi que leurs résolutions sont détaillées dans le fichier de documentation des erreurs.
 
