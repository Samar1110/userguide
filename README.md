# SeedSigner Navigation Guide with WaveShare LCD Hat Controls

![SeedSigner Logo](images/SeedSigner_Logo.png)

This guide provides step-by-step instructions for navigating all screens in the SeedSigner interface using the WaveShare 1.3inch LCD Hat. Each section contains detailed navigation paths and button control instructions to help users access every screen available in the SeedSigner firmware.

## Hardware Components

A SeedSigner device consists of:

1. Raspberry Pi Zero
2. Raspberry Pi Camera
3. WaveShare 1.3inch LCD Hat

## WaveShare LCD Hat Controls

![WaveShare LCD Hat](https://www.waveshare.com/w/upload/5/51/1.3inch_LCD_HAT-1.jpg)

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

   - Connect power to the device
   - You'll see the opening splash screen
     ![OpeningSplashView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/home__splash.png)
   - If partner logos are disabled, you'll see an alternate splash screen
     ![OpeningSplashView_no_partner_logos](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/home__splash_no_partner_logos.png)
   - **Controls**: No action required, wait for the splash screen to transition automatically

2. **Main Menu**
   - After the splash screen, you'll be taken to the main menu
     ![MainMenuView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/home__home.png)
   - **Controls**:
     - Use the **Joystick** to navigate between menu options
     - Press **Key1 (A)** to select a menu option
     - Press **Key2 (B)** to go back (if applicable)

### SD Card Notifications

1. **SD Card Removal Detected**

   - If an SD card is removed while the device is on, you'll see this notification
     ![MainMenuView_SDCardStateChangeToast_removed](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/home__sd_card_removed_toast.png)
   - **Controls**: No action required, notification will disappear automatically

2. **SD Card Insertion Detected**

   - If an SD card is inserted while the device is on, you'll see this notification
     ![MainMenuView_SDCardStateChangeToast_inserted](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/home__sd_card_inserted_toast.png)
   - **Controls**: No action required, notification will disappear automatically

3. **Remove SD Card Prompt**
   - In certain situations, you may be prompted to remove the SD card
     ![MainMenuView_RemoveSDCardToast](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/home__remove_sd_card_toast.png)
   - **Controls**: Remove the SD card as instructed, then press **Key1 (A)** to continue

### Power Options

1. **Accessing Power Menu**

   - From the main menu, use the **Joystick** to navigate to the power icon (top right)
   - Press **Key1 (A)** to select
     ![PowerOptionsView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__power.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between power options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back to the main menu

2. **Restart Device**

   - From the power menu, use the **Joystick** to select "Restart"
   - Press **Key1 (A)** to confirm
     ![RestartView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__restart.png)
   - **Controls**: Press **Key1 (A)** to confirm restart or **Key2 (B)** to cancel

3. **Power Off Device**
   - From the power menu, use the **Joystick** to select "Power Off"
   - Press **Key1 (A)** to confirm
     ![PowerOffView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__power_off.png)
   - **Controls**: Press **Key1 (A)** to confirm power off or **Key2 (B)** to cancel

## Seed Management

### Seed Creation and Loading

1. **Accessing Seeds Menu**

   - From the main menu, use the **Joystick** to navigate to the seeds icon (top left)
   - Press **Key1 (A)** to select
     ![SeedsMenuView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__create_or_load.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between seed options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back to the main menu

2. **Loading an Existing Seed**

   - From the Seeds menu, use the **Joystick** to select "Load Seed"
   - Press **Key1 (A)** to confirm
     ![LoadSeedView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__load_seed.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between load options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back to the seeds menu

3. **Entering a Seed Phrase**

   - If you select "Enter 12-Word Seed" or "Enter 24-Word Seed", you'll see this screen
     ![SeedMnemonicEntryView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__mnemonic_entry.png)
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a letter or button
     - Press **Key2 (B)** to delete the last letter
     - Press **Key3 (C)** to toggle between word suggestion lists
     - Navigate to "OK" and press **Key1 (A)** when done

4. **Invalid Seed Warning**

   - If the entered seed is invalid, you'll see this warning
     ![SeedMnemonicInvalidView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__mnemonic_invalid.png)
   - **Controls**: Press **Key1 (A)** to acknowledge and try again

5. **Finalizing Seed**
   - After entering a valid seed, you'll be taken to this screen to confirm
     ![SeedFinalizeView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__finalize.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back

### Seed Passphrase Management

1. **Adding a Passphrase (Lowercase)**

   - If you choose to add a passphrase, you'll start with the lowercase keyboard
     ![SeedAddPassphraseView_lowercase](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_lowercase.png)
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a letter or button
     - Press **Key2 (B)** to delete the last character
     - Use **Joystick** to navigate to "abc" and press **Key1 (A)** to switch to uppercase

2. **Adding a Passphrase (Uppercase)**

   - Switch to uppercase by selecting the "abc" button
     ![SeedAddPassphraseView_uppercase](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_uppercase.png)
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a letter or button
     - Press **Key2 (B)** to delete the last character
     - Use **Joystick** to navigate to "123" and press **Key1 (A)** to switch to digits

3. **Adding a Passphrase (Digits)**

   - Switch to digits by selecting the "123" button
     ![SeedAddPassphraseView_digits](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_digits.png)
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a digit or button
     - Press **Key2 (B)** to delete the last character
     - Use **Joystick** to navigate to "#$%" and press **Key1 (A)** to switch to symbols

4. **Adding a Passphrase (Symbols 1)**

   - Switch to symbols by selecting the "#$%" button
     ![SeedAddPassphraseView_symbols_1](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_symbols_1.png)
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a symbol or button
     - Press **Key2 (B)** to delete the last character
     - Use **Joystick** to navigate to "→" and press **Key1 (A)** to see more symbols

5. **Adding a Passphrase (Symbols 2)**

   - Access additional symbols by selecting the "→" button
     ![SeedAddPassphraseView_symbols_2](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_symbols_2.png)
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a symbol or button
     - Press **Key2 (B)** to delete the last character
     - Navigate to "DONE" and press **Key1 (A)** when finished

6. **Passphrase Exit Dialog**

   - If you try to exit while entering a passphrase, you'll see this confirmation
     ![SeedAddPassphraseExitDialogView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_exit_dialog.png)
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Exit"
     - Press **Key1 (A)** to confirm your selection

7. **Reviewing Passphrase**
   - After entering a passphrase, you'll be asked to review it
     ![SeedReviewPassphraseView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__review_passphrase.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back

### Seed Options and Management

1. **Seed Options Menu**

   - After loading or creating a seed, you'll see the seed options
     ![SeedOptionsView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__seed_options.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back to the previous menu

2. **Seed Backup Options**
   - If you select "Backup Seed" from the seed options, you'll see these options
     ![SeedBackupView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__backup.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back to seed options

### Seed Export and Xpub Management

1. **Export Xpub Signature Type Selection**

   - When exporting an Xpub, first select the signature type
     ![SeedExportXpubSigTypeView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_sig_type.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between signature types
     - Press **Key1 (A)** to select a signature type
     - Press **Key2 (B)** to go back

2. **Export Xpub Script Type Selection**

   - Then select the script type
     ![SeedExportXpubScriptTypeView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_script_type.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between script types
     - Press **Key1 (A)** to select a script type
     - Press **Key2 (B)** to go back

3. **Custom Derivation Path**

   - If needed, you can set a custom derivation path
     ![SeedExportXpubCustomDerivationView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_custom_derivation.png)
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard and input numbers
     - Press **Key1 (A)** to select a character or button
     - Press **Key2 (B)** to delete the last character
     - Navigate to "DONE" and press **Key1 (A)** when finished

4. **Selecting Coordinator**

   - Select which wallet coordinator to use
     ![SeedExportXpubCoordinatorView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_coordinator.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between coordinators
     - Press **Key1 (A)** to select a coordinator
     - Press **Key2 (B)** to go back

5. **Xpub Export Warning**

   - Before exporting, you'll see this privacy warning
     ![SeedExportXpubWarningView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_warning.png)
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **Key1 (A)** to confirm your selection

6. **Xpub Details**
   - View the xpub details before finalizing
     ![SeedExportXpubDetailsView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_details.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to scroll through the details
     - Press **Key1 (A)** to continue to the QR code
     - Press **Key2 (B)** to go back

### Seed Words Management

1. **Seed Words Warning**

   - Before showing seed words, you'll see this privacy warning
     ![SeedWordsWarningView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_warning.png)
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **Key1 (A)** to confirm your selection

2. **Seed Words View (Page 1)**

   - First page of seed words
     ![SeedWordsView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words.png)
   - **Controls**:
     - Press **Key1 (A)** to proceed to the next page or finish
     - Press **Key2 (B)** to go back
     - Use **Joystick Right** to advance to the next page (if available)

3. **Seed Words View (Page 2)**
   - Second page of seed words (for 24-word seeds)
     ![SeedWordsView_2](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_2.png)
   - **Controls**:
     - Press **Key1 (A)** to finish
     - Press **Key2 (B)** to go back to page 1
     - Use **Joystick Left** to go back to the previous page

### BIP85 Child Seed Generation

1. **BIP85 Application Mode**

   - Select which application to generate a child seed for
     ![SeedBIP85ApplicationModeView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__bip85_application_mode.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between applications
     - Press **Key1 (A)** to select an application
     - Press **Key2 (B)** to go back

2. **BIP85 Child Index Selection**

   - Select the index number for the child seed
     ![SeedBIP85SelectChildIndexView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__bip85_select_child_index.png)
   - **Controls**:
     - Use the **Joystick** to navigate the number pad
     - Press **Key1 (A)** to select a digit
     - Press **Key2 (B)** to delete the last digit
     - Navigate to "OK" and press **Key1 (A)** when finished

3. **BIP85 Invalid Child Index**
   - If you enter an invalid index, you'll see this error
     ![SeedBIP85InvalidChildIndexView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__bip85_invalid_child_index.png)
   - **Controls**: Press **Key1 (A)** to acknowledge and try again

### Seed Words Backup Test

1. **Backup Test Prompt**

   - If you choose to test your backup, you'll see this prompt
     ![SeedWordsBackupTestPromptView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test_prompt.png)
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **Key1 (A)** to confirm your selection

2. **Backup Test Entry**

   - Enter your backed-up seed words to test them
     ![SeedWordsBackupTestView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test.png)
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **Key1 (A)** to select a letter or button
     - Press **Key2 (B)** to delete the last letter
     - Press **Key3 (C)** to toggle between word suggestion lists
     - Navigate to "OK" and press **Key1 (A)** when done

3. **Backup Test Mistake**

   - If you make a mistake, you'll see this warning
     ![SeedWordsBackupTestMistakeView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test_mistake.png)
   - **Controls**: Press **Key1 (A)** to acknowledge and try again

4. **Backup Test Success**
   - If successful, you'll see this confirmation
     ![SeedWordsBackupTestSuccessView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test_success.png)
   - **Controls**: Press **Key1 (A)** to continue

### SeedQR Management

1. **SeedQR Format Selection**

   - When working with SeedQR, select the format
     ![SeedTranscribeSeedQRFormatView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_format.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between formats
     - Press **Key1 (A)** to select a format
     - Press **Key2 (B)** to go back

2. **SeedQR Warning**

   - Before proceeding, you'll see this warning
     ![SeedTranscribeSeedQRWarningView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_warning.png)
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **Key1 (A)** to confirm your selection

3. **SeedQR Display (12-word Compact)**

   - View the SeedQR for a 12-word seed in compact format
     ![SeedTranscribeSeedQRWholeQRView_12_Compact](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_whole_qr_12_compact.png)
   - **Controls**:
     - Press **Key1 (A)** to zoom in
     - Press **Key2 (B)** to go back
     - Press **Key3 (C)** to proceed to the next step

4. **SeedQR Zoomed In View**

   - View a zoomed-in portion of a SeedQR
     ![SeedTranscribeSeedQRZoomedInView_12_Compact](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_zoomed_in_12_compact.png)
   - **Controls**:
     - Use the **Joystick** to pan across the QR code
     - Press **Key1 (A)** to zoom out
     - Press **Key2 (B)** to go back

5. **SeedQR Confirmation Prompt**
   - When verifying a SeedQR, you'll see this prompt
     ![SeedTranscribeSeedQRConfirmQRPromptView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_confirm_qr_prompt.png)
   - **Controls**:
     - Use the **Joystick Left/Right** to select an option
     - Press **Key1 (A)** to confirm your selection

### Multisig and Address Verification

1. **Seed Selection for Address Verification**

   - Select which seed to use for address verification
     ![SeedSelectSeedView_address_verification](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__select_seed_address_verification.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between seeds
     - Press **Key1 (A)** to select a seed
     - Press **Key2 (B)** to go back

2. **Address Verification Signature Type Selection**

   - Select the signature type for address verification
     ![AddressVerificationSigTypeView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__address_verification_sig_type.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between signature types
     - Press **Key1 (A)** to select a signature type
     - Press **Key2 (B)** to go back

3. **Address Verification**

   - Verify the address matches the expected value
     ![SeedAddressVerificationView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__address_verification.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back

4. **Address Verification Success**
   - If the address is verified, you'll see this confirmation
     ![SeedAddressVerificationSuccessView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__address_verification_success.png)
   - **Controls**: Press **Key1 (A)** to continue

### Message Signing

1. **Seed Selection for Message Signing**

   - Select which seed to use for signing a message
     ![SeedSelectSeedView_sign_message](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__select_seed_sign_message.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between seeds
     - Press **Key1 (A)** to select a seed
     - Press **Key2 (B)** to go back

2. **Message Signing Confirmation**

   - Confirm the message to be signed
     ![SeedSignMessageConfirmMessageView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__sign_message_confirm_message.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to scroll through the message
     - Press **Key1 (A)** to confirm and continue
     - Press **Key2 (B)** to go back

3. **Message Signing Address Confirmation**
   - Confirm the address to be used for signing
     ![SeedSignMessageConfirmAddressView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__sign_message_confirm_address.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to confirm and sign the message
     - Press **Key2 (B)** to go back

## Transaction Signing (PSBT)

1. **Select Seed for Transaction Signing**

   - Choose which seed to use for signing a transaction
     ![PSBTSelectSeedView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/psbt__select_seed.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between seeds
     - Press **Key1 (A)** to select a seed
     - Press **Key2 (B)** to go back

2. **Transaction Overview**

   - View the overview of the transaction to be signed
     ![PSBTOverviewView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/psbt__overview.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option and view details
     - Press **Key2 (B)** to go back
     - Press **Key3 (C)** to proceed to signing

3. **Transaction Math Details**

   - View the detailed math of the transaction
     ![PSBTMathView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/psbt__math.png)
   - **Controls**:
     - Press **Key1 (A)** to continue
     - Press **Key2 (B)** to go back

4. **Address Details**

   - View the details of the recipient address
     ![PSBTAddressDetailsView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/psbt__address_details.png)
   - **Controls**:
     - Press **Key1 (A)** to continue
     - Press **Key2 (B)** to go back

5. **Transaction Finalization**
   - Confirm final details before signing
     ![PSBTFinalizeView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/psbt__finalize.png)
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Sign"
     - Press **Key1 (A)** to confirm your selection

## Tools

1. **Tools Menu**

   - Access the tools menu from the main menu
     ![ToolsMenuView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__tools.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between tools
     - Press **Key1 (A)** to select a tool
     - Press **Key2 (B)** to go back to the main menu

2. **Dice Entropy Entry**

   - Enter dice rolls for entropy
     ![ToolsDiceEntropyEntryView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__dice_entropy_entry.png)
   - **Controls**:
     - Use the **Joystick** to navigate the number pad
     - Press **Key1 (A)** to select a number (1-6)
     - Press **Key2 (B)** to delete the last roll
     - Press **Key3 (C)** to finish entering rolls
     - Navigate to "DONE" and press **Key1 (A)** when finished

3. **Calculator**

   - Use the built-in calculator tool
     ![ToolsCalculatorView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__calculator.png)
   - **Controls**:
     - Use the **Joystick** to navigate the calculator buttons
     - Press **Key1 (A)** to select a button
     - Press **Key2 (B)** to clear or go back
     - Navigate to "=" and press **Key1 (A)** to calculate the result

4. **Coin Flip Entropy**

   - Enter coin flips for entropy
     ![ToolsCoinFlipEntropyEntryView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__coin_flip_entropy_entry.png)
   - **Controls**:
     - Use the **Joystick Left/Right** to toggle between "H" (Heads) and "T" (Tails)
     - Press **Key1 (A)** to confirm and add the selection
     - Press **Key2 (B)** to delete the last flip
     - Press **Key3 (C)** to finish entering flips

5. **QR Scanner**
   - Scan a QR code with the camera
     ![ToolsQRScannerView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__qr_scanner.png)
   - **Controls**:
     - Hold the camera steady over a QR code
     - QR code will be detected automatically
     - Press **Key2 (B)** to go back to the tools menu

## Settings

1. **Settings Menu**

   - Access the settings menu from the main menu
     ![SettingsMenuView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__settings.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between settings
     - Press **Key1 (A)** to select a setting
     - Press **Key2 (B)** to go back to the main menu

2. **QR Scanner Settings**

   - Adjust settings for the QR scanner
     ![SettingsQRScannerView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__qr_scanner.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to toggle options on/off
     - Press **Key2 (B)** to go back to the settings menu

3. **Camera Settings**

   - Adjust camera settings
     ![SettingsCameraView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__camera.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option to adjust
     - Press **Key2 (B)** to go back to the settings menu

4. **Display Settings**

   - Adjust display settings
     ![SettingsDisplayView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__display.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option or toggle settings
     - Press **Key2 (B)** to go back to the settings menu

5. **QR Display Settings**

   - Adjust QR code display settings
     ![SettingsQRDisplayView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__qr_display.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option or adjust values
     - Press **Key2 (B)** to go back to the settings menu

6. **Direct Camera Settings**

   - Adjust advanced camera settings
     ![SettingsDirectCameraConfigView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__direct_camera_config.png)
   - **Controls**:
     - Use the **Joystick** to navigate between parameters and values
     - Press **Key1 (A)** to select and adjust values
     - Press **Key2 (B)** to go back
     - Press **Key3 (C)** to save changes

7. **Brightness Settings**

   - Adjust display brightness
     ![SettingsBrightnessView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__brightness.png)
   - **Controls**:
     - Use the **Joystick Left/Right** to decrease/increase brightness
     - Press **Key1 (A)** to save the setting
     - Press **Key2 (B)** to cancel and go back

8. **Keyboard Layout Settings**

   - Choose keyboard layout
     ![SettingsKeyboardLayoutView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__keyboard_layout.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between layouts
     - Press **Key1 (A)** to select a layout
     - Press **Key2 (B)** to go back to the settings menu

9. **Language Settings**

   - Choose language for the interface
     ![SettingsLanguageView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__language.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between languages
     - Press **Key1 (A)** to select a language
     - Press **Key2 (B)** to go back to the settings menu

10. **Partner Logos Settings**

    - Toggle partner logos on/off
      ![SettingsPartnerLogosView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__partner_logos.png)
    - **Controls**:
      - Use the **Joystick Up/Down** to navigate between options
      - Press **Key1 (A)** to select an option
      - Press **Key2 (B)** to go back to the settings menu

11. **Debug Settings**
    - Access debug settings
      ![SettingsDebugView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__debug.png)
    - **Controls**:
      - Use the **Joystick Up/Down** to navigate between options
      - Press **Key1 (A)** to toggle options on/off
      - Press **Key2 (B)** to go back to the settings menu

## Error Screens

1. **No Camera Error**

   - Displays when no camera is detected
     ![ErrorNoCameraView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/error__no_camera.png)
   - **Controls**: Press **Key1 (A)** to acknowledge and try again

2. **QR Code Error**

   - Displays when there's an issue with QR code scanning
     ![ErrorQRCodeView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/error__qr_code.png)
   - **Controls**: Press **Key1 (A)** to acknowledge and try again

3. **PSBT Format Error**
   - Displays when a PSBT file has format issues
     ![ErrorPSBTFormatView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/error__psbt_format.png)
   - **Controls**: Press **Key1 (A)** to acknowledge and go back

## Advanced Features

1. **Multisig Coordination**

   - Set up and manage multisig wallets
     ![MultisigCoordinatorSelectView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/multisig__coordinator_select.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select an option
     - Press **Key2 (B)** to go back

2. **Wallet Creation Options**

   - Configure wallet creation parameters
     ![WalletCreationOptionsView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/wallet__creation_options.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **Key1 (A)** to select and adjust an option
     - Press **Key2 (B)** to go back
     - Press **Key3 (C)** to proceed with wallet creation

3. **Seed Source Selection**
   - Choose how to create or load a seed
     ![SeedSourceSelectionView](https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__source_selection.png)
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between sources
     - Press **Key1 (A)** to select a source
     - Press **Key2 (B)** to go back

## Troubleshooting Tips

1. **Camera Connection Issues**

   - If the camera isn't detected:
     - Check the ribbon cable connection between the camera and the Raspberry Pi
     - Make sure the camera is enabled in Raspberry Pi configuration
     - Try a different camera module if available

2. **Display Issues**

   - If the display is dim or unresponsive:
     - Check the brightness settings in the Settings menu
     - Verify that the WaveShare LCD Hat is properly seated on the GPIO pins
     - Try power cycling the device

3. **Button Responsiveness**

   - If buttons are not responding correctly:
     - Clean the button contacts if accessible
     - Check for any physical damage to the joystick or buttons
     - Test each button in the system diagnostics (if available)

4. **SD Card Problems**

   - If SD card is not detected or has errors:
     - Try reformatting the SD card (FAT32 format recommended)
     - Use a high-quality, class 10 SD card from a reputable manufacturer
     - Verify the SD card is properly inserted in the slot

5. **QR Code Scanning Issues**
   - If QR codes are not scanning properly:
     - Ensure adequate lighting around the QR code
     - Hold the device steady and at an appropriate distance
     - Make sure the QR code is not damaged or blurry
     - Adjust camera settings in the Settings menu

## Maintenance and Care

1. **Power Management**

   - Always use the proper shutdown procedure (Power menu → Power Off)
   - Use a stable power source with adequate amperage (2.5A recommended)
   - Consider using a battery pack for portable operation

2. **Physical Protection**

   - Store in a dry, cool environment
   - Use a protective case when transporting
   - Avoid exposing to extreme temperatures, moisture, or dust

3. **Software Updates**
   - Check the SeedSigner website periodically for firmware updates
   - Follow update procedures carefully to avoid data loss
   - Consider maintaining a backup SD card with a working firmware image

## Security Best Practices

1. **Physical Security**

   - Keep your SeedSigner in a secure location when not in use
   - Be aware of your surroundings when using the device in public
   - Consider using a privacy screen protector to prevent shoulder surfing

2. **Seed Management**

   - Always verify seed words before using them for transactions
   - Test your seed backups regularly
   - Consider using a passphrase for additional security
   - Store seed backups in secure, geographically distributed locations

3. **Transaction Verification**

   - Always double-check recipient addresses before confirming transactions
   - Verify transaction amounts and fees before signing
   - When possible, use address verification to confirm wallet addresses match

4. **Operational Security**
   - Remove SD card when device is not in use
   - Consider using the SeedSigner in an air-gapped environment
   - Don't share photographs or video of your device while it's displaying sensitive information
   - Clear any saved seeds from the device after completing operations

## Conclusion

This comprehensive guide covers all essential navigation paths and control instructions for the SeedSigner with WaveShare LCD Hat. By understanding these controls and screens, you can securely manage your Bitcoin seeds, sign transactions, and perform various bitcoin-related operations in a fully air-gapped environment.

Remember that the SeedSigner is designed as a stateless device - it does not store your seeds permanently. Always ensure you have proper backups of your seed phrases stored securely offline.

For more information, visit the official SeedSigner repository at https://github.com/SeedSigner/seedsigner
