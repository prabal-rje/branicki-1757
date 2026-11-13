# DECODE records 5464 and 5465, second read: what supports the read, and what does not

Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597, DECODE records 5464 and 5465. Two letters. Record 5464 has two pages. Record 5465 has three pages in DECODE's count; its second image shows two of them, which we transcribe as two faces. Italian, in cipher.

**This is a partial read from the ciphertext alone, not checked against a key. Twins of this size read .94 of the shown letters right (twin).** No key sheet and no clear text checks it. Nobody has checked a decoded word against the ink.

Words on this page:

- A **sign token** is one written sign of the cipher text, as our transcription gives it. A **label** (for example `G023`) names one sign shape.
- A **shown letter** is a letter that the decode shows under the display rule of section 5. A shown letter is not a letter read.
- A **twin** is an artificial letter: real Italian, enciphered with a key of the same shape, then read by a simulated sign reader. On a twin we know the true letters, so we can count how many shown letters are right.
- Each number says "(real)" when it comes from the records, and "(twin)" when it comes from twins.

This is our second read of records 5464 and 5465.

- **It reads the two records as one text with one key.** Section 4 gives the test that joined them.
- The earlier reads, in `../r5464/` and `../r5465/`, read each record alone with its own key, on another transcription.
- Section 8 puts the reads side by side.

## 1. In short

| Measure | Record 5464 | Record 5465 | Both |
| --- | ---: | ---: | ---: |
| Sign tokens decoded (real) | 3,156 | 5,535 | 8,691 |
| Rows (real) | 83, on two pages | 145, on two images (three faces) | 228 |
| Sign tokens that show a letter (real) | .934 | .947 | .942 |
| The key letter equals the shown letter (real) | .971 | .962 | .965 |

| Measure | Value |
| --- | --- |
| Labels | 165, of which 149 are firm (real) |
| Fresh starts that end on the best hill | 66 of 100 (real) |
| Twins of this size: shown letters right | .929 to .948, mean .94 (twin, five twins at our declared reader noise) |
| The same steps on a pair-keeping shuffle | 15 of 100 starts on the best hill; .530 of tokens show a letter (real tokens, shuffled; section 7) |
| Held-out page (record 5464, page 2) | .637 of its tokens show a letter, and .976 of those agree with the full read (real) |
| The one-key test | one statistic of two says "same key"; the other cannot judge (section 4) |
| The cross-check on the other transcription, by page | record 5464: page 1 .948, page 2 .964; record 5465: page 1 .891; record 5465's page 2 cannot be aligned (real; section 8) |
| The earlier reads' decodes, by page | record 5464: page 1 .962, page 2 .967; record 5465: page 1 .933 (real; section 8) |
| Two blind readers | each record reads as sentences by the declared rule; shares about 70% to 75% of the shown letters (real; section 9) |

**The shown share proves nothing by itself.** The shuffle still shows a letter on .530 of its tokens (real tokens, shuffled).

- **The starts carry the read:** 66 of 100 starts end on the best hill, against 15 of 100 for the shuffle (real).
- The twins, the held-out page, the stretches that read and the blind readers support it.

## 2. The signs: our transcription

- The signs are our own machine transcription of the DECODE images, not verified. It is not in this repository, because DECODE marks the ciphertext of these letters as private. We share it with DECODE and with the archive on request.
- A label is a name for a sign shape. It is not a letter. No image and no crop of an image is in this repository.
- We transcribe the second page of record 5465 as two faces, left and right. Record 5465 also has margin, interlinear and cancelled rows. Each such row is its own text in the read; `decryption.txt` marks its kind.
- The labels are joined across the nine records of the box, so one label names the same shape on every page.
- **Checks of the transcription.** One machine reader read each page. A second model checked some places on page 1 of each record only. On the three faces with no such check, it read some sample rows again, blind:
  - record 5464, page 2: 199 of 275 signs agree (.72, real);
  - record 5465, page 2 left: 81 of 175 signs agree (.46, real);
  - record 5465, page 2 right: 103 of 140 signs agree (.74, real).
