# Yapiri Script — Font & Keyboard

[![License: OFL](https://img.shields.io/badge/License-OFL%201.1-gold.svg)](OFL.txt)
[![Keyman](https://img.shields.io/badge/Keyman%20Keyboard-coming%20soon-lightgrey)](https://keyman.com)

> The official font for the **Yapiri script** — a phonemic alphabet designed for the Kokborok language of the Borok people of Tripura, India.  
> *Yapiri (ᯌᯩᯇᯤᯔᯤ) means "footprints" in Kokborok.*

🌐 **Project website:** [yapiriscript.com](https://yapiriscript.com)  
📥 **Download:** [yapiriscript.com/download](https://yapiriscript.com/download)

---

## What's in This Repo

```
yapiri-font/
├── Yapiri.ttf                          # Compiled TrueType font
├── Yapiri Chart Reference - Official.pdf  # Official glyph chart reference
├── LICENSE.md                          # Font licence
└── OFL.txt                             # SIL Open Font License 1.1
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

> Since Yapiri uses PUA codepoints, glyphs will only render correctly if the Yapiri font is installed. See the **Yapiri Chart Reference PDF** in this repo for a visual glyph reference, or visit [yapiriscript.com/script](https://yapiriscript.com/script).

### Consonants

| Codepoint | Romanization |
|-----------|--------------|
| U+E000 | k |
| U+E001 | kh |
| U+E002 | g |
| U+E003 | ng (ŋ) |
| U+E004 | c |
| U+E005 | ch |
| U+E006 | j |
| U+E007 | t |
| U+E008 | th |
| U+E009 | d |
| U+E00A | n |
| U+E00B | n′ |
| U+E00C | p |
| U+E00D | ph |
| U+E00E | b |
| U+E00F | m |
| U+E010 | r |
| U+E011 | l |
| U+E012 | w |
| U+E013 | s |
| U+E014 | h |
| U+E015 | y |

### Vowels

| Codepoint | Romanization |
|-----------|--------------|
| U+E016 | a |
| U+E017 | i |
| U+E018 | u |
| U+E019 | e |
| U+E01A | o |
| U+E01B | ə (schwa) |

### Numerals

| Codepoint | Value |
|-----------|-------|
| U+E01C | 0 |
| U+E01D | 1 |
| U+E01E | 2 |
| U+E01F | 3 |
| U+E020 | 4 |
| U+E021 | 5 |
| U+E022 | 6 |
| U+E023 | 7 |
| U+E024 | 8 |
| U+E025 | 9 |

### Punctuation & Diacritics

| Codepoint | Purpose |
|-----------|---------|
| U+E026 | Word separator |
| U+E027 | Sentence terminator |
| U+E028 | High tone mark (base glyph) |
| U+E029 | Reduplication mark (base glyph) |
| U+E02A–U+E02F | Reserved |

---

## OpenType Features

### Mark-to-Base Anchors (GPOS)

Two anchor classes are defined for diacritic positioning:

| Anchor Class | Diacritic | Attaches To |
|---|---|---|
| `top_tone` | High tone mark (U+0301) | All base consonants and vowels |
| `top_reduplication` | Reduplication mark (U+030B) | All base consonants and vowels |

---

## Keyman Keyboard

A Keyman keyboard package for Yapiri is in the works. It will be available here and on [yapiriscript.com/download](https://yapiriscript.com/download) once released.

**Planned key mappings:**

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

---

## Yapiri Primer *(coming soon)*

A beginner's guide to reading and writing in the Yapiri script is in development. The Yapiri Primer will cover the full character set, pronunciation, tone marking, and example words in Kokborok. It will be made available in this repo and on [yapiriscript.com](https://yapiriscript.com).

---

## Roadmap

- [x] PUA codepoint mapping (U+E000 – U+E02F)
- [x] OpenType GPOS mark-to-base anchors
- [x] Official glyph chart reference (PDF)
- [ ] Keyman keyboard package (desktop + touch layout)
- [ ] Yapiri Primer
- [ ] Kerning pairs refinement
- [ ] Unicode submission via Script Encoding Initiative (UC Berkeley)

---

## License

The **Yapiri font** is released under the [SIL Open Font License 1.1](OFL.txt) — free to use, share, and modify with attribution.  
The Yapiri script design is the intellectual work of **Animesh Debbarma (Zitorin)**.

---

## Connect

- 🌐 [yapiriscript.com](https://yapiriscript.com)
- 📸 Instagram: [@yapiri_script](https://instagram.com/yapiri_script)
- 💬 WhatsApp Community: [Join here](https://yapiriscript.com/community)
