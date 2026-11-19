# Francia 346, the 22 digit records: the transcription of the cipher rows

The files in `transcription/` are my own transcription of the DECODE images. They hold the cipher rows of each cipher page of the 22 records R5626 to R5659, one line for each row.

The decode lines of the record pages `r5626.md` to `r5659.md`, the key-free read and `check.md` use these rows.

## Credit

- **DECODE**, the database of historical ciphers of the DECRYPT project: records R5626, R5635 to R5637, R5640, R5642, R5643 and R5645 to R5659. Record pages: https://de-crypt.org/decrypt-web/RecordsView/ followed by the record number, for example https://de-crypt.org/decrypt-web/RecordsView/5626.
- **The archive:** Archivio Apostolico Vaticano, Segreteria di Stato, Francia 346.
- **The database:** Héder and Megyesi (2022), "The DECODE Database of Historical Ciphers and Keys: Version 2", HistoCrypt, https://doi.org/10.3384/ecp188397.
- No DECODE image is published.

## The files

- 35 files, one for each cipher page: `<record>_f<folio>_digits.txt`. They hold 539 rows of 22 records.
- Four header lines start with `#`. Then each row is one line: its label, a space and the row.
- The label is the row of the decode line: `C01` in `R5626_f154r_digits.txt` is the line "R5626, f. 154r, C01" of `r5626.md`.
- The nine records of 13 November, the pages of `rereads.md` and the leaves R74 to R84 have no file here.
- Clear text is not copied. `[gap: cleartext dropped]` stands in its place.

## The marks

| Mark | Meaning |
| --- | --- |
| a digit | one cipher digit |
| a digit with `?` in brackets, for example `[7?]` | one doubtful digit |
| `[a\|b?]`, for example `[7\|3?]` | one sign with two or more readings; the decode takes the left one |
| `[?]` | one sign that I do not read |
| `[overwritten glyph]`, `[X-shaped sign]`, `[V-shaped sign]` | one sign that I do not read as a digit |
| `[unresolved cipher run]`, `[illegible]`, `[overwritten cipher signs: illegible]`, `[glyph count disputed]` | a stretch not read, of unknown length |
| `[gap: cleartext dropped]` | clear text stood here; the file does not copy it |
| a note that ends in `not a baseline digit`, `[rule to the right]`, `[sublinear strokes: attachment indistinct]` | a mark on the page that is not a digit; it takes no place |
| `⟦ ... ⟧` around a row | a row that I mark as tentative |

## Doubts

- 46 rows are tentative: every row of R5642 f. 246r and of R5657 f. 342r, and 5 rows of R5648 f. 279v.
- On R5642 f. 246r, R5656 f. 337r and R5657 ff. 342r–v, 8 is rare and 6 is common. So I may read some 8s as 6 there. `rereads.md` decodes a later transcription of these pages; its rows are not here.
