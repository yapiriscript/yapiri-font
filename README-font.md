# Yapiri Script — Font & Keyboard

[![License: OFL](https://img.shields.io/badge/License-OFL%201.1-gold.svg)](LICENSE)
[![FontForge](https://img.shields.io/badge/Built%20with-FontForge-222)](https://fontforge.org)
[![Keyman](https://img.shields.io/badge/Keyboard-Keyman-terracotta)](https://keyman.com)

> The official font source and keyboard package for the **Yapiri script** — a phonemic alphabet designed for the Kokborok language of the Borok people of Tripura, India.

🌐 **Project website:** [yapiriscript.com](https://yapiriscript.com)  
📥 **Download compiled files:** [yapiriscript.com/download](https://yapiriscript.com/download)

---

## What's in This Repo

```
yapiriscript-font/
├── source/
│   └── yapiri.sfd              # FontForge source file
├── fonts/
│   └── Yapiri.ttf              # Compiled TrueType font
├── keyman/
│   ├── yapiri.kmn              # Keyman keyboard source
│   ├── yapiri.kps              # Keyman package source
│   ├── yapiri.kmp              # Compiled Keyman package
│   └── touch_layout.keyman     # Touch layout for mobile
├── scripts/
│   └── build.py                # FontForge Python automation script
├── docs/
│   └── codepoint-map.md        # Full PUA codepoint reference
└── README.md
```

---

## About the Script

Yapiri is a **phonemic alphabet** — every sound in Kokborok is written explicitly. There are no inherent vowels (unlike an abugida). The only combining characters are:

| Diacritic | Unicode | Purpose |
|-----------|---------|---------|
| High tone mark | U+0301 | Marks high tone on a syllable |
| Reduplication mark | U+030B | Marks reduplicated syllables |

ZWNJ (U+200C) is used to prevent combining marks from attaching to unintended base characters.

---

## PUA Codepoint Map

The Yapiri font uses the **Unicode Private Use Area (PUA)**, range **U+E000 – U+E02F** (48 characters).

### Consonants

| Codepoint | Character | Romanization |
|-----------|-----------|--------------|
| U+E000 | ᯀ | k |
| U+E001 | ᯁ | kh |
| U+E002 | ᯂ | g |
| U+E003 | ᯃ | ng (ŋ) |
| U+E004 | ᯄ | c |
| U+E005 | ᯅ | ch |
| U+E006 | ᯆ | j |
| U+E007 | ᯇ | t |
| U+E008 | ᯈ | th |
| U+E009 | ᯉ | d |
| U+E00A | ᯊ | n |
| U+E00B | ᯋ | n′ |
| U+E00C | ᯌ | p |
| U+E00D | ᯍ | ph |
| U+E00E | ᯎ | b |
| U+E00F | ᯏ | m |
| U+E010 | ᯐ | r |
| U+E011 | ᯑ | l |
| U+E012 | ᯒ | w |
| U+E013 | ᯓ | s |
| U+E014 | ᯔ | h |
| U+E015 | ᯕ | y |

### Vowels

| Codepoint | Character | Romanization |
|-----------|-----------|--------------|
| U+E016 | ᯖ | a |
| U+E017 | ᯗ | i |
| U+E018 | ᯘ | u |
| U+E019 | ᯙ | e |
| U+E01A | ᯚ | o |
| U+E01B | ᯛ | ə (schwa) |

### Numerals

| Codepoint | Character | Value |
|-----------|-----------|-------|
| U+E01C | ᯜ | 0 |
| U+E01D | ᯝ | 1 |
| U+E01E | ᯞ | 2 |
| U+E01F | ᯟ | 3 |
| U+E020 | ᯠ | 4 |
| U+E021 | ᯡ | 5 |
| U+E022 | ᯢ | 6 |
| U+E023 | ᯣ | 7 |
| U+E024 | ᯤ | 8 |
| U+E025 | ᯥ | 9 |

### Punctuation & Diacritics

| Codepoint | Character | Purpose |
|-----------|-----------|---------|
| U+E026 | — | Word separator |
| U+E027 | — | Sentence terminator |
| U+E028 | — | High tone mark (base glyph) |
| U+E029 | — | Reduplication mark (base glyph) |
| U+E02A–U+E02F | — | Reserved |

> **Note:** Codepoints shown as `—` are non-spacing combining or punctuation glyphs without a direct Latin romanization. See `docs/codepoint-map.md` for full glyph details.

---

## OpenType Features

### Mark-to-Base Anchors (GPOS)

Two anchor classes are defined for diacritic positioning:

| Anchor Class | Diacritic | Attaches To |
|---|---|---|
| `top_tone` | High tone mark (U+0301) | All base consonants and vowels |
| `top_reduplication` | Reduplication mark (U+030B) | All base consonants and vowels |

Anchors are set per-glyph in FontForge to ensure consistent vertical alignment across the character set.

---

## Keyman Keyboard

### Key Mappings

| Key | Output | Character |
|-----|--------|-----------|
| `a` | U+E016 | Vowel a |
| `e` | U+E019 | Vowel e |
| `i` | U+E017 | Vowel i |
| `u` | U+E018 | Vowel u |
| `o` | U+E01A | Vowel o |
| `x` | U+E01B | Schwa ə |
| `q` | U+E003 | ng (ŋ) |
| `Q` | U+E00B | n′ |
| `Shift+P` | U+E00D | ph |
| `Shift+T` | U+E008 | th |
| `Shift+K` | U+E001 | kh |
| `Shift+C` | U+E005 | ch |
| `'` | U+0301 | High tone mark |
| `\` | U+030B | Reduplication mark |
| `Shift+\` | U+200C | ZWNJ |

### Installation

1. Download `yapiri.kmp` from [yapiriscript.com/download](https://yapiriscript.com/download) or the [releases page](../../releases)
2. Install [Keyman](https://keyman.com) for your platform
3. Open the `.kmp` file — Keyman will install the keyboard and font automatically

---

## Building from Source

### Prerequisites

- [FontForge](https://fontforge.org) (with Python scripting enabled)
- [Keyman Developer](https://keyman.com/developer) (for keyboard compilation)

### Build the Font

```bash
fontforge -script scripts/build.py
# Output: fonts/Yapiri.ttf
```

The build script handles glyph import, metrics normalization, PUA codepoint assignment, anchor attachment, and TTF export.

### Build the Keyman Package

Open `keyman/yapiri.kps` in Keyman Developer and compile, or use the CLI:

```bash
kmc build keyman/yapiri.kps
# Output: keyman/yapiri.kmp
```

---

## Roadmap

- [x] PUA codepoint mapping (U+E000 – U+E02F)
- [x] OpenType GPOS mark-to-base anchors
- [x] Keyman keyboard package (desktop + touch layout)
- [x] FontForge Python build automation
- [ ] Kerning pairs refinement
- [ ] Variable font exploration
- [ ] Unicode submission via Script Encoding Initiative (UC Berkeley)

---

## License

The **font** is released under the [SIL Open Font License 1.1](LICENSE) — free to use, share, and modify with attribution.  
The **keyboard source** is released under MIT.  
The Yapiri script design is the intellectual work of **Animesh Debbarma (Zitorin)**.

---

## Connect

- 🌐 [yapiriscript.com](https://yapiriscript.com)
- 📸 Instagram: [@yapiri_script](https://instagram.com/yapiri_script)
- 💬 WhatsApp Community: [Join here](https://yapiriscript.com/community)
