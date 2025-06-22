# SPV-256 — Seed Phrase Visualizer

**SPV-256 is the world's first visualizer for BIP39 seed phrases.**  
It transforms 256-bit entropy into a 16×16 editable pixel grid, enabling full control and reversible conversion between HEX, seed phrase, and PNG.

## Features

- Visual representation of 256-bit entropy (1 bit = 1 pixel)
- Support for 24-word BIP-39 seed phrases and raw 64-character hex input
- Editable 16×16 pixel grid
- Integrated decoder: convert PNG back to HEX and seed phrase
- Custom colors for bit 0, bit 1, and grid lines
- Dark mode (theme toggle reduces brightness to 80%)
- PNG export (323×323 px) with deterministic visual structure
- Checksum auto-validation and BIP-39 compliance
- Integrated English BIP-39 wordlist (2048 words)
- Airgap-ready: no internet connection required

## Specification

**Standard:**  
SPV-256 (Seed Phrase Visualizer – 256-bit)

**Input types:**  
- 24-word BIP-39 seed phrase  
- or 64-character hexadecimal string (256-bit entropy)  
- or PNG file previously exported from SPV-256

**Output types:**  
- 24-word BIP-39 seed phrase  
- and/or 64-character hexadecimal string  
- and/or PNG image (visual representation of entropy)

**Grid size:**  
16×16 pixels  
1 pixel = 1 bit (default: white = 0, black = 1)

**Checksum:**  
8 bits derived from SHA-256(entropy) — as per BIP-39

**Wordlist:**  
Built-in English BIP-39 (2048 words)

**Functionality:**  
- You can enter a 24-word seed phrase or a 64-character hex string to visualize entropy  
- You can draw manually on the pixel grid to generate corresponding HEX and seed phrase  
- You can upload a valid PNG from this tool to decode it back into entropy and mnemonic

**Core rule:**  
Bit value `1` must always appear visually darker than bit value `0`, regardless of selected colors. This is a strict requirement for consistency and interpretability.

## Security Notes

SPV-256 runs 100% offline in your browser. It is fully airgap-ready and requires no network access.  
A secure BIP-39 seed phrase can be generated manually by flipping a coin 256 times and entering the resulting bits directly into the pixel grid (dark pixel = 1, light pixel = 0), or by converting the binary string into a 64-character HEX value and pasting it into the HEX input field.

 Author: Aleksandr Yashchuk (2025)
  License: CC BY 4.0 — https://creativecommons.org/licenses/by/4.0/
  
 ## Links

- Website: [www.crownspv.com](https://www.crownspv.com)
- GitHub: [github.com/crownspv/spv-256](https://github.com/crownspv/spv-256)
- Twitter: [@crownspv](https://twitter.com/crownspv)
- Ordinals Collection "Complete Metamorphosis" Manifest: [www.crownspv.com/manifest-complete-metamorphosis](https://www.crownspv.com/manifest-complete-metamorphosis)
- Ordinals Collection "Complete Metamorphosis. Part 1. Mr Qubit.": [www.crownspv.com/ordinals-collection-part1](https://www.crownspv.com/ordinals-collection-part1)
- Ordinals Collection "Complete Metamorphosis. Part 2. Rare Mnemonic & Rare Entropy.": [www.crownspv.com/ordinals-collection-part-2](https://www.crownspv.com/ordinals-collection-part-2)
- Gmail: crownspv@gmail.com






