# Guide d'utilisation de SeedSigner

<div align="center">
    <img src="../fr/images/SeedSigner_Logo.png" alt="Logo SeedSigner" width="400"/>
</div>

SeedSigner est un outil de signature Bitcoin open source et isolé qui vous permet de gérer les phrases de signature et de signer des transactions en toute sécurité. Ce guide fournit des instructions étape par étape, organisées selon les flux de travail courants.

## 📋 Table des matières

### 🚀 Prise en main

- [Configuration initiale et démarrage](/guides/fr/getting_started/initial_setup_and_power_on.md)
- [Bases de la navigation](/guides/fr/getting_started/navigation_basics.md)
- [Mise hors tension en toute sécurité](/guides/fr/getting_started/powering_off_safely.md)
- [Redémarrage de votre appareil](/guides/fr/getting_started/restarting_your_device.md)

### 🌱 Gestion des graines

- **Création de nouvelles graines**
  - [Génération de graines par caméra](/guides/fr/seed_management/creating_new_seeds/camera_based_seed_generation.md)
  - [Génération de graines par dés Génération](/guides/fr/seed_management/creating_new_seeds/dice_based_seed_generation.md)
  - [Calcul de la génération des graines de mots 12e/24e](/guides/fr/seed_management/creating_new_seeds/calc_12th24th_word_seed_generation.md)

- **Chargement des graines existantes**
  - [Saisie manuelle des graines](/guides/fr/seed_management/load_existing_seeds/manual_seed_entry.md)
  - [Scan des graines QR](/guides/fr/seed_management/load_existing_seeds/seedqr_scanning.md)
  - [Ajout de BIP-39 Phrase secrète](/guides/fr/seed_management/load_existing_seeds/adding_bip_39_passphrase.md)

### 🔧 Utilisation des graines chargées

- [Exporter la clé publique (Xpub)](/guides/fr/working_with_loaded_seeds/export_public_key_xpub.md)
- [Générer les adresses de réception](/guides/fr/working_with_loaded_seeds/generate_receiving_addresses.md)
- [Générer les adresses de modification](/guides/fr/working_with_loaded_seeds/generate_change_addresses.md)
- [Afficher les mots clés](/guides/fr/working_with_loaded_seeds/view_seed_words.md)
- [Créer un QR code source Sauvegarde](/guides/fr/working_with_loaded_seeds/create_seedqr_backup.md)

### ✍️ Transactions et vérification

