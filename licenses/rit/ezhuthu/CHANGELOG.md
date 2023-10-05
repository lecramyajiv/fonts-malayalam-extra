Version 1.3
===========

- [MAJOR] Rewritten Malayalam shaping rules: form post-base u1/u2 forms of Ra, below-base La first and then the rest of the conjuncts. This fixes a large chunk of issues with limited character set fonts - they now form Ra forms consistently
- Updated build & release scripts for automatic relese via GitLab CI
- Build script: fix OTF size issue

Version 1.2
===========

- Fix shaping involving double consontants such as ക്ട്ട where ട്ട shouldn't break.
- Lift hyphen character glyph a little above the baseline, but below half the x-height

Version 1.1
===========

- [FIX #7] Fixes couple of vowel sign shaping issues with Adobe InDesign

Version 1.0
===========

- Add character set specimen PDF
- Generate TTF for release now (generated OTF size is large, to be investigated)
- Add AppStream metadata file
- Add a note for commitment to the Rachana cause, and glyph naming convention
- SFD: simplified all curves (automatically using FontForge). Resulting TTF has no discernible shape change, but size is lot smaller
- Beta version 18
- GSUB: fix according to glyph name corrections in 3ae6c17
- Fix glyph names of ഥു, ഥൂ, ഥ്ന, ഥ്നു, ദ്ധ്മു
- Add README
- Add test files
- Makefile: use 'OTF' for testing
- [FIX] GSUB features - fix the script to remove lines with non-existent glyph names matching exactly
- Add buildscript
- Add OpenType features. Glyphs not existing in the font were removed from mlm2-gsub using a sed script
- Update copyright in TTF names
- Ezhuthu → Ezhuthu-Regular in file name and metadata/TTF names
- Ezhuthu: Malayalam handwriting font designed by Narayana Bhattathiri. Initial version
