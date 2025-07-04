# SeedSigner User Guide

<div align="center">
  <img src="images/SeedSigner_Logo.png" alt="SeedSigner Logo" width="400"/>
</div>

SeedSigner is an air-gapped, open-source Bitcoin signing device that helps you manage seed phrases and sign transactions securely. This guide provides step-by-step instructions organized by common workflows.

## 📋 Table of Contents

### 🚀 Getting Started

- [Initial Setup and Power On](/guides/en/getting_started/initial_setup_and_power_on.md)
- [Navigation Basics](/guides/en/getting_started/navigation_basics.md)
- [Powering Off Safely](/guides/en/getting_started/powering_off_safely.md)
- [Restarting Your Device](/guides/en/getting_started/restarting_your_device.md)

### 🌱 Seed Management

- **Creating New Seeds**
  - [Camera-Based Seed Generation](/guides/en/seed_management/creating_new_seeds/camera_based_seed_generation.md)
  - [Dice-Based Seed Generation](/guides/en/seed_management/creating_new_seeds/dice_based_seed_generation.md)
  - [Calc 12th/24th Word Seed Generation](/guides/en/seed_management/creating_new_seeds/calc_12th24th_word_seed_generation.md)
- **Loading Existing Seeds**
  - [Manual Seed Entry](/guides/en/seed_management/load_existing_seeds/manual_seed_entry.md)
  - [SeedQR Scanning](/guides/en/seed_management/load_existing_seeds/seedqr_scanning.md)
  - [Adding BIP-39 Passphrase](/guides/en/seed_management/load_existing_seeds/adding_bip_39_passphrase.md)

### 🔧 Working with Loaded Seeds

- [Export Public Key (Xpub)](/guides/en/working_with_loaded_seeds/export_public_key_xpub.md)
- [Generate Receiving Addresses](/guides/en/working_with_loaded_seeds/generate_receiving_addresses.md)
- [Generate Change Addresses](/guides/en/working_with_loaded_seeds/generate_change_addresses.md)
- [View Seed Words](/guides/en/working_with_loaded_seeds/view_seed_words.md)
- [Create SeedQR Backup](/guides/en/working_with_loaded_seeds/create_seedqr_backup.md)

### ✍️ Transactions & Verification

- [Sign Bitcoin Transaction (PSBT)](/guides/en/transactions_and_verification/sign_bitcoin_transaction_psbt.md)
- [Verify Address Ownership](/guides/en/transactions_and_verification/verify_address_ownership.md)
- [Discard Loaded Seed](/guides/en/transactions_and_verification/discard_loaded_seed.md)

### ⚙️ Device Configuration

- **Basic Settings**
  - [Language Configuration](/guides/en/device_configuration/basic_settings/language_configuration.md)
  - [Persistent Settings](/guides/en/device_configuration/basic_settings/persistent_settings.md)
  - [Coordinator Software Support](/guides/en/device_configuration/basic_settings/coordinator_software_support.md)
  - [Denomination Display](/guides/en/device_configuration/basic_settings/denomination_display.md)
  - [Hardware I/O Testing](/guides/en/device_configuration/basic_settings/hardware_io_testing.md)
  - [Donation Information](/guides/en/device_configuration/basic_settings/donation_information.md)

- **Advanced Settings**
  - [Bitcoin Network Selection](/guides/en/device_configuration/advanced_settings/bitcoin_network_selection.md)
  - [QR Code Density](/guides/en/device_configuration/advanced_settings/qr_code_density.md)
  - [Xpub Export Configuration](/guides/en/device_configuration/advanced_settings/xpub_export_configuration.md)
  - [Signature Types Configuration](/guides/en/device_configuration/advanced_settings/signature_types_configuration.md)
  - [Script Types Configuration](/guides/en/device_configuration/advanced_settings/script_types_configuration.md)
  - [Show Xpub Details](/guides/en/device_configuration/advanced_settings/show_xpub_details.md)
  - [BIP-39 Passphrase Configuration](/guides/en/device_configuration/advanced_settings/bip-39_passphrase_configuration.md)
  - [Camera Rotation](/guides/en/device_configuration/advanced_settings/camera_rotation.md)
  - [Compact SeedQR](/guides/en/device_configuration/advanced_settings/compact_seedqr.md)
  - [BIP-85 Child Seeds](/guides/en/device_configuration/advanced_settings/bip-85_child_seeds.md)
  - [Electrum Seeds](/guides/en/device_configuration/advanced_settings/electrum_seeds.md)
  - [Message Signing](/guides/en/device_configuration/advanced_settings/message_signing.md)
  - [Privacy Warnings](/guides/en/device_configuration/advanced_settings/privacy_warnings.md)
  - [Dire Warnings](/guides/en/device_configuration/advanced_settings/dire_warnings.md)
  - [QR Brightness Tips](/guides/en/device_configuration/advanced_settings/qr_brightness_tips.md)
  - [Partner Logos](/guides/en/device_configuration/advanced_settings/partner_logos.md)

- **Hardware Settings**
  - [Display Type Configuration](/guides/en/device_configuration/hardware_settings/display_type_configuration.md)
  - [Color Inversion](/guides/en/device_configuration/hardware_settings/color_inversion.md)

### 🔧 Support & Resources

- [Troubleshooting](/guides/en/support_and_resources/troubleshooting.md)
- [Additional Resources](/guides/en/support_and_resources/additional_resources.md)
- [Security Considerations](/guides/en/support_and_resources/security_considerations.md)

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
