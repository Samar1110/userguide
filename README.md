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
- **Key1 (A)**: Selection/confirm button
- **Key2 (B)**: Selection/confirm button
- **Key3 (C)**: Selection/confirm button

### Button Functions

| Button         | Function                                    |
| -------------- | ------------------------------------------- |
| Joystick Up    | Move selection up                           |
| Joystick Down  | Move selection down                         |
| Joystick Left  | Move selection left                         |
| Joystick Right | Move selection right                        |
| Key1 (A)       | Select highlighted option or confirm action |
| Key2 (B)       | Select highlighted option or confirm action |
| Key3 (C)       | Select highlighted option or confirm action |

**Important Note**: All three keys (Key1, Key2, Key3) function identically for selection and confirmation. To go back to a previous screen, you must first navigate to the back icon/button on the screen using the joystick, then press any of the three keys to activate it.

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
     - Press **any key (A, B, or C)** to select a menu option
     - To go back (if applicable), navigate to the back icon and press **any key**

### SD Card Notifications

1. **SD Card Removal Detected**

   <div align="center">
     <img src="images/MainMenuViews/MainMenuView_SDCardStateChangeToast_removed.png" alt="SD Card Removed Toast" width="300"/>
   </div>

   - If an SD card is removed while the device is on, you'll see this notification
   - **Controls**: No action required, notification will disappear automatically

2. **SD Card Insertion Detected**

   <div align="center">
     <img src="images/MainMenuViews/MainMenuView_SDCardStateChangeToast_inserted.png" alt="SD Card Inserted Toast" width="300"/>
   </div>

   - If an SD card is inserted while the device is on, you'll see this notification
   - **Controls**: No action required, notification will disappear automatically

3. **Remove SD Card Prompt**

   <div align="center">
     <img src="images/MainMenuViews/MainMenuView_RemoveSDCardToast.png" alt="Remove SD Card Toast" width="300"/>
   </div>

   - In certain situations, you may be prompted to remove the SD card
   - **Controls**: Remove the SD card as instructed, then press **any key** to continue

### Power Options

1. **Accessing Power Menu**

   <div align="center">
     <img src="images/MainMenuViews/PowerOptionsView.png" alt="Power Options View" width="300"/>
   </div>

   - From the main menu, use the **Joystick** to navigate to the power icon (top right)
   - Press **any key** to select
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between power options
     - Press **any key** to select an option
     - To go back to the main menu, navigate to the back icon and press **any key**

2. **Restart Device**

   <div align="center">
     <img src="images/MainMenuViews/RestartView.png" alt="Restart View" width="300"/>
   </div>

   - From the power menu, use the **Joystick** to select "Restart"
   - Press **any key** to confirm
   - **Controls**: Press **any key** to confirm restart or navigate to cancel and press **any key** to cancel

3. **Power Off Device**

   <div align="center">
     <img src="images/MainMenuViews/PowerOffView.png" alt="Power Off View" width="300"/>
   </div>

   - From the power menu, use the **Joystick** to select "Power Off"
   - Press **any key** to confirm
   - **Controls**: Press **any key** to confirm power off or navigate to cancel and press **any key** to cancel

## Seed Management

### Seed Creation and Loading

1. **Accessing Seeds Menu**

   <div align="center">
     <img src="images/seed_views/SeedsMenuView.png" alt="Seeds Menu View" width="300"/>
   </div>

   * From the main menu, use the **Joystick** to navigate to the **Seeds icon** (top right)
   * Press **any key** to select
   * **Note**: This screen is shown **only if a seed has already been saved**.
     If no seed exists, you will first be prompted to **load a new seed**.
   * **Controls**:

     * Use the **Joystick Up/Down** to navigate between seed options
     * Press **any key** to select an option
     * To return to the main menu, navigate to the back icon and press **any key**

2. **Loading an Existing Seed**

   <div align="center">
     <img src="images/seed_views/LoadSeedView.png" alt="Load Seed View" width="300"/>
   </div>

   - From the Seeds menu, use the **Joystick** to select "Load Seed"
   - Press **any key** to confirm
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between load options
     - Press **any key** to select an option
     - To go back to the seeds menu, navigate to the back icon and press **any key**

