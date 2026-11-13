# DECODE records 5425 to 5430: what supports the read, and what does not

Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597, DECODE records 5425 to 5430. Six letters, which we read together with one key. Italian, in cipher.

**A partial read from the ciphertext alone, not checked against a key; twins of this size read .95 of the shown letters right (twin).** No key sheet and no clear text checks this read.

The signs are our own machine transcription of the DECODE images, not verified. Nobody has checked a decoded word against the ink.

**Words.**

- A sign is one written sign of the cipher text.
- A sign label is one label of our transcription, from `G001` to `G329`. Several labels can stand for one letter.
- A shown letter is not a letter read.
- A twin is an artificial letter. We encipher real Italian text, read it back with a simulated sign reader, and solve it with the same method. Then we can count how many shown letters are right.
- Each number says "real" (from the six records) or "twin" (from the twins).

## 1. In short

| Measure | Value |
| --- | --- |
| Signs decoded | 14,888 on six pages, in 189 rows; 124 sign labels (real) |
| Signs that show a letter | 87.1%, 12,963 of 14,888 (real) |
| Twins of this size: shown letters right | 94.1% to 95.4% in five twins at the main setting; 91.2% to 95.5% in all nine twins (twin) |
| Fresh starts that end on the best hill | 52 of 100 (real); 53 to 67 of 100 in the twins (twin) |
| The same steps on a pair-keeping shuffle | 11 of 100 starts on its best hill; 29.9% of its signs show a letter (real signs, shuffled) |
| A page held out of the fit | 69.5% of its 1,221 signs show a letter; 96.9% of those agree with the full read (real) |
| The ledger maintainer's transcription, read alone (his work; section 10) | 62.5% of its signs show a letter; where both reads show a letter, 88.3% of 7,507 aligned places agree (real) |
| Two blind readers | both read each record as Italian sentences; by their own estimates, 40% to 69% of its letters make sense (real), and 55% to 70% on a twin page with 95.0% right (twin); section 11 gives the bases |

**The shown share is no evidence by itself.** The evidence is the hill, the shuffle, the held-out page, the second transcription and the blind readers. Each has limits, and section 12 lists them.

## 2. The signs

- Our transcription is our own machine reading of the DECODE images. It is not verified.
- It gives each page its own labels. We joined the labels of the pages into one set, `G001` to `G329`.
- Where our transcription gives two options for a sign, the read uses the first option. This holds for 782 of the 14,888 signs, 5.3% (real). A test on twins chose this rule before the decode. The annealing of the real starts had begun before that choice, but it uses the first option under either rule.
- Where our transcription has a gap, joined ink or clear text, there is no sign. The decode breaks there. `decryption.txt` shows no mark at these places.
- Pages 2 of records 5425 and 5426 hold no cipher. Each other record has one page.
- **Our label transcription is not in this repository.** DECODE marks the ciphertext of these letters as private. We share it with DECODE and with the archive on request. In it, a label with two options is written `G016|G046`, and the read uses the first.
- Each row of `decryption.txt` has one character for each label of the same row of our transcription. We checked this with a script.
- A label is a name. No image and no image crop is in this repository.

## 3. Which pages share a key

- Before the read, we tested each pair of pages: the sign counts, the neighbours of signs, and two tests with our solver.
- We read the six letters as one text, because our tests cannot tell their pages from one key at this size. A key with a few changed values can pass.
- For two pairs, record 5425 with 5426 and record 5426 with 5427, the tests could not judge.
- Each test counts only when the two pages share enough of their signs (a floor). We declared these floors after a first look at real values. A floor can make a word more careful, but it can also turn "cannot judge" into "same key".

## 4. How we found the key

The method is the one of records 5463 to 5465, with fresh starts only. We declared the settings and seeds before the read, with two exceptions: the floors of the key tests (section 3) and the timing of the two-option rule (section 2).

- **The letter model:** the printed dispatches of the Milanese ambassadors of the 1460s and 1470s (Mandrot; Gingins-La Sarra), five volumes, 1.32 million letters.
- **The starts:** 100 fresh starts, each annealed for 600,000 moves on the letter model: 10 keys from the sign counts and 90 random keys.
- **No key from outside.** No start used an older key, the ledger's key or a key sheet.

| Measure | Value (real) |
| --- | ---: |
| Starts | 100 |
| Starts on the best hill | 52 |
| Hills | 49 |
| Starts on the next five hills | 1 each |
| Distinct keys of the best hill used for the decode | 5 |
| Signs on firm labels | 99.8% |

