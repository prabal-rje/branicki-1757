# Francia 346: cipher letters of 1632 to 1634 in the Vatican's France series

**Read with my own algorithm, from the ciphertext alone, without the key.**

**The key is known.** George Lasry rebuilt it and published it on DECODE. His key note there has the date 24 October 2020. For the papal ciphers of this archive, see G. Lasry, B. Megyesi and N. Kopal, "Deciphering papal ciphers from the 16th to the 18th Century", *Cryptologia* 45(6), 2021 (online 2020), doi:10.1080/01611194.2020.1755915. The key stayed out of my read. I compared the read with the key only after the read was fixed.

**The check, in short.** Where my read shows a letter code, 99.2% of its letters are right (6,953 of 7,012). But about a third of the shown tokens that the check could grade are not letter codes: 3,579 of 10,591. They are syllables, nulls or false pairs of my cut. Of those graded shown tokens, 65.7% show the true letter (6,953 of 10,591).

- **Where:** Archivio Apostolico Vaticano, Segreteria di Stato, Francia 346. The cipher ledger at https://github.com/dbourdeau/cyphersolver calls this cipher the Barberini-Ceva cipher of 1632 to 1634 (its file `targets/ceva1632/cipher.py`).
- **DECODE:** records R74, R75, R76, R77, R78, R5626, R5635, R5636, R5637, R5640, R5643, R5647 and R5648. The appendix adds R5642, R5645, R5646, R5649, R5650 and R5651. DECODE is the database of historical ciphers of the DECRYPT project.
- **The digits:** for R74 to R78, from a transcription that rests on human readings. For the later leaves, from a reconciled draft transcription.
- **Use:** research only. I copy no image and no transcription. Each line of `decryption.txt` gives the DECODE record, page and row, so that a reader with access to DECODE can follow it. When you use this material, cite DECODE and the record numbers.

## What the letters say

These are my readings of the decoded text. `reading.md` gives each one with its record, page and row. The check confirmed 19 of these 21 names and phrases, and confirmed 2 in part. It contradicted none.

- **Persons and powers.** Benavides, at seven places. The Imperial court, the Swedes and the Germans, and the plenipotentiaries.
- **Places.** Nuremberg and Regensburg.
- **Peace and war.** A "universal peace", "maritime forces", a "victory" and "a successor".
- **Business.** An embassy, a priory, "the offers of pensions" and a "writing", that is, a document.
- **Dates.** 30 November and 3 December; February; "the 23rd of last month".

## The check, in short

Precision is the share right of the true letters that my read shows. Recovery is the share right of all true letters.

`check.md` gives every number with its count.

| Measure | Value |
| --- | --- |
| Letter codes of the key that my key reads right | 39 of 40 |
| True letter tokens that my read shows | 93.8% (7,012 of 7,474) |
| Of those, right | 99.2% (6,953 of 7,012) |
| True letter tokens recovered | 93.0% (6,953 of 7,474) |
| Graded shown tokens that show the true letter | 65.7% (6,953 of 10,591) |
| Shown code types that have the right letter | 39 of 69 |
| Letters equal, record by record, by edit distance | 74.9% (7,966 of 10,641) |
| The same measure against a wrong record | 35.9% (the grade gives the share only) |
| Names and phrases confirmed | 19 of 21, and 2 in part |

## What the read gets wrong

- **Codes that are not letters.** My key gives one letter to each pair of digits. In the key that the check used, 22 of my 80 pair codes are syllables, such as che (that), per (for) and di (of). 8 are nulls. 10 are no code at all: my cut makes a false pair there. My read shows a letter for 29 of these 40 code types.
- Two of the 22 syllable values come from a re-read, not from the published key (`check.md`, section 1).
- **One letter code.** The code 07 stands for h. My key reads l (59 graded tokens).
- **Long codes.** The key has three-digit codes for words and names. My cut has none. So it reads none of their 780 tokens, and the pairs run out of step until the next word space.
- **The twins were too sure.** My artificial test letters ("twins") had only letter codes. Across the twins, 99.3% to 99.8% of the shown tokens are right. On the real letters, 65.7% of the graded shown tokens are right (6,953 of 10,591). The twins could not show codes for syllables, nulls or words.

## How it was read

From the ciphertext alone, with no key, no crib and no other cipher.

- **The form:** a lone 6 is a word space, a lone 2 is a null, and the other digits form pairs. This gives 80 pair codes. The method found the form from the digits.
- **The language:** Italian, from the archive's catalogue. The method alone could not choose: in one pool it preferred Spanish by a very small margin.
- **The letter model:** Italian letter counts from Muratori's writings.
- **The fit:** a search for a key that makes the decoded text likely as Italian, from 100 starts. All 100 end within 18.9 nats of the best. A nat is a unit of log likelihood. 37 starts stopped at the cap of 200 steps.
- **The display:** a code shows its letter when 90% or more of the starts within 100 nats agree. It must also have 3 or more tokens. This shows 69 of 80 codes and 90.4% of the code tokens (11,101 of 12,283).
- **The size:** 13 records, 12,283 tokens in the fit.

## Caveats

- **The later leaves.** For them, the check had no reference reading. The truth is the published key applied to the same draft transcription that I read. A misread digit hurts both sides in the same way.
- **The truth's cut** of R76 and the later leaves is a reconstruction from the key. On four records with a cut from earlier readings, it agrees on 98.1% of the letter codes (2,634 of 2,684).
- **Masked digits:** 1,041 true tokens hold a doubtful digit. They are not graded.
- **u and v** count as one letter, and **i and j** count as one letter.
- **Double letters** are often single in the decode: "fratelo" for "fratello" (brother), "toco" for "tocco" (touch). This can be the clerk's spelling or a fault of the read.
- **The appendix** of six records comes from a second key, read from all 19 records. It is less sure: 38 of its 76 shown code types are right.

## Words used here

- **Crib:** a piece of the plain text that the solver knows in advance.
- **Start:** one run of the search, from its own random key.
- **Plenipotentiary:** an envoy with full powers to negotiate.
- **Twin:** an artificial test letter, made with a known key and read by the same method.

- **Code:** a group of digits that stands for a letter, a syllable, a word or nothing.
- **Cut:** the division of the digit stream into codes.
- **Null:** a code that stands for nothing.
- **Token:** one code at one place in the text.
- **Nat:** a unit of log likelihood. A larger value is a better fit.

## Files

- `reading.md`: the names, phrases and stretches that read, with English translations and the check
- `check.md`: the comparison with the published key
- `decryption.txt`: the full decode, row by row, with gap marks
- `key.tsv`: my key, one row for each pair code
- `key_check.tsv`: each pair code's value beside the published key