- **A hidden test** on two other pages of the box gave the same sign to .70 of the labels that their halves share (real). So our labels have errors: some signs are split or joined wrongly.
- **Marks.** A token with two options (for example `G009|G023`) is read as its first option. A token that ends in `?` is doubtful; we read it as its sign. Joined ink (`[...~...]`), an unclassed sign (`[?]`), a gap (`[gap]`), clear text (`[cleartext]`) and the edges of struck signs (`<del>`, `</del>`) break the text. Record 5464 has 6 breaks and record 5465 has 46 (real).

## 3. How we found the key

- **The letter model:** an order-4 letter model of the printed dispatches of the Milanese ambassadors of the 1460s and 1470s (Mandrot; Gingins-La Sarra), five volumes, 1.32 million letters.
- **The starts:** 100 fresh starts on the two records together, each annealed for 600,000 moves on the letter model: 10 keys from the sign counts and 90 random keys.
- **No key from outside.** No start used an older key, the earlier reads' keys, the ledger's key or a key sheet.
- **The hills.** A start is on the best hill when its key gives the same letter as the best key on at least .9 of the tokens. 66 of the 100 starts end on the best hill (real). The other 34 starts form 32 small hills of 1 or 2 starts (real).
- **Firm labels.** A label is firm when at least 18 of the 20 best keys give it the best key's letter. 149 of the 165 labels are firm (real).
- **Two options.** On two twins, before the real read, the first option and a mixture of both options gave the same error within .005, so the read uses the first option.
- **A disclosure.** Before this read was frozen, we saw about 20 lines of our earlier read of record 5464: its twin numbers and one line with place names. Every rule and setting of this read was fixed before that, and no choice followed it.

## 4. One key for two records: the test, and its limits

**What it said.** A declared test said that records 5464 and 5465 share a key. One of its two statistics said "same key"; the other could not judge. **"Same key" means that our tests cannot tell these two records from one key at this size.** A key with a few changed values can pass. So the two records share most of a key at least. Whether they share all of it is open.

**Why there was a test.** An earlier screen of the five faces gave mixed signs.

- A test of sign counts said "different key" on five of the six face pairs across the two records.
- Three other tests said "same key", and the keys of single faces agreed on .84 to .94 of their shared signs (real).
- The stock floors of those earlier tests were declared after a first look at real values. A floor can turn "cannot judge" into "same key".

So we declared one test, with its twins and its rule, before any value of it, and ran it on the real records once.

**The twins of the test.** Twelve twin pairs at the sizes of the two records:

- six with one key, where each record's writer uses the homophones with its own habits (three habit strengths, two twins each);
- six with two keys from one sign stock.

| Statistic | Real value | One key (twin) | Two keys (twin) | Word |
| --- | ---: | --- | --- | --- |
| Cross-decode word cover: each record decoded with the other record's key, no refit (0 = a shuffle, 1 = its own key) | .536 | .504 to .921 | −.071 to .073 | same key |
| Held-out fit: one pooled key against two keys (nats a token) | −.313 | −.278 to −.063 | −.559 to −.399 | cannot judge |

- The real cover value lies in the one-key range, near its low end (.504), and far from the two-key range.
- The two directions differ: record 5464's key on record 5465 gives .367, and record 5465's key on record 5464 gives .704 (real). The value .536 is their mean.
- The real fit value lies between the two ranges, so that statistic gives no word.
- Judged against the other twins, no twin of either kind got the wrong word on either statistic (twin).
- The rule: one "same key" and no "different key" gives "same key".

**A check after the read.** Record 5465's own key, with no new fit, decodes record 5464. 2,223 of record 5464's 3,156 tokens have a sign that this key knows (real). The decode agrees with this read's best letters on .860, and on .885 where this read shows a letter (real).

**What this changes.** The earlier reads gave each record its own key. This read joins them. If the two records do not share a key, this read is wrong where their keys differ.

## 5. The decode, the display rule and the key

