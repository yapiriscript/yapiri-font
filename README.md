# Yapiri Script — Font & Keyboard

[![License: OFL](https://img.shields.io/badge/License-OFL%201.1-gold.svg)](OFL.txt)
[![Keyman](https://img.shields.io/badge/Keyman%20Keyboard-v2.0-gold)](https://yapiriscript.com/download)
[![UCSUR](https://img.shields.io/badge/UCSUR-Plane%2015%20U+F1CA0–U+F1CFF-blue)](https://yapiriscript.com/ucsur.html)
[![Version](https://img.shields.io/badge/Version-2.0-gold)](https://yapiriscript.com)

> The official font and keyboard for the **Yapiri script** — a phonemic alphabet designed for the Kokborok language of the Tiprasa people of Tripura, India.  
> *Yapiri means "footprints" in Kokborok.*

🌐 **Project website:** [yapiriscript.com](https://yapiriscript.com)  
📥 **Download:** [yapiriscript.com/download](https://yapiriscript.com/download)  
📋 **UCSUR Proposal:** [yapiriscript.com/ucsur.html](https://yapiriscript.com/ucsur.html)

---

## What's New in v2.0

- **Codepoints migrated** from BMP PUA (U+E000–U+E02D) to **UCSUR Plane 15 (U+F1CA0–U+F1CFF)**
- **Character inventory finalized at 45** — f, chh, reduplication mark, and Yapiri-specific hyphen removed
- **v now carries the former chh glyph design**
- **High tone mark** is now a native Yapiri character at U+F1CD1 (not standard U+0301)
- **UCSUR block reservation confirmed** by Rebecca Bettencourt (June 2026)
- **Keyman keyboard v2.0** rebuilt with full P15 codepoint support

---

## What's in This Repo

```
yapiri-font/
├── Yapiri.ttf                             # Compiled TrueType font (v2.0, Plane 15)
├── Yapiri.woff2                           # Web font (WOFF2, v2.0, Plane 15)
├── keyman/
│   └── kokborok_yapiri.kmp               # Keyman keyboard package v2.0
├── LICENSE.md                             # Font licence
└── OFL.txt                                # SIL Open Font License 1.1
```

---

## About the Script

Yapiri is a **phonemic alphabet** — every sound in Kokborok is written explicitly. There are no inherent vowels (unlike an abugida). Each character represents exactly one phoneme.

The only combining character is:

| Diacritic | Unicode | Purpose |
|-----------|---------|---------|
| High tone mark | U+F1CD1 | Native Yapiri combining diacritic — marks high tone on a syllable |

Standard ASCII hyphen (U+002D) is used for hyphenation. No Yapiri-specific hyphen exists in v2.0.

---

## UCSUR Plane 15 Codepoint Map

The Yapiri font uses the **UCSUR Plane 15 Private Use Area**, block **U+F1CA0 – U+F1CFF** (**45 characters assigned**, 96 slots total).

> Block reserved by Rebecca Bettencourt (UCSUR), June 2026. Full proposal at [yapiriscript.com/ucsur.html](https://yapiriscript.com/ucsur.html).

### Vowels (U+F1CA0–U+F1CA5) — 6 characters

| Codepoint | Name | Romanization |
|-----------|------|--------------|
| U+F1CA0 | YAPIRI LETTER A | a |
| U+F1CA1 | YAPIRI LETTER E | e |
| U+F1CA2 | YAPIRI LETTER I | i |
| U+F1CA3 | YAPIRI LETTER U | u |
| U+F1CA4 | YAPIRI LETTER O | o |
| U+F1CA5 | YAPIRI LETTER SCHWA | ə |

### Consonants (U+F1CA7–U+F1CBD) — 23 characters

#### Stops

| Codepoint | Name | Romanization |
|-----------|------|--------------|
| U+F1CA7 | YAPIRI LETTER PA | p |
| U+F1CA8 | YAPIRI LETTER TA | t |
| U+F1CA9 | YAPIRI LETTER KA | k |
| U+F1CAA | YAPIRI LETTER BA | b |
| U+F1CAB | YAPIRI LETTER DA | d |
| U+F1CAC | YAPIRI LETTER GA | g |
| U+F1CAD | YAPIRI LETTER PHA | ph |
| U+F1CAE | YAPIRI LETTER THA | th |
| U+F1CAF | YAPIRI LETTER KHA | kh |

#### Affricates

| Codepoint | Name | Romanization |
|-----------|------|--------------|
| U+F1CB0 | YAPIRI LETTER CHA | ch |
| U+F1CB1 | YAPIRI LETTER JA | j |

#### Nasals

| Codepoint | Name | Romanization |
|-----------|------|--------------|
| U+F1CB2 | YAPIRI LETTER MA | m |
| U+F1CB3 | YAPIRI LETTER NA | n |
| U+F1CB4 | YAPIRI LETTER NA WITH PRIME | n′ |
| U+F1CB5 | YAPIRI LETTER NGA | ng |

#### Fricatives, Liquids & Glides

| Codepoint | Name | Romanization | Notes |
|-----------|------|--------------|-------|
| U+F1CB6 | YAPIRI LETTER SA | s | Native |
| U+F1CB7 | YAPIRI LETTER RA | r | Native |
| U+F1CB8 | YAPIRI LETTER LA | l | Native |
| U+F1CB9 | YAPIRI LETTER HA | h | Native |
| U+F1CBA | YAPIRI LETTER YA | y | Native |
| U+F1CBB | YAPIRI LETTER WA | w | Native, word-initial only |
| U+F1CBC | YAPIRI LETTER VA | v | Secondary — loanword |
| U+F1CBD | YAPIRI LETTER ZA | z | Secondary — loanword |

### Numerals (U+F1CC0–U+F1CC9) — 10 characters

| Codepoint | Name | Value |
|-----------|------|-------|
| U+F1CC0 | YAPIRI DIGIT ZERO | 0 |
| U+F1CC1 | YAPIRI DIGIT ONE | 1 |
| U+F1CC2 | YAPIRI DIGIT TWO | 2 |
| U+F1CC3 | YAPIRI DIGIT THREE | 3 |
| U+F1CC4 | YAPIRI DIGIT FOUR | 4 |
| U+F1CC5 | YAPIRI DIGIT FIVE | 5 |
| U+F1CC6 | YAPIRI DIGIT SIX | 6 |
| U+F1CC7 | YAPIRI DIGIT SEVEN | 7 |
| U+F1CC8 | YAPIRI DIGIT EIGHT | 8 |
| U+F1CC9 | YAPIRI DIGIT NINE | 9 |

### Punctuation (U+F1CCB–U+F1CCF) — 5 characters

| Codepoint | Name | Purpose |
|-----------|------|---------|
| U+F1CCB | YAPIRI COMMA | , |
| U+F1CCC | YAPIRI FULL STOP | . |
| U+F1CCD | YAPIRI EXCLAMATION MARK | ! |
| U+F1CCE | YAPIRI QUOTATION MARK | " |
| U+F1CCF | YAPIRI QUESTION MARK | ? |

### Diacritic (U+F1CD1) — 1 character

| Codepoint | Name | Purpose |
|-----------|------|---------|
| U+F1CD1 | YAPIRI HIGH TONE MARK | Combining diacritic — placed after vowel of high-tone syllable |

### Deliberate Gaps

| Codepoint | Reason |
|-----------|--------|
| U+F1CA6 | Reserved — between vowels and consonants |
| U+F1CBE–U+F1CBF | Reserved — after consonants |
| U+F1CCA | Reserved — before punctuation |
| U+F1CD0 | Reserved — before high tone mark |

---

## OpenType Features

### Mark-to-Base Anchors (GPOS)

| Feature | Table | Description |
|---------|-------|-------------|
| mark | GPOS | High tone mark (U+F1CD1) positioning over all base vowels and consonants |
| kern | GPOS | Kerning pairs for common Kokborok phoneme sequences |

---

## Keyman Keyboard v2.0

The Yapiri Keyman keyboard package (v2.0) supports Windows, macOS, Android, and iOS.

**Key mappings (highlights):**

| Key | Codepoint | Character |
|-----|-----------|-----------|
| `A` | U+F1CA0 | Vowel a |
| `E` | U+F1CA1 | Vowel e |
| `I` | U+F1CA2 | Vowel i |
| `U` | U+F1CA3 | Vowel u |
| `O` | U+F1CA4 | Vowel o |
| `Q` | U+F1CA5 | Schwa ə |
| `P` | U+F1CA7 | p |
| `Shift+P` | U+F1CAD | ph |
| `T` | U+F1CA8 | t |
| `Shift+T` | U+F1CAE | th |
| `K` | U+F1CA9 | k |
| `Shift+K` | U+F1CAF | kh |
| `C` | U+F1CB0 | ch |
| `F` | U+F1CB5 | ng |
| `N` | U+F1CB3 | n |
| `Shift+N` | U+F1CB4 | n′ |
| `V` | U+F1CBC | v |
| `Z` | U+F1CBD | z |
| `'` | U+F1CD1 | High tone mark |

Full touch layout: 3 layers (consonants / vowels+numerals+punctuation / global symbols)

---

## Roadmap

- [x] UCSUR Plane 15 codepoint mapping (U+F1CA0–U+F1CFF)
- [x] OpenType GPOS mark-to-base anchors (TTF + WOFF2)
- [x] Keyman keyboard v2.0 (desktop + mobile, P15 codepoints)
- [x] UCSUR block reservation confirmed (June 2026)
- [x] Official glyph chart reference
- [ ] Dedicated mobile keyboard app (Android/iOS)
- [ ] Kerning pairs refinement
- [ ] Unicode submission via Script Encoding Initiative (UC Berkeley)

---

## License

The **Yapiri font** is released under the [SIL Open Font License 1.1](OFL.txt) — free to use, share, and modify with attribution. Reserved Font Name: **"Yapiri"**.

The Yapiri script design is the intellectual work of **Animesh Debbarma**.

---

## Connect

- 🌐 [yapiriscript.com](https://yapiriscript.com)
- 📋 [UCSUR Proposal](https://yapiriscript.com/ucsur.html)
- 📘 Facebook: [@YapiriKokborok](https://www.facebook.com/YapiriKokborok)
- 📸 Instagram: [@yapiri_script](https://instagram.com/yapiri_script)
- 🐦 X: [@yapiriscript](https://x.com/yapiriscript)
- ▶️ YouTube: [@YapiriScript26](https://www.youtube.com/@YapiriScript26)
- 💬 WhatsApp: [Join here](https://whatsapp.com/channel/0029Vb7nZNk4o7qV793yfz1d)
