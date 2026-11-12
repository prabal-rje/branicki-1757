# Morosini, 1587 to 1589: cipher despatches of the Vatican's France series

**Read in part, with my own algorithm, from the ciphertext alone, without the key.**

**The key is known from print.** A. Meister printed it in 1906, and George Lasry rebuilt it in part on DECODE in 2020. I used the key only for the check, after my read was fixed. No part of the key went into the read.

**The check, in short.** My cut of the digits matches some single-letter codes of the published key. On those, 95.1% of my letters are right (80,553 of 84,667). But my cut matches only 74.4% of all codes (91,903 of 123,582). In all, my read recovers 72.7% of the single-letter codes of the published key's decode (80,553 of 110,821).

The same method recovers more on artificial test letters ("twins"). Over the window sizes, the mean recovery on the real text is 49.7% to 72.7%. On twins of the same sizes, it is 81.1% to 96.6%.

**Correction, 12 November 2026.** A later check found a fault in this read. My rule cuts the digits under the best of 20 first starts. This read cut them under the second-best start. The cause is not known.

- The read under the rule gets 95.2% of the matched single-letter codes right (80,251 of 84,284). Its cut matches 74.0% of all codes (91,481 of 123,582). It recovers 72.4% of the single-letter codes (80,251 of 110,821).
- The two reads show a different value on 25 of their 135 shared code types.
- The 12 test windows of 10,000 tokens or fewer follow the rule. The 6 larger windows are not checked yet.
- Every number and file below is still that of the first read. I will rebuild them from the read under the rule.

- **Where:** Archivio Apostolico Vaticano, Segreteria di Stato, Francia 22 (records R18 to R58) and Francia 18/3 (record R17).
- **DECODE:** records R17, R18 to R22, R27 to R49, R51, R52 and R55 to R58, 35 records in all. DECODE is the database of historical ciphers of the DECRYPT project. DECODE's volunteers made the transcriptions.
- **Use:** research only. I copy no image and no transcription. Each line of `decryption.txt` gives the DECODE record, page and line, so that a reader with access to DECODE can follow it. When you use this material, cite DECODE and the record numbers.
- **The key:** A. Meister, *Die Geheimschrift im Dienste der päpstlichen Kurie* (Paderborn, 1906), pp. 393 to 394, no. 40. George Lasry's partial reconstruction is attached to DECODE record R18 (October 2020).

## What the read says

These are my readings of the decoded text, made without the key. `reading.md` gives each stretch with its record, page and line, and an English translation. The check compared letters, not these items one by one.

- **The Council of Trent.** Several despatches treat its publication in France (R18, R22, R33): "without any limitation" (R18), "without any condition" (R22).
- **The Church in France.** "The liberty of the church", perhaps the Gallican church (the Church of France). The nuncio, "monsignor of Rimini", the legate and the Holy See (R18, R19, R22).
- **The parties.** Guise, the King, Navarre, Épernon and Montmorency, and perhaps the League.
- **Places.** Paris, the Sorbonne, Chartres, Rome, Lyon, Orléans, Angers and Savoy.
- **Towns and soldiers (R52, R58).** The castellan of Angers and Monsieur de Brissac. A "martiale", perhaps a marshal, who is "to come back" with "possible speed". A castle, a bridge on a river, and soldiers who are paid.
- **A closing (R57).** "Most humble and most obedient servant", in June.

## The check, in short

Precision is the share right of the matched single-letter codes that my read shows. Recovery is the share right of all single-letter codes of the published key's decode.

`check.md` gives every number with its count.

| Measure | Value |
| --- | --- |
| Codes of the published key that my cut matches (same place and length) | 74.4% (91,903 of 123,582) |
| Precision: letters right, of the matched single-letter codes | 95.1% (80,553 of 84,667) |
| Letters right, of all my letter codes that match any code | 91.4% (80,553 of 88,127) |
| Recovery: single-letter codes of the published decode that my read recovers | 72.7% (80,553 of 110,821) |
| Recovery at each window size (mean of the three windows; all 35 records as one window) | 49.7% to 72.7% |
| Recovery on twins of the same sizes | 81.1% to 96.6% |
| Letters equal, line by line, by edit distance (this needs no cut) | 83.2% (98,964 of 118,881) |
| The same measure against a wrong line | 31.0% (36,533 of 117,814) |
| Code types right, of the 34 with 3 or more graded letter tokens | 31 of 34 |
| Windows that ended on a wrong key | 3 of 18 |

## What the read gets wrong

