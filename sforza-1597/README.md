# Sforza chancery letters in cipher (Milan): partial reads

This folder holds our partial reads of nine cipher letters of the Sforza chancery. The letters are DECODE records 5425 to 5430, 5463, 5464 and 5465 (Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597).

We read these letters from the ciphertext alone.

- We used no key from outside, and no letter value of any key sheet.
- For these reads, we opened no key sheet of this box, and no deciphered text of these letters.
- For our twins, we took the shape of one sheet (no. 14) from the ledger's transcription of it. That was on 7 November 2026, before we adopted the rule to read from the ciphertext alone.
- No key sheet and no clear text checks the reads.
- By the read bar of the cipher ledger, they are partial reads, not readings.

A sign is one written sign of the cipher text, as a transcription gives it. A shown letter is not a letter read. "94% of the signs show a letter" does not mean "94% read".

## What is read

| Read | Records | Signs from | Signs (real) | Signs that show a letter (real) | Starts on the best hill (real) | Twins: shown letters right (twin) | Folder |
| --- | --- | --- | ---: | ---: | --- | --- | --- |
| Earlier read | 5463 | the ledger maintainer's transcription | 1,372 | 78.0% | 16 of 50 fresh starts; a rival hill held 17 | 86% to 90% in four of five; one wrong key | `r5463/` |
| Second read | 5463 | our transcription | 1,137 | 97.6% | 94 of 100 | 87%, the mean of five | `r5463/second-read/` |
| Earlier read | 5464 | the ledger maintainer's transcription | 3,249 | 86.4% | 36 of 50 fresh starts | 90% to 95% in four of five; one wrong key | `r5464/` |
| Earlier read | 5465 | the ledger maintainer's transcription | 5,828 | 68.0% | 31 of 50 fresh starts | no twins | `r5465/` |
| Second read, one key | 5464 and 5465 | our transcription | 8,691 | 94.2% (5464: 93.4%; 5465: 94.7%) | 66 of 100 | 94%, the mean of five | `r5464-r5465/` |
| One key | 5425 to 5430 | our transcription | 14,888 | 87.1% | 52 of 100 | 95%, the mean of five | `r5425-r5430/` |

- **Our transcription** is our own machine transcription of the DECODE images, not verified. It is not in this repository, because DECODE marks the ciphertext of these letters as private. We share it with DECODE and with the archive on request.
- **A twin** is an artificial letter: real Italian, enciphered with a key of the same shape and read by a simulated sign reader. On a twin we can count the right letters. A twin value describes the twins, not the real read.
- **Two readings of one page agree.** We aligned the earlier and the second decode of each page. Where both show a letter, they agree on 93% to 97% of the places (real; records 5463, 5464 and page 1 of 5465). The same alignment gives 49% to 69% for two different pages (real). The two second-read check pages give the counts.
- **Two blind readers** judged each read. They are two large language models. Each saw our decode and two shuffled copies, with no name, date or source. By a rule that we declared before they ran, each record of the second reads and of records 5425 to 5430 reads as Italian sentences. The earlier read of record 5465 reads in patches only. Their shares are estimates, not counts, of the shown letters:
  - earlier reads: 5463, 65% to 75%; 5464, 65% to 70%; 5465, about 55% of the shown letters (real);
  - second reads: 5463, about 87% and 72%; 5464, about 75%; 5465, about 70% (real);
  - records 5425 to 5430: 40% to 69% of the shown letters (real);
  - twin pages with 94% to 95% of their shown letters right: 55% to 70% (twin).
- Each `check.md` gives the tests, the controls and the limits. Each `reading.md` gives the stretches that read, in Italian with an English translation.

## What stays open

- **No outside check.** No key sheet and no clear text checks any read. Nobody has checked a decoded word against the ink.
- **The transcriptions** are machine transcriptions, and nobody has verified them. On page 2 of record 5465, ours and the ledger maintainer's cannot be aligned.
- **The key groups.**
  - Our tests cannot tell the pages of records 5425 to 5430 from one key at this size. For two pairs of pages, they could not judge.
  - The second read joins records 5464 and 5465 under one key. One statistic of two says "same key"; the other cannot judge. So the two records share most of a key at least. The earlier reads give each record its own key.