3. **Entering a Seed Phrase**

   <div align="center">
     <img src="images/seed_views/SeedMnemonicEntryView.png" alt="Seed Mnemonic Entry View" width="300"/>
   </div>

   * If you choose to add a passphrase, you'll be presented with an **on-screen keyboard** to enter your words.
   * **Note**: Seed phrases are **case-insensitive**, so there is no distinction between lowercase and uppercase.
   * **Controls**:

     * Use the **Joystick** to move across the keyboard and highlight any letter
     * **Press the Joystick (center press)** to select a letter or button
     * To delete the last character, navigate to the **delete** button and press the **Joystick**
     * On the **right side** of the keyboard, a list of **completed word suggestions** is shown

       * To **navigate up** in the suggestion list, press **Key1 (A)**
       * To **navigate down**, press **Key3 (C)**
       * To **select a word** from the list, press **Key2 (B)**
     * Continue entering and selecting words until you have completed your **12 or 24-word** seed phrase


4. **Invalid Seed Warning**

   <div align="center">
     <img src="images/seed_views/SeedMnemonicInvalidView.png" alt="Seed Mnemonic Invalid View" width="300"/>
   </div>

   - If the entered seed is invalid, you'll see this warning
   - **Controls**: Press **any key** to acknowledge and try again

5. **Finalizing Seed**

   <div align="center">
     <img src="images/seed_views/SeedFinalizeView.png" alt="Seed Finalize View" width="300"/>
   </div>

   - After entering a valid seed, you'll be taken to this screen to confirm
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **any key** to select an option
     - To go back, navigate to the back icon and press **any key**

### Seed Passphrase Management

1. **Adding a Passphrase (Lowercase)**

   <div align="center">
     <img src="images/seed_views/SeedAddPassphraseView_lowercase.png" alt="Seed Add Passphrase View (Lowercase)" width="300"/>
   </div>

   - If you choose to add a passphrase, you'll start with the lowercase keyboard
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **any key** to select a letter or button
     - Navigate to the delete button and press **any key** to delete the last character
     - Use **Joystick** to navigate to "abc" and press **any key** to switch to uppercase

2. **Adding a Passphrase (Uppercase)**

   <div align="center">
     <img src="images/seed_views/SeedAddPassphraseView_uppercase.png" alt="Seed Add Passphrase View (Uppercase)" width="300"/>
   </div>

   - Switch to uppercase by selecting the "abc" button
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **any key** to select a letter or button
     - Navigate to the delete button and press **any key** to delete the last character
     - Use **Joystick** to navigate to "123" and press **any key** to switch to digits

3. **Adding a Passphrase (Digits)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_digits.png" alt="Seed Add Passphrase View (Digits)" width="300"/>
   </div>

   - Switch to digits by selecting the "123" button
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **any key** to select a digit or button
     - Navigate to the delete button and press **any key** to delete the last character
     - Use **Joystick** to navigate to "#$%" and press **any key** to switch to symbols

4. **Adding a Passphrase (Symbols 1)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_symbols_1.png" alt="Seed Add Passphrase View (Symbols 1)" width="300"/>
   </div>

   - Switch to symbols by selecting the "#$%" button
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **any key** to select a symbol or button
     - Navigate to the delete button and press **any key** to delete the last character
     - Use **Joystick** to navigate to "→" and press **any key** to see more symbols

5. **Adding a Passphrase (Symbols 2)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_symbols_2.png" alt="Seed Add Passphrase View (Symbols 2)" width="300"/>
   </div>

   - Access additional symbols by selecting the "→" button
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **any key** to select a symbol or button
     - Navigate to the delete button and press **any key** to delete the last character
     - Navigate to "DONE" and press **any key** when finished

6. **Passphrase Exit Dialog**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__add_passphrase_exit_dialog.png" alt="Seed Add Passphrase Exit Dialog View" width="300"/>
   </div>

   - If you try to exit while entering a passphrase, you'll see this confirmation
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Exit"
     - Press **any key** to confirm your selection

