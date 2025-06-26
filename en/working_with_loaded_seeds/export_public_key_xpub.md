# Export Public Key (Xpub)

Create watch-only wallets in your favorite Bitcoin software by exporting your public key. This allows you to monitor balances and prepare transactions without exposing your private keys.

## Complete Step-by-Step Process with All Screenshots

1. **Access Export**: From the seed's main screen, select **"Export Xpub"**

<div align="center">
     <img src="images/SeedMenuView.png" alt="Seed main menu with Export Xpub option" width="250"/>
</div>

2. **Choose Signature Type**:
   - **"Single Sig"** - For standard personal wallets
   - **"Multisig"** - For multi-signature wallets requiring multiple devices

<div align="center">
     <img src="images/SeedExportXpubSigTypeView.png" alt="Xpub signature type selection" width="250"/>
</div>

3. **Select Script Type**:
   - **Native Segwit** (bech32) - Recommended for lowest fees
   - **Nested Segwit** (P2SH) - For compatibility with older systems
   - **Taproot** - For advanced privacy and smart contract features

<div align="center">
     <img src="images/SeedExportXpubScriptTypeView.png" alt="Script type selection for Xpub" width="250"/>
</div>

4. **Choose Wallet Software**: Select your preferred wallet from supported options

<div align="center">
     <img src="images/SeedExportXpubCoordinatorView.png" alt="Wallet software selection" width="250"/>
</div>

5. **Acknowledge Privacy Warning**: Press **"I Understand"** after reading the xpub privacy implications

<div align="center">
     <img src="images/SeedExportXpubWarningView.png" alt="Xpub privacy warning screen" width="250"/>
</div>

6. **Generate QR Code**: Select **"Export XPub"** to display the shareable QR code

<div align="center">
     <img src="images/SeedExportXpubDetailsView.png" alt="Generated Xpub QR code" width="250"/>
</div>

7. **Import to Wallet**: Scan the QR code with your chosen wallet software

<div align="center">
     <img src="images/SeedExportXpubQRView.png" alt="Generated Xpub QR code" width="250"/>
</div>

> **🔒 Privacy Warning**: Your xpub (extended public key) reveals all your Bitcoin addresses and transaction history. Only share it with wallet software you trust, and never post it publicly online.