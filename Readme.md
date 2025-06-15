# Rapport de l’Activité Pratique n°1 – Utilisation de l’injection de dépendances avec Spring

---

## 🗂️ Organisation du projet

Voici la structure générale du projet tel qu’implémenté :
![Structure du projet](capture/img17.png)

---

## 🔧 Définition des interfaces et implémentations

### Interface `IDao`
L’interface définit la méthode `getData()` qui sera utilisée par la couche métier :
![Interface IDao](capture/img1.png)

### Implémentation de `IDao`
Une version concrète de cette interface est fournie dans la classe `DaoImpl` :
![Implémentation DaoImpl](capture/img2.png)

---

### Interface `IMetier`
Contient la méthode `calcul()` pour effectuer une opération à partir des données DAO :
![Interface IMetier](capture/img3.png)

### Implémentation de `IMetier`
Ici, l’injection de dépendance est réalisée pour découpler les composants :
![Implémentation MetierImpl](capture/img4.png)

---

## ⚙️ Techniques d’injection de dépendances utilisées

### ➤ Instanciation manuelle (statique)
Cette méthode consiste à créer les objets manuellement dans le code :
![Injection statique](capture/img5.png)

### ➤ Instanciation dynamique
Utilisation d’une approche plus souple avec des paramètres :
![Injection dynamique](capture/img6.png)

---

## 📁 Configuration et exécutions

### Configurations – Base de données
Fichier de configuration utilisé pour la version "base de données" :
![config.txt DB](capture/img12.png)

### Résultat – Base de données
Voici ce que le programme affiche avec cette configuration :
![Sortie base de données](capture/img8.png)

### Configurations – Web service
Un second fichier est utilisé pour la version "web service" :
![config.txt WS](capture/img13.png)

### Résultat – Web service
Affichage de la console avec ce paramétrage :
![Sortie web service](capture/img7.png)

---

## 🌿 Mise en œuvre avec le framework Spring

### 🔸 Configuration avec fichier XML
Injection gérée via un fichier `config;xml` :
![Spring XML](capture/img13.png)

### 🔸 Configuration avec annotations
Utilisation des annotations Spring pour automatiser l’injection :
![Spring Annotations](capture/img11.png)

---

## 📄 Fichiers de configuration supplémentaires

### Fichier `config.xml`
Déclaration des beans et liens entre composants :
![config.xml](capture/img14.png)

### Fichier `pom.xml`
Liste des dépendances Maven utilisées dans le projet :
![pom.xml](capture/img15.png)

---
