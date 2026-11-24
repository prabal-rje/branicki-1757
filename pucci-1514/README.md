# Antonio Pucci to Lorenzo de' Medici, Valladolid, 31 August 1514

Archivio di Stato di Firenze (ASF), Mediceo avanti il Principato (MAP), filza CXXXVII, doc. 644 (cc. 652r to 652 bis v). CypherSolver catalogue entry `2392` (vetted 6 November 2026 as open; no key tried, no reading on record).

- **State:** from ciphertext (partial read). The underlying alphabet is a simple `+1` Caesar shift on the 20-letter Renaissance Italian alphabet (`a->b` through `x->z`), combined with 12 syllable/digraph ligatures and 12 two-digit diplomatic nomenclator codes.
- **Digital source:** ASF MAP IIIF scans (`A0001399.ptif`, `A0001400.ptif`, `A0001402.ptif`). No scan image is redistributed here.
- **Statistical check:** evaluated strictly on `307` cipher-derived core plaintext letters (excluding all clear text and unconfirmed ligatures), the `+1` shift and ligature decode scores `-2.297` nats/char under a 5-gram Renaissance Florentine language model against random-key null `-9.220 +/- 0.939` (`Z = +7.37` sigma).

## What the letter says

Written from Valladolid on 31 August 1514, 24 days after the Anglo-French Treaty of London (7 August 1514), papal nuncio Antonio Pucci reports his 27 August audience with King Ferdinand the Catholic to Lorenzo de' Medici. Ferdinand is deeply discontented with `[43]` (contextually Pope Leo X) over the exclusion of the marriage pact of `[99]` through `[43]`'s mediation between `[94]` and `[32]`, a concession taken from `[100]`, the Crusade bull (`cruciata`), and suspicion of a secret understanding between `[43]` and `[32]` on Italian affairs. Over the last three months Ferdinand has committed grave injuries in spiritual matters while excusing them under ancient privileges; only the necessity of the times restrains him, and for now he desires peace between `[31]` and `[22]` and a league with `[43]` and all Italy for the defence of Italy.

## Files

- `key.tsv`: `+1` letter shift, 12 verified ligatures, and 12 two-digit nomenclator codes (with contextual hypotheses strictly separated from literal decode).
- `reading.md`: clear Italian opening, deciphered core (lines 4 to 14), and clear closing.
- `translation.md`: English translation.

## Limits

- Eight two-digit nomenclator codes (`22, 31, 42, 47, 77, 92, 97, 100`) have no key sheet and stay as raw numbers; the four contextual identifications (`43, 32, 94, 99`) are explicitly marked as hypotheses in `key.tsv`.
- Several rare non-alphabetic abbreviations/ligatures in lines 4 to 14 remain unconfirmed and are marked `[...]` in `reading.md`.
- Venetian and Spanish state papers for August to September 1514 have not yet been checked for parallel summaries of Pucci's audience.

## Credit

- **Archive:** Archivio di Stato di Firenze, Mediceo avanti il Principato, filza CXXXVII, doc. 644 (cc. 652r to 652 bis v).
- **Catalogue entry:** `dbourdeau/cyphersolver`, catalogue entry `2392` (MAP filza CXXXVII sweep, 6 November 2026).
