Version 1.2
===========

- Build: shrink OTF size, and fix version check. Also add additional packages requierd for CI
- [FIX] glyph name of ഷ്ര , and add missing shaping rule for it. Thanks to test script for identifying it.
- Add test to check if glyphs are assigned either a Unicode codepoint or a shaping rule
- Add fontfonfig file for Panmana
- AppStream metadata: move to subdirectory

Version 1.1
===========

- GitLab: automated release management
- Makefile: updated build directory & release targets; and adjusted TeX test file
- [FIX] Build script: generated OTF file size can be greatly reduced via the 'round' option
- [MAJOR] Rewritten Malayalam shaping rules: form post-base u1/u2 forms of Ra, below-base La first and then the rest of the conjuncts. This fixes a large chunk of issues with limited character set fonts - they now form Ra forms consistently

Version 1.0
===========

- Add GitLab CI/CD
- Fix font name in Makefile
- Fix glyph of ngngui (it was same as ngngu2)
- Remove test pdf from version control
- Add License file
- Updated description
- Add AppStream metadata
- Add description of font and details of dedication
- Add test cases
- Build tools
- OpenType shaping rules
- source: Panmana → Panmana-Regular
- Fix metadata: font names, weight in OS/2 & Panose, TTF names etc.
- Revision 10
- Panmana development version 6
