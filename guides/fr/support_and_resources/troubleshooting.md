# 🆘 Dépannage

## Problèmes courants et solutions

### L'appareil ne démarre pas

**Symptômes** : Écran noir, aucune réponse à la mise sous tension
**Solutions** :

- ✅ Vérifiez que la source d'alimentation fournit suffisamment de courant (2 A recommandés)
- ✅ Vérifiez que toutes les connexions matérielles sont sécurisées
- ✅ Essayez une autre carte SD avec une image SeedSigner récente
- ✅ Testez avec un autre câble d'alimentation

### Problèmes de lecture de codes QR

**Symptômes** : Codes QR non reconnus, délai de lecture expiré
**Solutions** :

- ✅ Assurez-vous que le code QR est bien éclairé
- ✅ Maintenez l'appareil stable à une distance appropriée (15 à 30 cm)
- ✅ Nettoyez l'objectif de la caméra avec un chiffon doux
- ✅ Essayez de régler la densité du code QR dans les paramètres
- ✅ Vérifiez les paramètres de rotation de la caméra
- ✅ Testez le fonctionnement de la caméra dans le test d'E/S matérielles

### Seed incorrect Génération

**Symptômes** : La graine générée ne correspond pas aux résultats attendus
**Solutions** :

- ✅ Vérifiez que vous utilisez des sources d'entropie appropriées (bon caractère aléatoire)
- ✅ Assurez-vous d'un éclairage approprié lors de la capture d'entropie par la caméra
- ✅ Pour les lancers de dés, utilisez des dés physiques appropriés (et non numériques)
- ✅ Vérifiez la transcription de la graine lors de la sauvegarde
- ✅ Exécutez le processus de vérification de la sauvegarde

### Problèmes de réponse des boutons

**Symptômes** : Les boutons ne répondent pas, saisie incohérente
**Solutions** :

- ✅ Exécutez un test d'E/S matérielle pour isoler le problème
- ✅ Nettoyez autour des boutons pour éliminer les débris
- ✅ Vérifiez que le casque WaveShare n'est pas endommagé
- ✅ Essayez différentes combinaisons de boutons (A, B, C fonctionnent tous de manière identique)

### Problèmes d'affichage

**Symptômes** : L'écran scintille, affiche partiellement, affiche incorrectement Couleurs
**Solutions** :

- ✅ Vérifiez les connexions du chapeau WaveShare
- ✅ Exécutez le test d'affichage des E/S matérielles
- ✅ Essayez une autre source d'alimentation
- ✅ Vérifiez l'intégrité de la carte SD

## Messages d'erreur

### « Type de QR inconnu »

**Signification** : Le format du code QR scanné n'est pas reconnu par SeedSigner
**Solutions** :

- ✅ Vérifiez que vous scannez un type de QR pris en charge (PSBT, SeedQR, etc.)
- ✅ Vérifiez la qualité et la clarté du code QR
- ✅ Assurez-vous que l'éclairage et le positionnement de la caméra sont corrects

### « Semence invalide »

**Signification** : La phrase de départ saisie ne passe pas la validation BIP-39
**Solutions** :

- ✅ Vérifiez chaque mot de votre phrase de départ
- ✅ Vérifiez que l'ordre des mots est correct
- ✅ Assurez-vous que tous les mots proviennent de la liste de mots BIP-39
- ✅ Vérifiez les fautes de frappe dans la saisie manuelle

### « Erreur de somme de contrôle »

**Signification** : Le dernier mot ne correspond pas à la somme de contrôle requise
**Solutions** :

- ✅ Utilisez l'outil « Calculer le 12e/24e mot » pour trouver le dernier mot correct
- ✅ Vérifiez que tous les mots précédents sont corrects
- ✅ Vérifiez les erreurs de transcription
