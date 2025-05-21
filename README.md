# SeedSigner Navigation Guide with WaveShare LCD Hat Controls

<div align="center">
  <img src="images/SeedSigner_Logo.png" alt="SeedSigner Logo" width="400"/>
</div>

This guide provides step-by-step instructions for navigating all screens in the SeedSigner interface using the WaveShare 1.3inch LCD Hat. Each section contains detailed navigation paths and button control instructions to help users access every screen available in the SeedSigner firmware.

## Hardware Components

A SeedSigner device consists of:

1. Raspberry Pi Zero
2. Raspberry Pi Camera
3. WaveShare 1.3inch LCD Hat

## WaveShare LCD Hat Controls

<div align="center">
  <img src="images/WaveShare_LCD_Hat.png" alt="WaveShare LCD Hat" width="350"/>
</div>

The WaveShare LCD Hat has the following controls:

- **Joystick**: Used for navigating menus (Up, Down, Left, Right)
- **Key1 (A)**: Primary select/confirm button
- **Key2 (B)**: Back/cancel button
- **Key3 (C)**: Context-specific functions

### Button Functions

| Button         | Function                                      |
| -------------- | --------------------------------------------- |
| Joystick Up    | Move selection up                             |
| Joystick Down  | Move selection down                           |
| Joystick Left  | Move selection left or go back                |
| Joystick Right | Move selection right or advance               |
| Key1 (A)       | Select highlighted option or confirm action   |
| Key2 (B)       | Go back to previous screen or cancel action   |
| Key3 (C)       | Context-specific functions (varies by screen) |

## Table of Contents

