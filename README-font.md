# Yapiri Script — Font & Keyboard

[![License: OFL](https://img.shields.io/badge/License-OFL%201.1-gold.svg)](OFL.txt)
[![Keyman](https://img.shields.io/badge/Keyman%20Keyboard-coming%20soon-lightgrey)](https://keyman.com)

> The official font for the **Yapiri script** — a phonemic alphabet designed for the Kokborok language of the Borok people of Tripura, India.  
> *Yapiri means "footprints" in Kokborok.*

🌐 **Project website:** [yapiriscript.com](https://yapiriscript.com)  
📥 **Download:** [yapiriscript.com/download](https://yapiriscript.com/download)

---

## What's in This Repo

```
yapiri-font/
├── Yapiri.ttf                             # Compiled TrueType font
├── Yapiri Chart Reference - Official.pdf  # Official glyph chart reference
├── LICENSE.md                             # Font licence
└── OFL.txt                                # SIL Open Font License 1.1
```

---

## About the Script

Yapiri is a **phonemic alphabet** — every sound in Kokborok is written explicitly. There are no inherent vowels (unlike an abugida). The only combining characters are:

| Diacritic | Unicode | Purpose |
|-----------|---------|---------|
| High tone mark | U+0301 | Marks high tone on a syllable |
| Reduplication mark | U+030B | Marks reduplicated syllables |

The **hyphen** (U+002D) is an integral part of the script, used to mark reduplication — a common grammatical feature of Kokborok where a word or syllable is repeated to form a new meaning.

ZWNJ (U+200C) is used to prevent combining marks from attaching to unintended base characters.

---

## PUA Codepoint Map

The Yapiri font uses the **Unicode Private Use Area (PUA)**, range **U+E000 – U+E02D** (46 characters).

> Since Yapiri uses PUA codepoints, glyphs will only render correctly if the Yapiri font is installed. See the **Yapiri Chart Reference PDF** in this repo for a visual glyph reference, or visit [yapiriscript.com/script](https://yapiriscript.com/script).

### Vowels

| Codepoint | Romanization |
|-----------|--------------|
| U+E000 | a |
| U+E001 | e |
| U+E002 | i |
| U+E003 | u |
| U+E004 | o |
| U+E005 | ə (schwa) |

### Consonants

| Codepoint | Romanization |
|-----------|--------------|
| U+E006 | p |
| U+E007 | t |
| U+E008 | k |
| U+E009 | ph |
| U+E00A | th |
| U+E00B | kh |
| U+E00C | b |
| U+E00D | d |
| U+E00E | g |
| U+E00F | ch |
| U+E010 | j |
| U+E012 | m |
| U+E013 | n |
| U+E014 | n′ |
| U+E015 | ng (ŋ) |
| U+E016 | s |
| U+E017 | r |
| U+E018 | l |
| U+E01C | y |
| U+E01D | w |
| U+E01E | h |

### Loanword Characters

Characters for sounds not native to Kokborok, used when writing loanwords from other languages.

| Codepoint | Romanization |
|-----------|--------------|
| U+E011 | chh |
| U+E019 | v |
| U+E01A | f |
| U+E01B | z |

### Numerals

| Codepoint | Value |
|-----------|-------|
| U+E01F | 0 |
| U+E020 | 1 |
| U+E021 | 2 |
| U+E022 | 3 |
| U+E023 | 4 |
| U+E024 | 5 |
| U+E025 | 6 |
| U+E026 | 7 |
| U+E027 | 8 |
| U+E028 | 9 |

### Punctuation

| Codepoint | Purpose |
|-----------|---------|
| U+E029 | Comma |
| U+E02A | Full stop |
| U+E02B | Exclamation mark |
| U+E02C | Quotation mark |
| U+E02D | Question mark |
| U+E02E–U+E02F | Reserved |

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

| Key | Codepoint | Character |
|-----|-----------|-----------|
| `a` | U+E000 | Vowel a |
| `e` | U+E001 | Vowel e |
| `i` | U+E002 | Vowel i |
| `u` | U+E003 | Vowel u |
| `o` | U+E004 | Vowel o |
| `x` | U+E005 | Schwa ə |
| `q` | U+E015 | ng (ŋ) |
| `Q` | U+E014 | n′ |
| `Shift+P` | U+E009 | ph |
| `Shift+T` | U+E00A | th |
| `Shift+K` | U+E00B | kh |
| `Shift+C` | U+E00F | ch |
| `'` | U+0301 | High tone mark |
| `\` | U+030B | Reduplication mark |
| `Shift+\` | U+200C | ZWNJ |

---

## Yapiri Primer *(coming soon)*

A beginner's guide to reading and writing in the Yapiri script is in development. The Yapiri Primer will cover the full character set, pronunciation, tone marking, and example words in Kokborok. It will be made available in this repo and on [yapiriscript.com](https://yapiriscript.com).

---

## Roadmap

- [x] PUA codepoint mapping (U+E000 – U+E02D)
- [x] OpenType GPOS mark-to-base anchors
- [x] Official glyph chart reference (PDF)
- [ ] Keyman keyboard package (desktop + touch layout)
- [ ] Yapiri Primer
- [ ] Kerning pairs refinement
- [ ] Unicode submission via Script Encoding Initiative (UC Berkeley)

---

## License

The **Yapiri font** is released under the [SIL Open Font License 1.1](OFL.txt) — free to use, share, and modify with attribution.  
The Yapiri script design is the intellectual work of **Animesh Debbarma**.

---

## Connect

- 🌐 [yapiriscript.com](https://yapiriscript.com)
- 📸 Instagram: [@yapiri_script](https://instagram.com/yapiri_script)
- 💬 WhatsApp Community: [Join here](https://whatsapp.com/channel/0029Vb7nZNk4o7qV793yfz1d)
