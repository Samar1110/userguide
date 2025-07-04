# Calc 12th/24th Word Seed Generation

This seed creation method allows you to generate a cryptographically secure seed phrase by entering 11 words (for 12-word seed) or 23 words (for 24-word seed) manually, then calculating the final word with proper checksum validation. The final word (12th or 24th) incorporates additional entropy and ensures the seed phrase meets BIP39 standards.

## Complete Process with All Screenshots

1. **Navigate**: Main Menu → **Tools** → **"Calc 12th/24th word"**

<div align="center">
     <img src="images/ToolsOptionSelectView.png" alt="Tools menu selection" width="250"/>
</div>
<div align="center">
     <img src="images/SeedGenerateCalcMethodView.png" alt="Dice method selection" width="250"/>
</div>

2. **Choose Length**: Select **12 words** or **24 words**

<div align="center">
     <img src="images/SeedMnemonicLengthCalcView.png" alt="Final word calculation seed length" width="250"/>
</div>

3. **Enter Existing Words**: Use the on-screen keyboard with intelligent word suggestions:
   - **Key A**: Move up in the suggestions list
   - **Key C**: Move down in the suggestions list  
   - **Key B**: Select the highlighted suggested word

<div align="center">
     <img src="images/WordEntry.png" alt="On-screen keyboard with word suggestions" width="250"/>
</div>

<div align="center">
     <img src="images/ToolsCalcFinalWordEnterSeedView.png" alt="Entering existing seed words" width="250"/>
</div>

## Entropy Methods for Final Word Calculation

The system provides three different entropy sources to calculate the final word, ensuring cryptographic security:
<div align="center">
     <img src="images/ToolsCalcFinalWordFinalizePromptView.png" alt="Final seed word" width="250"/>
</div>

**🪙 Coin Flip Entropy Method**

- Flip a physical coin exactly 7 times
- For each flip, select **1 for Heads** or **0 for Tails** by pressing the **Joystick**
- This method provides 7 bits of entropy for the final word calculation

<div align="center">
     <img src="images/ToolsCalcFinalWordCoinFlipsView.png" alt="Coin flip entropy interface" width="250"/>
</div>

- The system displays your binary string and calculates the checksum

<div align="center">
     <img src="images/ToolsCalcFinalWordCoinFlipResultView.png" alt="Coin flip result display" width="250"/>
</div>

**📝 Word Selection Entropy Method**

- Choose any word from the BIP39 wordlist as your entropy source
- The selected word provides the entropy bits needed for final word calculation

<div align="center">
     <img src="images/ToolsCalcFinalWordEntropyView.png" alt="Word selection entropy method" width="250"/>
</div>

<div align="center">
     <img src="images/ToolsCalcFinalWordEntropyResultView.png" alt="Word selection entropy method" width="250"/>
</div>

**🔢 Finalize with Zeros Method**

- Uses a simple 7-bit string of zeros plus the calculated 4-bit checksum
- This is the simplest method but still produces a valid final word

<div align="center">
     <img src="images/ToolsCalcFinalWordZerosMethodView.png" alt="Zeros method selection" width="250"/>
</div>

## Final Word Display and Completion

**Final Word Display**

- Shows the calculated final word with full derivation details
- Displays the entropy source used and checksum calculation

<div align="center">
     <img src="images/ToolsCalcFinalWordShowFinalWordView.png" alt="Final word calculation screen" width="250"/>
</div>

**Completion Screen**

- Review the complete seed phrase with the calculated final word
- Your seed is now ready for backup and use

<div align="center">
     <img src="images/ToolsCalcFinalWordDoneView.png" alt="Final word calculation completion" width="250"/>
</div>

> **📚 Technical Note**: The final word in any BIP39 seed contains both entropy bits and checksum bits. The checksum ensures the seed phrase is mathematically valid and helps detect transcription errors.