7. **Reviewing Passphrase**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__review_passphrase.png" alt="Seed Review Passphrase View" width="300"/>
   </div>

   - After entering a passphrase, you'll be asked to review it
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **any key** to select an option
     - To go back, navigate to the back icon and press **any key**

### Seed Options and Management

1. **Seed Options Menu**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__seed_options.png" alt="Seed Options View" width="300"/>
   </div>

   - After loading or creating a seed, you'll see the seed options
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **any key** to select an option
     - To go back to the previous menu, navigate to the back icon and press **any key**

2. **Seed Backup Options**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__backup.png" alt="Seed Backup View" width="300"/>
   </div>

   - If you select "Backup Seed" from the seed options, you'll see these options
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **any key** to select an option
     - To go back to seed options, navigate to the back icon and press **any key**

### Seed Export and Xpub Management

1. **Export Xpub Signature Type Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_sig_type.png" alt="Seed Export Xpub Sig Type View" width="300"/>
   </div>

   - When exporting an Xpub, first select the signature type
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between signature types
     - Press **any key** to select a signature type
     - To go back, navigate to the back icon and press **any key**

2. **Export Xpub Script Type Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_script_type.png" alt="Seed Export Xpub Script Type View" width="300"/>
   </div>

   - Then select the script type
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between script types
     - Press **any key** to select a script type
     - To go back, navigate to the back icon and press **any key**

3. **Custom Derivation Path**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_custom_derivation.png" alt="Seed Export Xpub Custom Derivation View" width="300"/>
   </div>

   - If needed, you can set a custom derivation path
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard and input numbers
     - Press **any key** to select a character or button
     - Navigate to the delete button and press **any key** to delete the last character
     - Navigate to "DONE" and press **any key** when finished

4. **Selecting Coordinator**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_coordinator.png" alt="Seed Export Xpub Coordinator View" width="300"/>
   </div>

   - Select which wallet coordinator to use
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between coordinators
     - Press **any key** to select a coordinator
     - To go back, navigate to the back icon and press **any key**

5. **Xpub Export Warning**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_warning.png" alt="Seed Export Xpub Warning View" width="300"/>
   </div>

   - Before exporting, you'll see this privacy warning
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **any key** to confirm your selection

6. **Xpub Details**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__export_xpub_details.png" alt="Seed Export Xpub Details View" width="300"/>
   </div>

   - View the xpub details before finalizing
   - **Controls**:
     - Use the **Joystick Up/Down** to scroll through the details
     - Press **any key** to continue to the QR code
     - To go back, navigate to the back icon and press **any key**

### Seed Words Management

1. **Seed Words Warning**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_warning.png" alt="Seed Words Warning View" width="300"/>
   </div>

   - Before showing seed words, you'll see this privacy warning
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **any key** to confirm your selection

2. **Seed Words View (Page 1)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words.png" alt="Seed Words View" width="300"/>
   </div>

   - First page of seed words
   - **Controls**:
     - Press **any key** to proceed to the next page or finish
     - To go back, navigate to the back icon and press **any key**
     - Use **Joystick Right** to advance to the next page (if available)

3. **Seed Words View (Page 2)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_2.png" alt="Seed Words View (Page 2)" width="300"/>
   </div>

   - Second page of seed words (for 24-word seeds)
   - **Controls**:
     - Press **any key** to finish
     - To go back to page 1, navigate to the back icon and press **any key**
     - Use **Joystick Left** to go back to the previous page

### BIP85 Child Seed Generation

1. **BIP85 Application Mode**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__bip85_application_mode.png" alt="Seed BIP85 Application Mode View" width="300"/>
   </div>

   - Select which application to generate a child seed for
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between applications
     - Press **any key** to select an application
     - To go back, navigate to the back icon and press **any key**

2. **BIP85 Child Index Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__bip85_select_child_index.png" alt="Seed BIP85 Select Child Index View" width="300"/>
   </div>

   - Select the index number for the child seed
   - **Controls**:
     - Use the **Joystick** to navigate the number pad
     - Press **any key** to select a digit
     - Navigate to the delete button and press **any key** to delete the last digit
     - Navigate to "OK" and press **any key** when finished

