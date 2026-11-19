# Cosimo I de' Medici to Agnolo Niccolini, 1537 to 1539: the cipher passages

Cosimo I de' Medici, Duke of Florence, writes to his envoy Agnolo Niccolini. The letters run from December 1537 to August 1539. Their secret passages are in a number cipher with no spaces between the codes. Two systems occur.

| Letters | System | State |
| --- | --- | --- |
| R4034 to R4038 (December 1537 to March 1538) | the earlier system | from key (the archive's key table, DECODE record R4033) |
| R4039, R4041 to R4050, R4052 to R4054 (October 1538 to August 1539) | the main system | from ciphertext; not checked against a key |
| R4040 | another system, with too few codes | too small |
| R4051 | no cipher | – |

- **The earlier system.** The rows show the key table's own values. A read from ciphertext, made before, agrees with the archive's key table on 16 of 17 codes. The key of that read is `key-earlier.tsv`.
- **The main system** is not checked against a key. The archive's key table is for the earlier system.

The rows come from my own transcription of the DECODE images. The word cuts in the rows are mine. Each English gloss gives the sense of the letter as far as the decoded rows carry it. The key table is cited, not copied.

## What the letters say

- **4 October 1538 (R4039), the longest passage.** A marriage alliance and "the matter of the wife". Cosimo's intention "has always been the same". He sends a copy of a letter to cut off the negotiation entirely. He warns Niccolini about a man who is not to be trusted: he fears to lose "his penitentiary", and he acted against Duke Alessandro and against Cosimo. Cosimo would speak of a wife only as far as "His Majesty" commanded.
- **10 October 1538 (R4041).** Short pieces: "this negotiation", "the matter of Giulio", "ridiculous and frivolous causes".
- **28 October 1538 (R4042).** Short pieces: "Don Giovanni", an examination, men "sent to Spain", news, "a most noble person".
- **17 November 1538 (R4046).** An order to watch "the movements, orders and plans" of certain people.
- **18 January 1539 (R4047).** A papal "motu proprio" that "would turn to our great advantage, more than theirs". Cosimo wants to act "at the right time and place", and to make the other side feel "a great suspicion".
- **9 February 1539 (R4048).** "Those ministers" and "Francesco Valori".
- **28 February 1539 (R4049).** A short note on where "Signor Stefano da Palestrina" is; "Ugolino"; a journey to Pisa; "the ambassadors".
- **22 May 1539 (R4052).** "A great accident"; the rest is broken.
- **11 August 1539 (R4054), the second longest passage.** The arrest of one Biagio della Campana, a companion of "the sons of Bartolomeo Valori". He was taken and examined two years before, condemned and sent to the fortress of Pisa, and later freed. The passage names "my mother", Gian Francesco da Mantova, de' Mar[z]i, "his most reverend lordship" and Giulio, "the natural son of Duke Alessandro". Something went on "without my knowledge". Biagio was caught when he had left the city, probably for Rome. The passage fits the affair of Biagio della Campana that Luigi Alberto Ferrai printed in 1882. One verb, "auel[en]are" ("to poison"), is a restoration. The record page gives the sources and the limits.
- **The other letters of the main system** (R4043, R4044, R4045, R4050, R4053) have short passages. The reading shows only fragments of them.
- **The earlier system, read with the key table:**
  - **17 December 1537 (R4034).** The tithes. Cosimo asks that the state be spared for now, as it is exhausted by such an exaction. Niccolini is to draw the matter out, with no offer, because time can bring much advantage. The King of France and the Emperor's mind toward Italy are named.
  - **24 December 1537 (R4035), in part.** His Holiness; to proceed in this business as the prince does at Genoa.
  - **8 February 1538 (R4036).** Only one row reads, in part.
  - **16 February 1538 (R4037).** The two papal tithes on Florence. Cosimo will act as Prince Doria acts for the city of Genoa. A proposal: half of the two tithes, one raised now and one a year later, by a Florentine commissioner whom His Holiness appoints. Church censures and an interdict are named.
  - **4 March 1538 (R4038).** Niccolini is to accept the extension, and to seek a better condition.

## The numbers

| Measure | Value |
| --- | ---: |
| Main system, 13 of its 14 letters: code tokens that show a letter or a word (not a share that is right) | .865 of 4,726 |
| Main system: codes that the reading shows | 21: 20 letter codes for 18 letters, and 1 word code |
| Earlier system, the key table: code tokens that the table holds | .886 to .978, by letter |

## Files

- `records/r<number>.md`: one page for each letter with a reading (19 of 21): what it says, the rows as read, and the state.
- `key-main.tsv`: my own key of the main system, from ciphertext: each code, its value, its count and its doubt. Its counts differ a little from the 4,726 code tokens of the reading.
- `key-earlier.tsv`: my own key of the earlier system, from ciphertext, made before the key table was used.
- [`TRANSCRIPTION.md`](TRANSCRIPTION.md): my own transcription of the cipher rows, in `transcription/`, and how to read it.

## Credit

- **DECODE**, the database of historical ciphers of the DECRYPT project: records R4034 to R4054, and R4033 (the key table). Each record page links its DECODE record.
- **The archive:** Florence, Archivio Niccolini di Camugliano, Fondo antico 214, inserto 1.
- **DECODE's record pages:** https://de-crypt.org/decrypt-web/RecordsView/ followed by the record number, for example https://de-crypt.org/decrypt-web/RecordsView/4039.

DECODE's images are for research use only. They may not be redistributed or published without permission from the archive. No DECODE image is in this repository. The cipher rows in `transcription/` are my own transcription of the DECODE images.
