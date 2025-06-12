# SeedSigner User Guide

<div align="center">
  <img src="images/SeedSigner_Logo.png" alt="SeedSigner Logo" width="400"/>
</div>

SeedSigner is an air-gapped, open-source Bitcoin signing device that helps you manage seed phrases and sign transactions securely. This guide provides step-by-step instructions organized by common workflows.

## 📋 Table of Contents

### 🚀 Getting Started

- [Initial Setup and Power On](/getting_started/initial_setup_and_power_on.md)
- [Navigation Basics](/getting_started/navigation_basics.md)
- [Powering Off Safely](/getting_started/powering_off_safely.md)
- [Restarting Your Device](/getting_started/restarting_your_device.md)

### 🌱 Seed Management

- **Creating New Seeds**
  - [Camera-Based Seed Generation](/seed_management/creating_new_seeds/camera_based_seed_generation.md)
  - [Dice-Based Seed Generation](/seed_management/creating_new_seeds/dice_based_seed_generation.md)
  - [Calc 12th/24th Word Seed Generation](/seed_management/creating_new_seeds/calc_12th24th_word_seed_generation.md)
- **Loading Existing Seeds**
  - [Manual Seed Entry](/seed_management/load_existing_seeds/manual_seed_entry.md)
  - [SeedQR Scanning](/seed_management/load_existing_seeds/seedqr_scanning.md)
  - [Adding BIP-39 Passphrase](/seed_management/load_existing_seeds/adding_bip_39_passphrase.md)

### 🔧 Working with Loaded Seeds

- [Export Public Key (Xpub)](#export-public-key-xpub)
- [Generate Receiving Addresses](#generate-receiving-addresses)
- [View Seed Words](#view-seed-words)
- [Create SeedQR Backup](#create-seedqr-backup)

### ✍️ Transactions & Verification

- [Sign Bitcoin Transaction (PSBT)](#sign-bitcoin-transaction-psbt)
- [Verify Address Ownership](#verify-address-ownership)
- [Discard Loaded Seed](#discard-loaded-seed)

### ⚙️ Device Configuration

- **Basic Settings**
  - [Language Configuration](#language-configuration)
  - [Persistent Settings](#persistent-settings)
  - [Coordinator Software Support](#coordinator-software-support)
  - [Denomination Display](#denomination-display)
  - [Hardware I/O Testing](#hardware-io-testing)
  - [Donation Information](#donation-information)

- **Advanced Settings**
  - [Bitcoin Network Selection](#bitcoin-network-selection)
  - [QR Code Density](#qr-code-density)
  - [Xpub Export Configuration](#xpub-export-configuration)
  - [Signature Types Configuration](#signature-types-configuration)
  - [Script Types Configuration](#script-types-configuration)
  - [Show Xpub Details](#show-xpub-details)
  - [BIP-39 Passphrase Configuration](#bip-39-passphrase-configuration)
  - [Camera Rotation](#camera-rotation)
  - [Compact SeedQR](#compact-seedqr)
  - [BIP-85 Child Seeds](#bip-85-child-seeds)
  - [Electrum Seeds](#electrum-seeds)
  - [Message Signing](#message-signing)
  - [Privacy Warnings](#privacy-warnings)
  - [Dire Warnings](#dire-warnings)
  - [QR Brightness Tips](#qr-brightness-tips)
  - [Partner Logos](#partner-logos)

- **Hardware Settings**
  - [Display Type Configuration](#display-type-configuration)
  - [Color Inversion](#color-inversion)

### 🔧 Support & Resources

- [Troubleshooting](#-troubleshooting)
- [Additional Resources](#-additional-resources)
- [Security Considerations](#-security-considerations)

> 💡 **Quick Navigation Tip**: Use Ctrl+F (or Cmd+F on Mac) to search for specific topics within this guide.

---

## Hardware Components

A SeedSigner device consists of:

1. **Raspberry Pi Zero** - The main computing unit
2. **Raspberry Pi Camera** - For QR code scanning and entropy capture
3. **WaveShare 1.3inch LCD Hat** - Display and control interface

### WaveShare LCD Hat Controls

<div align="center">
  <img src="images/WaveShare_LCD_Hat.png" alt="WaveShare LCD Hat" width="350"/>
</div>

The WaveShare LCD Hat provides the following controls:

- **Joystick**: Four-directional navigation (Up, Down, Left, Right) plus center press
- **Key1 (A)**: Primary action button
- **Key2 (B)**: Secondary action button  
- **Key3 (C)**: Tertiary action button

### Button Functions Reference

| Control        | Function                                    |
| -------------- | ------------------------------------------- |
| Joystick Up    | Move selection up                           |
| Joystick Down  | Move selection down                         |
| Joystick Left  | Move selection left                         |
| Joystick Right | Move selection right                        |
| Joystick Press | Alternative selection/confirm (context-dependent) |
| Key1 (A)       | Select highlighted option or confirm action |
| Key2 (B)       | Select highlighted option or confirm action |
| Key3 (C)       | Select highlighted option or confirm action |

**Important Navigation Notes**:

- All three keys (A, B, C) function identically for selection and confirmation
- To go back to a previous screen, navigate to the back arrow/button using the joystick first, then press any key to activate it
- The joystick center press may have different functions depending on the current screen context

---

## 🏁 Conclusion

SeedSigner provides a secure, open-source solution for Bitcoin key management and transaction signing. By following the workflows in this guide, you can:

- ✅ Generate truly random seed phrases using multiple entropy sources
- ✅ Securely load and manage existing seed phrases
- ✅ Sign Bitcoin transactions without exposing private keys to networked devices
- ✅ Export public keys for watch-only wallet setup
- ✅ Verify address ownership and transaction details
- ✅ Maintain complete air-gap security throughout all operations

### Remember the Golden Rules

1. **Never skip seed backup verification** - One wrong word means lost Bitcoin
2. **Always verify transaction details** - Bitcoin transactions are irreversible
3. **Maintain air-gap security** - Never connect SeedSigner to networks
4. **Use private environments** - Protect against surveillance and recording
5. **Store backups securely** - Treat seed phrases like the valuable assets they protect

### Getting Help

If you encounter issues not covered in this guide:

- Check the official SeedSigner GitHub repository for updates
- Visit community forums and chat groups for peer support
- Review the troubleshooting section for common solutions
- Consider reaching out to the development community for complex technical issues

**Remember**: Your Bitcoin security is ultimately your responsibility. Take time to understand each step, practice with small amounts, and never rush through security-critical operations.

---

*This guide is maintained by the SeedSigner community and updated regularly. For the latest version and additional resources, visit the official SeedSigner GitHub repository.*
