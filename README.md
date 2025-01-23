# Calco

**Calco** est une application conçue pour récupérer les plannings des salles de réunion sur une période de deux jours et les afficher sur un écran à encre électronique. Cette solution est idéale pour les environnements professionnels où la consultation rapide et claire des disponibilités des salles est essentielle.

## 🛠️ Fonctionnalités

- **Récupération des plannings** : Extraction des plannings des salles pour les deux jours suivants.
- **Affichage clair** : Les informations sont affichées sur un écran à encre électronique, offrant une lisibilité optimale tout en économisant de l'énergie.
- **Compatibilité avec Raspberry Pi** : Le projet fonctionne sous **Raspbian**, le système d'exploitation pour Raspberry Pi.
- **Python 3** : Application entièrement développée en Python 3 pour sa simplicité et sa flexibilité.

## 📋 Pré-requis

Pour exécuter ce projet, vous aurez besoin de :
- Un **Raspberry Pi** (modèle recommandé : Raspberry Pi 3 ou supérieur).
- Un écran à encre électronique compatible.
- **Raspbian** installé sur le Raspberry Pi.
- **Python 3** installé avec les bibliothèques nécessaires (voir ci-dessous).

## ⚙️ Installation

1. Clonez ce dépôt sur votre Raspberry Pi :
   ```bash
   git clone https://github.com/KevinP93/CalCo.git
   cd calco
   ```

2. Installez les dépendances nécessaires :
   ```bash
   pip install -r requirements.txt
   ```

3. Configurez les paramètres (comme les API pour récupérer les plannings, si applicable) dans le fichier de configuration fourni :
   ```bash
   cp config_template.json config.json
   nano config.json
   ```

4. Lancez l'application :
   ```bash
   python3 main.py
   ```

## 🖥️ Matériel supporté

- **Raspberry Pi** : Tous les modèles prenant en charge Raspbian.
- **Écrans à encre électronique** : Vérifiez la compatibilité avec votre matériel. Les pilotes spécifiques peuvent être nécessaires.

## 📄 Fonctionnement

1. **Connexion aux sources des plannings** : L'application récupère les données depuis une API, un fichier, ou une base de données (selon la configuration).
2. **Traitement des données** : Les informations sur les disponibilités des salles sont filtrées et formatées.
3. **Affichage** : Les données sont affichées sur l'écran à encre électronique avec un design minimaliste pour une meilleure lisibilité.

## 🌟 Points forts

- **Économie d'énergie** : L'écran à encre électronique consomme très peu d'énergie.
- **Accessibilité** : Une interface simple et efficace.
- **Open-source** : Personnalisez et améliorez l'application selon vos besoins.

## 🚀 Prochaines évolutions

- Ajouter une gestion des événements en temps réel.
- Améliorer l’interface utilisateur sur l’écran à encre électronique.
- Intégration avec des calendriers populaires comme Google Calendar ou Microsoft Outlook.

## 📧 Contact

Si vous avez des questions ou des suggestions, n’hésitez pas à me contacter :
- **Email** : c.kevinpereira@gmail.com
- **GitHub** : https://github.com/KevinP93
