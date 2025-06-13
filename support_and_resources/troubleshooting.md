# 🆘 Troubleshooting

## Common Issues and Solutions

### Device Won't Boot

**Symptoms**: Black screen, no response when powered on
**Solutions**:

- ✅ Verify power source provides sufficient current (2A recommended)
- ✅ Check all hardware connections are secure
- ✅ Try a different SD card with fresh SeedSigner image
- ✅ Test with a different power cable

### QR Code Scanning Problems

**Symptoms**: QR codes not recognized, scanning timeouts
**Solutions**:

- ✅ Ensure adequate lighting on the QR code
- ✅ Hold the device steady at proper distance (6-12 inches)
- ✅ Clean the camera lens with a soft cloth
- ✅ Try adjusting QR code density in settings
- ✅ Check camera rotation settings
- ✅ Test camera functionality in Hardware I/O Test

### Incorrect Seed Generation

**Symptoms**: Generated seed doesn't match expected results
**Solutions**:

- ✅ Verify you're using proper entropy sources (good randomness)
- ✅ Ensure proper lighting during camera entropy capture
- ✅ For dice rolls, use proper physical dice (not digital)
- ✅ Double-check seed word transcription during backup
- ✅ Run the backup verification process

### Button Response Issues

**Symptoms**: Buttons not responding, inconsistent input
**Solutions**:

- ✅ Run Hardware I/O Test to isolate the problem
- ✅ Clean around buttons to remove debris
- ✅ Check for physical damage to the WaveShare hat
- ✅ Try different button combinations (A, B, C all function identically)

### Display Problems

**Symptoms**: Screen flickering, partial display, wrong colors
**Solutions**:

- ✅ Check WaveShare hat connections
- ✅ Run Hardware I/O Test display test
- ✅ Try different power source
- ✅ Verify SD card integrity

## Error Messages

### "Unknown QR Type"

**Meaning**: The scanned QR code format isn't recognized by SeedSigner
**Solutions**:

- ✅ Verify you're scanning a supported QR type (PSBT, SeedQR, etc.)
- ✅ Check QR code quality and clarity
- ✅ Ensure proper lighting and camera positioning

### "Invalid Seed"

**Meaning**: The entered seed phrase doesn't pass BIP-39 validation
**Solutions**:

- ✅ Double-check every word in your seed phrase
- ✅ Verify word order is correct
- ✅ Ensure all words are from the BIP-39 wordlist
- ✅ Check for typos in manual entry

### "Checksum Error"

**Meaning**: The final word doesn't match the required checksum
**Solutions**:

- ✅ Use the "Calc 12th/24th word" tool to find the correct final word
- ✅ Verify all previous words are correct
- ✅ Check for transcription errors
