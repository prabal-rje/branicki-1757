# DECODE record 5465: what supports the read, and what does not

Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597, DECODE record 5465. Two pages. Italian, in cipher.

**This is a partial read from the ciphertext alone. It reads in patches only.** No key sheet and no clear text checks it. The signs are a machine transcription of the images. We give no reading page for it.

A sign is one written sign of the cipher text. A sign class is one label of the transcription, from `s00` to `s79`. Several sign classes can stand for one letter.

## 1. In short

| Measure | Value |
| --- | --- |
| Signs decoded | 5,828, in 89 lines on two pages; 80 sign classes |
| Signs that show a letter | 68.0% (3,961 of 5,828) |
| Shown letters that make sense, by two blind readers | about 55% and about 55% |
| The same, as a share of all signs | 37% |
| Fresh starts that end on the main hill | 31 of 50 |
| Artificial letters of this size | none |

## 2. The signs

- The cipher ledger's sign reader made the transcription from the DECODE images. We cannot see the images.
- The file is `targets/sforza1597/ctts/r5465_best/tokens.txt` in https://github.com/dbourdeau/cyphersolver. We do not copy it.
- We decode all its 89 lines. Page 2 line n is its line 45 + n.
- The last line (6 signs) may be a stamp, a number or clear writing.
- The transcription makes errors: it merges, splits or misses signs. Nobody has measured its error rate for this record.

## 3. How we found the key

The method is the one of record 5464. `../r5464/check.md` gives it in full.

- **The letter model:** the printed dispatches of the Milanese ambassadors of the 1460s and 1470s, five volumes, 1.32 million letters.
- **The starts:** 50 fresh starts (5 keys from the sign counts and 45 random keys), and 50 starts from the best fresh key with 15% of the sign classes changed.
- **The result:** 31 of the 50 fresh starts end on the main hill, that is, they agree with the best key on at least 90% of the signs. 25 of them give exactly the best key. In all, 80 of the 100 starts end on the main hill.
- **No key from outside.** No start used the ledger's key or a key sheet.
- **Firm signs:** the 20 best keys give every sign class the same letter. So all 80 classes are firm.

The main hill holds 5 distinct keys.

- The decode uses the one whose fitted table fits the signs best.
- It differs from the best key on 4 sign classes (3.0% of the signs).
- `key.tsv` gives the best key. Its column `decoded_as` gives the value that the decode gives each class most often.

## 4. The decode and the display rule

- The decode and the display rule are the same as for record 5464.
- Here, the decodes from the 5 keys of the main hill must agree before a letter shows.
- The fitted table changes the main letter of 17 sign classes. So `key.tsv` alone does not give `decryption.txt`.
- The decode takes 207 signs as nulls. They show as `·`, like every sign with no shown letter.

## 5. No artificial letters of this size

We made no artificial letters of this size and shape (5,828 signs, 80 sign classes). So we do not know how many of the shown letters are right.

- The tests at the size of records 5425 to 5430 and of record 5464 do not measure this record.
- At the size of record 5464, one test of five ended on a wrong key, and the display rule did not catch it.

## 6. The pair-keeping shuffle

We ran this control on records 5425 to 5430, not on this record. It shuffles the signs and keeps the count of each pair of neighbouring signs.

- No fresh start of 50 ended on a main hill.
- The display rule still showed a letter on 28% of the signs.
- So a share of shown letters does not show by itself that there is a text.

## 7. Two blind readers

The test is the one of record 5464 (`../r5464/check.md`, section 7). The two readers are large language models: GPT-6.1 Sol (max effort) and Grok 4.7 (xhigh effort). Our decode left out the 207 nulls.

| Text | Reader 1 (Sol): share | Reader 2 (Grok): share | Rank by both |
| --- | ---: | ---: | --- |
| Our decode | about 55% | about 55% | first |
| Control W (words shuffled) | about 30% | 15% to 20%, in phrases | second |
| Control L (letters shuffled inside words) | about 1% | about 3% | third |

- As a share of all 5,828 signs, the first line is 37%.
- Both readers name Italian. The gap to control W is 25 to 35 points. For record 5464 it is about 55 points.
- Reader 1: "Sentence structure survives in substantial patches", but "I cannot confidently extract a long, fully intact sentence."

## 8. What does not support the read

- No key sheet and no clear text. Nobody has checked a decoded word against the ink.
- The transcription is a machine reading.
- No artificial letter measures this read.
- No shuffle control ran on this record itself.
- The blind readers give estimates, not counts. They find patches, not sentences.

## 9. Credits

- **DECODE**, the database of historical ciphers of the DECRYPT project: record 5465. The document is in the Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597.
- **The sign transcription** is the work of the cipher ledger's maintainer (https://github.com/dbourdeau/cyphersolver, `targets/sforza1597/ctts/r5465_best/tokens.txt`). A reader needs that file to follow our decode sign by sign.
- The ledger's maintainer also tested this record. On 12 November 2026, the ledger listed signals and fragments of Latin and Italian, but no reading.
