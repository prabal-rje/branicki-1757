# Francia 346, the later letters: a full decode with the published key

These are cipher letters of 1633 from Rome to Francesco Adriano Ceva, extraordinary nuncio in France. Their clear endorsements name Cardinal Barberini. This folder decodes all 35 cipher pages of 22 DECODE records with the published key. It gives a reading and an English translation of each record.

The transcription is a machine transcription of the DECODE images, made in my pipeline. Nobody verified it. Every number here is real.

## What came first

The order of events is part of the result.

1. **A key from the ciphertext alone.** My algorithm found a key from 13 records of this file, without the published key. I fixed it at 01:27 on 12 November 2026 (UTC−3). `../francia-346-leaves/` has that read and its check.
   - Those 13 records include an earlier transcription of 8 records here: R5626, R5635, R5636, R5637, R5640, R5643, R5647 and R5648.
   - The other 14 records here were not in that fit.
2. **A read of the new pages, frozen.** I applied that key to the 22 records here, with no new fit. I fixed that read at 17:00 the same day.
3. **The published key, then.** After that, I opened the published key. I graded the frozen read against it and made the full decode.

## The numbers

**The frozen read** (`check.md`): of the true letters that it shows, 98.8% are right (6,930 of 7,017). All 87 wrong letters are code 07, which is h. But only 62.0% of its graded shown tokens are letter codes (7,017 of 11,324). The rest are syllables, nulls or false pairs of my cut.

On the 8 records inside the key's fit, 99.0% of the shown true letters are right (3,091 of 3,122). On the 14 records outside it, 98.6% are right (3,839 of 3,895).

**The full decode:** 10,919 code tokens, of which 92.3% have a value (10,081). Three-digit codes: 351 tokens have a value from the ledger, and 803 tokens have none.

| Record | Key-free check | Code tokens | With a value | Three-digit, ledger value | Three-digit, no value | Bits per letter |
| --- | --- | ---: | --- | ---: | ---: | ---: |
| [R5626](r5626.md) | fits | 682 | 93.7% (639) | 15 | 43 | 4.90 |
| [R5635](r5635.md) | fits | 410 | 94.6% (388) | 16 | 21 | 4.58 |
| [R5636](r5636.md) | fits | 1,104 | 94.6% (1,044) | 45 | 57 | 4.25 |
| [R5637](r5637.md) | fits | 832 | 92.7% (771) | 24 | 59 | 4.43 |
| [R5640](r5640.md) | fits | 652 | 93.6% (610) | 21 | 42 | 4.74 |
| [R5642](r5642.md) | differs | 586 | 82.9% (486) | 15 | 91 | 5.77 |
| [R5643](r5643.md) | fits | 38 | 84.2% (32) | 2 | 6 | 5.54 |
| [R5645](r5645.md) | differs | 198 | 93.9% (186) | 3 | 12 | 4.62 |
| [R5646](r5646.md) | fits | 818 | 92.1% (753) | 26 | 65 | 4.52 |
| [R5647](r5647.md) | fits | 60 | 90.0% (54) | 3 | 6 | 4.58 |
| [R5648](r5648.md) | fits | 855 | 92.6% (792) | 33 | 60 | 4.63 |
| [R5649](r5649.md) | differs | 376 | 91.8% (345) | 11 | 27 | 4.59 |
| [R5650](r5650.md) | fits | 739 | 94.0% (695) | 30 | 44 | 4.48 |
| [R5651](r5651.md) | differs | 1,042 | 91.9% (958) | 36 | 84 | 4.49 |
| [R5652](r5652.md) | differs | 586 | 91.3% (535) | 7 | 51 | 4.54 |
| [R5653](r5653.md) | fits | 162 | 95.7% (155) | 2 | 7 | 4.51 |
| [R5654](r5654.md) | differs | 205 | 93.2% (191) | 6 | 13 | 4.46 |
| [R5655](r5655.md) | fits | 573 | 93.9% (538) | 24 | 31 | 4.24 |
| [R5656](r5656.md) | too small | 325 | 89.8% (292) | 10 | 33 | 5.29 |
| [R5657](r5657.md) | too small | 546 | 91.4% (499) | 18 | 44 | 5.57 |
| [R5658](r5658.md) | too small | 107 | 90.7% (97) | 3 | 5 | 4.76 |
| [R5659](r5659.md) | too small | 23 | 91.3% (21) | 1 | 2 | 5.64 |

