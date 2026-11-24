# Lord Cobham to Sir Francis Walsingham, May to June 1588

British Library, Harley MS 287, ff. 80r to 81r, 88r, 92r to 93v, and 96r to 97v. DECODE records `R8490` (5 May 1588, Ostend), `R8492` (1588, undated), `R8495` (27 May 1588, "Belgia"), and `R8496` (9 June 1588, Bourbourg).

- **State:** from key (three alphabet corrections extracted strictly from contemporary interlinear glosses on native scans of sibling letters `R8488` f. 75r and `R8493` f. 89r, then tested blind on all four unglossed letters).
- **Prior work:** Daniel Bourdeau and Brice Dudout studied these four letters on CypherSolver (`targets/cobham1588`, updated 14 November 2026), where the four letters stood classed as "decoded, not read" at 25% sure words (42 of 166 words across all four letters; 7 of 38 on `R8495`, 7 of 55 on `R8492`, 7 of 30 on `R8496`, 21 of 43 on `R8490`). Brice Dudout also established the held-out key test on `R8489` f. 78v and the code values `22` (Sir James Croft), `27` (Dr. Dale), `26` (Dr. Rogers), and square (the States).
- **What this folder adds:** three systematic key corrections from native-resolution inspection of `R8493` (f. 89r), plus zero-touch validation on Brice Dudout's pre-registered 13 November 2026 sign TSVs and full readings of `R8495`, `R8496`, `R8492`, and `R8490`.

## The three key corrections (from `R8493`, f. 89r)

1. **Hooked stem `rho` (transcribed `Y`) = `m`, not `r/y`.** Attested in contemporary interlinear glosses on `R8493` f. 89r in *may*, *them*, *from*, *my*, and *remove*. Unlocks *men*, *number*, *promises made*, *monthly*, *is namid*, *demande*, *monday*, *Dismuyde* (Dixmude), *Westmorland*, and *enemys*.
2. **Right-angled/barred `Gamma` (transcribed `T`) = `e`, not `t`.** Attested on `R8493` f. 89r in *entend*, *Pretend*, *proceed*, and *heer*. Unlocks *liftenant*, *men*, *charged*, *number*, *intelligens*, *winter*, *entised*, *written*, *passed*, and *treates*.
3. **Crossed-circle `phi` (transcribed `L`) is polyphonic `{l, p}`.** Attested on `R8493` f. 89r where *place* uses two identical `phi` signs, and independently confirmed on `R8496` f. 96v where cipher `V c L 7 V` decodes to *Roper*, matching the plain English postscript at the foot of the same folio ("with him cometh one Roper").

In addition, native-scan inspection settles three local readings: `A R` is polyphonic `{so, to}` ("how falce so ever yt ys" on `R8496`), `R8495` line 19 clear text reads "the cawse ys not knowen", and `R8492` line 7 reads complete "deliver" (`o 7 L I u 7 V`).

## Coverage across the four letters

| Record | Date | Prior CypherSolver (sure / any) | This reading (resolved / total) |
| --- | --- | ---: | ---: |
| `R8495` (f. 92r) | 27 May 1588 | 7 / 12 of 38 | 35 of 38 (92.1%) |
| `R8496` (f. 96v) | 9 June 1588 | 7 / 18 of 30 | 28 of 30 (93.3%) |
| `R8492` (f. 88r) | 1588, undated | 7 / 20 of 55 | 40 of 55 (72.7%) |
| `R8490` (ff. 80r to 80v) | 5 May 1588 | 21 / 35 of 43 | 39 of 43 (90.7%) |
| **Total** | | **42 / 85 of 166** | **142 of 166 (85.5%)** |

## Files

- `key.tsv`: corrected sign table with attestations on `R8488` and `R8493`.
- `reading.md`: readings of `R8495`, `R8496`, `R8492`, and `R8490`, with clear text in roman, decoded cipher in bold, and every unresolved word explicitly bracketed.
- `check.md`: blind statistical checks on Brice Dudout's untouched 13 November 2026 TSVs (`Z = +5.69` sigma) and on scan-verified rows (`Z = +7.42` sigma).

## Limits

- `24` of `166` cipher words across the four letters remain open or uncertain (mostly proper names and words containing the unglossed sign `K` in `R8492`) and stay bracketed in `reading.md`.
- No DECODE image and no DECODE transcription file is copied here.

## Credit

- **DECODE**, the database of historical ciphers of the DECRYPT project: records `R8488`, `R8490`, `R8492`, `R8493`, `R8495`, `R8496` (`https://de-crypt.org/decrypt-web/RecordsView/<n>`).
- **Archive:** British Library, Harley MS 287.
- **Database reference:** Mihály Héder and Beáta Megyesi, "The DECODE Database of Historical Ciphers and Keys: Version 2", HistoCrypt 2022, https://doi.org/10.3384/ecp188397.
- **Prior work credited:** Daniel Bourdeau and Brice Dudout (`dbourdeau/cyphersolver`, `targets/cobham1588`).