- **The cut.** The published key has three-digit letter codes with no dot. My form allows three digits only with a dotted middle digit. So all 10,520 of these tokens are cut wrong, 8.5% of all tokens (10,520 of 123,582). This is the largest error.
- **A frequent letter.** The single digit 2 stands for a. My key reads it as i (3,398 graded tokens). Many decoded words end in "ai" where the sense needs "a".
- **A letter read as a null.** The single digit 1 stands for r. My key reads it as a null (679 graded tokens).
- **Nulls read as letters.** The published key makes 8, alone or with any next digit, a null. My key gives these codes letters. All 949 true nulls with a matched code show a letter.
- **Syllables and words.** Some two-digit codes stand for syllables, such as et (and), con (with) and qu: 4,608 tokens. Others stand for short words, such as che (that), per (for) and non (not): 3,346 tokens. A key with one letter for each code cannot read them.
- **Three windows on a wrong key.** I also read 18 smaller windows, each by itself. Three of them ended on a wrong key: 1,000 tokens in R17, 10,000 tokens in R35 to R38, and 50,000 tokens in R30 to R44. Their starts agreed, so nothing in the read flagged them.

`check.md` gives the counts and the causes.

## A second search

After the check, I planned a second search for the code forms that my form missed. These were two-digit codes missing from my form, three-digit codes without a dot, and codes for words.

- Before it could run on the real text, it had to pass a test on twins with such forms hidden in them.
- It failed that test. It found a frequent hidden null pair, but it named it a word code. It missed the rarer hidden forms.
- So it did not run on the real text. The read on this page is the first read.

## How it was read

From the ciphertext alone, with no key, no crib and no other cipher.

- **The input:** DECODE's transcriptions, as digits, with the dot marks. All 35 records form one text of 232,130 digits.
- **The form:** codes of one or two digits, or of three digits with a dotted middle digit. A code with a dotted digit is a code type of its own. A three-digit code is a word code and gets no letter.
- **The letter model:** Italian letter counts. Each letter is scored on the four letters before it (order 5). The counts come from 11.2 million letters: Milanese dispatches of the 15th century and ten historical Italian prose texts.
- **The fit:** a search for a key that makes the decoded text likely as Italian, from 100 starts. 13 starts reach the best score, and 16 more come within 0.13 nats of it.
- **The display:** a code shows its value when 90% of those 29 starts agree, and it has 3 or more tokens. This shows a value on 99.0% of the tokens (133,724 of 135,052). The gaps are the word codes and rare codes.
- **Nulls:** my key makes 7.3% of the tokens nulls (9,870 of 135,052). These are the single 1 and the codes 19, 56, 65 and 76, with some dotted codes.

## Caveats

- **The truth is a decode.** It is the published key applied to DECODE's transcription. By an earlier estimate, it has letter slips of about 1 to 3%. So a perfect read would score a little below 100%.
- **The truth's cut.** Where the digits allow two cuts, the truth holds one. The match of my cut depends on it.
- **41 tokens** of the truth have no place that my read can match. They count against my read.
- **Artificial test letters.** I made twins of the same sizes and form before I saw the check, and read them by the same method. At the size of all 35 records, 99.6% to 99.9% of their shown letters are right, and their recovery is 95.4% to 95.8%. They used my own form, so they could not show the error of the cut. No twin ended on a wrong key. The real numbers are lower.
- **One count known early.** Before the read, I knew one number of the published decode: its count of code tokens, 123,582. The method did not use it, and I tuned nothing to it.
- **Double letters** are often single in the decode ("dela", "tuto"). This can be the scribe's spelling. I do not count it as an error.
- **The years** do not read. I did not test which codes stand for numbers.
- **The language.** Most records are in Italian. By earlier readings of these records, R35 is a Spanish memorandum. My read used an Italian letter model for all of them. R35 has the lowest precision of the 35 records.

## Words used here

- **Crib:** a piece of the plain text that the solver knows in advance.
- **Start:** one run of the search, from its own random key.
- **Nuncio:** the Pope's ambassador.
- **Twin:** an artificial test letter, made with a known key and read by the same method.
- **Nat:** a unit of log likelihood. A larger value is a better fit.

- **Code:** a group of one to three digits that stands for a letter, a syllable, a word or nothing.
- **Cut:** the division of the digit stream into codes.
- **Null:** a code that stands for nothing.
- **Nomenclator:** the part of a key with codes for whole words and names.
- **Token:** one code at one place in the text.
- **Window:** a run of the text that the algorithm reads by itself.

## Files

- `reading.md`: the stretches that read, with English translations
- `check.md`: the comparison with the published key
- `decryption.txt`: the full decode, line by line, with gap marks
- `key.tsv`: my key, one row for each code
- `key_check.tsv`: each code's value beside the published key, where the check graded it
