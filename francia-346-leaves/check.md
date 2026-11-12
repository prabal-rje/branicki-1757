# Francia 346: the check against the published key

## 1. What was compared

- **My side:** the read as fixed before the check (`key.tsv`, `decryption.txt`, `reading.md`).
- **The key:** George Lasry's key, published on DECODE. His key note there has the date 24 October 2020. See also G. Lasry, B. Megyesi and N. Kopal, "Deciphering papal ciphers from the 16th to the 18th Century", *Cryptologia* 45(6), 2021 (online 2020), doi:10.1080/01611194.2020.1755915.
- **Two values** come from a re-read of these letters in the cipher ledger at https://github.com/dbourdeau/cyphersolver (22 to 23 October 2026), against contemporary decipherments. 88 is del; the published key has quel. 33 is gli; the published key does not have it. My key reads 88 as i and 33 as l, so no verdict depends on them.
- **The truth:** the published key applied to the same digits that I read.
  - For R74, R77 and R78, the cut into codes comes from Lasry's published readings. For R75, it comes from the ledger's third reading pass.
  - For R76 and the later leaves, the cut is a reconstruction from the key.
- **The times:** the read was fixed at 01:27 on 12 November 2026 (UTC−3). The comparison ran from 01:40 to 02:00. Nothing in the read changed after it.

## 2. The cipher, as my read found it, and as the key has it

| Part | My form, from the digits | The published key |
| --- | --- | --- |
| Word space | a lone 6 | 6 (no code holds a 6) |
| Nulls | a lone 2 | every pair 2x |
| Pairs | 80 pair codes, one letter each | 61 pair codes: letters, and syllables such as che (that), per (for) and di (of) |
| Long codes | none | three digits: a prefix digit and a pair, for words and names |

The truth's tokens by class:

| Class | Tokens |
| --- | ---: |
| letter | 7,474 |
| word space | 1,936 |
| syllable | 1,793 |
| null | 1,648 |
| three-digit code, value open | 445 |
| three-digit code, a word | 243 |
| three-digit code, a name | 92 |
| a doubtful digit (not graded) | 1,041 |
| a pair that the key does not use (published cuts only) | 10 |

## 3. My key against the published key

`key_check.tsv` gives each of my 80 pair codes.

- **The key that the check used** is the published key with the two re-read values of section 1. `key_check.tsv` gives both where they differ.
- **Letter codes:** 40 of my codes are letters in the published key. My key reads 39 of them right. Code 07 is h; my key reads l.
- **Syllable codes:** 22 of my codes are syllables. My key gives each one a single letter. For 205 tokens it gives the syllable's first letter.
- **Null codes:** 8 of my codes are nulls (pairs 2x). My key gives them letters.
- **False pairs:** 10 of my codes are no code of the cipher: 05, 60, 61, 63, 64, 65, 67, 68, 69 and 99. Eight of them start with 6: my cut joins a word space with the next digit. The key does not use the pairs 05 and 99.
- **All codes:** 39 of 80 right.

The display hides 11 codes. All 11 are not letters: nulls 20, 24, 27 and 28; syllables 54, 73 and 94; false pairs 64, 68, 69 and 99. It shows 69 codes: 40 letters, 19 syllables, 4 nulls and 6 false pairs.

| Rule | Codes shown | Right | Share |
| --- | ---: | ---: | --- |
| The display (90% of the starts agree) | 69 | 39 | 56.5% |
| The 2 best starts agree | 78 | 39 | 50.0% |
| The 5 best starts agree | 74 | 39 | 52.7% |

**My notes before the check.** They named code 14 as probably wrong: it read h inside words, where Italian has no h. The key makes 14 the syllable mi. My notes also expected wrong l, d and i at short words. The key agrees: the l codes 21, 23, 25 and 29 are nulls, 33 and 77 are syllables, and the d code 89 is qu.

## 4. The letters

| Records | True letter tokens | Shown | Right | Recovery |
| --- | ---: | --- | --- | --- |
| All 13 | 7,474 | 93.8% (7,012) | 99.2% (6,953 of 7,012) | 93.0% (6,953 of 7,474) |
| R74 to R78 | 4,214 | 93.7% (3,947) | 99.2% (3,917 of 3,947) | 93.0% (3,917 of 4,214) |
| The 8 later records | 3,260 | 94.0% (3,065) | 99.1% (3,036 of 3,065) | 93.1% (3,036 of 3,260) |

All 59 wrong letter tokens are code 07. Every other letter token that my read shows is right.

**All shown tokens.** My read shows 11,101 tokens. 510 of them touch a doubtful digit or an unmapped part of the truth, and are not graded. Of the other 10,591, 65.7% show the true letter (6,953). The table gives what the 10,591 graded tokens are in the truth.

