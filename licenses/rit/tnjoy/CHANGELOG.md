Version 1.4.1
=============

- Fixes to metadata - fontconfig & appstream

Version 1.4
===========

- Remove unused glyphs (half forms, accent references etc.)
- Sources: remove unnecessary old shaping rules from SFD
- [FIX] glyph name of shr3 ഷ്ര
- Makefile: run glyph test by default
- Add test for checking glyphs have either Unicode codepoint or shaping rule
- [FIX] Build script: use cffsubr to actually shrink OTF
- Gitlab CI: add packages for OTF building
- Build script: shrink OTF file size even further
- Makefile: update for metadata location change
- TNJoy: fontconfig file
- Move AppStream medatata to subdirectory

Version 1.3
===========

- Makefile: updated build directory & release targets; and adjusted TeX test file
- Fix AppStream metadata license
- [FIX] Build script: generated OTF file size can be greatly reduced via the 'round' option
- [MAJOR] Rewritten Malayalam shaping rules: form post-base u1/u2 forms of Ra, below-base La first and then the rest of the conjuncts. This fixes a large chunk of issues with limited character set fonts - they now form Ra forms consistently

Version 1.2
===========

- Update PS/TTF names to follow proper style naming
- Add AppStream metadata
- Add description
- Move bold/extrabold SFD to sources dir and Glyphnames: follow naming convention for ി andീ  glyphs
- Kerning: remove non-existent glyphs and adjust kerning values
- Glyphnames: follow naming convention for ി andീ  glyphs
- Test: use TTF file
- Shaping rules: remove substitutions of non-existent glyphs
- Complete new test cases
- New make file
- New OpenType lookup rules and kerning
- New build tool
- Move SFD files to sources directory

Version 1.1
===========

- [FIX #1] Credit/copyright issue raised by Santhosh Thottingal. Add proper copyright and license files to features, build tool and test data

Version 1.0
===========

- TN Joy Regular: adjust kerning for chandrakkala. TODO: verify if same kern values are good for Bold/ExtraBold
- TN Joy Regular: adjust kerning for 'ya/yu/yU' sign. TODO: verify if same kern values are good for Bold/ExtraBold
- TN Joy Regular: adjust kerning for 'va' sign. TODO: verify if same kern values are good for Bold/ExtraBold
- TN Joy Extra Bold: initial version. Kerning values to be adjusted
- TN Joy Bold: initial version. Kerning values to be adjusted
- TN Joy Regular: set OS/2 PFM family to 'Sans Serif' instead of 'Decorative'
- TN Joy: glyphs updated by Hussain
- TN Joy: conditional akhn for k1n1 and t3t3
- Metadata: fix Manufacturer name
- Add OFL 1.1 license
- Fix minor typo (space before ndash)
- Font name: tnjoy -> tnjoy-regular
- Conditional akhn lookup for '[s1/h1/zh] + xx + consonant + [u1/u2/r1]' conjuncts without u1/u2/r1 glyphs
- Conditional akhn lookup for 'sh + xx + consonant + u1/u2/r1' conjuncts without u1/u2/r1 glyphs
- Conditional akhn lookup for '[m1/y1/l3/z1]+xx+consonant+u1/u2/r1' conjuncts without u1/u2/r1 glyphs
- Conditional akhn lookup for 'p3+xx+consonant+u1/u2/r1' conjuncts without u1/u2/r1 glyphs
- Conditional akhn lookup for 'p2+xx+consonant+u1/u2/r1' conjuncts without u1/u2/r1 glyphs
- Conditional akhn for 't3/nh/th1/p1'+xx+consontant+u1/u2/r1 combination
- Kerning of 'ya' symbol -- reduce kern
- Conditional akhn lookup for ch2/ch3/nj. Test cases: ച്ഛ  ച്ഛോ  ച്ഛു  ച്ഛൂ  ജ്ഞ  ജ്ഞോ  ജ്ഞു  ജ്ഞൂ  ഞ്ഛ  ഞ്ഛോ  ഞ്ഛു  ഞ്ഛൂ
- Kerning: more combinations by Hussain KH
- Conditional akhn lookup for k3, k4. Test cases: ഗ്ദ  ഗ്ദ്ധ  ഗ്ദോ  ഗ്ദ്രോ  ഗ്ദു  ഗ്ദൂ  ഗ്ദ്ധോ  ഗ്ദ്ധ്രോ  ഗ്ദ്ധു  ഗ്ദ്ധൂ  ഗ്ന  ഗ്നോ  ഗ്നു  ഗ്നൂ  ഗ്മ  ഗ്മോ  ഗ്മു  ഗ്മൂ  ഘ്ന  ഘ്നോ  ഘ്നു  ഘ്നൂ
- Conditional akhn lookup for more 'k1...' conjuncts. Test cases: ക്സ  ക്സ്സ  ക്സോ  ക്സു  ക്സൂ  ക്റ്റ  ക്റ്റോ  ക്റ്റു  ക്റ്റൂ
- Conditional akhn lookup for ക്ഷ്ണ and ക്ഷ്മ. Test cases: ക്ഷ്ണ  ക്ഷ്ണ്ണ  ക്ഷ്ണോ  ക്ഷ്ണു  ക്ഷ്ണൂ  ക്ഷ്മ  ക്ഷ്മ്മ  ക്ഷ്മോ  ക്ഷ്മു  ക്ഷ്മൂ
- Lookup rules: many conjuncts don't have 'u1/u2' forms such as 'k1t1u1 ക്ടു' and in that case 'k1t1 u1' is not correct, instead 'k1 t1u1' should be used. This is achievable with a single conditional lookup ignoring subsequent '[xx u1 u2]' but further complicates 'k1t1r3' which is formed by 'k1 xx t1 xx r3'. But 'k1t1r3' also don't have 'u1/u2' shapes, but 't1r3' has 'u1/u2' form, so they should form 'k1 t1r3u1'.
- tnjoy -> tnjoy-regular
- Remove vim swap file
- Add test files
- Build tools and makefile
- Opentype features. In addition to Sundar, more kerning pairs and 'akhn' for k3th3th4 glyph added
- TN Joy: update metadata - font name, copyright, weight etc.
- RIT 'TN Joy': initial version of font
