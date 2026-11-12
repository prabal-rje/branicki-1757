# Morosini, 1587 to 1589: the check against the published key

## 1. What was compared

- **My side:** the read of all 35 records, as fixed before the check (`key.tsv`, `decryption.txt`). Also 18 smaller windows, each read by itself in the same way.
- **The key:** A. Meister, *Die Geheimschrift im Dienste der päpstlichen Kurie* (Paderborn, 1906), pp. 393 to 394, no. 40, with George Lasry's partial reconstruction on DECODE (attached to record R18, October 2020).
- **The truth:** the published key applied to DECODE's transcriptions of the 35 records (R17, R18 to R22, R27 to R49, R51, R52 and R55 to R58). It is cut into 123,582 code tokens. 110,821 of them are letters.
- **The times:** the read was fixed by 01:27 on 12 November 2026 (UTC−3). The comparison ran from 01:30 to 01:53. Nothing in the read changed after it.

Definitions:

- **Matched:** a code of my read with the same record, the same starting position and the same length as a code of the truth.
- **Right:** a matched letter code whose value equals the truth's letter. j and y count as i, k as c, v and w as u.
- **Precision:** right, of the matched single-letter codes that show a value.
- **Recovery:** right, of all single-letter codes of the truth.

## 2. The numbers for all 35 records

| Measure | Value |
| --- | --- |
| Codes of the truth that my cut matches | 74.4% (91,903 of 123,582) |
| Matched letter codes that show a value | 100% (84,667 of 84,667) |
| Precision | 95.1% (80,553 of 84,667) |
| Recovery | 72.7% (80,553 of 110,821) |
| All tokens right, of all tokens of the truth | 65.2% (80,553 of 123,582) |

The truth by class, and what my read gives there:

| Class in the truth | Tokens | Matched | Right |
| --- | ---: | ---: | ---: |
| letter (single-letter codes) | 110,821 | 84,667 | 80,553 |
| syllable | 4,610 | 2,776 | 0 |
| word | 5,324 | 3,508 | 0 |
| null | 2,625 | 949 | 0 |
| not fixed in the truth | 202 | 3 | 0 |

- A key with one letter for each code cannot be right at a syllable or a word.
- All 949 matched true nulls show a letter.
- My key makes 680 matched letter codes, 718 syllable codes and 1,097 word codes nulls.

By record, the precision lies between 91.4% (R35, 1,146 of 1,254) and 96.8% (R31, 2,592 of 2,679; R43, 2,881 of 2,977). The recovery lies between 60.4% (R35, 1,146 of 1,896) and 77.0% (R44, 1,608 of 2,088).

## 3. A second view that needs no cut

For each line of the transcription, I join my letters in order, and I join the truth's letters of the same line. An edit-distance alignment pairs them. The main number is the share of equal letters among the aligned pairs.

| Measure | Value |
| --- | --- |
| Equal letters, of aligned pairs | 83.2% (98,964 of 118,881) |
| The same, with the truth cut to letter codes only | 87.6% (95,169 of 108,621) |
| Control: each line against the line 7 places later | 31.0% (36,533 of 117,814) |
| Control: each line against its own truth in a random order (3 seeds) | 33.5% (118,636 of 353,868) |

So about 31% is what chance gives. The read is far above both controls.

## 4. The windows

I read windows of 1,000, 2,000, 5,000, 10,000, 20,000 and 50,000 tokens, three of each size, each by itself. The sizes count the tokens of my own first cut. The three windows of one size start in different records.