- A start is on a hill when its key gives the same letter as the hill's best key on at least 90% of the signs.
- A label is firm when at least 90% of the 20 best keys give it the same letter. Three labels are not firm: `G036`, `G056` and `G079`, with 25 signs in all.
- A table of P(sign | letter), with nulls and missed letters, is fitted by EM from each distinct key of the best hill. The decode uses the key whose table fits best. `key.tsv` gives that key.
- The decode takes the most probable letter at each sign, under a letter model of order 4. So one label can get different letters in different places. `key.tsv` alone does not give `decryption.txt`.
- **What `key.tsv` gives.** Applied to our transcription, the column `letter` gives the shown letter of `decryption.txt` on 92.0% of the shown signs (11,923 of 12,963, real). The column `decoded_as` gives it on 92.9% (12,040 of 12,963, real). On the other shown signs, the decode gives the label another letter in that place.
- **The fitted table** is `channel.tsv`. It is the table that the decode uses. In it, one label can stand for more than one letter. For each label, it lists each letter, and the null, that the fit gives at least 1% of the label's signs:
  - `weight`: that share of the label's signs (real);
  - `emission`: the table's value P(sign | letter), or P(sign | null) for the null.
- The fit's null rate is 0.028 (real).
- **The letter model** of the decode is an order-4 letter model of the printed Milanese dispatches of the 1460s and 1470s (Mandrot; Gingins-La Sarra).
- An exact rebuild of `decryption.txt` needs that letter model and our code. We do not publish them here.

`key.tsv` has these columns:

- `sign`, `letter`, `firm` (`yes` when the label is firm, as defined above) and `tokens` (the number of signs with that label, first options only);
- `decoded_as` and `share`: the value that the decode gives the label most often, and the share of its signs with that value. `null` means a sign with no letter.
- `shown` and `shown_as_key`: the number of the label's signs that show a letter, and the share of them that show the key's letter. A `-` means that no sign of the label shows a letter.

## 5. The display rule

A sign shows its letter only when all three tests pass:

- its label is firm;
- the decodes from the 5 distinct keys of the best hill agree on it;
- the decode's probability for that letter is at least 0.7.

The table's form and the value 0.7 were fixed before any real result. The decode takes 75 signs as nulls (real). They show as `·`, like every sign with no shown letter.

## 6. Twins of this size

Each twin is real Italian, enciphered and then read by a simulated sign reader.

- **The text:** printed Milanese dispatches, from a volume that the letter model of the twins leaves out.
- **The size:** the six pages at their real sign counts and row lengths.
- **The key's shape:** the number of signs for each letter, the signs for words, doubled letters and nulls. The twins take this shape from one key sheet of the same box. They take only the shape; the twin's key is drawn at random. We chose this shape on 7 November, before we fixed our rule to read from the ciphertext alone. No key sheet was read for this read.
- **The reader:** it misses, adds, splits and joins signs, and it can join labels of two pages wrongly. Three settings each match a disagreement that we measured in our transcription: a page read in two halves against the same page read whole. The main setting is the middle one.
- **Right:** a shown letter counts as right only when the true sign is that single letter. A word sign, a null or a damaged sign counts as wrong.

| Twin | Reader | Starts on the best hill | Signs that show a letter | Shown letters right | Key right |
| --- | --- | ---: | ---: | ---: | ---: |
| 1 | main setting | 61 of 100 | 86.6% | 95.4% | 95.1% |
| 2 | main setting | 61 of 100 | 84.7% | 94.1% | 93.3% |
| 3 | main setting | 67 of 100 | 84.7% | 94.9% | 92.3% |
| 4 | main setting | 62 of 100 | 86.8% | 94.7% | 94.4% |
| 5 | main setting | 59 of 100 | 84.9% | 94.4% | 94.5% |
| 6 | cleaner reader, more join errors | 63 of 100 | 87.7% | 95.5% | 90.6% |
| 7 | noisier reader, no join errors | 62 of 100 | 80.5% | 93.7% | 91.1% |
| 8 | one pooled set of 70 labels, like the ledger maintainer's transcription | 53 of 100 | 72.6% | 91.8% | 90.1% |
| 9 | the same | 63 of 100 | 71.7% | 91.2% | 87.5% |
| The six records | unknown | 52 of 100 (real) | 87.1% (real) | not measured | not measured |

All values in the twin rows are twin values.

- The label ".95" is the rounded mean (.947) of the five twins at the main setting.
- **The real best hill holds fewer starts than any twin's:** 52 (real) against 53 to 67 (twin). The difference is small, but it is a difference.
- **Each twin has one writer,** and its key shape comes from one key sheet of the same box. On our key tests, the twin pages look less alike than the real pages do. So the value .95 describes these twins. It is not a measured accuracy of the real read.
- We do not know which reader fits our real transcription.

## 7. The pair-keeping shuffle

This control shuffles the signs of the six pages and goes through the same steps.

