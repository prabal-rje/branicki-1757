# The Duke of Sessa to Charles V: the transcription of the cipher rows

The files in `transcription/` are my own transcription of the DECODE images. They hold the cipher rows and the mixed rows of each record, one line for each row.

## Credit

- **DECODE**, the database of historical ciphers of the DECRYPT project: records R9873 to R9881, R9883 to R9887, R9889 to R9901 and R9903 to R9905. Record pages: https://de-crypt.org/decrypt-web/RecordsView/ followed by the record number, for example https://de-crypt.org/decrypt-web/RecordsView/9873.
- **The archive:** Real Academia de la Historia, Madrid, Colección Salazar y Castro A-31 (9/31) and A-34 (9/34).
- **The database:** Héder and Megyesi (2022), "The DECODE Database of Historical Ciphers and Keys: Version 2", HistoCrypt, https://doi.org/10.3384/ecp188397.
- No DECODE image is published.

## The files

- 30 files, one for each record: `<record>_<folios>_rows.txt`. They hold 1,347 rows.
- R9902 has no cipher rows, so it has no file.
- Four header lines start with `#`. Then each row is one line: `<page>/<row>`, a space, and the units, split by spaces. `<page>` is the image page of the DECODE record.
- A row with a label and no units is an empty row.

## The marks

| Token | Meaning |
| --- | --- |
| Latin letters, digits or a sign | one unit |
| `?` | writing that is not cipher, or a sign that I did not read |
| a unit that ends in `~` | a unit that I doubt |

- A unit of Latin letters has one to three letters. A longer run of letters is cut into such units.
- My names of the signs hold for their own page. One sign can have different names on different pages.

## Doubts

- 2,901 units are marked as doubtful, and 4,910 places hold `?`.
- `?` does not tell clear writing apart from a sign that I did not read.
- Some short units of the mixed rows are clear words, not cipher.
