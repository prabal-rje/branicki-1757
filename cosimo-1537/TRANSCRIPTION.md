# Cosimo I to Niccolini: the transcription of the cipher rows

The files in `transcription/` are my own transcription of the DECODE images. They hold the digit rows of the cipher passages, one line for each row.

## Credit

- **DECODE**, the database of historical ciphers of the DECRYPT project: records R4034 to R4039, R4041 to R4050 and R4052 to R4054. Record pages: https://de-crypt.org/decrypt-web/RecordsView/ followed by the record number, for example https://de-crypt.org/decrypt-web/RecordsView/4039.
- **The archive:** Florence, Archivio Niccolini di Camugliano, Fondo antico 214, inserto 1.
- **The database:** Héder and Megyesi (2022), "The DECODE Database of Historical Ciphers and Keys: Version 2", HistoCrypt, https://doi.org/10.3384/ecp188397.
- No DECODE image is published.

## The files

- 19 files, one for each letter: `<record>_digits.txt`. They hold 306 rows and 12,056 digits.
- Four header lines start with `#`. Then each row is one line with three columns, split by tabs: DECODE's image number in the record, the row label and the row.
- Row labels: `Cnn` is a cipher row. `Lnn` is a line that holds cipher digits inside clear text.
- The rows do not hold later marks: foliation, endorsements, dates and notes in the margin.

## The marks

| Mark | Meaning |
| --- | --- |
| a digit | one cipher digit |
| `~` after a digit | a doubtful digit |
| `‾` after a digit | a digit under a bar (the earlier system only) |
| `[?]` | a clear word, or a stretch of the row that does not read |
| `#` | a sign that is not a digit |
| a space, `.`, `/` | a space, a point or a slash of the row |

## Doubts

- 239 digits are marked as doubtful.