3. **BIP85 Invalid Child Index**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__bip85_invalid_child_index.png" alt="Seed BIP85 Invalid Child Index View" width="300"/>
   </div>

   - If you enter an invalid index, you'll see this error
   - **Controls**: Press **any key** to acknowledge and try again

### Seed Words Backup Test

1. **Backup Test Prompt**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test_prompt.png" alt="Seed Words Backup Test Prompt View" width="300"/>
   </div>

   - If you choose to test your backup, you'll see this prompt
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **any key** to confirm your selection

2. **Backup Test Entry**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test.png" alt="Seed Words Backup Test View" width="300"/>
   </div>

   - Enter your backed-up seed words to test them
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **any key** to select a letter or button
     - Navigate to the delete button and press **any key** to delete the last letter
     - Navigate to the word suggestion toggle and press **any key** to toggle between word suggestion lists
     - Navigate to "OK" and press **any key** when done

3. **Backup Test Mistake**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test_mistake.png" alt="Seed Words Backup Test Mistake View" width="300"/>
   </div>

   - If you make a mistake, you'll see this warning
   - **Controls**: Press **any key** to acknowledge and try again

4. **Backup Test Success**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__words_backup_test_success.png" alt="Seed Words Backup Test Success View" width="300"/>
   </div>

   - If successful, you'll see this confirmation
   - **Controls**: Press **any key** to continue

### SeedQR Management

1. **SeedQR Format Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_format.png" alt="Seed Transcribe SeedQR Format View" width="300"/>
   </div>

   - When working with SeedQR, select the format
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between formats
     - Press **any key** to select a format
     - To go back, navigate to the back icon and press **any key**

2. **SeedQR Warning**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_warning.png" alt="Seed Transcribe SeedQR Warning View" width="300"/>
   </div>

   - Before proceeding, you'll see this warning
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **any key** to confirm your selection

3. **SeedQR Display (12-word Compact)**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_whole_qr_12_compact.png" alt="Seed Transcribe SeedQR Whole QR View (12-word Compact)" width="300"/>
   </div>

   - View the SeedQR for a 12-word seed in compact format
   - **Controls**:
     - Press **any key** to zoom in
     - To go back, navigate to the back icon and press **any key**
     - Navigate to the next step button and press **any key** to proceed

4. **SeedQR Zoomed In View**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_zoomed_in_12_compact.png" alt="Seed Transcribe SeedQR Zoomed In View (12-word Compact)" width="300"/>
   </div>

   - View a zoomed-in portion of a SeedQR
   - **Controls**:
     - Use the **Joystick** to pan across the QR code
     - Press **any key** to zoom out
     - To go back, navigate to the back icon and press **any key**

5. **SeedQR Confirmation Prompt**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__transcribe_seedqr_confirm_qr_prompt.png" alt="Seed Transcribe SeedQR Confirm QR Prompt View" width="300"/>
   </div>

   - When verifying a SeedQR, you'll see this prompt
   - **Controls**:
     - Use the **Joystick Left/Right** to select an option
     - Press **any key** to confirm your selection

### Multisig and Address Verification

1. **Seed Selection for Address Verification**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__select_seed_address_verification.png" alt="Seed Select Seed View (Address Verification)" width="300"/>
   </div>

   - Select which seed to use for address verification
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between seeds
     - Press **any key** to select a seed
     - To go back, navigate to the back icon and press **any key**

2. **Address Verification Signature Type Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__address_verification_sig_type.png" alt="Address Verification Sig Type View" width="300"/>
   </div>

   - Select the signature type for address verification
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between signature types
     - Press **any key** to select a signature type
     - To go back, navigate to the back icon and press **any key**

3. **Address Verification**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__address_verification.png" alt="Seed Address Verification View" width="300"/>
   </div>

   - Verify the address matches the expected value
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between options
     - Press **any key** to select an option
     - To go back, navigate to the back icon and press **any key**

4. **Address Verification Success**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__address_verification_success.png" alt="Seed Address Verification Success View" width="300"/>
   </div>

   - If the address is verified, you'll see this confirmation
   - **Controls**: Press **any key** to continue

### Message Signing