- [Startup and Main Menu](#startup-and-main-menu)
- [Seed Management](#seed-management)
  - [Seed Creation and Loading](#seed-creation-and-loading)
  - [Seed Options and Management](#seed-options-and-management)
  - [Seed Backup and Export](#seed-backup-and-export)
  - [Multisig and Address Verification](#multisig-and-address-verification)
  - [Message Signing](#message-signing)
- [Transaction Signing (PSBT)](#transaction-signing-psbt)
- [Tools](#tools)
- [Settings](#settings)
- [Power Options](#power-options)
- [Error Screens](#error-screens)

## Startup and Main Menu

### Startup Process

1. **Power on the SeedSigner**

   <div align="center">
     <img src="images/MainMenuViews/OpeningSplashView.png" alt="Opening Splash Screen" width="300"/>
   </div>

   - Connect power to the device
   - You'll see the opening splash screen as shown above
   - **Controls**: No action required, wait for the splash screen to transition automatically

   <div align="center">
     <img src="images/MainMenuViews/OpeningSplashView_no_partner_logos.png" alt="Opening Splash Screen without Partner Logos" width="300"/>
   </div>

   - If partner logos are disabled, you'll see the alternate splash screen shown above

2. **Main Menu**

   <div align="center">
     <img src="images/MainMenuViews/MainMenuView.png" alt="Main Menu View" width="300"/>
   </div>

   - After the splash screen, you'll be taken to the main menu
   - **Controls**:
     - Use the **Joystick** to navigate between menu options
     - Press **Key1 (A)** to select a menu option
     - Press **Key2 (B)** to go back (if applicable)

### SD Card Notifications

1. **SD Card Removal Detected**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/home__sd_card_removed_toast.png" alt="SD Card Removed Toast" width="300"/>
   </div>

   - If an SD card is removed while the device is on, you'll see this notification
   - **Controls**: No action required, notification will disappear automatically

2. **SD Card Insertion Detected**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/home__sd_card_inserted_toast.png" alt="SD Card Inserted Toast" width="300"/>
   </div>

   - If an SD card is inserted while the device is on, you'll see this notification
   - **Controls**: No action required, notification will disappear automatically

3. **Remove SD Card Prompt**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/home__remove_sd_card_toast.png" alt="Remove SD Card Toast" width="300"/>
   </div>

   - In certain situations, you may be prompted to remove the SD card
   - **Controls**: Remove the SD card as instructed, then press **Key1 (A)** to continue

### Power Options

1. **Accessing Power Menu**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__power.png" alt="Power Options View" width="300"/>
   </div>

   - From the main menu, use the **Joystick** to navigate to the power icon (top right)
   - Press **Key1 (A)** to select
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between power options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back to the main menu

2. **Restart Device**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__restart.png" alt="Restart View" width="300"/>
   </div>

   - From the power menu, use the **Joystick** to select "Restart"
   - Press **Key1 (A)** to confirm
   - **Controls**: Press **Key1 (A)** to confirm restart or **Key2 (B)** to cancel

3. **Power Off Device**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__power_off.png" alt="Power Off View" width="300"/>
   </div>

   - From the power menu, use the **Joystick** to select "Power Off"
   - Press **Key1 (A)** to confirm
   - **Controls**: Press **Key1 (A)** to confirm power off or **Key2 (B)** to cancel

## Seed Management

### Seed Creation and Loading

1. **Accessing Seeds Menu**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__create_or_load.png" alt="Seeds Menu View" width="300"/>
   </div>

   - From the main menu, use the **Joystick** to navigate to the seeds icon (top left)
   - Press **Key1 (A)** to select
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between seed options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back to the main menu

2. **Loading an Existing Seed**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__load_seed.png" alt="Load Seed View" width="300"/>
   </div>

   - From the Seeds menu, use the **Joystick** to select "Load Seed"
   - Press **Key1 (A)** to confirm
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between load options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back to the seeds menu

3. **Entering a Seed Phrase**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__mnemonic_entry.png" alt="Seed Mnemonic Entry View" width="300"/>
   </div>

   - If you select "Enter 12-Word Seed" or "Enter 24-Word Seed", you'll see this screen
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a letter or button
     - Press **Key2 (B)** to delete the last letter
     - Press **Key3 (C)** to toggle between word suggestion lists
     - Navigate to "OK" and press **Key1 (A)** when done

4. **Invalid Seed Warning**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__mnemonic_invalid.png" alt="Seed Mnemonic Invalid View" width="300"/>
   </div>

   - If the entered seed is invalid, you'll see this warning
   - **Controls**: Press **Key1 (A)** to acknowledge and try again

5. **Finalizing Seed**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__finalize.png" alt="Seed Finalize View" width="300"/>
   </div>

   - After entering a valid seed, you'll be taken to this screen to confirm
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back

### Seed Passphrase Management

1. **Adding a Passphrase (Lowercase)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_lowercase.png" alt="Seed Add Passphrase View (Lowercase)" width="300"/>
   </div>

   - If you choose to add a passphrase, you'll start with the lowercase keyboard
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a letter or button
     - Press **Key2 (B)** to delete the last character
     - Use **Joystick** to navigate to "abc" and press **Key1 (A)** to switch to uppercase

2. **Adding a Passphrase (Uppercase)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_uppercase.png" alt="Seed Add Passphrase View (Uppercase)" width="300"/>
   </div>

   - Switch to uppercase by selecting the "abc" button
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a letter or button
     - Press **Key2 (B)** to delete the last character
     - Use **Joystick** to navigate to "123" and press **Key1 (A)** to switch to digits

3. **Adding a Passphrase (Digits)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_digits.png" alt="Seed Add Passphrase View (Digits)" width="300"/>
   </div>

   - Switch to digits by selecting the "123" button
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a digit or button
     - Press **Key2 (B)** to delete the last character
     - Use **Joystick** to navigate to "#$%" and press **Key1 (A)** to switch to symbols

4. **Adding a Passphrase (Symbols 1)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_symbols_1.png" alt="Seed Add Passphrase View (Symbols 1)" width="300"/>
   </div>

   - Switch to symbols by selecting the "#$%" button
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a symbol or button
     - Press **Key2 (B)** to delete the last character
     - Use **Joystick** to navigate to "→" and press **Key1 (A)** to see more symbols

5. **Adding a Passphrase (Symbols 2)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_symbols_2.png" alt="Seed Add Passphrase View (Symbols 2)" width="300"/>
   </div>

   - Access additional symbols by selecting the "→" button
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a symbol or button
     - Press **Key2 (B)** to delete the last character
     - Navigate to "DONE" and press **Key1 (A)** when finished

6. **Passphrase Exit Dialog**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_exit_dialog.png" alt="Seed Add Passphrase Exit Dialog View" width="300"/>
   </div>

   - If you try to exit while entering a passphrase, you'll see this confirmation
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Exit"
     - Press **Key1 (A)** to confirm your selection

7. **Reviewing Passphrase**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__review_passphrase.png" alt="Seed Review Passphrase View" width="300"/>
   </div>

   - After entering a passphrase, you'll be asked to review it
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back

### Seed Options and Management

1. **Seed Options Menu**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__seed_options.png" alt="Seed Options View" width="300"/>
   </div>

   - After loading or creating a seed, you'll see the seed options
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back to the previous menu

2. **Seed Backup Options**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__backup.png" alt="Seed Backup View" width="300"/>
   </div>

   - If you select "Backup Seed" from the seed options, you'll see these options
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back to seed options

### Seed Export and Xpub Management

1. **Export Xpub Signature Type Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_sig_type.png" alt="Seed Export Xpub Sig Type View" width="300"/>
   </div>

   - When exporting an Xpub, first select the signature type
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between signature types
     - Press **Key1 (A)** to select a signature type
     - Press **Key2 (B)** to go back

2. **Export Xpub Script Type Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_script_type.png" alt="Seed Export Xpub Script Type View" width="300"/>
   </div>

   - Then select the script type
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between script types
     - Press **Key1 (A)** to select a script type
     - Press **Key2 (B)** to go back

3. **Custom Derivation Path**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_custom_derivation.png" alt="Seed Export Xpub Custom Derivation View" width="300"/>
   </div>

   - If needed, you can set a custom derivation path
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard and input numbers
     - Press **Key1 (A)** to select a character or button
     - Press **Key2 (B)** to delete the last character
     - Navigate to "DONE" and press **Key1 (A)** when finished

4. **Selecting Coordinator**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_coordinator.png" alt="Seed Export Xpub Coordinator View" width="300"/>
   </div>

   - Select which wallet coordinator to use
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between coordinators
     - Press **Key1 (A)** to select a coordinator
     - Press **Key2 (B)** to go back

5. **Xpub Export Warning**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_warning.png" alt="Seed Export Xpub Warning View" width="300"/>
   </div>

   - Before exporting, you'll see this privacy warning
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **Key1 (A)** to confirm your selection

6. **Xpub Details**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_details.png" alt="Seed Export Xpub Details View" width="300"/>
   </div>

   - View the xpub details before finalizing
   - **Controls**:
     - Use the **Joystick Up/Down** to scroll through the details
     - Press **Key1 (A)** to continue to the QR code
     - Press **Key2 (B)** to go back

### Seed Words Management

1. **Seed Words Warning**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_warning.png" alt="Seed Words Warning View" width="300"/>
   </div>

   - Before showing seed words, you'll see this privacy warning
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **Key1 (A)** to confirm your selection

2. **Seed Words View (Page 1)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words.png" alt="Seed Words View" width="300"/>
   </div>

   - First page of seed words
   - **Controls**:
     - Press **Key1 (A)** to proceed to the next page or finish
     - Press **Key2 (B)** to go back
     - Use **Joystick Right** to advance to the next page (if available)

3. **Seed Words View (Page 2)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_2.png" alt="Seed Words View (Page 2)" width="300"/>
   </div>

   - Second page of seed words (for 24-word seeds)
   - **Controls**:
     - Press **Key1 (A)** to finish
     - Press **Key2 (B)** to go back to page 1
     - Use **Joystick Left** to go back to the previous page

### BIP85 Child Seed Generation

1. **BIP85 Application Mode**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__bip85_application_mode.png" alt="Seed BIP85 Application Mode View" width="300"/>
   </div>

   - Select which application to generate a child seed for
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between applications
     - Press **Key1 (A)** to select an application
     - Press **Key2 (B)** to go back

2. **BIP85 Child Index Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__bip85_select_child_index.png" alt="Seed BIP85 Select Child Index View" width="300"/>
   </div>

   - Select the index number for the child seed
   - **Controls**:
     - Use the **Joystick** to navigate the number pad
     - Press **Key1 (A)** to select a digit
     - Press **Key2 (B)** to delete the last digit
     - Navigate to "OK" and press **Key1 (A)** when finished

3. **BIP85 Invalid Child Index**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__bip85_invalid_child_index.png" alt="Seed BIP85 Invalid Child Index View" width="300"/>
   </div>

   - If you enter an invalid index, you'll see this error
   - **Controls**: Press **Key1 (A)** to acknowledge and try again

### Seed Words Backup Test

1. **Backup Test Prompt**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test_prompt.png" alt="Seed Words Backup Test Prompt View" width="300"/>
   </div>

   - If you choose to test your backup, you'll see this prompt
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **Key1 (A)** to confirm your selection

2. **Backup Test Entry**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test.png" alt="Seed Words Backup Test View" width="300"/>
   </div>

   - Enter your backed-up seed words to test them
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a letter or button
     - Press **Key2 (B)** to delete the last letter
     - Press **Key3 (C)** to toggle between word suggestion lists
     - Navigate to "OK" and press **Key1 (A)** when done

3. **Backup Test Mistake**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test_mistake.png" alt="Seed Words Backup Test Mistake View" width="300"/>
   </div>

   - If you make a mistake, you'll see this warning
   - **Controls**: Press **Key1 (A)** to acknowledge and try again

4. **Backup Test Success**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test_success.png" alt="Seed Words Backup Test Success View" width="300"/>
   </div>

   - If successful, you'll see this confirmation
   - **Controls**: Press **Key1 (A)** to continue

### SeedQR Management

1. **SeedQR Format Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_format.png" alt="Seed Transcribe SeedQR Format View" width="300"/>
   </div>

   - When working with SeedQR, select the format
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between formats
     - Press **Key1 (A)** to select a format
     - Press **Key2 (B)** to go back

2. **SeedQR Warning**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_warning.png" alt="Seed Transcribe SeedQR Warning View" width="300"/>
   </div>

   - Before proceeding, you'll see this warning
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **Key1 (A)** to confirm your selection

3. **SeedQR Display (12-word Compact)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_whole_qr_12_compact.png" alt="Seed Transcribe SeedQR Whole QR View (12-word Compact)" width="300"/>
   </div>

   - View the SeedQR for a 12-word seed in compact format
   - **Controls**:
     - Press **Key1 (A)** to zoom in
     - Press **Key2 (B)** to go back
     - Press **Key3 (C)** to proceed to the next step

4. **SeedQR Zoomed In View**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_zoomed_in_12_compact.png" alt="Seed Transcribe SeedQR Zoomed In View (12-word Compact)" width="300"/>
   </div>

   - View a zoomed-in portion of a SeedQR
   - **Controls**:
     - Use the **Joystick** to pan across the QR code
     - Press **Key1 (A)** to zoom out
     - Press **Key2 (B)** to go back

5. **SeedQR Confirmation Prompt**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_confirm_qr_prompt.png" alt="Seed Transcribe SeedQR Confirm QR Prompt View" width="300"/>
   </div>

   - When verifying a SeedQR, you'll see this prompt
   - **Controls**:
     - Use the **Joystick Left/Right** to select an option
     - Press **Key1 (A)** to confirm your selection

### Multisig and Address Verification

1. **Seed Selection for Address Verification**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__select_seed_address_verification.png" alt="Seed Select Seed View (Address Verification)" width="300"/>
   </div>

   - Select which seed to use for address verification
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between seeds
     - Press **Key1 (A)** to select a seed
     - Press **Key2 (B)** to go back

2. **Address Verification Signature Type Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__address_verification_sig_type.png" alt="Address Verification Sig Type View" width="300"/>
   </div>

   - Select the signature type for address verification
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between signature types
     - Press **Key1 (A)** to select a signature type
     - Press **Key2 (B)** to go back

3. **Address Verification**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__address_verification.png" alt="Seed Address Verification View" width="300"/>
   </div>

   - Verify the address matches the expected value
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back

4. **Address Verification Success**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__address_verification_success.png" alt="Seed Address Verification Success View" width="300"/>
   </div>

   - If the address is verified, you'll see this confirmation
   - **Controls**: Press **Key1 (A)** to continue

### Message Signing

1. **Seed Selection for Message Signing**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__select_seed_sign_message.png" alt="Seed Select Seed View (Sign Message)" width="300"/>
   </div>

   - Select which seed to use for signing a message
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between seeds
     - Press **Key1 (A)** to select a seed
     - Press **Key2 (B)** to go back

2. **Message Signing Confirmation**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__sign_message_confirm_message.png" alt="Seed Sign Message Confirm Message View" width="300"/>
   </div>

   - Confirm the message content that you want to sign
   - **Controls**:
     - Use the **Joystick Up/Down** to scroll through the message if needed
     - Press **Key1 (A)** to confirm and sign the message
     - Press **Key2 (B)** to cancel and go back

3. **Message Signing Script Type Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__sign_message_script_type.png" alt="Seed Sign Message Script Type View" width="300"/>
   </div>

   - Select the script type for message signing
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between script types
     - Press **Key1 (A)** to select a script type
     - Press **Key2 (B)** to go back

4. **Message Signing Address Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__sign_message_address_index.png" alt="Seed Sign Message Address Index View" width="300"/>
   </div>

   - Select the address index for message signing
   - **Controls**:
     - Use the **Joystick Up/Down** to increase/decrease the address index
     - Press **Key1 (A)** to confirm the selected address index
     - Press **Key2 (B)** to go back

5. **Message Signature QR Code Display**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__sign_message_signature_qr.png" alt="Seed Sign Message Signature QR View" width="300"/>
   </div>

   - The QR code containing the signed message is displayed
   - **Controls**:
     - Press **Key1 (A)** to zoom in on the QR code
     - Press **Key2 (B)** to go back
     - Press **Key3 (C)** to toggle to text view of the signature

6. **Message Signature Text Display**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__sign_message_signature_text.png" alt="Seed Sign Message Signature Text View" width="300"/>
   </div>

   - View the text representation of the signature
   - **Controls**:
     - Use the **Joystick Up/Down** to scroll through the signature text
     - Press **Key1 (A)** to continue
     - Press **Key2 (B)** to go back
     - Press **Key3 (C)** to toggle back to QR code view

## Transaction Signing (PSBT)

1. **Accessing PSBT Signing**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/transaction__main.png" alt="Transaction Main View" width="300"/>
   </div>

   - From the main menu, use the **Joystick** to navigate to the Transaction icon
   - Press **Key1 (A)** to select
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back to the main menu

2. **Scan QR PSBT Loading**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/transaction__scan_qr_progress.png" alt="Transaction Scan QR Progress View" width="300"/>
   </div>

   - When scanning a QR PSBT, you'll see this loading screen
   - **Controls**: No action required, hold the camera steady pointing at the QR code

3. **PSBT Loading from SD Card**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/transaction__select_psbt_from_sd_card.png" alt="Transaction Select PSBT from SD Card View" width="300"/>
   </div>

   - If loading from SD card, select the PSBT file
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between files
     - Press **Key1 (A)** to select a file
     - Press **Key2 (B)** to go back

4. **PSBT Processing**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/transaction__preparing_psbt.png" alt="Transaction Preparing PSBT View" width="300"/>
   </div>

   - After scanning/selecting a PSBT, it will be processed
   - **Controls**: No action required, wait for processing to complete

5. **Seed Selection for PSBT Signing**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/transaction__select_seed_sign_psbt.png" alt="Transaction Select Seed View" width="300"/>
   </div>

   - Select which seed to use for signing the transaction
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between seeds
     - Press **Key1 (A)** to select a seed
     - Press **Key2 (B)** to go back

6. **PSBT Transaction Overview**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/transaction__overview.png" alt="Transaction Overview View" width="300"/>
   </div>

   - Review the transaction overview before signing
   - **Controls**:
     - Use the **Joystick** to navigate to "Continue" or "Cancel"
     - Press **Key1 (A)** to select your choice
     - Press **Key2 (B)** to go back

7. **PSBT Output Details**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/transaction__output_details.png" alt="Transaction Output Details View" width="300"/>
   </div>

   - Review the transaction output details
   - **Controls**:
     - Use the **Joystick Up/Down** to scroll through outputs if needed
     - Press **Key1 (A)** to continue to the next step
     - Press **Key2 (B)** to go back

8. **PSBT Signing Confirmation**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/transaction__sign_psbt.png" alt="Transaction Sign PSBT View" width="300"/>
   </div>

   - Final confirmation before signing the transaction
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Sign"
     - Press **Key1 (A)** to confirm your selection

9. **Signed PSBT QR Code Display**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/transaction__sign_psbt_qr.png" alt="Transaction Sign PSBT QR View" width="300"/>
   </div>

   - View the QR code for the signed PSBT
   - **Controls**:
     - Press **Key1 (A)** to zoom in on the QR code
     - Press **Key2 (B)** to go back
     - Press **Key3 (C)** to toggle to file save options

10. **Signed PSBT File Save Options**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/transaction__sign_psbt_file_options.png" alt="Transaction Sign PSBT File Options View" width="300"/>
   </div>

   - Choose how to save the signed PSBT
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back
     - Press **Key3 (C)** to toggle back to QR code view

## Tools

1. **Accessing Tools Menu**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__main.png" alt="Tools Main View" width="300"/>
   </div>

   - From the main menu, use the **Joystick** to navigate to the Tools icon
   - Press **Key1 (A)** to select
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between tools
     - Press **Key1 (A)** to select a tool
     - Press **Key2 (B)** to go back to the main menu

2. **Dice Tool Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__dice_rolls.png" alt="Tools Dice Rolls View" width="300"/>
   </div>

   - Use dice to generate randomness for seed creation
   - **Controls**:
     - Use the **Joystick** to navigate the number pad
     - Press **Key1 (A)** to select a number
     - Press **Key2 (B)** to delete the last number
     - Navigate to "OK" and press **Key1 (A)** when finished

3. **Coin Flip Tool**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__coin_flips.png" alt="Tools Coin Flips View" width="300"/>
   </div>

   - Use coin flips to generate randomness for seed creation
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Heads" or "Tails"
     - Press **Key1 (A)** to confirm each flip
     - Press **Key2 (B)** to undo the last flip
     - Continue until you have enough flips

4. **Calculator Tool**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__calculator.png" alt="Tools Calculator View" width="300"/>
   </div>

   - Use the built-in calculator
   - **Controls**:
     - Use the **Joystick** to navigate the calculator keypad
     - Press **Key1 (A)** to select a button
     - Press **Key2 (B)** to clear the last entry or go back
     - Use **Key3 (C)** for additional functions (if available)

## Settings

1. **Accessing Settings Menu**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__main.png" alt="Settings Main View" width="300"/>
   </div>

   - From the main menu, use the **Joystick** to navigate to the Settings icon
   - Press **Key1 (A)** to select
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between settings
     - Press **Key1 (A)** to select a setting
     - Press **Key2 (B)** to go back to the main menu

2. **QR Code Settings**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__qr.png" alt="Settings QR View" width="300"/>
   </div>

   - Configure QR code-related settings
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back

3. **Display Settings**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__display.png" alt="Settings Display View" width="300"/>
   </div>

   - Configure display-related settings
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back

4. **Display Rotation Setting**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__display_rotation.png" alt="Settings Display Rotation View" width="300"/>
   </div>

   - Adjust the display rotation angle
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between rotation options
     - Press **Key1 (A)** to select a rotation option
     - Press **Key2 (B)** to go back

5. **Display Brightness Setting**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__display_brightness.png" alt="Settings Display Brightness View" width="300"/>
   </div>

   - Adjust the display brightness
   - **Controls**:
     - Use the **Joystick Left/Right** to decrease/increase brightness
     - Press **Key1 (A)** to confirm the selected brightness
     - Press **Key2 (B)** to go back

6. **Language Settings**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__language.png" alt="Settings Language View" width="300"/>
   </div>

   - Select the interface language
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between languages
     - Press **Key1 (A)** to select a language
     - Press **Key2 (B)** to go back

7. **Factory Reset**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__factory_reset.png" alt="Settings Factory Reset View" width="300"/>
   </div>

   - Restore factory default settings
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Reset"
     - Press **Key1 (A)** to confirm your selection

## Error Screens

1. **Camera Error**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/error__camera.png" alt="Error Camera View" width="300"/>
   </div>

   - If there's an issue with the camera, you'll see this error
   - **Controls**: Press **Key1 (A)** to acknowledge and try to resolve the issue

2. **SD Card Error**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/error__sd_card.png" alt="Error SD Card View" width="300"/>
   </div>

   - If there's an issue with the SD card, you'll see this error
   - **Controls**: Press **Key1 (A)** to acknowledge and try to resolve the issue

3. **Invalid QR Code Error**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/error__invalid_qr.png" alt="Error Invalid QR View" width="300"/>
   </div>

   - If an invalid QR code is scanned, you'll see this error
   - **Controls**: Press **Key1 (A)** to acknowledge and try again

## Troubleshooting Tips

1. **If the screen is not responding:**
   - Check that the WaveShare LCD Hat is properly connected to the Raspberry Pi Zero
   - Make sure the device has adequate power supply

2. **If the camera is not working:**
   - Ensure the ribbon cable is properly connected to both the camera and the Raspberry Pi Zero
   - Check that the camera is enabled in the SeedSigner settings

3. **If QR codes are not scanning properly:**
   - Ensure adequate lighting in the room
   - Hold the QR code steady and at a proper distance from the camera
   - Make sure the QR code is within the guide markers on the screen
   - Clean the camera lens if it appears dirty or smudged

4. **If the SD card is not being recognized:**
   - Try reformatting the SD card to FAT32
   - Ensure the SD card is properly inserted
   - Try a different SD card to rule out hardware issues

5. **If the device is behaving erratically:**
   - Try restarting the device
   - Consider performing a factory reset through the settings menu
   - Check for firmware updates on the SeedSigner website

## Conclusion

This comprehensive navigation guide covers all the screens and functions available in the SeedSigner interface using the WaveShare 1.3inch LCD Hat controls. By following this guide, users can efficiently navigate the SeedSigner menus and perform various Bitcoin-related operations securely.

Remember that the SeedSigner is an airgapped device designed to enhance the security of your Bitcoin operations. Always ensure your environment is private and secure when working with sensitive information like seed phrases and private keys.

For the latest updates and more information, visit the official SeedSigner documentation and community resources.