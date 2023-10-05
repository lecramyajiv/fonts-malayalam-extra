Version 2.2
===========

- Makefile: updated build directory & release targets; and adjusted TeX test file
- [FIX] Build script: generated OTF file size can be greatly reduced via the 'round' option
- [MAJOR] Rewritten Malayalam shaping rules: form post-base u1/u2 forms of Ra, below-base La first and then the rest of the conjuncts. This fixes a large chunk of issues with limited character set fonts - they now form Ra forms consistently

Version 2.1
===========

- Add details of font
- Add AppStream metadata
- Completely new Makefile to build and test fonts
- Completely new tests
- Completely new Malayalam OpenType shaping rules, supporting only mlm2 script tag
- Complete new build tool
- Update font PS/TTF name and copright details
- Remove all OpenType features from SFD
- Sundar: completely remove OpenType features for Malayalam, build tool and test files, preparing for a rewrite.
- Remove half forms and reference glyphs

Version 2.0.1
=============

- [FIX #3] Credit/copyright issue raised by Santhosh Thottingal. Add proper copyright and license files to features, build tool and test data
- Fix shaping of k3th3th4 --- ഗ്ദ്ധ

Version 2.0.0
=============

- RIT-Sundar: License
- RIT Sundar: makefile to compile source and generate TTF/WOFF
- RIT-Sundar: test files
- RIT-Sundar: build script
- RIT-Sundar: Opentype Lookup Features
- RIT-Sundar: initial glyph source