1. **Seed Selection for Message Signing**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__select_seed_sign_message.png" alt="Seed Select Seed View (Sign Message)" width="300"/>
   </div>

   - Select which seed to use for signing a message
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between seeds
     - Press **any key** to select a seed
     - To go back, navigate to the back icon and press **any key**

2. **Message Signing Confirmation**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__sign_message_confirm_message.png" alt="Seed Sign Message Confirm Message View" width="300"/>
   </div>

   - Confirm the message content that you want to sign
   - **Controls**:
     - Use the **Joystick Up/Down** to scroll through the message if needed
     - Press **any key** to confirm and sign the message
     - To cancel and go back, navigate to the cancel option and press **any key**

3. **Message Signing Script Type Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__sign_message_script_type.png" alt="Seed Sign Message Script Type View" width="300"/>
   </div>

   - Select the script type for message signing
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between script types
     - Press **any key** to select a script type
     - To go back, navigate to the back icon and press **any key**

4. **Message Signing Success**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/seed__sign_message_signature_display.png" alt="Seed Sign Message Signature Display View" width="300"/>
   </div>

   - After successful message signing, view the signature
   - **Controls**:
     - Use the **Joystick Up/Down** to scroll through the signature details
     - Press **any key** to continue or export
     - To go back, navigate to the back icon and press **any key**

## Transaction Signing (PSBT)

### PSBT Loading and Verification

1. **PSBT Overview**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/psbt__overview.png" alt="PSBT Overview View" width="300"/>
   </div>

   - View the transaction overview before signing
   - **Controls**:
     - Use the **Joystick Up/Down** to scroll through transaction details
     - Press **any key** to proceed to signing options
     - To go back, navigate to the back icon and press **any key**

2. **PSBT Change Warning**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/psbt__change_warning.png" alt="PSBT Change Warning View" width="300"/>
   </div>

   - Warning about change outputs in the transaction
   - **Controls**:
     - Use the **Joystick Left/Right** to select "Cancel" or "Continue"
     - Press **any key** to confirm your selection

3. **PSBT Seed Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/psbt__seed_selection.png" alt="PSBT Seed Selection View" width="300"/>
   </div>

   - Select which seed to use for signing the transaction
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between available seeds
     - Press **any key** to select a seed
     - To go back, navigate to the back icon and press **any key**

4. **PSBT Address Verification**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/psbt__address_verification.png" alt="PSBT Address Verification View" width="300"/>
   </div>

   - Verify that addresses in the transaction are correct
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between verification options
     - Press **any key** to select an option
     - To go back, navigate to the back icon and press **any key**

5. **PSBT Signing Complete**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/psbt__signing_complete.png" alt="PSBT Signing Complete View" width="300"/>
   </div>

   - Transaction has been successfully signed
   - **Controls**:
     - Press **any key** to view the signed transaction QR code
     - To go back, navigate to the back icon and press **any key**

### PSBT Export and QR Display

1. **PSBT Export QR Code**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/psbt__export_qr.png" alt="PSBT Export QR View" width="300"/>
   </div>

   - Display the signed transaction as a QR code for export
   - **Controls**:
     - Use **Joystick Left/Right** to navigate between QR code parts (if animated)
     - Press **any key** to pause/resume animation
     - To go back, navigate to the back icon and press **any key**

## Tools

### Tools Menu

1. **Tools Overview**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__overview.png" alt="Tools Overview View" width="300"/>
   </div>

   - Access various utility tools
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between tool options
     - Press **any key** to select a tool
     - To go back to main menu, navigate to the back icon and press **any key**

### Image Processing Tools

1. **Image Processing Options**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__image_processing.png" alt="Tools Image Processing View" width="300"/>
   </div>

   - Select image processing operations
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between processing options
     - Press **any key** to select an option
     - To go back, navigate to the back icon and press **any key**

2. **Camera Preview**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__camera_preview.png" alt="Tools Camera Preview View" width="300"/>
   </div>

   - Live camera preview before capturing
   - **Controls**:
     - Press **any key** to capture the image
     - To go back, navigate to the back icon and press **any key**