- **Code tokens** are the two- and three-digit codes, without word spaces and nulls. **With a value** counts letters, syllables and the three-digit codes that have a ledger value.
- **Bits per letter** measure how Italian the decoded letters look, under a letter model of 17th- and 18th-century Italian prose. Lower is more Italian. The same letters in a shuffled order give 9.4 on average.
- **The key-free check** compared the code counts of each record with those of the earlier letters, before I opened the key. "Too small" means that no page of the record passed its page test with read digits.
- **A check against the decipherment leaves** of three records: 58% to 79% of the decoded letters align with equal letters of the leaf. Other leaves give 32% to 49%. `check.md`, section 7, gives the method and its limits.

## The six records that differ

The key-free check found that six records differ a little in their code counts: R5642, R5645, R5649, R5651, R5652 and R5654.

- **Five of them read as Italian under the published key.** Their bits per letter lie between 4.46 and 4.62. The twelve that fit give 4.52 (the mean weighted by letters).
- **R5642 does not read** (5.77). Its main page, f. 246r, carries a tentative reading in the source. The page has a high share of 6 and a low share of 8, so I suspect that the transcription reads some 8s as 6. Its last four rows read in part.
- So the published key reads five of the six. For R5642, this test cannot show whether another key was used.

## What the letters say

The readings are partial. Each record page gives the Italian, the English and the place of each name.

- **The peace talks of 1633.** Rome urges the nuncio to keep the talks going and not to "break the thread" (R5648, R5651). It names plenipotentiaries (R5635, R5636) and a universal [?peace] (R5640, R5650). R5655 names something "in luogo terzo" (in a third place) and a suspension of arms.
- **Benavides.** The name recurs in nine records, often with a writing and Rome's view of how to answer it (R5637, R5640, R5645, R5646, R5650, R5651, R5652, R5653, R5654).
- **Lorraine.** Rome names the fortresses of Lorraine (R5636) and "the invasion of Lorraine" (R5653). It hears of the events in Lorraine "con disgusto", with displeasure (R5654, R5655).
- **Germany and the Swedes.** A rumour of a fortress on this side of the [?Rhine] held by the "Svezesi", probably the Swedes (R5636); aid to a people (code 104) under old alliances (R5651); a violated neutrality and the Imperial court (R5655).
- **Church affairs.** A priory, offers of pensions (R5636, R5637), and the bull "de non infeudandis": the letter says that it also covers exchanges, and it names censures (R5649).
- **A woman who is ill.** Rome hopes that she will be reconciled with a "f…uolo", perhaps her son, and return (R5646, R5648). The decode does not name her.

## The key

- **The published key** gives 61 pair codes: 40 letter codes for 19 letters, and 21 syllable codes such as che, per and di. George Lasry reconstructed it, and it stands on DECODE with a key note of 24 October 2020.
- **The form of the cipher,** as the ledger rebuilt it from Lasry's own readings: a lone 6 is a word space, and the ten pairs 2x are nulls.
- **The published key gives no three-digit code a value.**
- **The cipher ledger** at https://github.com/dbourdeau/cyphersolver gives values to three-digit codes.
  - Its file `targets/ceva1632/cipher.py` gives 23 values.
  - Its notes on a re-read of 22 to 23 October 2026 (`targets/ceva1632/NOTES.md`) add five values and change one: 104 is Olandesi, not Svedesi.
  - The same notes change two pairs: 88 is del, not quel, and 33 is gli.
  - I use these 28 three-digit values and the two pairs. The decode marks the three-digit values `{word}`.
- **Some ledger values do not fit these letters.** For example, code 470 ("hor") stands where no "hor" can stand. Each record page lists such places, and the reading marks them `[?word]`.

