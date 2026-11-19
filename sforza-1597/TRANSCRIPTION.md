# Sforza chancery letters, nine records: the transcription of the cipher rows

The files in `transcription/` are my own transcription of the DECODE images, as sign labels. They hold the cipher rows of each page, one line for each row.

The reads in `r5425-r5430/`, `r5463/second-read/` and `r5464-r5465/` use these rows. The earlier reads in `r5463/`, `r5464/` and `r5465/` use the sign transcription of the cipher ledger's maintainer. That transcription is not copied here.

## Credit

- **DECODE**, the database of historical ciphers of the DECRYPT project: records R5425 to R5430, R5463, R5464 and R5465. Record pages: https://de-crypt.org/decrypt-web/RecordsView/ followed by the record number, for example https://de-crypt.org/decrypt-web/RecordsView/5425.
- **The archive:** Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597.
- **The database:** Héder and Megyesi (2022), "The DECODE Database of Historical Ciphers and Keys: Version 2", HistoCrypt, https://doi.org/10.3384/ecp188397.
- No DECODE image is published.

## The files

- 12 files, one for each page or face with cipher rows: `<record>_p<page>_signs.txt`. `p` alone is the one page of a record. Page 2 of R5465 is a spread, with one file for each face.
- They hold 454 rows: 438 main rows, one of them struck out, and 16 rows between the lines or in the margin.
- Pages 2 of R5425 and R5426 are address faces with no cipher. They have no file.
- Three header lines start with `#`. Then each row is one line: its label, a flag in brackets for a row that stands apart or is struck out, and the tokens, split by spaces.
- The labels are those of the decode lines in `decryption.txt`, for example `L01` or `M01a`. A flag is `(interlinear)`, `(margin)` or `(cancelled)`.
- 24,716 tokens are signs. Each sign gives one character of the decode line of its row.
- Clear text is not in the rows. `[cleartext]` stands in its place.

## The marks

| Mark | Meaning |
| --- | --- |
| `G012` | one sign; a label names one sign shape across the nine records |
| `G012{...}` | one sign with a visible feature, in short words: `{3}`, `{dots?}`, `{faint}` |
| `G012?`, `[G012?]` | one sign; its label is not sure |
| `[G012\|G020?]` | one sign: G012 or G020; the left one is the better choice, and the read uses it |
| `G012\|G020` | one sign whose join across the pages stays open: G012 or G020; the read uses the left one |
| `[G012~G020]` | joined or touching ink: one sign or more; it gives no character in the decode |
| `[gap]`, `[gap:U01]` | a stretch not read, of unknown length |
| `[cleartext]` | clear words stood here; the file does not copy them |
| `<del>` ... `</del>` | signs struck through on the page |
| `_` | a wider space |
| `/` | R5425 page 1 only: a seam between two parts of the image, not ink |
| `[at:J01]`, `[above:I01]` | the place of a row that stands apart |

Inside a join, `x` is a stroke without a label, and `↑` and `↓` mark an upper and a lower part at one place.

## Doubts

- 432 tokens are not sure: 359 signs whose label carries `?`, and 73 places of joined ink.
- A second reading of the images checked some places of nine pages. It checked none of R5464 page 2 and the two faces of R5465 page 2.