| In the truth | Shown tokens |
| --- | ---: |
| a letter, right | 6,953 |
| a letter, wrong | 59 |
| a syllable, shown as its first letter | 205 |
| a syllable, shown as another letter | 1,217 |
| a null | 600 |
| a pair that the key does not use | 1 |
| no true code at this place (a wrong cut) | 1,556 |

By record, the precision lies between 95.7% (R5647, 22 of 23) and 100% (R5643, 16 of 16). The recovery lies between 73.3% (R5647, 22 of 30) and 97.5% (R77, 664 of 681). R5643 and R5647 are the smallest records, with 20 and 30 true letter tokens.

## 5. The cut

- **True tokens with a code of mine at the same place and length:** 82.3% (11,225 of 13,641). R74 to R78: 83.1% (6,448 of 7,755). The later 8: 81.2% (4,777 of 5,886).
- By class:
  - letters 93.8% (7,012 of 7,474);
  - syllables 93.6% (1,679 of 1,793);
  - word spaces 75.2% (1,456 of 1,936);
  - nulls 65.2% (1,074 of 1,648);
  - three-digit codes 0% (0 of 780).
- Most lost word spaces lie where my read makes a false pair with a 6 (480 tokens). After a three-digit code, my pairs run out of step until the next word space.

## 6. A second view that needs no cut

For each record, I join my decoded letters and the truth's letters. An edit-distance alignment pairs them.

| Records | Equal letters, of aligned pairs | Control: a wrong record | Control: the record's own words shuffled (equal, of true letters) |
| --- | --- | --- | --- |
| All 13 | 74.9% (7,966 of 10,641) | 35.9% | 30.0% |
| R74 to R78 | 75.3% (4,564 of 6,062) | 37.2% | 29.8% |
| The 8 later records | 74.3% (3,402 of 4,579) | 34.2% | 30.4% |

Every record lies above its control. The margin is smallest for R5643, the smallest record (41 true letters).

**Witnesses that do not use the key.** Four records have a decipherment or a clear text that does not come from the key. Two are contemporary decipherments of the later leaves.

| Record | Witness | My read: equal, of aligned pairs | The key's decode: equal, of aligned pairs |
| --- | --- | --- | --- |
| R75 | the decipherment on f. 82r | 76.8% | 95.3% |
| R76 | an interlinear decipherment (the plaintext lines of DECODE's transcription) | 66.6% | 87.7% |
| R5626 | a contemporary decipherment | 59.0% | 68.2% |
| R5637 | a contemporary decipherment | 63.5% | 80.6% |

So the key also holds on the later leaves.

## 7. The names, phrases and stretches

- **The names and phrases (21 items): 19 confirmed, 2 confirmed in part, 0 contradicted.** `reading.md` gives each verdict.
- **The stretches (22 rows):** in 20 rows, every content word that I restored stands in the truth. In 2 rows, one restored word differs. `reading.md` gives both.
- The grader's test did not cover restored small words, such as di, il and e. In one of the 20 rows the content word stands, but the key's decode has "no" (not) before it. `reading.md` notes this and the small words that differ.

## 8. The appendix

Six records differ a little from the others in their code counts. I read them with a second key, fitted on all 19 records.

| Records | Shown | Right | Recovery |
| --- | --- | --- | --- |
| R5642, R5645, R5646, R5649, R5650, R5651 | 91.3% of 1,877 true letter tokens | 97.4% (1,669 of 1,714) | 88.9% |

This key reads two letter codes wrong: 07 (l for h) and 79 (l for b). 38 of its 76 shown codes are right.

## 9. My estimate before the check

| Measure | Twins | Real |
| --- | --- | --- |
| Shown tokens right | 99.3% to 99.8% | 65.7% of graded shown tokens (6,953 of 10,591) |
| Shown code types right | 93.8% to 95.0% | 56.5% (39 of 69) |
| True letter tokens right, of those shown | (the twins had only letters) | 99.2% (6,953 of 7,012) |

- On true letter codes, the read is as good as the twins said.
- But a third of the shown tokens are not single letters in the truth. The twins had no codes for syllables, nulls or words, so they could not show this.
- My notes before the check called the twin figure "an optimistic calibration, not a proven bound".

## 10. Limits

- **The later leaves.** For them, the check had no reference reading. The truth is the key applied to my own digits. A misread digit hurts both sides.
- **The truth's cut** of R76 and the later leaves is a reconstruction. On the four records with a published cut, the two cuts give numbers within 0.5 percentage points of each other.
- **Doubtful digits:** 1,041 true tokens hold one. They are not graded.
- **Digits that do not map:** for R74 to R78, 233 of 5,226 tokens of the published readings could not be placed on my digits. They are not graded.
- The verdicts of section 7 rest on the grader's judgement of each cited row.
- The check ran once and changed no value of the key and no line of the decode.