- **The twins** have one writer. Their key shape comes from one key sheet of this box, sheet no. 14. It gave the form of a key: the number of signs for each letter, nulls, doubled letters and word signs. It gave no letter value for these letters. If the real key has another shape, the twins can overstate the accuracy.
- **The shown share proves nothing alone.** Shuffled signs still show a letter on 30% to 58% of the signs (real signs, shuffled).
- **The key alone does not give the decode.** In the three reads on our transcription, the key's letter is the shown letter on 92.0% to 97.2% of the shown signs (real). The decode also uses a letter model. That model is not in this repository.
- **Names.** The letter model learned from printed Milanese dispatches of the 1460s and 1470s. It names many of the places and people of the decodes, so one such name proves little. Some names of the decodes do not occur in that text at all, such as "Antonio da Trezo" and "Zohane Antonio da Pavia".
- **Dates.** No year is read. Some days are read in part.
- **The earlier read of record 5463** has a rival key that scores almost as well. `r5463/check.md` gives it.
- **Six more records** of the box (5437, 5443 to 5445, 5447 and 5467): the same method did not read them.

## The files

- `r5463/` and `r5464/`: `reading.md`, `decryption.txt` (line by line), `key.tsv` and `check.md`. These are the earlier reads.
- `r5465/`: `decryption.txt`, `key.tsv` and `check.md`. It has no reading page, because the earlier read gives patches only.
- `r5463/second-read/`, `r5464-r5465/` and `r5425-r5430/`, the reads on our transcription:
  - `reading.md`: the stretches that read, with an English translation;
  - `decryption.txt`: our decode, row by row;
  - `key.tsv`: our key, one row for each label;
  - `channel.tsv`: the fitted table that the decode uses;
  - `check.md`: what supports the read, and what does not.
- The columns of `channel.tsv` differ between these folders. In `r5425-r5430/`, `weight` is the share of the label's signs, and `emission` is P(sign | letter). In the two second-read folders, `weight` is P(sign | letter), and `share_of_label` is the decode's share of the label's signs. Each `check.md` defines its own columns.
- The `.tsv` files have no source-credit header of their own. This page and each `check.md` give their source.
- `sforza-1597-a-sealed-2026-11-12.tar.gpg`: our read of records 5425 to 5430, sealed on 12 November 2026.
  - GnuPG encrypted it (symmetric, AES-256).
  - We keep its passphrase. We will show it when the date of this read must be proven.
  - With the passphrase, anyone can decrypt it with `gpg --decrypt sforza-1597-a-sealed-2026-11-12.tar.gpg` and see what we held on this date.
  - It holds an earlier read of these six records. The read in `r5425-r5430/` is a new one.

## Dates

- We froze the reads on 12 November 2026, in our own records.
- We committed the pages of the second reads and of records 5425 to 5430 on 13 November 2026.
- The sealed file of 12 November 2026 holds an earlier read of records 5425 to 5430.

## Credits

- **The signs of the earlier reads** are the sign transcription of the cipher ledger (https://github.com/dbourdeau/cyphersolver, target `sforza1597`). Its maintainer made it from the DECODE images with his sign reader.
  - Our files do not copy his token files. A reader needs them to follow our earlier decodes sign by sign.
  - Record 5463: `targets/sforza1597/ctts/r5463_best/tokens.txt`.
  - Record 5464: `targets/sforza1597/ctts/r5464_best/tokens.txt`.
  - Record 5465: `targets/sforza1597/ctts/r5465_best/tokens.txt`.
  - Records 5425 to 5430: `targets/sforza1597/ctts/a_best/tokens.txt`. `r5425-r5430/check.md` uses it as a cross-check.
- **The signs of the other reads** are our own machine transcription of the DECODE images, not verified. It is not in this repository. No image is in this repository.
- **The ledger's maintainer read part of record 5464 first.**
  - His partial reading of 7 November 2026: by his count, 27% of the letters fall in words of four letters or more.
  - His key found the main letters first.
  - Our earlier key gives the same letter as his on 87% of the signs.
- **He also saw fragments of record 5463 first:** "desideroso", "sperare" and "perche".
- **The ledger applied our three earlier keys to its own tokens** (pull request 494). The shown shares of records 5463, 5464 and 5465 came out the same.

## Source and terms

DECODE, the database of historical ciphers of the DECRYPT project: records 5425 to 5430, 5463, 5464 and 5465. We also tried records 5437, 5443, 5444, 5445, 5447 and 5467. The documents are in the Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597. We thank the DECODE team and the Archivio di Stato di Milano.

DECODE's images are for research use only. None is in this repository.