- **The fitted table.** From each distinct key of the best hill (5 keys here), an EM fit gives a table of P(sign | letter), with nulls and missed letters. The read uses the table that fits best. The fitted null rate is .005 (real), and the miss rate is .03 (a fixed setting). `channel.tsv` gives that table, one row for each label and each letter (or the null):
  - `weight`: the fitted P(sign | letter). For each letter, the full table's weights sum to 1 over all labels of the box, before the filter and the rounding. A label's weights do not sum to 1.
  - `share_of_label`: the decode's mean probability of that letter over the label's tokens. For each label, these shares sum to 1.
  - A row is kept when either value is .01 or more. The table is our own fit output; it holds no DECODE material.
- **The decode** takes the most probable letter at each sign token, under the table and the order-4 letter model. So one label can take other letters in context.
- **The key and the decode.** `key.tsv` gives each label with its key letter, its token count, the letter that the fitted table gives it most (`table_letter`), its shown tokens (`shown`) and the share of those that take the key letter (`shown_as_key`). The key letter equals the shown letter on 7,901 of the 8,186 shown letters: **.965 (real)**. For 46 of the 165 labels, the fitted table's main letter differs from the key letter (real). So `key.tsv` alone does not give `decryption.txt`.
- **The display rule.** A token shows its letter only when all three tests pass:
  - its label is firm;
  - the decodes from the 5 distinct keys of the best hill agree on it;
  - the decode's probability for that letter is at least .7.
- The table's form and the value .7 were chosen before any real result, on twins.
- The decode takes 10 tokens as nulls (real). They show as `·`, like every token with no shown letter.
- **An exact rebuild** of `decryption.txt` needs the letter model and our code. We do not publish them here. We reran our own read stage from the saved starts, and it gave the same decode on every token.

## 6. Twins of this size

Each twin is real Italian, enciphered and then read by a simulated sign reader.

