# Francia 346: a full decode with the published key

The letters that this folder decodes are cipher letters of 1632 to 1634 from Rome to Francesco Adriano Ceva, extraordinary nuncio in France. Their clear endorsements name Cardinal Barberini. This folder decodes the digit pages of the DECODE records of Francia 346 with the published key: "read with the known key".

The transcription is a machine transcription of the DECODE images, made in my pipeline. Nobody verified it. Every number here is real.

## The whole file at a glance

DECODE holds 73 records of Francia 346 (260 scans).

| Records | How many | State | Where |
| --- | ---: | --- | --- |
| R5626, R5635 to R5637, R5640, R5642, R5643, R5645 to R5659: the first 22 digit records | 22 | read with the known key; a summary and a reading for each | the sections below; `r5626.md` to `r5659.md` |
| R5627 to R5633, R5641, R5644 | 9 | read with the known key (R5641 is too small to judge); each carries a decipherment of the time | [The records added on 13 November](#the-records-added-on-13-november-2026) |
| R74 to R78, the earlier leaves | 5 | read with the known key from my pilot transcription; R74 to R76 in fragments | the same section |
| R5660 to R5666, R5669 to R5671 | 10 | do not read with the known key: another cipher; content from the clerk's decipherment or a clear copy; no decode | [Thirteen records in another cipher](#thirteen-records-in-another-cipher) |
| R5634, R5638, R5639 | 3 | do not read with the known key: another cipher; each carries a decipherment of the time; a blind read is in progress | the same section |
| R5667, R5668, R5672 to R5686 | 17 | other signs; a blind fit is in progress | [The other records](#the-other-records-of-the-file) |
| R79 to R84 | 6 | my pipeline has no transcription yet | the same section |
| R5625 | 1 | a letter in clear | the same section |

Ten pages that read badly were read again. `rereads.md` gives their decode.

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

**The full decode, first pass:** 10,919 code tokens, of which 92.3% had a value (10,081). Three-digit codes: 351 tokens had a value from the ledger, and 803 had none. **Second pass (graded):** the pages now give 515 three-digit tokens a value: 142 certain, 131 probable, 242 conjecture. 639 stay open. So 10,245 code tokens (93.8%) show a value. The table of the first pass below keeps its first-pass figures.

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

## The grades of the code values (second pass)

A second pass graded every value of a three-digit code. It took no new value from outside the ledger: the test below gave no other source a measured accuracy. All numbers are real.

| Grade | Codes | Tokens | Source |
| --- | ---: | ---: | --- |
| certain | 14 | 142 | values that the ledger adopted, with no whole-word doubt in these letters: 498 tanto, 854 guerra, 149 piazza, 315 S.E., 988 negotio, 338 stato, 441 bene, 857 Germania, 334 Sueco, 454 grandi, 488 quale, 541 armi, 473 mentre, 491 quell- |
| probable | 7 | 131 | values that the ledger adopted, with a doubt at whole-word places in one record: 411 V.S., 439 ancora, 481 però, 493 questa, 495 quanto, 830 Francia, 938 Monsieur |
| conjecture | 25 | 242 | 6 values that the ledger adopted but that these letters put in doubt in two or more records (470 hor, 127 Imperiali, 104 Olandesi, 171 regno, 474 mente, 497 tutt-), and 19 values that the ledger read off the decipherments of 1632 (ff. 82r and 136r) but did not adopt |
| open | — | 639 | no value |

- **A doubt** is a place where the earlier reading of a record marks the ledger's word as not fitting.
- **The ledger's unadopted values** come from its readings of R75 and R84: 153 pace, 451 fatto, 471 molto, 485 perché, 110 Principe, 998 nella, 357 Schomberg, 581 Card. Richelieu, 197 Religione Cattolica, 844 Gostavo, 309 and 107 S.M.tà, 930 Mons.r, 957 Nuntio, 380 trattato, 831 Francesi, 397 Valtellina, 170 Re, 445 tanto.
- **The test.** Each ledger value was hidden in turn, and three sources tried to find it again:
  - the decipherments of the time in seven records, aligned with the decode under strict rules: no place passed the rules, so they gave no value;
  - a word-level score in context: it found 0 of 21 values;
  - two readers who saw only the contexts: they found 5 and 1 of 21.
- So no new value reaches "probable". The pages show no value from those three sources.
- **Shown and not shown:** a further 69 conjectures (252 tokens) from the word-level score and the readers stay in the internal table, because the test gave those sources no measured accuracy. The counts on these pages count the shown values only.
- **Unchanged:** the cut and the letters of the decode.

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
- **Letters of other nuncios.** Ten records in another cipher hold letters from Vienna and Madrid, 1632 to 1634. Their content comes from the clerks' decipherment of the time or from a clear copy in the same record, not from a decode. See [Thirteen records in another cipher](#thirteen-records-in-another-cipher).

## The records added on 13 November 2026

### Nine records with a decipherment of the time

DECODE's catalogue marks 22 more records of the file "Inline Plaintext: Yes". A clerk of the time wrote a decipherment between the cipher rows. My pipeline read them as reference pages. I decoded their cipher rows with the published key, as above. The pages do not copy the clerk's text.

| Record | Date | Code tokens | With a value (first pass) | Three-digit, ledger value (first pass) | Three-digit, no value (first pass) | Bits per letter | Letters equal to the clerk's |
| --- | --- | ---: | --- | ---: | ---: | ---: | ---: |
| [R5627](r5627.md) | 15 Jan. 1633 | 751 | 92.5% (695) | 16 | 55 | 4.23 | 81.8% (control 34.1%) |
| [R5628](r5628.md) | 15 Jan. 1633 | 1,249 | 93.8% (1,172) | 45 | 73 | 4.46 | 74.8% (31.3%) |
| [R5629](r5629.md) | 23 Jan. 1633 | 753 | 91.5% (689) | 19 | 63 | 4.74 | 77.1% (36.3%) |
| [R5630](r5630.md) | 5 Feb. 1633 | 355 | 94.1% (334) | 10 | 21 | 4.23 | 82.4% (30.3%) |
| [R5631](r5631.md) | 12 Feb. 1633 | 671 | 93.4% (627) | 23 | 44 | 4.17 | 73.8% (32.7%) |
| [R5632](r5632.md) | 19 Feb. 1633 | 518 | 93.4% (484) | 13 | 33 | 4.88 | 73.2% (32.8%) |
| [R5633](r5633.md) | 23 Feb. 1633 | 1,189 | 93.6% (1,113) | 47 | 76 | 4.27 | 77.5% (33.3%) |
| [R5641](r5641.md) | May 1633 | 40 | 82.5% (33) | 2 | 7 | 5.15 | too small |
| [R5644](r5644.md) | June 1633 | 104 | 94.2% (98) | 2 | 5 | 4.04 | 63.7% (37.0%) |

- **All nine:** 5,630 code tokens. In the first pass, 5,245 had a value (93.2%), and three-digit tokens had 177 ledger values and 377 none. The graded pages show three-digit tokens as certain 67, probable 76, conjecture 119 and open 292.
- **The cipher ledger decoded R5630 before me.** Its notes of 29 October 2026 (Brice Dudout, `targets/ceva1632/NOTES.md`) decode R5630 f. 175 with Lasry's key, at 0.84 character agreement with the interlinear decipherment.
- **Letters equal to the clerk's:** the share of the shorter text's letters that align with equal letters of the clerk's decipherment. The method is that of `check.md`, section 7. The control aligns the same decode with the other records' decipherments.
- **What these letters say,** in short:
  - The death of "the Swede" (Gustavus Adolphus, killed at Lützen in November 1632) is in two letters of 15 January 1633 (R5627, R5628).
  - The French court agrees to send plenipotentiaries to a third place (R5630, 5 February 1633). The "third place" rests on the decipherment of the time.
  - The priory of San Martino for Signor Antonio, and Cardinal Richelieu's part in it (R5628, R5629, R5631). The name Antonio rests on the decipherment of the time.
  - The Duke of Rohan offered to serve the Republic of Venice, which did not accept (R5632). These names rest on open codes and on the clerk's text.
  - A person of rank (code 370) had to leave Rome; Rome insists that this was not done to avoid a test of precedence (R5633).
  - Father Joseph and a writing of Benavides (R5644). The name Father Joseph rests on the decipherment of the time.
  - Letters in clear name the business of the Bishop of Chalcedon (R5629, R5632) and a covering letter of Cardinal Antonio Barberini (R5633).

### The earlier leaves R74 to R78

- My pipeline read these ten scans in a pilot.
- Lasry, Megyesi and Kopal (2020) published readings of R74, R77 and R78.
- DECODE marks R74 and R76 "Decrypted", and R75, R77 and R78 "Partially decrypted".

| Record | Code tokens | With a value (first pass) | Three-digit, ledger value (first pass) | Three-digit, no value (first pass) | Bits per letter |
| --- | ---: | --- | ---: | ---: | ---: |
| [R74](r74.md) | 107 | 86.0% (92) | 5 | 15 | 4.34 |
| [R75](r75.md) | 181 | 80.7% (146) | 6 | 17 | 4.89 |
| [R76](r76.md) | 1,477 | 85.7% (1,266) | 48 | 202 | 4.83 |
| [R77](r77.md) | 987 | 95.1% (939) | 44 | 44 | 4.04 |
| [R78](r78.md) | 1,362 | 92.1% (1,254) | 38 | 85 | 4.21 |

- R74 to R76 read in fragments only. The pilot did not verify their digits.
- The decode leaves out R75 f. 81v and R76 f. 101r. The pipeline marks every digit row there as an inherited candidate that it did not verify.
- These five records were in the fit of my key-free key, so they give no key-free check.

### Thirteen records in another cipher

R5634, R5638, R5639, R5660 to R5666 and R5669 to R5671 do not read with the published key: 5.3 to 6.7 bits per letter. Their own decode agrees with the clerk's decipherment no more than with other records' decipherments.

- **One rule for the counts of these 13 records:** they cover all their cipher rows. That is the rows that the transcription labels as cipher, and 117 rows that it labels as text. Three rows with clear script inside them are left out.

- **R5634, R5638 and R5639** use digits only. The digit 6 is 2.9% to 7.7% of their digits. This is an observation; it does not show what 6 does there.
- **R5660 to R5671** mix digits with letter forms: 12 to 24 letter forms that the transcription reads without doubt (none in R5661, which has 55 doubtful ones). Each record page gives its counts and the rule. The key-free page test finds no pair structure on 23 of their 24 pages. The other page, R5666 f. 398v, passes only because it has too few runs to judge (17).
- The cipher ledger's notes of 29 October 2026 already say that R5670 uses a different system.
- **Twelve of the 13 carry a decipherment of the time between the cipher rows,** in my transcription. R5666 shows none there. A letter in clear stands on its later leaves, and I take it as the text of that cipher letter. This is my inference.
  - **R5634, R5638 and R5639:** a blind read is in progress. Their pages give no decode and no content yet.
  - **R5660 to R5666 and R5669 to R5671:** my tests found no cut of their rows that fits a letter cipher. No decode of mine exists. Their pages say what each letter says, in my words. The source is the clerk's decipherment of the time, or a clear copy on the leaves of the same record. The pages do not copy these texts.
- One page, R5669 f. 407r, has no transcription yet.

**What the ten letters say.** They come from Vienna and Madrid, 1632 to 1634.

- The address of R5670 names the extraordinary nuncio at Paris. Most of the others speak to a nuncio "costì" (there). In R5664, R5665, R5666 and R5671, the content points to the French court.
- A cover sheet in R5660 (f. 383r) says, in short, that it holds ciphers written to Mons. [?Ceva] by other nuncios.
- The pages report what the clerks' text, or a clear copy, says.

| Record | Place and date | What the letter says, in one line |
| --- | --- | --- |
| [R5660](r5660.md) | Vienna, 1 Sept. 1634 | Should the addressee find out, or disclose, a will for friendship with the Emperor? (sparse) |
| [R5661](r5661.md) | Madrid, 17 [?month] [?1632] | A good disposition at Madrid toward a settlement (sparse) |
| [R5662](r5662.md) | Madrid, 24 Sept. 1632 | One short line only; no summary |
| [R5663](r5663.md) | 1632; and Vienna, 20 Oct. [1632] | Bautru and Spain (sparse); a clear copy of R5664 |
| [R5664](r5664.md) | Vienna, 20 Oct. 1632 | The Imperial view of a union with France; Richelieu's letters to the Swede; a third place for talks |
| [R5665](r5665.md) | Vienna, [?3] Nov. 1632 | The Imperial side wants a sign of French good will, but not in its own name |
| [R5666](r5666.md) | Madrid, 20 Nov. 1632 | Bautru at Madrid, with no faculty to treat |
| [R5669](r5669.md) | Madrid, 19 Jan. 1633 | No peace talks before satisfaction for a French approach at Brussels |
| [R5670](r5670.md) | Madrid, 19 Feb. 1633 | [?Benavides] brings Spain's answers; the addressee may enter the treaty |
| [R5671](r5671.md) | Madrid, 9 [?March] 1633 | A commission for [?Benavides] and Aitona to enter the peace treaty |

**Three striking items.** Each comes from the clerk's text or a clear copy, in a machine transcription that nobody verified.

1. **Richelieu's letters to the Swede.** At Vienna on 20 October 1632, people at the Imperial court told the writer that they held letters of Cardinal Richelieu. In them, they said, Richelieu assured the Swede that the French King would never leave his alliance (R5664 f. 392r; the clear copy in R5663 f. 391r agrees).
2. **A message that must not look Imperial.** At Vienna in November 1632, the Imperial side asked for a sign of French good will. A letter of the King, or a spoken message in his name, would do. The addressee was to present the idea as his own, never as the idea of the Emperor or his ministers (R5665 ff. 395r, 396r and 396v).
3. **A commission to treat.** At Madrid in [?March] 1633, the writer obtained an order of the King of Spain. Ambassador [?Benavides] may now enter the peace treaty, and so may the [?Marquis] of Aitona in Flanders (R5671 f. 416v). A later letter notes that Bautru could not get such a faculty (R5671 f. 418r; see R5666).

## The key

- **The published key** gives 61 pair codes: 40 letter codes for 19 letters, and 21 syllable codes such as che, per and di. George Lasry reconstructed it, and it stands on DECODE with a key note of 24 October 2020.
- **The form of the cipher,** as the ledger rebuilt it from Lasry's own readings: a lone 6 is a word space, and the ten pairs 2x are nulls.
- **The published key gives no three-digit code a value.**
- **The cipher ledger** at https://github.com/dbourdeau/cyphersolver gives values to three-digit codes.
  - Its file `targets/ceva1632/cipher.py` gives 23 values.
  - Its notes on a re-read of 22 to 23 October 2026 (`targets/ceva1632/NOTES.md`) add five values and change one: 104 is Olandesi, not Svedesi.
  - The same notes change two pairs: 88 is del, not quel, and 33 is gli.
  - The first pass used these 28 three-digit values and the two pairs. The second pass grades 27 of them (129 regno is withdrawn by the ledger) and adds 19 values that the ledger read but did not adopt, as conjectures (see "The grades of the code values").
- **Some ledger values do not fit these letters.** For example, code 470 ("hor") stands where no "hor" can stand. Each record page lists such places, and the reading marks them `[?word]`.

## How to read the decode

Each record page ends with the decode, row by row, as the key gives it.

| Mark | Meaning |
| --- | --- |
| a space | the word space, a lone 6 |
| `abc` | letters and syllables of the key; the code for u and v is written u |
| `{word}` | a three-digit code with a **certain** value: a value that the ledger adopted, with no whole-word doubt in these letters |
| `{~word}` | a three-digit code with a **probable** value: a value that the ledger adopted, with a doubt at one place in one record |
| `[123 ?word]` | a three-digit code with a **conjecture**: a value that the ledger questioned or read off one decipherment of 1632 but did not adopt |
| `[123]` | a three-digit code with no value |
| `⟨a⟩` | a code that holds a doubtful digit of the transcription |
| `{word?}`, `{~word?}`, `[123?]` | a three-digit code that holds a doubtful digit; the value or the code as before |
| `·` | a code that holds an unread sign, or a lone digit that fits no code |
| `[…]` | an unread span of the transcription |
| `‖` | clear text stood here; this page does not copy it |

The cipher writes no double letters, so "sarebe" stands for "sarebbe". The readings mostly keep this spelling. In the readings, `[abc]` is supplied or changed by me, `[?word]` is a doubtful word, and `[…]` does not read. Where a silent repair remains, the decode line is the reference.

## Who read these letters before

- **Decipherment leaves.** Some records hold a decipherment in Italian on another leaf: R5626 (f. 155r), R5637 (f. 212v) and R5646 (f. 269r). Brice Dudout's notes in the ledger (29 October 2026) call such leaves contemporary. They add R5655 (f. 324) and find none in R5640. So some of these letters were read before.
- **Copies in clear** may also exist in other volumes. This folder does not copy the decipherment leaves, and it takes no code value from the decipherment leaves of these 22 records. The conjectures that it shows come from the ledger's readings of two 1632 decipherments in other records (ff. 82r and 136r).
- **DECODE.** On 12 November 2026, the public record pages of R5625 to R5659 all give the status "N/A" and the cipher type "Unknown". The word "Decryption" stands on each page, but its documents need a login, so I could not check them.
- **The cipher ledger.** Its entry 880 lists R5625 to R5686 as "N/A" with no decipherment filed, and says that none of them is in the repository. Its notes of 29 October 2026 name R5626, R5640 and R5655 in a sample, and say which leaves hold decipherments. They decode R5630 (now in this folder; see above), and none of the first 22 records. I checked the live catalogue and notes on 12 November 2026.
- **Print.** I found no edition of these letters. A. Iommelli's study of Ceva (Fondazione 1563, 2022) cites his own deciphered despatches, "Francia, 78", and Bichi's letters from Paris. In the first pass I found no citation of Francia 346 in it; the second pass did not check this again.

**No modern decipherment of these 22 records shows on DECODE's public record pages or is on file at the ledger.** This does not mean that nobody read them: the decipherment leaves show that some were read long ago.

**Most records added on 13 November were read at the time too.**

- Of the 22 records with "Inline Plaintext: Yes", 21 carry a clerk's decipherment between the rows in my transcription. R5666 has a letter in clear on its later leaves.
- Lasry, Megyesi and Kopal (2020) published readings of R74, R77, R78 and R82.

**A book of 1920.** A. Leman (1920) used the Barberini library's minutes of the cipher despatches to Ceva. So clear drafts of letters of this series were in use in print in 1920. I did not check which letters those minutes hold.

## Limits

- **The transcription** is a machine transcription. Nobody verified it against the images. A misread digit gives a wrong letter or a broken cut.
- **The cut** of the decode into two- and three-digit codes comes from a search with an Italian letter model. Where it picks a three-digit code, the letters around it can be wrong.
- **The readings** are mine. They supply words where the context allows, and they mark each supply. Many rows do not read.
- **639 three-digit tokens** stay open after the second pass (803 after the first). They hide names and words that the published key does not give.
- **Three records give almost nothing:** R5643, R5658 and R5659. Most of their cipher rows are unread in the source.
- **Four pages in three records do not read:** R5642 f. 246r, R5656 f. 337r and R5657 ff. 342r–v. On all four, 8 is rare and 6 is common, so the transcription may read some 8s as 6. A declared correction of misread digits failed its own check on a page that reads. My pipeline read these pages and those of R5643, R5658 and R5659 again; `rereads.md` decodes the newer transcription.

## The other records of the file

- **R5625** is a letter in clear. It holds no cipher. DECODE catalogues 9 pages but shows 2 scans.
- **17 records use other signs:** R5667, R5668 and R5672 to R5686. A test before the key found another system. Their pages name Madrid and Vienna. They stay open.
- **R79 to R84** have no transcription of my pipeline yet. DECODE holds its own transcription of them, and marks them "Decrypted" or "Partially decrypted". R83 uses another system.
- **Francia 32** is another file (1590 to 1592) in another cipher. See `../francia-32/README.md`.

## Credits

- **DECODE**, the database of historical ciphers of the DECRYPT project: records R74, R75, R76, R77, R78, R5626 to R5634, R5635 to R5639, R5640 to R5644, R5645 to R5659, R5660 to R5666 and R5669 to R5671. https://de-crypt.org/decrypt-web/RecordsList
- **The archive:** Archivio Apostolico Vaticano, Segreteria di Stato, Francia 346.
- **The key:** George Lasry, Beáta Megyesi and Nils Kopal (2020). The ledger's values for three-digit codes and two pairs: the cipher ledger at https://github.com/dbourdeau/cyphersolver.

DECODE's images are for research use only. They may not be redistributed or published without permission from the archive. No DECODE image is in this repository. I copy no row of cipher digits: each decode line gives its record, folio and row.

## Files

- `check.md`: the grade of the frozen read against the published key, and the checks of 13 November
- `r5626.md` to `r5659.md`: one page for each of the first 22 records, with the reading, the translation, the names and the decode row by row
- `r5627.md` to `r5644.md` (nine pages) and `r74.md` to `r78.md`: the records added on 13 November, with a summary, the names and the decode
- `r5660.md` to `r5666.md` and `r5669.md` to `r5671.md`: ten records in another cipher: what each letter says, from the decipherment of the time or a clear copy; no decode
- `r5634.md`, `r5638.md`, `r5639.md`: three records in another cipher, without a decode or content; a blind read is in progress
- `rereads.md`: the decode of ten pages that my pipeline read again