## How to read the decode

Each record page ends with the decode, row by row, as the key gives it.

| Mark | Meaning |
| --- | --- |
| a space | the word space, a lone 6 |
| `abc` | letters and syllables of the key; the code for u and v is written u |
| `{word}` | a three-digit code with a value from the ledger |
| `[123]` | a three-digit code with no value |
| `⟨a⟩` | a code that holds a doubtful digit of the transcription |
| `·` | a code that holds an unread sign, or a lone digit that fits no code |
| `[…]` | an unread span of the transcription |
| `‖` | clear text stood here; this page does not copy it |

The cipher writes no double letters, so "sarebe" stands for "sarebbe". The readings mostly keep this spelling. In the readings, `[abc]` is supplied or changed by me, `[?word]` is a doubtful word, and `[…]` does not read. Where a silent repair remains, the decode line is the reference.

## Who read these letters before

- **Decipherment leaves.** Some records hold a decipherment in Italian on another leaf: R5626 (f. 155r), R5637 (f. 212v) and R5646 (f. 269r). Brice Dudout's notes in the ledger (29 October 2026) call such leaves contemporary. They add R5655 (f. 324) and find none in R5640. So some of these letters were read before.
- **Copies in clear** may also exist in other volumes. This folder does not copy the decipherment leaves, and it takes no code value from them.
- **DECODE.** On 12 November 2026, the public record pages of R5625 to R5659 all give the status "N/A" and the cipher type "Unknown". They list no decryption. Their documents need a login, so I could not check them.
- **The cipher ledger.** Its entry 880 lists R5625 to R5686 as "N/A" with no decipherment filed, and says that none of them is in the repository. Its notes of 29 October 2026 name R5626, R5640 and R5655 in a sample, and say which leaves hold decipherments. They decode R5630, which is not in this set, and none of these 22 records. I checked the live catalogue and notes on 12 November 2026.
- **Print.** I found no edition of these letters. A. Iommelli's study of Ceva (Fondazione 1563, 2022) cites his own deciphered despatches, "Francia, 78", and Bichi's letters from Paris. It does not cite Francia 346.

**No modern decipherment of these 22 records shows on DECODE's public record pages or is on file at the ledger.** This does not mean that nobody read them: the decipherment leaves show that some were read long ago.

## Limits

- **The transcription** is a machine transcription. Nobody verified it against the images. A misread digit gives a wrong letter or a broken cut.
- **The cut** of the decode into two- and three-digit codes comes from a search with an Italian letter model. Where it picks a three-digit code, the letters around it can be wrong.
- **The readings** are mine. They supply words where the context allows, and they mark each supply. Many rows do not read.
- **803 three-digit tokens** have no value. They hide names and words that the published key does not give.
- **Three records give almost nothing:** R5643, R5658 and R5659. Most of their cipher rows are unread in the source.

## The other records of the file

- **R5625** is a letter in clear. It holds no cipher.
- **17 records use other signs:** R5667, R5668 and R5672 to R5686. A test before the key found another system. Their pages name Madrid and Vienna. They stay open.

## Credits

- **DECODE**, the database of historical ciphers of the DECRYPT project: records R5626, R5635, R5636, R5637, R5640, R5642, R5643, R5645, R5646, R5647, R5648, R5649, R5650, R5651, R5652, R5653, R5654, R5655, R5656, R5657, R5658 and R5659. https://de-crypt.org/decrypt-web/RecordsList
- **The archive:** Archivio Apostolico Vaticano, Segreteria di Stato, Francia 346.
- **The key:** George Lasry, Beáta Megyesi and Nils Kopal (2020). The ledger's values for three-digit codes and two pairs: the cipher ledger at https://github.com/dbourdeau/cyphersolver.

DECODE's images are for research use only. They may not be redistributed or published without permission from the archive. No DECODE image is in this repository. I copy no row of cipher digits: each decode line gives its record, folio and row.

## Files

- `check.md`: the grade of the frozen read against the published key
- `r5626.md` to `r5659.md`: one page for each record, with the reading, the translation, the names and the decode row by row
