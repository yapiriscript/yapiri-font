# Yapiri Script — Font & Keyboard

[![License: OFL](https://img.shields.io/badge/License-OFL%201.1-gold.svg)](OFL.txt)
[![Keyman](https://img.shields.io/badge/Keyman%20Keyboard-v1.0-gold)](https://yapiriscript.com/download)

> The official font for the **Yapiri script** — a phonemic alphabet designed for the Kokborok language of the Tiprasa people of Tripura, India.  
> *Yapiri means "footprints" in Kokborok.*

🌐 **Project website:** [yapiriscript.com](https://yapiriscript.com)  
📥 **Download:** [yapiriscript.com/download](https://yapiriscript.com/download)

---

## What's in This Repo

```
yapiri-font/
├── Yapiri.ttf                             # Compiled TrueType font
├── Yapiri.woff2                           # Web font (WOFF2)
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

The **hyphen** (U+002D) is an integral part of the script, used to mark word-level reduplication — a common grammatical feature of Kokborok where a word is repeated to form a new meaning. It is a standard Unicode character, not a PUA glyph.

ZWNJ (U+200C) is used to prevent combining marks from attaching to unintended base characters.

---

## PUA Codepoint Map

The Yapiri font uses the **Unicode Private Use Area (PUA)**, range **U+E000 – U+E02D** (**48 characters**), plus 1 global symbol (U+002D hyphen) = **48+1 total**.

> Since Yapiri uses PUA codepoints, glyphs will only render correctly if the Yapiri font is installed. See the **Yapiri Chart Reference PDF** in this repo for a visual glyph reference, or visit [yapiriscript.com/script](https://yapiriscript.com/script).

### Vowels (U+E000–U+E005)

| Codepoint | Romanization |
|-----------|--------------|
| U+E000 | a |
| U+E001 | e |
| U+E002 | i |
| U+E003 | u |
| U+E004 | o |
| U+E005 | ə (schwa) |

### Consonants (U+E006–U+E01E)

#### Stops — Voiceless, Aspirated, Voiced

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

#### Affricates

| Codepoint | Romanization | Notes |
|-----------|--------------|-------|
| U+E00F | ch | |
| U+E010 | j | |
| U+E011 | chh | Secondary — pending linguistic documentation; no active lexical examples confirmed |

#### Nasals

| Codepoint | Romanization |
|-----------|--------------|
| U+E012 | m |
| U+E013 | n |
| U+E014 | n′ |
| U+E015 | ng (ŋ) |

#### Fricatives, Liquids & Glides

| Codepoint | Romanization |
|-----------|--------------|
| U+E016 | s |
| U+E017 | r |
| U+E018 | l |
| U+E01C | y |
| U+E01D | w |
| U+E01E | h |

#### Extended & Secondary Characters (loanword / optional use)

| Codepoint | Romanization | Classification |
|-----------|--------------|----------------|
| U+E019 | v | Secondary — loanword; no native phonemic equivalent |
| U+E01A | f | Optional extended; *ph* is standard in native Kokborok text |
| U+E01B | z | Secondary — loanword; phonetically distinct from /j/ |

### Numerals (U+E01F–U+E028)

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

### Punctuation (U+E029–U+E02D)

| Codepoint | Purpose |
|-----------|---------|
| U+E029 | Comma |
| U+E02A | Full stop |
| U+E02B | Exclamation mark |
| U+E02C | Quotation mark |
| U+E02D | Question mark |

### Global Symbol

| Character | Unicode | Purpose |
|-----------|---------|---------|
| Hyphen ‐ | U+002D | Word-level reduplication marker — standard Unicode, not PUA |

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

The Yapiri Keyman keyboard package (v1.0) is available for download at [yapiriscript.com/download](https://yapiriscript.com/download). It supports Windows, macOS, Linux, and Android.

**Key mappings:**

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
| *(verify in .kmn source)* | U+030B | Reduplication mark |
| `Shift+\` | U+200C | ZWNJ |

> **Note:** The key binding for the reduplication mark (U+030B) has been flagged for verification against the `.kmn` source — the previously documented `\` mapping may be incorrect.

---

## Yapiri Primer

A complete beginner's guide to reading and writing in the Yapiri script is now live at [yapiriscript.com/primer](https://yapiriscript.com/primer.html). It covers the full character set, pronunciation, tone marking, diacritics, writing rules, and example words in Kokborok. A printable PDF version is also available.

---

## Roadmap

- [x] PUA codepoint mapping (U+E000 – U+E02D)
- [x] OpenType GPOS mark-to-base anchors (TTF + WOFF2)
- [x] Official glyph chart reference (PDF)
- [x] Keyman keyboard package (desktop + Android)
- [x] Yapiri Primer (web + printable PDF)
- [ ] Keyman touch layout refinement (iOS / mobile)
- [ ] Kerning pairs refinement
- [ ] UCSUR registration of PUA codepoints
- [ ] Unicode submission via Script Encoding Initiative (UC Berkeley)

---

## License

The **Yapiri font** is released under the [SIL Open Font License 1.1](OFL.txt) — free to use, share, and modify with attribution.  
The Yapiri script design is the intellectual work of **Animesh Debbarma**.

---

## Connect

- 🌐 [yapiriscript.com](https://yapiriscript.com)
- 📘 Facebook: [@YapiriKokborok](https://www.facebook.com/YapiriKokborok)
- 📸 Instagram: [@yapiri_script](https://instagram.com/yapiri_script)
- 🐦 X: [@yapiriscript](https://x.com/yapiriscript)
- ▶️ YouTube: [@YapiriScript26](https://www.youtube.com/@YapiriScript26)
- 💬 WhatsApp Community: [Join here](https://whatsapp.com/channel/0029Vb7nZNk4o7qV793yfz1d)