- It keeps the count of each pair of neighbouring signs in the text of all runs joined together.
- A run ends where our transcription has a gap, joined ink or clear text. Run ends are 0.92% of those pairs (real). So at most that share of pairs moves across a break, and the shuffle does not keep the pairs of each run exactly.

- 11 of 100 starts ended on its best hill (real signs, shuffled). The real read has 52 (real).
- The display rule still showed a letter on 29.9% of its signs (real signs, shuffled). The real read shows 87.1% (real).
- Its longest stretches in the letter model's text are 10 to 13 letters (real signs, shuffled; section 9).

## 8. A page held out

- We left page R5429-P (1,221 signs) out of the fit. Its table, fitted on the other five pages, then decoded it.
- **By the display rule of section 5,** that decode shows a letter on 69.5% of the page's signs (real). 96.9% of those shown letters agree with the full read (real).
- Other counts of the same decode (real): its best letter agrees with the full read on 81.2% of all signs; on 86.4% of the signs where the full read shows a letter; and 73.2% of its signs have a probability of at least 0.7.
- So the table of five pages reads most of the sixth page as the full read does, where it shows a letter.

## 9. The text check

After the read, we looked for the longest stretch of each page's decode (the best letter at each sign) in the letter model's text.

| Decode | Longest stretch in the letter model's text, by page |
| --- | --- |
| The six records (real) | 20, 20, 17, 18, 18 and 17 letters |
| Twin 1 (twin) | 29, 27, 18, 28, 19 and 22 letters |
| Twin 2 (twin) | 34, 21, 24, 26, 24 and 33 letters |
| All nine twins (twin) | 14 to 41 letters |
| The pair-keeping shuffle (real signs, shuffled) | 12, 12, 10, 13, 12 and 10 letters |

- The real stretches are "stiadibonauogliachen", "qualemandaialauostra", "andolichequandola", "hopotutointenderee", "dibonauogliaquanto" and "alaconfederatione".
- The real stretches (17 to 20 letters) lie inside the range of the twins (14 to 41 letters). The twins' decodes come from true Italian. So the real decode does not copy longer passages of the letter model's text than a decode of true Italian does.
- This check does not separate the real decode from the twins. It measures only the longest exact match. It does not exclude many short stretches or wording that the letter model favours.
- **Names.** The letter model's text names France, Burgundy and Savoy hundreds of times, and the Swiss and Bern often. So a name in the decode proves little by itself. `reading.md` gives the counts.

## 10. The two transcriptions, side by side

The cipher ledger's maintainer made his own transcription of these pages from the DECODE images, with his sign reader (https://github.com/dbourdeau/cyphersolver, `targets/sforza1597/ctts/a_best/tokens.txt`). The numbers of this section use his transcription; the credit for it is his. We read it alone with the same method, as a cross-check. We never merged the two reads.

- 13,356 signs; 63 of 100 starts on the best hill; 62.5% of its signs show a letter (all real).
- We aligned the two decodes page by page, with the nulls left out.
- Where both reads show a letter, they agree on 88.3% of 7,507 aligned places (real).
- So two transcriptions, by two sign readers, give mostly the same letters.

## 11. Two blind readers

- **The readers:** two large language models, GPT-6.1 Sol (max effort) and Grok 4.7 (xhigh effort). Each read each case once, on 12 November 2026.
- **What they saw:** for each record, three texts in a random order, with no spaces, and no name, date, archive, key or note.
  - Our decode of the record, with the signs that the decode takes as sure nulls left out.
  - Control W: the words of our decode, shuffled over the whole text, then cut into lines of the same lengths.
  - Control L: our decode with the letters shuffled inside each word. The gaps keep their places.
- **A calibration case** in the same form: one page of twin 1, at the size of record 5427. After both readers had answered, we counted its shown letters: 95.0% are right (1,805 of 1,900, twin).
- **The share** is each reader's own estimate of the letters that make sense, mostly of the shown letters. Three values have no clear base (below). It is an estimate, not a count. Where a reader gave its share over the letters and the gaps, we divide by the text's share of shown letters.
- **We declared the rule before any reader ran.** A reader "reads" a record when it names Italian, says that the decode reads as sentences, ranks the decode first, quotes at least two stretches of 12 or more letters that stand in the decode, and gives at least 0.7 times its own share for the twin.

