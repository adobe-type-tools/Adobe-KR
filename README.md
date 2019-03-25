# The Adobe-KR-9 Character Collection
---
© 2019 Adobe Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy of this documentation file to use, copy, publish, distribute, sublicense, and/or sell copies of the documentation, and to permit others to do the same, provided that:

No modification, editing or other alteration of this document is allowed; and

The above copyright notice and this permission notice shall be included in all copies of the documentation.

Permission is hereby granted, free of charge, to any person obtaining a copy of this documentation file, to create their own derivative works from the content of this document to use, copy, publish, distribute, sublicense, and/or sell the derivative works, and to permit others to do the same, provided that the derived work is not represented as being a copy or version of this document.

Adobe shall not be liable to any party for any loss of revenue or profit or for indirect, incidental, special, consequential, or other similar damages, whether based on tort (including without limitation negligence or strict liability), contract or other legal or equitable grounds even if Adobe has been advised or had reason to know of the possibility of such damages. The Adobe materials are provided on an "AS IS" basis. Adobe specifically disclaims all express, statutory, or implied warranties relating to the Adobe materials, including but not limited to those concerning merchantability or fitness for a particular purpose or non-infringement of any third party rights regarding the Adobe materials.

Adobe holds no patents on the subject matter of this specification.

Last updated 2019-03-25

---
## Introduction

The purpose of this document is to define and describe the *Adobe-KR-9* character collection, which enumerates 22,897 glyphs, and whose designation is derived from the following three /CIDSystemInfo dictionary entries:

* /Registry (Adobe)
* /Ordering (KR)
* /Supplement 9

CIDFont resources that reference this character collection must include a /CIDSystemInfo dictionary that matches the /Registry and /Ordering strings shown above.

