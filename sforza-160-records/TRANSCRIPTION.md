# Sforza chancery letters, 160 more records: the transcription of the cipher rows

The files in `transcription/` are my own transcription of the DECODE images, as sign labels. They hold the cipher rows of each page, one line for each row.

## Credit

- **DECODE**, the database of historical ciphers of the DECRYPT project: the records of the pages that `README.md` shows, between R5297 and R5584. Record pages: https://de-crypt.org/decrypt-web/RecordsView/ followed by the record number, for example https://de-crypt.org/decrypt-web/RecordsView/5521.
- **The archive:** Archivio di Stato di Milano, Carteggio Sforzesco. The header of each file gives its cartella.
- **The database:** Héder and Megyesi (2022), "The DECODE Database of Historical Ciphers and Keys: Version 2", HistoCrypt, https://doi.org/10.3384/ecp188397.
- No DECODE image is published.

## The files

- 46 files, one for each of the 47 pages that this folder gives, except R5501 page 1: `<record>_p<page>_signs.txt`. They hold 1,103 rows of 39 records.
- The pages read with the cipher ledger's keys have no file here.
- Three header lines start with `#`; R5582 page 1 has four. Then each row is one line: its label (`C01`, `C02`, ...) and the signs, split by spaces.
- Clear text is not in the rows.

## The marks

| Mark | Meaning |
| --- | --- |
| a label of capital letters, sometimes with digits (`BO`, `U01`, `CL01`) | one sign; a label names one sign shape of its own page only |
| `?` | a sign that I do not read |

## Doubts

- Some signs differ only by a small stroke or a dot. So two labels can be one sign, or one label two signs.
- The file of R5582 page 1 holds rows 1 to 16 only.
- R5297: the header of its two files says cartella 1591, and its record page says cartella 1598. I have not settled which is right.