3. **Image Capture Success**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__image_capture_success.png" alt="Tools Image Capture Success View" width="300"/>
   </div>

   - Confirmation that image was captured successfully
   - **Controls**:
     - Press **any key** to continue with processing
     - To retake, navigate to the retake option and press **any key**

### Address Explorer

1. **Address Explorer Input**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__address_explorer_input.png" alt="Tools Address Explorer Input View" width="300"/>
   </div>

   - Enter an address to explore
   - **Controls**:
     - Use the **Joystick** to navigate the keyboard
     - Press **any key** to select a character
     - Navigate to delete button and press **any key** to delete last character
     - Navigate to "DONE" and press **any key** when finished

2. **Address Explorer Results**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__address_explorer_results.png" alt="Tools Address Explorer Results View" width="300"/>
   </div>

   - View address exploration results
   - **Controls**:
     - Use the **Joystick Up/Down** to scroll through results
     - Press **any key** to select an option or continue
     - To go back, navigate to the back icon and press **any key**

### Dice Roll Entropy

1. **Dice Roll Instructions**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__dice_instructions.png" alt="Tools Dice Instructions View" width="300"/>
   </div>

   - Instructions for using dice to generate entropy
   - **Controls**:
     - Press **any key** to continue to dice input
     - To go back, navigate to the back icon and press **any key**

2. **Dice Roll Input**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__dice_input.png" alt="Tools Dice Input View" width="300"/>
   </div>

   - Enter dice roll results
   - **Controls**:
     - Use the **Joystick** to navigate between dice values (1-6)
     - Press **any key** to select a dice value
     - Navigate to delete button and press **any key** to remove last roll
     - Navigate to "DONE" and press **any key** when sufficient entropy is collected

### Coin Flip Entropy

1. **Coin Flip Instructions**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__coin_flip_instructions.png" alt="Tools Coin Flip Instructions View" width="300"/>
   </div>

   - Instructions for using coin flips to generate entropy
   - **Controls**:
     - Press **any key** to continue to coin flip input
     - To go back, navigate to the back icon and press **any key**

2. **Coin Flip Input**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/tools__coin_flip_input.png" alt="Tools Coin Flip Input View" width="300"/>
   </div>

   - Enter coin flip results
   - **Controls**:
     - Use the **Joystick Left/Right** to select "H" (Heads) or "T" (Tails)
     - Press **any key** to record the flip result
     - Navigate to delete button and press **any key** to remove last flip
     - Navigate to "DONE" and press **any key** when sufficient entropy is collected

## Settings

### Settings Menu

1. **Settings Overview**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__overview.png" alt="Settings Overview View" width="300"/>
   </div>

   - Access device configuration options
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between setting categories
     - Press **any key** to select a category
     - To go back to main menu, navigate to the back icon and press **any key**

### Display Settings

1. **Display Settings Menu**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__display.png" alt="Settings Display View" width="300"/>
   </div>

   - Configure display-related settings
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between display options
     - Press **any key** to select an option
     - To go back, navigate to the back icon and press **any key**

2. **Brightness Control**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__brightness.png" alt="Settings Brightness View" width="300"/>
   </div>

   - Adjust screen brightness
   - **Controls**:
     - Use the **Joystick Left/Right** to decrease/increase brightness
     - Press **any key** to confirm the setting
     - To go back, navigate to the back icon and press **any key**

### Network Settings

1. **Network Settings Menu**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__network.png" alt="Settings Network View" width="300"/>
   </div>

   - Configure network-related settings
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between network options
     - Press **any key** to select an option
     - To go back, navigate to the back icon and press **any key**

### Wallet Settings

1. **Wallet Settings Menu**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__wallet.png" alt="Settings Wallet View" width="300"/>
   </div>

   - Configure wallet-related settings
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between wallet options
     - Press **any key** to select an option
     - To go back, navigate to the back icon and press **any key**

2. **Wallet Selection**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__wallet_selection.png" alt="Settings Wallet Selection View" width="300"/>
   </div>

   - Select default wallet software
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between wallet options
     - Press **any key** to select a wallet
     - To go back, navigate to the back icon and press **any key**

### Hardware Settings

