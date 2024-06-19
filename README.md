# Projet de Firmware Marlin pour Imprimante 3D Connectée

## Description du Projet

Ce projet consiste en la création et l'optimisation d'un firmware Marlin personnalisé pour une imprimante 3D connectée, intégrant diverses fonctionnalités avancées visant à améliorer la sécurité, l'efficacité et la qualité des impressions. Les fonctionnalités principales incluent :

### Fonctionnalités du Firmware

1. **Connexion par Caméra** :
    - Intégration d'une caméra pour la surveillance en temps réel des impressions.
    - Possibilité de visualisation à distance via une interface web ou une application mobile.

2. **Capteurs de Début et Fin de Course** :
    - Mise en place de capteurs pour détecter les positions de début et de fin de course de l'imprimante.
    - Amélioration de la précision et de la sécurité des mouvements de l'imprimante.

3. **Extinction Automatique** :
    - Système d'extinction automatique de l'imprimante après la fin d'une impression ou en cas de détection d'une anomalie.
    - Réduction de la consommation d'énergie et prévention des risques de surchauffe.

4. **Régulation de la Vitesse** :
    - Ajustement automatique de la vitesse d'impression en fonction de la complexité du modèle.
    - Optimisation de la qualité d'impression tout en maintenant une efficacité maximale.

5. **Systèmes de Sécurité** :
    - **Déclenchement d'Alarme à Incendie** : Détection de fumée ou de températures anormales avec déclenchement automatique d'une alarme.
    - **Détection de Surconsommation d'Énergie** : Surveillance de la consommation énergétique pour prévenir les risques de surcharge et de court-circuit.
    - **Arrêt d'Urgence à Distance** : Possibilité d'arrêter l'imprimante à distance en cas d'urgence via une interface web ou une application mobile.

### Installation et Configuration

1. **Prérequis** :
    - Imprimante 3D compatible avec le firmware Marlin.
    - Capteurs et caméra compatibles.
    - Connexion internet pour les fonctionnalités de surveillance à distance.
    - **IDE Utilisé** : PlatformIO, une extension de Visual Studio Code, pour la compilation et le flashage du firmware.
    - Microcontrôleurs compatibles comme l'ESP32 pour la connectivité Wi-Fi et les fonctionnalités avancées.
    - Cartes mères compatibles :
        - BigTreeTech SKR V1.4 / V1.4 Turbo
        - BigTreeTech SKR Mini E3 V2.0
        - BigTreeTech SKR 2
        - BigTreeTech Octopus
        - MKS Robin Nano V3
        - MKS Gen L V2.1

2. **Installation du Firmware** :
    - Téléchargez les fichiers du firmware depuis le dépôt GitHub.
    - Installez Visual Studio Code et ajoutez l'extension PlatformIO.
    - Ouvrez le projet Marlin dans Visual Studio Code via PlatformIO.
    - Sélectionnez la carte mère appropriée dans le fichier `platformio.ini` en fonction de votre matériel (par exemple, `default_envs = STM32F103RE_bigtree` pour une carte BigTreeTech SKR V1.4).
    - Compilez le firmware en suivant les instructions fournies dans le fichier `platformio.ini`.
    - Flashez le firmware sur votre imprimante 3D en connectant votre imprimante à l'ordinateur et en utilisant les outils de PlatformIO.

3. **Configuration** :
    - Configurez les paramètres de la caméra et des capteurs dans le fichier `configuration.h`.
    - Paramétrez les options de sécurité et d'optimisation de la vitesse selon vos besoins spécifiques.
    - Configurez les broches des capteurs et des fonctionnalités avancées dans `pins_MYBOARD.h` si nécessaire.
    - Sauvegardez et rechargez le firmware après modification des configurations.

### Utilisation

1. **Surveillance en Temps Réel** :
    - Accédez à l'interface web ou à l'application mobile pour surveiller vos impressions en direct via l'ESP32.
    - Recevez des notifications en cas de détection de problèmes ou de fin d'impression.

2. **Gestion des Impressions** :
    - Planifiez vos impressions en tenant compte des optimisations automatiques de vitesse et de qualité.
    - Utilisez les fonctionnalités d'arrêt d'urgence et d'extinction automatique pour une gestion sécurisée.

### Contribution

Les contributions à ce projet sont les bienvenues. Vous pouvez soumettre des pull requests pour des améliorations ou signaler des problèmes via le système de tickets GitHub.

### Licence

Ce projet est sous licence MIT. Veuillez consulter le fichier LICENSE pour plus de détails.

## Remerciements

Merci à la communauté Marlin et aux contributeurs pour leur soutien et leurs contributions continues.
