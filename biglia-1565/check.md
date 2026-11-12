# Biglia, December 1565: the check against Dudout's reading

Milan, Veneranda Biblioteca Ambrosiana, Trotti 22, letter 2: fol. 7r, lines 33 to 45, and fol. 7v, lines 1 to 23. No DECODE record is known for this letter.

## 1. What was compared

- **My side:** the read as fixed before the check, one value for each code (`decryption.txt`, first part).
- **The reading:** Brice Dudout's reading of letter 2 and his key, rebuilt from the ciphertext alone (L'Europe chiffrée, 29 October 2026; https://bdudout.github.io/europe-chiffree/en/documents.html). I used the copy in the cipher ledger at https://github.com/dbourdeau/cyphersolver (folder `targets/biglia1565`). No key of the time is known.
- **The cut of his reading into codes** is mine: 1,275 codes, by the fewest-codes rule.
- **The times:** my read was fixed at 00:22 on 12 November 2026 (UTC−3). The comparison ran from 00:31 to 00:38. Nothing in the read changed after it.

Before the comparison, both sides are made plain: lower case, v as u and j as i.

## 2. The cipher, as my read found it, and as the key has it

| Part | My form, from the digits | Dudout's key |
| --- | --- | --- |
| Word space | `00` | `00` |
| Single digits | each digit is one code, with a table of letters | a single digit has a letter value; some have a vowel value and a consonant value, for example 5 is a or n |
| Pairs | none | two digits make a syllable, mostly a consonant digit and then a vowel digit |
| Words | none | a small set of codes for words, for example 4 for "quel" |
| `000` | a word space, then the code 0 | mostly a word space, then a pair that starts with 0 |

`key_check.tsv` gives, for each digit, my letters beside the values that the digit has as a one-digit code in his reading.

## 3. The cut

| Codes of the reading | With a code of mine at the same place and length |
| --- | --- |
| All | 55.1% (702 of 1,275) |
| Not word spaces | 35.8% (318 of 888) |
| One digit | 100% (326 of 326) |
| Two digits | 40.4% (376 of 931): all of them are word spaces |
| Three digits or more (words that the reading does not split) | 0% (0 of 18) |

- **Word spaces.** My read and the reading agree at 376 of 379 `00` places. No word space of mine falls inside a word of the reading.
- **Runs of three zeros (32).** In the reading, each run is a word space and then something more:
  - a pair that starts with 0, at 21 runs;
  - a word that the reading does not split, at 3;
  - a lone zero, at 8.

  My read takes all 32 as a word space and then a code 0.
- **Runs of four zeros (3).** The reading has a word space and then the code 00. My read has one word space.

## 4. The letters on the codes that my cut matches

| Codes of the reading | Shown | Right, of shown | Right, of all codes |
| --- | --- | --- | --- |
| All | 94.2% (660 of 701) | 91.7% (605 of 660) | 47.5% (605 of 1,275) |
| Not word spaces | 87.7% (278 of 317) | 82.4% (229 of 278) | 25.8% (229 of 888) |

These numbers count codes. Most of the matched codes are word spaces, which my form gives without a key. So section 6 measures the letters in another way.

By class:

| Class in the reading | Codes | Matched | Right, of shown |
| --- | ---: | --- | --- |
| letter | 288 | 98.6% (284) | 85.1% (212 of 249) |
| syllable | 521 | 0% (0) | none matched |
| word | 47 | 48.9% (23) | 50.0% (11 of 22) |
| word space | 387 | 99.2% (384) | 98.4% (376 of 382) |
| not fixed in the reading | 32 | 34.4% (11) | 85.7% (6 of 7) |

- The 23 matched word codes are the single digits 9 ("e", 12 places), 4 ("quel", 8) and 3 ("questo", 3). All 11 right answers are "e". At 4, my read shows e all 8 times.
- The 6 wrong word spaces are letters that my read gives at the lone zeros of section 3.
- "Not fixed" holds 22 words that the reading does not split, and 10 single digits with a bare value.

## 5. Syllables, when two letters are joined

My read often gives the first digit of a pair its consonant and the second digit its vowel. So I join my letters inside each code of the reading.

| Codes of the reading | Joined letters right, of all | Right, of codes with no gap |
| --- | --- | --- |
| syllable | 58.9% (307 of 521) | 79.5% (307 of 386) |
| letter | 73.6% (212 of 288) | 84.8% (212 of 250) |
| all but word spaces | 60.4% (536 of 888) | 79.4% (536 of 675) |

So the read is better than the cut numbers show.

## 6. The letters, word by word

Each decoded word is paired with the word of the reading at the same digits. An edit-distance alignment pairs their letters.

| Measure | Gaps left out | Gaps counted as misses |
| --- | --- | --- |
| Equal letters, of aligned pairs | **82.2%** (957 of 1,164) | 67.7% (953 of 1,407) |
| Equal letters, of the reading's letters | 63.3% (957 of 1,513) | 63.0% (953 of 1,513) |

- 359 of 381 words are scored. 22 have no letters in the reading.
- Words spelled exactly: 42.1% (151 of 359).

| Control (gaps left out) | Equal letters, of aligned pairs |
| --- | --- |
| Each word against the word 1 to 5 places later | 27.7% to 32.4% |
| Words in a random order (20 seeds) | 29.0% on average (26.4% to 31.5%) |
| Words of equal length in a random order (20 seeds) | 26.4% on average (24.3% to 31.1%) |

**One alignment of the whole letter:** 79.6% equal (969 of 1,218). Against the reading turned by half its length: 38.6% (465 of 1,206). Against its words shuffled (20 seeds): 39.3% on average.

So the decode follows this letter.

- Most of the letters that the comparison leaves out are under a gap.
- The reading has 1,513 letters in the scored words; my read has 1,409 symbols there. Some codes spell more letters than they have digits, such as "che" and "qua". A cut of one letter for each digit cannot spell them.

## 7. My estimate before the check

| Measure | Twins (4 test letters) | Real |
| --- | --- | --- |
| Shown letters right | 88.2% to 91.8% | 82.2% word by word (957 of 1,164) |
| Letter codes shown | 89.6% on average | 81.0% (1,246 of 1,539) |

- The twins used my own form: one code for each digit. They could not show the cost of a wrong form.
- So the twins overstate the read: by 6.0 to 9.6 points of precision and 8.6 points of coverage.

## 8. Limits

- **The reading is a modern reconstruction.** It is 95.0% read by sense: 313 words certain, 42 probable, 7 restored and 19 unresolved. I count probable and restored words as true.
- **The cut of the reading into codes** is mine. Some words allow more than one cut. 9 codes are one digit off.
- **The values are those of the reading in context**, not every value that the key allows. Under any value that the key allows, 93.3% of the shown codes are right (616 of 660).
- **Doubtful digits** in the transcription touch both sides in the same way.
- **The gaps** are not graded. My read gives no value there.
- The check ran once and changed no value of the key and no line of the decode.
