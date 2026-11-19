# Francia 32: the transcription of the cipher rows

The files in `transcription/` are my own transcription of the DECODE images. They hold the cipher rows of each cipher page, one line for each row.

## Credit

- **DECODE**, the database of historical ciphers of the DECRYPT project: records R5612 to R5618, R5620 and R5621. Record pages: https://de-crypt.org/decrypt-web/RecordsView/ followed by the record number, for example https://de-crypt.org/decrypt-web/RecordsView/5612.
- **The archive:** Archivio Apostolico Vaticano, Segreteria di Stato, Francia 32.
- **The database:** Héder and Megyesi (2022), "The DECODE Database of Historical Ciphers and Keys: Version 2", HistoCrypt, https://doi.org/10.3384/ecp188397.
- No DECODE image is published.

## The files

- 30 files, one for each cipher page: `<record>_f<folio>_digits.txt`. They hold 383 rows of 9 records.
- R5619 has no images on DECODE, so it has no file. R5618 and R5620 have rows but no reading.
- Four header lines start with `#`. Then each row is one line: its label, a space and the row.
- Most labels are cipher rows: `C01`, `C02`, .... On ff. 62r and 62v, cipher and clear text share the lines, so the label is the line of the page: `L02`, `L04`, ....
- Clear text is not copied. `‖` stands in its place.

## The marks

| Mark | Meaning |
| --- | --- |
| a digit, alone or with a mark | one cipher digit; the mark above it is a vowel sign (2̈, 3̂, 4̄, 5⁺ ...) or a dot |
| `[d?]` | one doubtful digit |
| `[a\|b?]` | one sign with two readings; the decode takes the left one if it is a digit |
| `[?]` | one sign not read |
| a lone lower-case letter | a sign that my transcription reads as a letter; the key reads it as a code letter |
| `⟨...⟩`, `[... sign]`, `[... glyph]` | a sign that my transcription describes and does not read as a digit |
| `ω`, `∞`, `△`, `Δ`, `#` and other symbols | signs that my transcription gives as symbols |
| `^{...}` | a raised mark above the digit before it |
| `[unresolved span]` and other `[unresolved ...]` notes | a stretch not read, of unknown length |
| other `[...]` notes | a note on the place of the row on the page |
| `⟦ ... ⟧` | a stretch of cipher that my transcription marks as tentative |
| `//` | a break in the cipher run |
| `{C01: ...}` | on f. 62v, a cipher group inside a line of the page |
| `‖` | clear text stood here |

## Doubts

- The files hold only the rows with 10 or more digit signs. Shorter cipher groups inside clear text are not in them, for example on f. 71r.
