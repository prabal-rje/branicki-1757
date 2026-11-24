# Hopken and Carlson, Constantinople, December 1739 (11 bare pages)

Riksarkivet (Stockholm), Diplomatica Turcica `SE/RA/2119/2119.1/I/9/21`, IIIF series `R0003582` (568 images), images `p114R`, `p115L`, `p115R`, `p116L`, `p116R`, `p117L`, `p117R`, `p118L`, `p118R`, `p120L`, and `p120R` (`1,610` four-digit Code-1 cipher groups across 11 completely bare, unglossed pages).

- **State:** from key (Tier 1 frozen gloss-only key of `245` groups from `dbourdeau/cyphersolver/targets/hopken1739/key.tsv` plus Swedish chancery glosses read from `R0003582` images 18, 34, and 50; plus `48` bare-inferred Swedish syllables strictly tagged `bare_inferred` in `key.tsv`).
- **Prior work credited:** WAINUT (`LcCompany`) and Daniel Bourdeau (`dbourdeau/cyphersolver`, `targets/hopken1739`, catalogue item `1771`) reconstructed the French-glossed portion of this Code-1 key from images `255` to `257` and `260`, and decoded one short bare postscript (`263`, "decoded, not read"), noting that no bare despatch had yet been broken out of the volume. (`targets/hopken1740` covers a different key, Code 2, images `321` to `342`.)
- **Zero-leakage mechanical coverage across all 11 bare pages:**
  - **Tier 1 frozen gloss-only key (zero bare-page leakage):** **`1516` of `1610` groups (`94.2%`)**, ranging from `90.9%` to `97.5%` on every single page.
  - **Tier 1+2 expanded key (`+48` bare-inferred Swedish syllables):** **`1604` of `1610` groups (`99.6%`)**, with 7 pages at `100.0%` and only 6 single-occurrence tokens left bracketed (`1113, 1475, 1195, 1492, 1186, 1726`).

## Files

- `key.tsv`: provenance-tagged Code-1 key (`hopken1739`, `swedish_gloss`, and `bare_inferred`).
- `transcription.txt`: line-by-line transcription of all 11 bare pages (`p114R` to `p118R`, `p120L` to `p120R`).
- `decryption_frozen.txt`: unedited mechanical decode using only the Tier-1 frozen gloss key (`94.2%`).
- `decryption_expanded.txt`: unedited mechanical decode using the Tier 1+2 key (`99.6%`).
- `reading.md`: Swedish reading and English translation across all 11 bare pages.

## Limits and historical note

- Six single-occurrence groups (`1113, 1475, 1195, 1492, 1186, 1726`) remain open and stay bracketed.
- Sweden and the Ottoman Empire signed their *Defensivallians* on 24 December 1739; historians studying Swedish-Ottoman diplomacy in Riksarkivet *Diplomatica Turcica* (including work on the 1739 alliance at Umea University) may hold archival notes not online. No published edition or decipherment of `R0003582` images `114R` to `120R` was found online.
- No Riksarkivet scan image is redistributed here.

## Credit

- **Archive:** Riksarkivet (Stockholm), Diplomatica Turcica `SE/RA/2119/2119.1/I/9/21` (`https://lbiiif.riksarkivet.se/arkis!R0003582/manifest`).
- **Prior key work credited:** WAINUT (`LcCompany`) and `dbourdeau/cyphersolver` (`targets/hopken1739`, catalogue item `1771`).
