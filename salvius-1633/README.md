# Johan Adler Salvius to Axel Oxenstierna, Lubeck, 27 June 1633

Riksarkivet (Stockholm), Oxenstiernska samlingen E 708. Target record: `DECODE R4339` (`Oxenstiernska_samlingen_E_708-2`, dated "Datum Lubeck den 27. Junij Stil. vet. Ao 1633", signed `JAS`, 4 pages, completely unglossed).

- **State:** from key (1633 two-digit homophonic alphabet `12` to `82`, 16-code null block `84` to `99`, and 13 core nomenclator/function codes extracted strictly from contemporary interlinear glosses on sibling records `R4338` [8/18 June 1633] and `R4340` [15 August 1633], then tested blind on unglossed `R4339`).
- **Prior work:** Tracked on CypherSolver (`targets/oxenstierna1633`, catalogue item 207) as not solved ("text not obtained; Still open: Everything"). Brice Dudout (PR #569, 14 November 2026) identified Johan Adler Salvius as probable writer from the Riksarkivet volume listing; no transcription, key, or decode existed.
- **Catalogue correction:** `DECODE R4341` is dated Stockholm, `1/11 February 1635` (signed `JAS`) and uses a separate 1635 nomenclator, correcting DECODE's dating of all four E 708 records to 1646 and CypherSolver's grouping of all four under June 1633.

## Summary of result

- **15 of 15** two-digit alphabetical cipher runs in unglossed `R4339` are decoded: `liws`, `obscure`, `ambigue`, `videntur`, `dilation`, `balance`, `condolera`, `denigrera`, `ambiguum`, `Lebzelters`, `incuriosus`, `prevenire`, `gener`, `aurem`, and `separationem`.
- **Zero-leakage blind test:** glossed codes from `R4338 + R4340` alone directly cover `93` of `137` two-digit tokens (`67.9%`) in `R4339`. Under an automatic `+/-2` contiguous-block rule with zero tuning on `R4339`, the decode beats 1,000 exact letter-permutation nulls at `Z = +5.57` sigma (`Z = +5.95` sigma on the full 1633 key).

## Files

- `key.tsv`: complete 1633 two-digit homophonic alphabet, null block, and 13 core nomenclator/function codes with witness attestations.
- `transcription_r4339.txt`: my transcription of all 15 unglossed two-digit cipher runs in `R4339`.
- `reading.md`: full table of all 15 decoded runs, surrounding Swedish/Latin text, English translation, and historical summary.
- `check.md`: blind statistical validation against 1,000 letter-permutation nulls on an independent classical Latin character 4-gram model.

## Limits

- Roughly 18 rare 4-digit nomenclator codes in `R4339` that do not appear in the glosses of `R4338` or `R4340` (for example `828`, `2523`, `2066 1/2`, `2320`, `2888`, `3841`) and two trailing numbers (`20.18`) after `aurem` stay open and are left bracketed.
- No DECODE image is copied here.

## Credit

- **DECODE**, the database of historical ciphers of the DECRYPT project: records `R4338`, `R4339`, `R4340`, `R4341` (`https://de-crypt.org/decrypt-web/RecordsView/<n>`).
- **Archive:** Riksarkivet (Stockholm), Oxenstiernska samlingen E 708.
- **Database reference:** Mihály Héder and Beáta Megyesi, "The DECODE Database of Historical Ciphers and Keys: Version 2", HistoCrypt 2022, https://doi.org/10.3384/ecp188397.
- **Prior note credited:** Brice Dudout (`dbourdeau/cyphersolver`, PR #569, identifying Salvius).