This document is designed for font developers, for the purpose of developing OpenType Korean fonts. It is also useful for application developers and end users who need to know more about the glyphs in this character collection. This document expects that its readers are familiar with the CID-keyed font file format, which is described in [Adobe Technical Note #5014](https://www.adobe.com/devnet/font.html), entitled *Adobe CMap and CIDFont Files Specification*.

A character collection contains the glyphs that are required to develop font products for a specific language, region, or set of scripts. Specific encodings are defined through the use of CMap resources that are instantiated as files, and generally reference a subset of the glyphs in the character collection.

The character collection that results from each Supplement includes the glyphs associated with all earlier Supplements. For example, Supplement 9 includes all glyphs defined in Supplements 0 through 8.

The Adobe-KR-9 character collection enumerates 22,897 glyphs, specifically CIDs 0 through 22896, among 10 Supplements, designated 0 through 9. Adobe-KR-9 completely supports the current [KS (*Korean Standard*) X 1001](http://www.kssn.net/stdks/KS_detail.asp?k1=X&k2=1001&k3=1) character set standard and all 11,172 modern hangul syllables, and also includes the hanja (aka ideographs) in the [KS X 1002](http://www.kssn.net/stdks/KS_detail.asp?k1=X&k2=1002&k3=1) character set standard, along with additional hanja from the [*Inmyeong-yong Hanja*](https://help.scourt.go.kr/nm/images/hanja/hanja_2015.pdf) (인명용 한자/人名用漢字) set that is published by the Supreme Court of Korea (*Daebeobwon*/대법원/大法院). The following table summarizes these 10 Supplements, and also provides the pages on which their representative glyphs are shown in the [*Adobe-KR-9.pdf*](https://github.com/adobe-type-tools/Adobe-KR/raw/master/Adobe-KR-9.pdf) file:

**Supplement** | **Additional CIDs** | **CID Range** | **Total CIDs** | **Date of Establishment** | **Pages**
--- | --- | --- | --- | --- | ---
0 | *n/a* | 0–3058 | 3,059 | 2018-07-19 | 1–7, 46
1 | 1,578 | 3059–4636 | 4,637 | 2018-07-19 | 7–10
2 | 6,814 | 4637–11450 | 11,451 | 2018-07-19 | 10–23
3 | 280 | 11451–11730 | 11,731 | 2018-07-19 | 23–24
4 | 147 | 11731–11877 | 11,878 | 2018-07-19 | 24
5 | 357 | 11878–12234 | 12,235 | 2018-07-19 | 24–25
6 | 2,003 | 12235–14237 | 14,238 | 2018-07-19 | 25–29
7 | 4,620 | 14238–18857 | 18,858 | 2018-07-19 | 29–38
8 | 3,622 | 18858–22479 | 22,480 | 2018-07-19 | 38–45
9 | 417 | 22480–22896 | 22,897 | 2018-07-19 | 45–46

Each CID (*Character ID*) in a character collection is associated with a class of character shapes or glyphs. The specific shape of a glyph from a given glyph class is dependent on the typeface style, typeface design, and possibly other factors. Glyphs for all CIDs are illustrated in this specification, providing a specific example or instance of the correspondence between a CID and its glyph shape class. Font developers should design glyphs for each CID of the character collection, and may use this document as a reference when proofing or otherwise validating CIDFont resources.

The following sections detail the history and contents of each of the 10 Supplements of the Adobe-KR-9 character collection.

---
## Supplement 0—Adobe-KR-0

Supplement 0, which includes a modest 3,059 glyphs, specifically CIDs 0 through 3058, is intended to provide a core set of glyphs that are expected to be in modern OpenType Korean fonts, and includes a minimal set of glyphs for modern hangul syllables, along with glyphs to support basic Korean and Latin typography. Of course, glyphs for the core set of 2,350 modern hangul syllables are included, along with glyphs for 418 additional high-frequency modern hangul syllables whose set was determined by KFA (*Korea Font Association*). Glyphs for a small number of additional modern hangul syllables are also included. In total, glyphs for 2,780 modern hangul syllables are included in Supplement 0. The table below specifies the number of glyphs for modern hangul syllables that are included in Supplement 0 for four character set standards, KS X 1001 (ROK), KS X 1002 (ROK), KPS 9566 (DPRK), and GB/T 12052 (PRC):

**Standard** | **Number of Glyphs**
--- | ---
KS X 1001 | 2,350 (all)
KS X 1002 | 372
KPS 9566 | 2,483
GB/T 12052 | 2,555

Also included in Supplement 0 are glyphs for ASCII, some ISO Latin 1 (aka ISO/IEC 8859-1) characters, punctuation, and some symbols. Several of the glyphs, such as those for punctuation, include both Western and Korean forms, and the short-term intent is to use the OpenType &#x27;[locl](https://docs.microsoft.com/en-us/typography/opentype/spec/features_ko#a-namelocl-idloclatag-locl)&#x27; (*Localized Forms*) GSUB feature to switch between them. The long-term goal is to possibly define Standardized Variation Sequences (SVSes) for them.

---
## Supplement 1—Adobe-KR-1

Supplement 1 adds 1,578 glyphs, specifically CIDs 3059 through 4636, all of which are for modern hangul syllables that are included in the KS X 1002 (ROK), KPS 9566 (DPRK), and GB/T 12052 (PRC) character set standards. The table below includes the number of glyphs for modern hangul syllables that are included in Supplement 1 for each of these three character set standards:

**Standard** | **Number of Glyphs**
--- | ---
KS X 1002 | 1,558
KPS 9566 | 196
GB/T 12052 | 818

In other words, Supplements 0 and 1 together provide basic support for the three regions with Korean-speaking populations for which regional standards have been established, at least in terms of the glyphs for modern hangul syllables.

---
## Supplement 2—Adobe-KR-2

Supplement 2 adds 6,814 glyphs, specifically CIDs 4637 through 11450, all of which are for modern hangul syllables that, when combined with those in Supplements 0 and 1, complete the set of 11,172 modern hangul syllables that have been included in Unicode since Version 2.0 (1996).

---
## Supplement 3—Adobe-KR-3

Supplement 3 adds 280 glyphs, specifically CIDs 11451 through 11730, for enclosed or otherwise annotated characters, such as digits, Latin characters, and hangul letters/syllables. The scope goes beyond what is found in regional character set standards, and includes appropriate characters found in the Unicode blocks named [Enclosed Alphanumerics](https://www.unicode.org/charts/PDF/U2460.pdf), [Dingbats](https://www.unicode.org/charts/PDF/U2700.pdf), [Enclosed CJK Letters and Months](https://www.unicode.org/charts/PDF/U3200.pdf), and [Enclosed Alphanumeric Supplement](https://www.unicode.org/charts/PDF/U1F100.pdf).

### Special Notes

Per [this page on the KS website](https://www.ksa.or.kr/ks.do), the glyph for U+327F &#x327F; KOREAN STANDARD SYMBOL (CID+11688) is generic, and its design should follow the described specification. Font developers who need this glyph can either reference the Adobe Illustrator file that is provided in the ZIP file whose link is at the bottom of that page, or reference one of the example fonts in the [latest release](https://github.com/adobe-type-tools/Adobe-KR/releases/latest) of this project whose glyph follows the speciication.

---
## Supplement 4—Adobe-KR-4

Supplement 4 adds 147 glyphs, specifically CIDs 11731 through 11877, for full-width punctuation, full-width Latin characters, and vertical forms.

---
## Supplement 5—Adobe-KR-5

Supplement 5 adds 357 glyphs, specifically CIDs 11878 through 12234, mainly for the purpose of KS X 1001 compatibility, for the benefit of font developers who feel that they need to support this particular character set standard in its entirety. Included in Supplement 5 are glyphs for math (only the basic math symbols are included in Supplement 0), line-drawing characters, and other symbols.

### Special Notes

Additional glyphs for KS X 1001 compatibility glyphs that correspond to Latin and specific scripts&mdash;Greek, Cyrillic, and Japanese kana&mdash;are included in Supplement 9.

---
## Supplement 6—Adobe-KR-6

Supplement 6 adds 2,003 glyphs, specifically CIDs 12235 through 14237, for the two hangul tone marks and their vertical forms, a modest set of 161 archaic (aka pre-modern) hangul syllables that fall outside the modern set of 11,172 that are necessary for the Jeju dialect (제주말 *jejumal*), nominal (aka encoded) forms of combining jamo, and the combining forms themselves. Included in the latter are six sets of leading jamo (L), two sets of vowel jamo (V), and four sets of trailing jamo (T). The OpenType &#x27;[ljmo](https://docs.microsoft.com/en-us/typography/opentype/spec/features_ko#ljmo)&#x27; (*Leading Jamo Forms*), &#x27;[vjmo](https://docs.microsoft.com/en-us/typography/opentype/spec/features_uz#vjmo)&#x27; (*Vowel Jamo Forms*), and &#x27;[tjmo](https://docs.microsoft.com/en-us/typography/opentype/spec/features_pt#tag-tjmo)&#x27; (*Trailing Jamo Forms*) GSUB features are expected to be used. The 1,838 glyphs for combining jamo can represent a staggering 1,638,750 hangul syllables (11,875 LV plus 1,626,875 LVT sequences), with the 11,172 modern hangul syllables being a very tiny subset.

### Special Notes

The [*ArchaicHangul161-Regular.pdf*](https://github.com/adobe-type-tools/Adobe-KR/raw/master/ArchaicHangul161-Regular.pdf) and [*ArchaicHangul161-Bold.pdf*](https://github.com/adobe-type-tools/Adobe-KR/raw/master/ArchaicHangul161-Bold.pdf) PDF files show the sequences and glyphs that correspond to the 161 archaic hangul syllables.

---
## Supplement 7—Adobe-KR-7

Supplement 7 adds 4,620 glyphs, specifically CIDs 14238 through 18857, for the 4,888 hanja (aka CJK Unified Ideographs) that are included in the KS X 1001 standard. The number of glyphs is actually 4,620, because 268 of the 4,888 hanja are genuine duplicates that are included in that character set standard due to multiple readings.

### Special Notes

The 268 hanja that are genuine duplicates are handled by mapping, via the Unicode [CMap resources](https://github.com/adobe-type-tools/cmap-resources/tree/master/Adobe-KR-9/), the corresponding CJK Compatibility Ideograph code points to the corresponding glyphs for their canonical equivalents, all of which are CJK Unified Ideographs. In addition, the UVS definition file also specifies SVSes that correspond to 270 CJK Compatibility Ideographs: U+F900 through U+FA0B, U+FA2E &amp; U+FA2F.

---
## Supplement 8—Adobe-KR-8

Supplement 8 adds 3,622 glyphs, specifically CIDs 18858 through 22479, for additional hanja beyond those in Supplement 7. Glyphs for the 2,856 hanja in the KS X 1002 character set standard are included. The rest of the glyphs in Supplement 8 are mainly for hanja that are included in the [*Inmyeong-yong Hanja*](https://help.scourt.go.kr/nm/images/hanja/hanja_2015.pdf) (인명용 한자/人名用漢字) set that is published by the Supreme Court of Korea (*Daebeobwon*/대법원/大法院), 665 of which are encoded in the URO and Extensions A, B, E, and F. 18 are supported by the IVD (Ideographic Variation Database) via the registered KRName IVD collection, and one outlier will be in Extension G and is therefore not yet encoded. Also included are 81 additional hanja, 73 of which are from GB/T 12052 (PRC), with the remaining eight from KPS 9566 (DPRK).

### Special Notes

Although the CID that corresponds to the glyph for Extension G ideograph ⿰氵恩, CID+22461, is stable, its identity&mdash;as specified in the fourth column of the [*Adobe-KR-9_ordering.txt*](https://github.com/adobe-type-tools/Adobe-KR/raw/master/Adobe-KR-9_ordering.txt) ordering file as the glyph named *u01200*, named after its U-Source source reference, UTC-01200&mdash;will eventually change to reflect the final Extension G code point, and it will then become encoded.

---
## Supplement 9—Adobe-KR-9

Supplement 9 adds 417 glyphs, specifically CIDs 22480 through 22896, foreign languages, such as those for extended Latin, Greek, Cyrillic, and Japanese kana. While most of the characters that are supported by these glyphs are in the KS X 1001 character set standard, I need to point out that this Supplement actually includes glyphs for characters outside of that standard, such as U+03C2 ς GREEK SMALL LETTER FINAL SIGMA for making Greek functional, and additional kana and kana-related characters, such as U+30FC ー KATAKANA-HIRAGANA PROLONGED SOUND MARK, which is necessary for katakana, along with appropriate vertical forms.

---
## Example OpenType Fonts

In the [latest release](https://github.com/adobe-type-tools/Adobe-KR/releases/latest) of this project you will find two fully-functional, ready-to-install, and style-linked example OpenType fonts that include all 22,897 glyphs of Adobe-KR-9. The fonts are based on the open source [*Source Han Serif*](https://github.com/adobe-fonts/source-han-serif/) Pan-CJK typeface design.

Recommended OpenType GSUB feature definitions, along with specific definitions of the &#x27;[halt](https://docs.microsoft.com/en-us/typography/opentype/spec/features_fj#a-namehalt-idhaltatag-halt)&#x27; (*Alternate Half Widths*) and &#x27;[vhal](https://docs.microsoft.com/en-us/typography/opentype/spec/features_uz#a-namevhal-idvhalatag-vhal)&#x27; (*Alternate Vertical Half Metrics*) GPOS features, will be published at a later date.

---
## Special Glyphs & Other Notes

The following sections detail special glyphs and other notes that are of interest to font developers. Several glyph classes are complex, and deserve some amount of explanation and clarification.

### Hangul Glyphs

The [*akr9-hangul.txt*](https://github.com/adobe-type-tools/Adobe-KR/raw/master/akr9-hangul.txt) datafile provides additional information for all 11,172 modern hangul syllables whose glyphs are included in Adobe-KR-9, specifically in Supplements 0 through 2.

### Space Glyphs

The following table lists all of the Adobe-KR-9 glyphs that are classified as a space, and provides the Unicode code point and character name, along with their recommended set widths (based on a 1000-unit em) and their values in the example OpenType fonts:

**CID** | **Unicode** | **Recommendation** | **Example Fonts**
--- | --- | --- | ---
1 | U+0020 SPACE | Proportional for Western use | 258 (Regular), 251 (Bold)
3006 | U+0020 SPACE | Proportional for Korean use | 310
108 | U+2002 EN SPACE | One-half of hangul syllable width | 483
109 | U+2003 EM SPACE | Hangul syllable width | 966
110 | U+2004 THREE-PER-EM SPACE | One-third of hangul syllable width | 322
111 | U+2005 FOUR-PER-EM SPACE | One-fourth of hangul syllable width | 242
112 | U+2006 SIX-PER-EM SPACE | One-sixth of hangul syllable width | 161
113 | U+2007 FIGURE SPACE | Figure width | 539 (Regular), 584 (Bold)
114 | U+2009 THIN SPACE | One-eighth of hangul syllable width | 121
115 | U+200A HAIR SPACE | One-sixteenth of hangul syllable width | 60
12105 | U+3000 IDEOGRAPHIC SPACE | Hanja width | 1000

### KS X 1001 Compatibility Glyphs

A small number of KS X 1001 characters map to different Unicode code points depending on the OS or other implementation, and while most of the glyphs are in Supplement 5, some of them are in earlier Supplements. The table below lists the KS X 1001 code points and the implementation-specific Unicode mappings (the Supplement of the corresponding glyph is indicated in parentheses):

**KS X 1001 (GR)** | Windows OS | macOS | Adobe
--- | --- | --- | ---
01-09 (0xA1A9) | U+00AD &#x00AD; (0) | U+2013 &#x2013; (0) | U+2013 &#x2013; (0)
01-10 (0xA1AA) | U+2015 &#x2015; (0) | U+2014 &#x2014; (0) | U+2014 &#x2014; (0)
01-11 (0xA1AB) | U+2225 &#x2225; (5) | U+2016 &#x2016; (5) | U+2016 &#x2016; (5)
01-13 (0xA1AD) | U+223C &#x223C; (5) | U+301C &#x301C; (4) | U+FF5E &#xFF5E; (4)
01-43 (0xA1CB) | U+FFE0 &#xFFE0; (5) | U+00A2 &#x00A2; (0) | U+FFE0 &#xFFE0; (5)
01-44 (0xA1CC) | U+FFE1 &#xFFE1; (5) | U+00A3 &#x00A3; (0) | U+FFE1 &#xFFE1; (5)
01-45 (0xA1CD) | U+FFE5 &#xFFE5; (5) | U+00A5 &#x00A5; (0) | U+FFE5 &#xFFE5; (5)
01-76 (0xA1EC) | U+226A &#x226A; (5) | U+226A &#x226A; (5) | U+00AB &#x00AB; (5)
01-77 (0xA1ED) | U+226B &#x226B; (5) | U+226B &#x226B; (5) | U+00BB &#x00BB; (5)
01-94 (0xA1FE) | U+FFE2 &#xFFE2; (5) | U+00AC &#x00AC; (5) | U+FFE2 &#xFFE2; (5)
02-06 (0xA2A6) | U+FF5E &#xFF5E; (5) | U+02DC &#x02DC; (5) | U+02DC &#x02DC; (5)
02-16 (0xA2B0) | U+02D0 &#x02D0; (5) | U+02D0 &#x02D0; (5) | U+2236 &#x2236; (5)
02-33 (0xA2C1) | U+2299 &#x2299; (5) | U+25C9 &#x25C9; (5) | U+25C9 &#x25C9; (5)
03-94 (0xA3FE) | U+FFE3 &#xFFE3; (4) | U+203E &#x203E; (5) | U+FFE3 &#xFFE3; (4)

### Glyph Set Widths

The following table provides CIDs and CID ranges that explicitly indicate which glyphs are intended to be designed with what set widths, though implementations are free to tailor the Full-width glyphs to be monospaced, or the Monospaced ones to be full-width: 

**Set Width** | **CIDs & CID Ranges**
--- | ---
Full-width | 0, 119, 128, 132, 135, 136, 138–147, 152–155, 158–169, 11451–11877, 11895, 11923–11925, 11932–11976, 11978–12107, 12151–12234, 14238–22479, 22690–22896
Proportional | 1–108, 110–118, 120–127, 129–131, 133, 134, 137, 148–151, 156, 157, 3001–3052, 11878–11894, 11896–11922, 11926–11931, 11977, 22480–22689
Monospaced | 109, 170–3000, 3053–3056, 3059–11450, 12108–12150, 12237–13500
Two-em | 3057
Three-em | 3058
Quarter-width | 12235, 12236
Zero-width | 13501–14237

The glyph table that included with this specification includes registration marks that serve to indicate relative set width. Explicitly specifying width classes, such as in the above table, is clearly more accurate and reliable than measuring the distance between registration marks. Please use both resources as your guide, and feel free to deviate on a case-by-case basis.

Note that the registration marks used in the glyph table are in a separate layer, and if their presence is annoying, that layer can be turned off, thus preventing their display.

---
## OpenType Development

As stated earlier in this specification, recommended OpenType feature definitions will be provided at a later date. Besides OpenType features, font developers are encouraged to implement subsets that may completely exclude one or more Supplements. Font developers are further encouraged to support Supplement 0&mdash;Adobe-KR-0&mdash;at a minimum. There is no particular requirement that all Supplements be supported, nor that all glyphs in a particular Supplement must be supported. Of course, some Supplements, if supported, are best supported in their entirety, such as Supplements 1, 2, and 7.

For example, it is possible to develop fonts that include only the glyphs for Supplements 0, 1, 2, and 7, which would therefore include the core glyphs, the glyphs for all 11,172 modern hangul syllables, and the glyphs for all hanja included in the KS X 1001 character set standard.

### Special Notes

Font developers should be aware that fonts which include all 22,897 glyphs&mdash;or nearly all of them&mdash;cannot be built with complete [Format 4 &#x27;cmap&#x27; subtables](https://docs.microsoft.com/en-us/typography/opentype/spec/cmap#format-4-segment-mapping-to-delta-values) due to the fragmented nature of the resulting mappings that cause that particular subtable to overflow beyond its 64K size limit. The [AFDKO](https://github.com/adobe-type-tools/afdko/) *makeotf* tool will truncate the subtable to include only the first two segments under such conditions. Our testing has revealed that some environments, particularly the Excel and Notepad apps running on Windows, make use of heuristics that require particular mappings to be present in the Format 4 &#x27;cmap&#x27; subtable. The two fully-functional example OpenType fonts in the [latest release](https://github.com/adobe-type-tools/Adobe-KR/releases/latest) worked around this issue by tailoring the Format 4 &#x27;cmap&#x27; subtable to exclude the mappings for all CJK Unified Ideographs and CJK Compatibility Ideographs. (The Format 4 &#x27;cmap&#x27; subtable is used only for the purpose of heuristics, and the glyphs for CJK Unified Ideographs and CJK Compatibility Ideographs work correctly because the [Format 12 &#x27;cmap&#x27; subtable](https://docs.microsoft.com/en-us/typography/opentype/spec/cmap#format-12-segmented-coverage) is used for actual rendering of those and other glyphs in the font.)

---
## CMap Resources

The CMap resources associated with the Adobe-KR-9 character collection, along with the [*cid2code.txt*](https://github.com/adobe-type-tools/cmap-resources/raw/master/Adobe-KR-9/cid2code.txt) datafile that provides additional details for font developers, are available as part of the [*CMap Resources*](https://github.com/adobe-type-tools/cmap-resources/) open source project.

Other than the Identity CMap resources that are provided for each of the 10 Supplements, only Unicode CMap resources—available for UTF-8, UTF-16 (UTF-16BE), and UTF-32 (UTF-32BE) encodings, and kept perfectly synchronized—are included, with the UTF-32 one being intended for use in developing OpenType fonts.

---
## Unicode Variation Sequences

The 36 Ideographic Variation Sequences (IVSes) that are specified in the [*Adobe-KR_sequences.txt*](https://github.com/adobe-type-tools/Adobe-KR/raw/master/Adobe-KR_sequences.txt) datafile are registered by The Unicode Consortium in the [IVD](http://www.unicode.org/ivd/) (*Ideographic Variation Database*) per [UTS #37](http://www.unicode.org/reports/tr37/) (*Unicode Ideographic Variation Database*), and correspond to the registered *KRName* IVD collection. This datafile also includes 270 [Standardized Variation Sequences](http://www.unicode.org/Public/UCD/latest/ucd/StandardizedVariants.txt) (SVSes), all of which correspond to CJK Compatibility Ideographs.

---
## Glyph Tables

Representative glyphs for CIDs 0 through 22896 are provided in the [*Adobe-KR-9.pdf*](https://github.com/adobe-type-tools/Adobe-KR/raw/master/Adobe-KR-9.pdf) file that is included in this repository, with 500 glyphs shown per page. And, for reader convenience, the beginning of each Supplement is clearly marked. The typeface used to exemplify each glyph is *Source Han Serif AKR9 Regular* (aka SourceHanSerifAKR9-Regular or 본명조 AKR9 Regular), designed by Adobe, and a derivative of the open source [*Source Han Serif*](https://github.com/adobe-fonts/source-han-serif/) Pan-CJK typeface design. The specific font instance is Version 1.001, as reflected in its /CIDFontVersion dictionary entry.

---
## Adobe-KR-9 Versus Adobe-Korea1-2

One of the purposes of the Adobe-KR-9 character collection is to replace the Adobe-Korea1-2 character collection, which was last updated in late 1998, and is no longer useful for developing modern Unicode-based Korean font resources. [Adobe Technical Note #5093](https://github.com/adobe-type-tools/Adobe-KR/raw/master/5093.Adobe-Korea1-2.pdf), *The Adobe-Korea1-2 Character Collection*, is included in this repository for reference purposes.

---
## Providing Feedback

Please send any feedback to the Adobe-KR-9 Character Collection specification author, [Dr. Ken Lunde](mailto:lunde@adobe.com?subject=[GitHub]%20The%20Adobe-KR-9%20Character%20Collection), for consideration.

---
## Changes Since Earlier Versions

The following sections detail the history of this document:

### Since the 2018-05-15—Supplement 9—Beta Version

Three Supplement 5 glyphs&mdash;*uni2260*, *uni2264*, and *uni2265*&mdash;were made proportional, and moved to Supplement 0. 21 KR-tagged glyphs&mdash;*uni002B.kr*, *uni0030.kr* through *uni0039.kr*, *uni003C.kr* through *uni003E.kr*, *uni00B1.kr*, *uni00D7.kr*, *uni00F7.kr*, *uni2212.kr*, *uni2260.kr*, *uni2264.kr*, and *uni2265.kr*&mdash;were added to Supplement 0. A Supplement 8 glyph, *u30726*, was renamed to *u01200* to reflect its UTC-01200 U-Source source reference, and is not yet encoded because Extension G is not yet stable.

### Since the 2018-07-19—Supplement 9—Version

A [**Special Notes**](#special-notes-4) subsection was added to the [**OpenType Development**](#opentype-development) section that describes possible Format 4 &#x27;cmap&#x27; subtable overflow.

### Since the 2018-08-01—Supplement 9—Version

The representative glyph for U+327F &#x327F; (Supplement 3 CID+11688) was adjusted to conform to the specifications of this particular character, and the two example fonts in the [latest release](https://github.com/adobe-type-tools/Adobe-KR/releases/latest) were updated accordingly.

### Since the 2018-09-04—Supplement 9—Version

The introductory paragraph of the [**Glyph Set Widths**](#glyph-set-widths) section was updated to allow tailoring of Full-width and Monospaced glyphs.

That is all.