- **The text:** a printed Milanese dispatch, from a volume that the letter model of the twins leaves out (the twins' letter model uses the other four volumes).
- **The key:** its shape (the number of signs for each letter, signs for words, doubled letters and nulls) comes from one key sheet of the same box, cartella 1597 no. 14. That choice dates from 7 November 2026, before we adopted the rule of reading from the ciphertext alone. We read no key sheet for this read.
- **The reader:** it clusters the signs of each face and joins them across pages, with errors. Three reader settings each give about the same disagreement as the hidden test of section 2. We declared five twins at one setting, and one twin at each of the two others.
- **The size:** the five real faces, at their token counts and row lengths.
- **Right:** a shown letter counts as right only when the true sign is that single letter. A word sign, a null or a damaged sign counts as wrong.

| Twin | Reader setting | Starts on the best hill (twin) | Share shown (twin) | Shown letters right (twin) |
| --- | --- | ---: | ---: | ---: |
| 1 | declared | 69 of 100 | .862 | .941 |
| 2 | declared | 74 of 100 | .864 | .944 |
| 3 | declared | 67 of 100 | .844 | .929 |
| 4 | declared | 64 of 100 | .868 | .948 |
| 5 | declared | 61 of 100 | .848 | .939 |
| 6 | cleaner | 61 of 100 | .901 | .958 |
| 7 | noisier | 68 of 100 | .808 | .931 |
| Records 5464 and 5465 | unknown | 66 of 100 (real) | .942 (real) | not measured |

- The label ".94" is the mean of the five declared twins.
- The real records have 66 of 100 starts on the best hill. The twins at the declared setting have 61 to 74 (twin).
- The real records show a larger share than any twin (.942 real, against .808 to .901 twin). We do not know why. One possible cause: the real transcription has fewer and cleaner labels than the twins' simulated reader. A larger shown share does not mean more right letters.
- These twins have one key for both records. They do not measure the error that two keys would give.
- **Limits of the twins.** Every twin has one writer, while these records may have two writers of one key. Its key shape comes from one key sheet of the same box. On tests of sameness, the halves of the real pages look more alike than the halves of the twins, so the twins may not copy our transcription well.
- Two more twins, with a noisier reader, have the size of the ledger maintainer's transcription of record 5464 (3,249 tokens). They are not twins of this read. Section 8 gives them.
- We do not know which reader setting fits the real transcription.

## 7. Controls

- **The pair-keeping shuffle.** This control shuffles the tokens of the two records. It keeps the pair counts of the joined text: all runs joined into one stream. Run ends are .0077 of those pairs (real), so at most that share of pairs moves across a run end. The shuffle goes through the same steps. 15 of 100 starts end on its best hill, and .530 of its tokens show a letter (real tokens, shuffled).
- **The held-out page.** We ran the read again without record 5464's page 2 (1,228 tokens), the smallest page. Its fitted table, frozen, then decoded that page. On that page (real):
  - by the display rule, .637 of its tokens show a letter, and .976 of those agree with the full read;
  - over all its tokens, the best letters agree with the full read's best letters on .726.
- So a key that never saw this page reads much of it the same way. The held-out run still saw record 5464's page 1 and all of record 5465.
- **The text check.** After the read, we looked for the longest stretch of the best-letter decode that occurs in the letter model's text, page by page (real):
  - record 5464, page 1: 24 letters, `elabonadispositionedeque`;
  - record 5464, page 2: 18 letters, `elnostrosignoredio`;
  - record 5465, page 1: 20 letters, `elprefatosignoreduca`;
  - record 5465, page 2 left: 26 letters, `llustrissimasignoriauostra`;
  - record 5465, page 2 right: 31 letters, `delaillustrissimasignoriauostra`.
- The seven twins give 13 to 54 letters by page (twin). The shuffle gives 12 to 14 letters by page (real tokens, shuffled). So this check separates the read from the shuffle, not from the twins.
- **Names.** The decode shows "Antonio da Trezo", "Pierantonio", "Iacomo dal Borgo" and "Piero Feli·e". In the letter model's text, "antoniodatrezo", "pierantonio", "iacomodalborgo" and "pierofelice" occur 0 times (real). So the letter model did not copy these names. The decode also shows "uenetia" (Venice); that text holds it 84 times.

## 8. The earlier reads and the second read, side by side

The reads use two transcriptions of the same DECODE images. We never merge them.

| | Earlier reads (`../r5464/`, `../r5465/`) | Cross-checks | Second read (this folder) |
| --- | --- | --- | --- |
| Transcription | the ledger maintainer's | the ledger maintainer's | ours |
| Records read | each alone | each alone | both together |
| Method | 50 fresh starts and 50 starts from the best fresh key | the method of this page: 100 fresh starts | the method of this page: 100 fresh starts |
| Record 5464: sign tokens (real) | 3,249 | 3,249 | 3,156 |
| Record 5464: share shown (real) | .864 | .864 | .934 |
| Record 5464: starts on the best hill (real) | 36 of 50 fresh starts | 77 of 100 | 66 of 100, both records |
| Record 5465: sign tokens (real) | 5,828 | 5,822 | 5,535 |
| Record 5465: share shown (real) | .680 | .684 | .947 |
| Record 5465: starts on the best hill (real) | 31 of 50 fresh starts | 61 of 100 | 66 of 100, both records |
| Twins: shown letters right (twin) | record 5464: .92 to .95 in three of five, .90 in one, and one wrong key. Record 5465: no twins | .877 and .877, with 2 and 78 of 100 starts on the best hill (two twins at the size of record 5464 in this transcription) | .929 to .948, mean .94 |

- **The cross-checks** are separate runs of this page's method on the ledger maintainer's transcription, one for each record. They are not the earlier reads. The cross-check of record 5465 leaves out its last row (6 signs), which may be a stamp.
- **Agreement.** We aligned each cross-check and the second read letter by letter, page by page (an edit-distance alignment of the two best-letter decodes, nulls left out). We counted the places where both show a letter (real):
  - record 5464, page 1: .948; page 2: .964; the whole record: .954 of 2,701 places;
  - record 5465, page 1: .891.
- **Record 5465, page 2: the two transcriptions cannot be aligned there.** The ledger maintainer's transcription has this page as one page; ours has it as two faces, left and right. The order of the rows on the earlier page is not known. Under the two possible orders of our faces, the agreement is .396 (left then right) and .460 (right then left) (real). The cause is open: the row layout, a transcription or a read.
- **Against the earlier reads' decodes.** We also aligned the second read with `../r5464/decryption.txt` and `../r5465/decryption.txt`, page by page. A global alignment pairs the two shown decodes letter by letter, and a `·` there matches any letter. Where both show a letter, they agree (real):
  - record 5464, page 1: .962 of 1,620 places; page 2: .967 of 1,060; the whole record: .964 of 2,680;
  - record 5465, page 1: .933 of 1,190. Page 2 is not aligned, for the reason above.
- **Two controls** use the same alignment (real). The second read with its letters shuffled gives .336 to .391. Four pairs of different pages of records 5463 to 5465 give .487 to .689. So this alignment gives about .4 to .7 for text that is not the same.
- **By eye.** The earlier read of record 5464 (`../r5464/reading.md`) shows the alliance by marriage, the league for the defence of the states with the Pope, the secret writings, the king and the return to Milan. The second read shows the same stretches. The earlier read of record 5465 read in patches only. The second read of record 5465 reads in long stretches (`reading.md`).

## 9. Two blind readers

- **The readers:** two large language models, GPT-6.1 Sol (max effort) and Grok 4.7 (xhigh effort). Each read each case once, on 12 November 2026, in a fresh session. Record 5464 and record 5465 were separate cases.
- **What they saw:** three texts in a random order, with no spaces, and no name, date, archive, key or note:
  - our decode of one record, with the agreed nulls left out and each break shown as `…`;
  - control W: the words of our decode, shuffled over the whole text, then cut into lines of the same lengths;
  - control L: our decode with the letters shuffled inside each word; the gaps keep their places.
- **The words** for the controls come from one unigram split over the vocabulary of the Milanese dispatches.
- **A calibration case:** the same test on twin 1 of section 6, in the layout of record 5465. Its shown letters there are .942 right (twin). The readers did not know that it was a twin.
- **Declared in advance.** We fixed the cases, the seeds, the prompt and the rule for a word before any reader ran.
- **The share** is each reader's own estimate of the letters that make sense. It is an estimate, not a count. Where a reader counted the gaps (`·`) too, we divide its share by the shown fraction of the text: 2,947 shown letters of 3,150 letters and gaps for record 5464 (real), and 4,771 of 5,305 for the twin (twin). So every converted share below is a share of the shown letters. The reader's own figure follows in brackets. "As given" marks a share whose basis the reader did not state.
- **One reader ran twice.** On record 5464, reader 2's first session tried to read a file outside its folder and gave no answer. So it ran a second time, as declared, and that run gave the answer below.

| Case | Our decode: Sol | Our decode: Grok | Control W: Sol / Grok | Control L: Sol / Grok | Rank by both |
| --- | --- | --- | --- | --- | --- |
| Record 5464 (real) | about 75% (70% of letters and gaps) | about 75% (70%, gaps counted as failures) | about 11% (10%) / 10% (as given) | 1% or less (under 1%) / 2% (as given, of about 3,100 letters) | our decode first |
| Record 5465 (real) | about 70%, 60 to 80 (of the shown letters) | about 70%, 60 to 80 (gaps not counted) | 25%, 15 to 35 / 30% (as given) | 2%, 0 to 5 / 8% (as given) | our decode first |
| The twin, in record 5465's layout (twin) | about 67% (60% of letters and gaps) | about 60% (as given) | about 11% (10%) / 25% (as given) | 1% or less / 1% (as given) | the twin's decode first |

- Both readers name Italian for each decode. On record 5464, reader 1 calls our decode "damaged prose", and reader 2 says: "It reads as sentences, with missing letters (·) and local damage." On record 5465, reader 1 says: "despite substantial damage, it reads as correspondence containing connected statements", and reader 2: "It does read as sentences, with gaps and some bad patches."
- **The word, by the declared rule: both records read as sentences.** For each record, both readers rank our decode first, name one language and say that it reads as sentences. The twin case gets the same word, so the rule is not too strict for these texts.
- **Against the twin.** Both readers give each record (real) a share at or above their share for the twin's decode (twin). The twin's shown letters are .942 right (twin). We do not turn a reader's share into a share of right letters.
- **Control W keeps real words.** So the gap between our decode and control W is the evidence for sentences. Reader 1: record 5464, 64 points (real); record 5465, 45 points (real); the twin, 56 points (twin). Reader 2: 65 and 40 points (real) and 35 points (twin), with its control W shares as given.
- **The quotes.** A script checked each quoted stretch against the text that the reader saw. All 28 quotes of reader 1 on the two records stand. Of the 33 quotes of reader 2, 19 stand as quoted, 2 stand when the gap marks are ignored, 3 stand only when split at the reader's own ellipses or brackets, and 9 do not stand. In those 9, the reader changed, doubled or filled in letters, for example "ambasciata" for `ambasiata` and "affinita" for `afini`. Reader 2 says in one answer that it filled in some gaps.
- **The twin's quotes.** All 14 quotes of reader 1 on the twin's decode stand. Of the 13 quotes of reader 2, 6 stand as quoted, 1 stands when the gap marks are ignored, 3 stand only when split at the reader's own ellipses or brackets, and 3 do not stand.
- Reader 2 names, from our decode of record 5465, "Antonio da Trezo as ambassador of Your Highness, Naples, Pier Antonio in a place of suspicion, a protest of loyalty, a plea for pardon, and a close".
- **The earlier reads**, on the other transcription, got about 65% and about 70% (record 5464) and about 55% and about 55% (record 5465) from the same two models (`../r5464/check.md`, `../r5465/check.md`).

## 10. What does not support the read

- No key sheet and no clear text. Nobody has checked a decoded word against the ink.
- The transcription is a machine reading, not verified. On record 5465's page 2 left, a blind second reading of sample rows agreed on only .46 of the signs (real).
- The read joins two records under one key. The test could not tell them from one key at this size, but one of its two statistics gave no word, and its two directions differ (.367 and .704, real). An earlier count test said "different key" on five of six face pairs.
- On record 5465's page 2, the two transcriptions cannot be aligned: .396 or .460 (real). The cause is open.
- The twins have one writer and one key for both records, and they take their key shape from one key sheet of the same box. The real pages look more alike than the twins do.
- The real records show a larger share than any twin, and we do not know why.
- The text check does not separate the read from the twins.
- The display rule alone does not catch a wrong key. In the tests of the earlier read of record 5464, one twin at that read's size (3,249 tokens) ended on a wrong key and still showed 38% of its signs (twin).
- The blind readers give estimates, not counts. They are language models, not historians.
- The letter model can write a word or a phrase that is common in the dispatches, such as "illustrissima signoria vostra". So a single word proves little. Repeated words, names and long stretches are stronger.
- The readings in `reading.md` are ours. They supply letters and mark doubts.

## 11. The files

- `reading.md`: the stretches that read, with an English translation, for each record.
- `decryption.txt`: our decode, row by row, one character for each token of our transcription.
- `key.tsv`: our key, one row for each label.
- `channel.tsv`: the fitted table.
- `check.md`: this page.
- `decryption.txt` has a short header with its source. `key.tsv` and `channel.tsv` have no header of their own. This page gives their source and credits.

## 12. Credits

- **DECODE**, the database of historical ciphers of the DECRYPT project: records 5464 and 5465. The documents are in the Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597. DECODE's images are for research use only. No DECODE image is in this repository.
- **The cipher ledger's maintainer** (https://github.com/dbourdeau/cyphersolver) made the transcription that the earlier reads and the cross-checks of section 8 use.
- **His partial reading of record 5464**, of 7 November 2026, gave, for example, "sempre desiderat amici" and "facto stamatina tornare". He also tested record 5465; on 12 November 2026, his ledger listed signals and fragments of Latin and Italian.