1. **Hardware Settings Menu**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__hardware.png" alt="Settings Hardware View" width="300"/>
   </div>

   - Configure hardware-related settings
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between hardware options
     - Press **any key** to select an option
     - To go back, navigate to the back icon and press **any key**

2. **Camera Settings**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__camera.png" alt="Settings Camera View" width="300"/>
   </div>

   - Configure camera settings
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between camera options
     - Press **any key** to select an option
     - To go back, navigate to the back icon and press **any key**

### Advanced Settings

1. **Advanced Settings Menu**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__advanced.png" alt="Settings Advanced View" width="300"/>
   </div>

   - Access advanced configuration options
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between advanced options
     - Press **any key** to select an option
     - To go back, navigate to the back icon and press **any key**

2. **Debug Settings**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/settings__debug.png" alt="Settings Debug View" width="300"/>
   </div>

   - Configure debugging options
   - **Controls**:
     - Use the **Joystick Up/Down** to navigate between debug options
     - Press **any key** to toggle an option
     - To go back, navigate to the back icon and press **any key**

## Error Screens

### Common Error Messages

1. **Invalid QR Code Error**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/error__invalid_qr.png" alt="Error Invalid QR View" width="300"/>
   </div>

   - Displayed when an invalid QR code is scanned
   - **Controls**: Press **any key** to acknowledge and try again

2. **Camera Error**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/error__camera.png" alt="Error Camera View" width="300"/>
   </div>

   - Displayed when camera cannot be accessed
   - **Controls**: Press **any key** to acknowledge and return to previous screen

3. **SD Card Error**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/error__sd_card.png" alt="Error SD Card View" width="300"/>
   </div>

   - Displayed when there's an SD card issue
   - **Controls**: Press **any key** to acknowledge, check SD card, and try again

4. **Low Battery Warning**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/error__low_battery.png" alt="Error Low Battery View" width="300"/>
   </div>

   - Warning when battery is running low
   - **Controls**: Press **any key** to acknowledge and consider charging the device

5. **Generic Error**

   <div align="center">
     <img src="https://github.com/SeedSigner/seedsigner-screenshots/raw/dev/en/error__generic.png" alt="Error Generic View" width="300"/>
   </div>

   - Generic error message for unexpected issues
   - **Controls**: Press **any key** to acknowledge and try again or restart the device

## Navigation Tips

### General Navigation Rules

1. **Moving Between Options**

   - Always use the **Joystick Up/Down** to navigate vertically through menu items
   - Use **Joystick Left/Right** to navigate horizontally when applicable
   - All three keys (A, B, C) perform the same selection function

2. **Going Back**

   - Look for the back arrow icon on each screen
   - Navigate to the back icon using the joystick
   - Press any key to activate and return to the previous screen

3. **Text Entry**

   - Use the joystick to navigate on-screen keyboards
   - Press any key to select characters
   - Look for delete buttons to remove characters
   - Navigate to "DONE" or "OK" to complete text entry

4. **Scrolling Content**

   - On screens with long content, use **Joystick Up/Down** to scroll
   - Content that extends beyond the screen will have scroll indicators

5. **QR Code Interaction**
   - On QR code screens, press any key to zoom in/out
   - Use the joystick to pan when zoomed in
   - Some QR codes may be animated - press any key to pause/resume

### Troubleshooting Navigation Issues

1. **Screen Not Responding**

   - Ensure the joystick is being pressed firmly in the desired direction
   - Try pressing one of the three keys (A, B, or C) to select the highlighted option
   - If still unresponsive, try restarting the device

2. **Can't Find Back Button**

   - Look for arrow icons, typically in corners of the screen
   - Some screens may use text labels like "Cancel" or "Exit"
   - Navigate to these options using the joystick, then press any key

3. **Text Entry Problems**
   - Make sure you're navigating to individual characters before pressing keys
   - Use the word suggestion toggles when entering seed words
   - Look for keyboard mode switches (abc, 123, symbols) for different character sets

This comprehensive guide covers all the major screens and navigation paths in the SeedSigner interface. Remember that the key to successful navigation is patience and systematic use of the joystick to highlight options before pressing any of the three selection keys.