| Window | Records | Precision | Recovery |
| --- | --- | --- | --- |
| 1,000 (1) | R17 | **48.5%** (263 of 542) | 32.5% (263 of 810) |
| 1,000 (2) | R36 | 85.7% (523 of 610) | 64.8% (523 of 807) |
| 1,000 (3) | R58 | 80.8% (449 of 556) | 51.8% (449 of 866) |
| 2,000 (1) | R17 | 87.9% (1,007 of 1,145) | 61.4% (1,007 of 1,639) |
| 2,000 (2) | R36 | 92.1% (1,116 of 1,212) | 68.8% (1,116 of 1,621) |
| 2,000 (3) | R58 | 96.6% (1,281 of 1,326) | 75.0% (1,281 of 1,707) |
| 5,000 (1) | R17 to R18 | 93.1% (2,723 of 2,924) | 66.7% (2,723 of 4,083) |
| 5,000 (2) | R36 to R37 | 95.6% (3,004 of 3,142) | 72.9% (3,004 of 4,122) |
| 5,000 (3) | R57 to R58 | 98.8% (3,302 of 3,341) | 77.2% (3,302 of 4,276) |
| 10,000 (1) | R17 to R19 | 94.2% (5,532 of 5,870) | 67.1% (5,532 of 8,241) |
| 10,000 (2) | R35 to R38 | **71.2%** (4,099 of 5,756) | 49.7% (4,099 of 8,248) |
| 10,000 (3) | R55 to R58 | 98.4% (6,386 of 6,492) | 75.2% (6,386 of 8,487) |
| 20,000 (1) | R17 to R20 | 95.9% (11,865 of 12,372) | 71.2% (11,865 of 16,654) |
| 20,000 (2) | R33 to R38 | 92.7% (11,384 of 12,275) | 68.4% (11,384 of 16,650) |
| 20,000 (3) | R48 to R57 | 94.3% (12,018 of 12,750) | 71.4% (12,018 of 16,830) |
| 50,000 (1) | R17 to R32 | 95.3% (30,591 of 32,084) | 72.6% (30,591 of 42,136) |
| 50,000 (2) | R30 to R44 | **49.5%** (14,941 of 30,177) | 35.6% (14,941 of 42,010) |
| 50,000 (3) | R42 to R58 | 95.2% (30,946 of 32,515) | 73.3% (30,946 of 42,205) |
| All 35 records | R17 to R58 | 95.1% (80,553 of 84,667) | 72.7% (80,553 of 110,821) |

**Three windows ended on a wrong key:** 1,000 (1), 10,000 (2) and 50,000 (2), with a precision below 75%.

- Their starts agreed. They showed a value on 98.4% to 99.0% of their tokens (1,008 of 1,024; 10,467 of 10,583; 51,744 of 52,262), and on 99.8% to 100% of their matched letter codes. So the display rule did not flag them.
- In the 50,000 (2) window, whole letters are swapped: o and a, l and n.
- In the read of all 35 records, each record of that window reads at 91% to 97% precision. So the text alone does not explain the failure.
- The 20,000 (2) window holds R33 to R38, so it holds all the records of the 10,000 (2) window. It did not fail.
- Leave out the wrong window of a size. Then the other two windows agree within 13.0 points of recovery (1,000), 8.1 points (10,000) and 0.7 points (50,000).
- At 20,000 tokens, the three recoveries agree within 3.0 points.

The windows from 2,000 tokens up that did not fail read at 87.9% to 98.8% precision, and 61.4% to 77.2% recovery.

## 5. My key against the published key

`key_check.tsv` gives each code. The check graded each code type with 3 or more matched letter tokens. It compared my value with the commonest true letter of its tokens.

- **31 of 34 code types are right.** Every wrong letter of section 2 is in the three wrong types below, or in one rare code. Together they hold 3,398 + 679 + 36 + 1 = 4,114 tokens.
- **The single digit 2** stands for a. My key reads i (3,398 graded tokens).
- **The single digit 1** stands for r. My key reads a null (679 graded tokens).
- **The code 07** stands for p. My key reads e (36 graded tokens).
- One more wrong token falls on a rare dotted code.

Before I saw the check, my notes named the first error. The decode has too many i's: 19.9% of the shown letters (24,643 of 123,854), against about 10% in Italian. Words end in "ai" where the sense needs "a": "delai chiesi" for "della chiesa", of the church (R18 p1 l08).

The codes that the check could not grade by letter:

- **8 and 8 with a next digit** are nulls in the published key. My key gives them letters: 8 is e (1,445 tokens).
- **56** is a word code in the published key. My key reads it as a null (1,555 tokens).
- **Dotted codes.** In the published key, dotted three-digit codes stand for words and names. My read treats five dotted three-digit codes as word codes and gives them no value. It cuts the other dotted digits as codes of one or two digits and gives them letters.

In the three windows on a wrong key, 8 of 25, 19 of 31 and 13 of 34 code types are right.

## 6. Why the cut fails

The published key has these parts:

- Letters have codes of one, two or three digits. The three-digit letter codes carry no dot, for example 212 for a and 171 for i.
- 8 alone, and 8 with any next digit, are nulls.
- Some two-digit codes stand for syllables, for example et (and), con (with) and qu. Others stand for short words, for example che (that), per (for) and non (not).
- Dotted three-digit codes stand for words and names.

