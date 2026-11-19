# The Botti letters: the transcription of the cipher rows

The files in `transcription/` are my own transcription of the DECODE images. They hold the cipher rows of each page, one line for each row.

## Credit

- **DECODE**, the database of historical ciphers of the DECRYPT project: records R8468 to R8470, R8617, R8618 and R8659 to R8718. Record pages: https://de-crypt.org/decrypt-web/RecordsView/ followed by the record number, for example https://de-crypt.org/decrypt-web/RecordsView/8659.
- **The archive:** British Library, Add MS 20443 (papers of Cardinal F. A. Gualterio).
- **The database:** Héder and Megyesi (2022), "The DECODE Database of Historical Ciphers and Keys: Version 2", HistoCrypt, https://doi.org/10.3384/ecp188397.
- No DECODE image is published.

## The files

- 191 files, one for each page that holds cipher digits. They hold 2,568 rows of 51 records.
- File name: `<record>_<page>_digits.txt`. The page label (`T001` and so on) follows the order of the images in DECODE's record. It is not a folio.
- Four header lines start with `#`. Then each row is one line: its label (`C01`, `C02`, ...) and the row.
- Clear words of the page are not copied. `[not copied]` stands in their place.
- The record pages in `records/` give the rows as read, page by page.

## The marks

| Mark | Meaning |
| --- | --- |
| a digit, `.` | a cipher digit; a dot of the page after a code |
| a space | a space of the page |
| `a`, `u` | a letter-like sign among the codes |
| `ω`, `g`, `β` and other labels | on some pages without dots, a sign that my transcription labels; a label holds for its own page only |
| `[a\|b?]`, `⟦a\|b?⟧` | one sign with two or more readings; the leading reading stands before the bar |
| `[d?]`, `[?]` | a doubtful sign |
| `⟨...⟩` | a sign that my transcription describes |
| `[not copied]` | clear words of the page |
| other `[...]` or `⟦...⟧` | a note on the page: a stretch not read, damage or a mark |

## Doubts

- My transcription may read the sign for u as the code 10. I did not check this.
- On six pages, the line numbers of the record pages do not always follow the row labels here. The pages are R8668 T003, R8671 T007, R8680 T006, R8683 T002, R8691 T002 and R8707 T001.
