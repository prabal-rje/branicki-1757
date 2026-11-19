# Francia 346, the later leaves: the transcription of the cipher rows

The files in `transcription/` are my own transcription of the DECODE images, a reconciled draft. They hold the cipher rows of the 19 pages of the later leaves that `decryption.txt` decodes, one line for each row.

## Credit

- **DECODE**, the database of historical ciphers of the DECRYPT project: records R5626, R5635, R5636, R5637, R5640, R5642, R5643 and R5645 to R5651. Record pages: https://de-crypt.org/decrypt-web/RecordsView/ followed by the record number, for example https://de-crypt.org/decrypt-web/RecordsView/5626.
- **The archive:** Archivio Apostolico Vaticano, Segreteria di Stato, Francia 346.
- **The database:** Héder and Megyesi (2022), "The DECODE Database of Historical Ciphers and Keys: Version 2", HistoCrypt, https://doi.org/10.3384/ecp188397.
- No DECODE image is published.

## The files

- 19 files, one for each page: `<record>_f<folio>_digits.txt`. They hold 303 rows of 14 records.
- Four header lines start with `#`. The first gives the page label of `decryption.txt`, for example `006_154r_R5626_P5`. Then each row is one line: its label, a space and the row.
- The label is the row of the decode line: `C01` in `R5626_f154r_digits.txt` is the line `006_154r_R5626_P5 C01` of `decryption.txt`.
- The digits of R74 to R78 rest on other people's readings. They have no file here.
- Clear text is not copied. `[gap: cleartext dropped]` stands in its place.

## The marks

| Mark | Meaning |
| --- | --- |
| a digit | one cipher digit |
| a digit with `?` in brackets, for example `[7?]` | one doubtful digit |
| `[a\|b?]`, for example `[7\|3?]` | one sign with two or more readings; the left one is the reconciled reading |
| `[?]` | one sign that I do not read |
| `[overwritten glyph]`, `[X-shaped sign]`, `[V-shaped sign]` | one sign that I do not read as a digit |
| `[unresolved cipher run]`, `[illegible]`, `[overwritten cipher signs: illegible]`, `[glyph count disputed]` | a stretch not read, of unknown length |
| `[gap: cleartext dropped]` | clear text stood here; the file does not copy it |
| a note that ends in `not a baseline digit`, `[rule to the right]`, `[sublinear strokes: attachment indistinct]` | a mark on the page that is not a digit; it takes no place |
| `⟦ ... ⟧` around a row | a row that I mark as tentative |

## Doubts

- This is my earlier transcription of these pages. `../francia-346-full/transcription/` holds a later one of the same 19 pages. 93 of the 303 rows differ between the two.
- 5 rows of R5648 f. 279v are tentative.