My form allows three digits only with a dotted middle digit. The table counts the truth's tokens of each kind and how many my cut matches.

| Tokens of the truth | Tokens | Matched by my cut |
| --- | ---: | --- |
| one digit, letter | 26,435 | 63.5% (16,797) |
| two digits, letter | 73,848 | 91.9% (67,869) |
| three digits without a dot, letter | 10,520 | 0% (0) |
| two digits, syllable | 4,608 | 60.2% (2,776) |
| two digits, word | 3,346 | 66.6% (2,228) |
| three digits with a dot, word | 1,978 | 64.7% (1,280) |
| null, one or two digits | 2,625 | 36.2% (949) |

- **Three-digit letter codes.** All 10,520 are cut wrong, 8.5% of all tokens. Most become two digits plus one (6,426). So 212 becomes 21 and 2: "a" and "i". This explains the "ai" endings of section 5.
- **Single digits.** 9,638 one-digit letters are joined with a neighbour into a two-digit code.
- **Pairs.** 3,457 two-digit codes are cut into two single digits.
- **The count.** My read has 135,052 codes, 9.3% more than the truth's 123,582.

## 7. The artificial test letters

Before I saw the check, I made artificial letters ("twins") with the form that my read found. I read them by the same method, at the same sizes.

- There are five twins at each size from 1,000 to 50,000 tokens, and three at the size of all 35 records.
- The twin columns give the lowest and the highest twin.
- The real columns give the three windows of each size, in the order of section 4. A star marks a window that ended on a wrong key.

| Size | Twins: precision | Twins: recovery | Real: precision | Real: recovery | Real: mean recovery |
| --- | --- | --- | --- | --- | --- |
| 1,000 | 93.8% to 99.7% | 81.1% to 90.2% | 48.5%\*, 85.7%, 80.8% | 32.5%\*, 64.8%, 51.8% | 49.7% |
| 2,000 | 97.2% to 99.9% | 86.3% to 95.9% | 87.9%, 92.1%, 96.6% | 61.4%, 68.8%, 75.0% | 68.4% |
| 5,000 | 99.3% to 100% | 91.5% to 95.8% | 93.1%, 95.6%, 98.8% | 66.7%, 72.9%, 77.2% | 72.3% |
| 10,000 | 99.4% to 99.9% | 94.0% to 96.6% | 94.2%, 71.2%\*, 98.4% | 67.1%, 49.7%\*, 75.2% | 64.0% |
| 20,000 | 99.7% to 100% | 94.5% to 96.6% | 95.9%, 92.7%, 94.3% | 71.2%, 68.4%, 71.4% | 70.3% |
| 50,000 | 99.6% to 100% | 94.5% to 96.0% | 95.3%, 49.5%\*, 95.2% | 72.6%, 35.6%\*, 73.3% | 60.5% |
| All 35 records | 99.6% to 99.9% | 95.4% to 95.8% | 95.1% | 72.7% | 72.7% |

- Over all sizes, the real mean recovery is 49.7% to 72.7%. Twin recovery is 81.1% to 96.6%.
- The three wrong windows pull down the means at 1,000, 10,000 and 50,000 tokens.
- The twins match 86.2% to 97.2% of their codes. The real windows match 63.5% to 76.5%. The twins used my own form, so they could not show the error of the cut.
- No twin ended on a wrong key. Three real windows did.
- The twin grade counts nulls and word codes in the base of its recovery. The real grade counts single-letter codes only. So the two measures are close, not equal.
- So the twins overstate the real read.

## 8. Limits

- **The truth is a decode.** By an earlier estimate, it has letter slips of about 1 to 3%. So precision has a ceiling below 100%.
- **The truth's cut.** Where the digits allow two cuts, the truth holds one.
- **41 tokens can never match:** 23 have no place in my read, and 18 hold a `?` or `%` mark.
- **Record R17** has a `%` sign (371 times) that the truth's figures do not hold. R17 is in the first window of each size.
- **Small windows.** A 1,000-token window holds 807 to 866 letter codes. The counts matter more than the shares there.
- **The names and phrases** of `reading.md` were not checked one by one.
- The check ran once and changed no value of the key and no line of the decode.