- [Signature d'une transaction Bitcoin (PSBT)](/guides/fr/transactions_and_verification/sign_bitcoin_transaction_psbt.md)
- [Vérification de la propriété de l'adresse](/guides/fr/transactions_and_verification/verify_address_ownership.md)
- [Supprimer la graine chargée](/guides/fr/transactions_and_verification/discard_loaded_seed.md)

### ⚙️ Configuration de l'appareil

- **Paramètres de base**
  - [Configuration de la langue](/guides/fr/device_configuration/basic_settings/language_configuration.md)
  - [Persistant Paramètres](/guides/fr/device_configuration/basic_settings/persistent_settings.md)
  - [Support logiciel du coordinateur](/guides/fr/device_configuration/basic_settings/coordinator_software_support.md)
  - [Affichage de la valeur nominale](/guides/fr/device_configuration/basic_settings/denomination_display.md)
  - [Tests d'E/S matérielles](/guides/fr/device_configuration/basic_settings/hardware_io_testing.md)
  - [Informations sur les dons](/guides/fr/device_configuration/basic_settings/donation_information.md)

- **Paramètres avancés**
  - [Sélection du réseau Bitcoin](/guides/fr/device_configuration/advanced_settings/bitcoin_network_selection.md)
  - [Code QR Densité](/guides/fr/device_configuration/advanced_settings/qr_code_density.md)
  - [Configuration d'exportation Xpub](/guides/fr/device_configuration/advanced_settings/xpub_export_configuration.md)
  - [Configuration des types de signature](/guides/fr/device_configuration/advanced_settings/signature_types_configuration.md)
  - [Configuration des types de script](/guides/fr/device_configuration/advanced_settings/script_types_configuration.md)
  - [Afficher les détails Xpub](/guides/fr/device_configuration/advanced_settings/show_xpub_details.md)
  - [Phrase secrète BIP-39 Configuration](/guides/fr/device_configuration/advanced_settings/bip-39_passphrase_configuration.md)
  - [Rotation de la caméra](/guides/fr/device_configuration/advanced_settings/camera_rotation.md)
  - [Compact SeedQR](/guides/fr/device_configuration/advanced_settings/compact_seedqr.md)
  - [Enfants Seeds BIP-85](/guides/fr/device_configuration/advanced_settings/bip-85_child_seeds.md)
  - [Enfants Seeds Electrum](/guides/fr/device_configuration/advanced_settings/electrum_seeds.md)
  - [Signature des messages](/guides/fr/device_configuration/advanced_settings/message_signing.md)
  - [Avertissements relatifs à la confidentialité](/guides/fr/device_configuration/advanced_settings/privacy_warnings.md)
  - [Avertissements importants](/guides/fr/device_configuration/advanced_settings/dire_warnings.md)
  - [Conseils concernant la luminosité du QR Code](/guides/fr/device_configuration/advanced_settings/qr_brightness_tips.md)
  - [Logos partenaires](/guides/fr/device_configuration/advanced_settings/partner_logos.md)

- **Paramètres matériels**
  - [Configuration du type d'affichage](/guides/fr/device_configuration/hardware_settings/display_type_configuration.md)
  - [Inversion des couleurs](/guides/fr/device_configuration/hardware_settings/color_inversion.md)

### 🔧 Assistance et ressources

- [Dépannage](/guides/fr/support_and_resources/troubleshooting.md)
- [Ressources supplémentaires](/guides/fr/support_and_resources/additional_resources.md)
- [Considérations de sécurité](/guides/fr/support_and_resources/security_considerations.md)

> 💡 **Conseil de navigation rapide** : Utilisez Ctrl+F (ou Cmd+F sur Mac) pour rechercher des rubriques spécifiques dans ce guide.

---

## Composants matériels

Un appareil SeedSigner se compose de :

1. **Raspberry Pi Zero** - L'unité de calcul principale
2. **Caméra Raspberry Pi** - Pour la lecture de codes QR et la capture d'entropie
3. **WaveShare LCD Hat 1,3 pouce** - Interface d'affichage et de contrôle

### Commandes du WaveShare LCD Hat

<div align="center">
    <img src="../fr/images/WaveShare_LCD_Hat.png" alt="WaveShare LCD Hat" width="350"/>
</div>

Le WaveShare LCD Hat offre les commandes suivantes :

- **Joystick** : Navigation quadridirectionnelle (haut, bas, gauche, droite) et appui central
- **Touche 1 (A)** : Bouton d'action principal
- **Touche 2 (B)** : Bouton d'action secondaire
- **Touche 3 (C)** : Bouton d'action tertiaire

### Référence des fonctions des boutons

| Commande | Fonction |
| -------------- | ------------------------------------------- |
| Joystick Haut | Déplacer la sélection vers le haut |
| Joystick Bas | Déplacer la sélection vers le bas |
| Joystick Gauche | Déplacer la sélection vers la gauche |
| Joystick Droite | Déplacer la sélection vers la droite |
| Appuyer sur le joystick | Sélection alternative/confirmation (selon le contexte) |
| Touche 1 (A) | Sélectionner l'option en surbrillance ou confirmer l'action |
| Touche 2 (B) | Sélectionner l'option en surbrillance ou confirmer l'action |
| Touche 3 (C) | Sélectionner l'option en surbrillance ou confirmer l'action |

**Notes de navigation importantes** :

- Les trois touches (A, B, C) fonctionnent de manière identique pour la sélection et la confirmation.
- Pour revenir à un écran précédent, naviguez d'abord jusqu'à la flèche/le bouton Retour à l'aide du joystick, puis appuyez sur n'importe quelle touche pour l'activer.
- L'appui central du joystick peut avoir différentes fonctions selon le contexte de l'écran.

---

## 🏁 Conclusion

SeedSigner fournit une solution open source sécurisée pour la gestion des clés Bitcoin et la signature des transactions. En suivant les procédures décrites dans ce guide, vous pouvez :

- ✅ Générer des phrases de données véritablement aléatoires à l'aide de plusieurs sources d'entropie
- ✅ Charger et gérer en toute sécurité les phrases de données existantes
- ✅ Signer des transactions Bitcoin sans exposer les clés privées aux appareils en réseau
- ✅ Exporter les clés publiques pour la configuration d'un portefeuille en lecture seule
- ✅ Vérifier la propriété des adresses et les détails des transactions
- ✅ Maintenir une sécurité air-gap complète pour toutes les opérations

### Règles d'or :

1. **Ne jamais ignorer la vérification de la sauvegarde des graines** - Un mot erroné peut entraîner la perte de vos bitcoins
2. **Toujours vérifier les détails des transactions** - Les transactions Bitcoin sont irréversibles
3. **Maintenir une sécurité air-gap** - Ne jamais connecter SeedSigner aux réseaux
4. **Utiliser des environnements privés** - Se protéger contre la surveillance et l'enregistrement
5. **Stocker les sauvegardes en toute sécurité** - Traiter les phrases de données comme les actifs précieux qu'elles protègent

### Obtenir de l'aide

Si vous rencontrez des problèmes non abordés dans ce guide :

- Consultez le dépôt GitHub officiel de SeedSigner pour Mises à jour
- Consultez les forums et groupes de discussion de la communauté pour obtenir de l'aide.
- Consultez la section Dépannage pour trouver des solutions courantes.
- N'hésitez pas à contacter la communauté de développement pour les problèmes techniques complexes.

**N'oubliez pas** : la sécurité de vos Bitcoins est votre responsabilité. Prenez le temps de comprendre chaque étape, entraînez-vous avec de petites sommes et ne vous précipitez jamais sur les opérations critiques pour la sécurité.

---

*Ce guide est géré par la communauté SeedSigner et mis à jour régulièrement. Pour obtenir la dernière version et des ressources supplémentaires, consultez le dépôt GitHub officiel de SeedSigner.*