| Text | Reader 1 (Sol): share | Reader 2 (Grok): share | Rank by both | Word |
| --- | ---: | ---: | --- | --- |
| Twin page (95.0% right, twin) | 70% | 55% | 1 | the scale |
| Record 5425 | 50% | 46% | 1 | reads |
| Record 5426 | 69% | 40% | 1 | reads |
| Record 5427 | 65% | 52% | 1 | reads |
| Record 5428 | 65% | 45% | 1 | reads |
| Record 5429 | 60% | 51% | 1 | reads |
| Record 5430 | 55% | 65% | 1 | reads |
| Control W, over all seven cases | 10% to 60% | 9% to 50% | 2 | |
| Control L, over all seven cases | 1% to 10% | 2% to 9%, and "under 5%" once | 3 | |

The record rows are real. The twin row is twin. The control rows cover the six records (real) and the twin page (twin).

**How each reader gave its share.** Each value above is the reader's own point estimate.

- Over the shown letters, as given: reader 1 on every text but record 5426; reader 2 on records 5427 (about 1,000 of 1,932 letters, "a little over half") and 5430.
- Over the letters and the gaps, converted to the shown letters: reader 1 on record 5426 (60%); reader 2 on records 5425 (40%) and 5429 (45%).
- Base not stated, used as given: reader 2 on the twin page (55%) and on record 5426 (40%). Base unclear, used as given: reader 2 on record 5428 (45%).
- Some readers gave ranges: reader 1 on record 5425, 40% to 60%; reader 1 on record 5426, about ten points either way around its 60% before the conversion; reader 1 on records 5427 and 5428, about ten points either way; reader 2 on record 5425, 30% to 50% before the conversion.
- The bar for reader 2 rests on its twin share of 55%, whose base it did not state.

- **Every record reads as sentences by the declared rule.** Both readers named Italian for every decode, and ranked it above both controls in all 14 sessions.
- **The bar of 0.7 times the twin share** is 49% for reader 1 and 38.5% for reader 2. Two values are close to it: reader 1 on record 5425 (50%) and reader 2 on record 5426 (40%). Two ranges cross a bar: reader 1 gave 40% to 60% for record 5425 (bar 49%), and reader 2 gave 30% to 50%, about 35% to 58% after the conversion (bar 38.5%). The word uses the middle value, as declared.
- **Record 5430 has the weakest words.** Reader 1: "It reads locally as clauses and phrases from prose, although I cannot read it continuously." Reader 2: "It reads as sentences in patches, broken by · and by some spans I cannot parse."
- **As a share of all signs of each page,** the values with a clear base are 40% to 60% (real). For the twin page, reader 1 gives 61% (twin). We do not convert the three values whose base is not clear.
- **The quotes.** A script checked 96 quoted parts of the decode texts. 88 stand in the decode. The other 8 are the readers' own spellings of stretches that stand close by.
- Reader 1 on record 5426: "It often reads as damaged, connected political or diplomatic prose." Reader 2 on record 5427: "Yes, over much of the text."
- Control W keeps real words, so a reader can still find many words in it. In 13 of the 14 sessions, the reader judged the order of control W as disturbed or not natural. In the other, reader 1 on record 5428 called it "mixed or badly damaged".

## 12. What does not support the read

- **No key sheet and no clear text checks it.** Nobody has checked a decoded word against the ink.
- **The transcription is a machine reading,** and nobody has verified it.
- **The twins' key shape comes from one key sheet of the same box,** and each twin has one writer. If the real key has another shape, the twins can overstate the accuracy. The value .95 describes the twins only.
- **The real best hill holds fewer starts than any twin's:** 52 (real) against 53 to 67 (twin).
- **The held-out page shows a letter on 69.5% of its signs only** (real), against 87.3% in the full read of that page (real).
- **The shuffle control is not exact.** It can move up to 0.92% of the sign pairs across a break (real).
- **One sign may be wrong in the key.** The decode often shows "li" where the sense wants "ssi". `reading.md` gives the words.
- **The letter model's text names many of the places and people that the decode shows.** So a single name proves little. Long stretches that make sense are stronger.
- **The group of six pages** rests on tests that cannot tell one key from a key with a few changed values. For two pairs of pages, the tests could not judge. We declared the floors of those tests after a first look at real values.
- **The blind readers give estimates, not counts.** They are language models, not historians.
- **The readings in `reading.md` are ours.** They supply letters and mark doubts.

## 13. Credits

- **DECODE**, the database of historical ciphers of the DECRYPT project: records R5425 to R5430. The documents are in the Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597.
- DECODE's images are for research use only. No DECODE image is in this repository.
- **The ledger maintainer's transcription** (section 10) is the work of the cipher ledger's maintainer (https://github.com/dbourdeau/cyphersolver, `targets/sforza1597/ctts/a_best/tokens.txt`). Our files do not copy it.
- These credits cover every file of this folder: `reading.md`, `decryption.txt`, `key.tsv`, `channel.tsv` and this page. Each comes from DECODE records R5425 to R5430 through our own machine transcription of the DECODE images, not verified.
