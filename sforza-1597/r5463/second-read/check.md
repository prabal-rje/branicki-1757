# DECODE record 5463, second read: what supports the read, and what does not

Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597, DECODE record 5463. One page. Italian, in cipher.

**This is a partial read from the ciphertext alone, not checked against a key. Twins of this size read .87 of the shown letters right (twin).** No key sheet and no clear text checks it. Nobody has checked a decoded word against the ink.

Words on this page:

- A **sign token** is one written sign of the cipher text, as our transcription gives it. A **label** (for example `G023`) names one sign shape.
- A **shown letter** is a letter that the decode shows under the display rule of section 4. A shown letter is not a letter read.
- A **twin** is an artificial letter: real Italian, enciphered with a key of the same shape, then read by a simulated sign reader. On a twin we know the true letters, so we can count how many shown letters are right.
- Each number says "(real)" when it comes from the record, and "(twin)" when it comes from twins.

This is our second read of record 5463. The earlier read, in `../check.md`, used another transcription. Section 7 puts the two side by side.

## 1. In short

| Measure | Value |
| --- | --- |
| Sign tokens decoded | 1,137 (real), in 37 rows on one page; 37 labels |
| Sign tokens that show a letter | .976, 1,110 of 1,137 (real) |
| Fresh starts that end on the best hill | 94 of 100 (real) |
| Twins of this size: shown letters right | .843 to .900, mean .87 (twin, five twins at our declared reader noise) |
| The same steps on a pair-keeping shuffle of this record | 25 of 100 starts on the best hill; .581 of tokens show a letter (real tokens, shuffled; section 6) |
| The key letter equals the shown letter | .972 of the shown letters (real) |
| The cross-check on the other transcription | the two reads agree on .920 of 984 places where both show a letter (real) |
| The earlier read's decode | the two decodes agree on .949 of 976 places where both show a letter (real; section 7) |
| Two blind readers | reads as sentences by the declared rule; shares about 87% and about 72% of the shown letters (real; section 8) |

**The shown share proves nothing by itself.** The shuffle of this record still shows a letter on .581 of its tokens (real tokens, shuffled).

- **The starts carry the read:** 94 of 100 starts end on the best hill, against 25 of 100 for the shuffle (real).
- The twins, the stretches that read and the blind readers support it.
- The text check agrees but does not confirm (section 6).

## 2. The signs: our transcription

- The signs are our own machine transcription of the DECODE images, not verified. It is not in this repository, because DECODE marks the ciphertext of these letters as private. We share it with DECODE and with the archive on request.
- A label is a name for a sign shape. It is not a letter. No image and no crop of an image is in this repository.
- One machine reader read each page. A second model checked some places only. Most of the page has no second reading.
- The labels are joined across the nine records of the box, so one label names the same shape on every page.
- **A hidden test of the transcription.** The two halves of this page went to the readers again as separate pages, with new names. The two halves share 26 labels. The joining gave 16 of them the same sign (.62, real). So our labels have errors: some signs are split or joined wrongly.
- **Marks.** A token with two options (for example `G009|G023`) is read as its first option. A token that ends in `?` is doubtful; we read it as its sign. Joined ink (`[...~...]`), an unclassed sign (`[?]`), a gap (`[gap]`) and clear text (`[cleartext]`) break the text. This page has 3 breaks, all joined ink (real).

## 3. How we found the key

- **The letter model:** an order-4 letter model of the printed dispatches of the Milanese ambassadors of the 1460s and 1470s (Mandrot; Gingins-La Sarra), five volumes, 1.32 million letters.
- **The starts:** 100 fresh starts, each annealed for 600,000 moves on the letter model: 10 keys from the sign counts and 90 random keys.
- **No key from outside.** No start used an older key, the earlier read's key, the ledger's key or a key sheet.
- **The hills.** A start is on the best hill when its key gives the same letter as the best key on at least .9 of the tokens. 94 of the 100 starts end on the best hill (real). The starts form 5 hills; the others hold 3, 1, 1 and 1 starts (real).
- **Firm labels.** A label is firm when at least 18 of the 20 best keys give it the best key's letter. All 37 labels are firm (real).
- **Two options.** On two twins, the first option and a mixture of both options gave the same error within .005, so the read uses the first option. The starts use the first option in both cases. The read stage ran after this choice.

## 4. The decode, the display rule and the key

- **The fitted table.** From the key of the best hill, an EM fit gives a table of P(sign | letter), with nulls and missed letters. The fitted null rate is .005 (real), and the miss rate is .03 (a fixed setting). `channel.tsv` gives the table, one row for each label and each letter (or the null):
  - `weight`: the fitted P(sign | letter). For each letter, the full table's weights sum to 1 over all labels of the box, before the filter and the rounding. A label's weights do not sum to 1.
  - `share_of_label`: the decode's mean probability of that letter over the label's tokens. For each label, these shares sum to 1.
  - A row is kept when either value is .01 or more. The table is our own fit output; it holds no DECODE material.
- **The decode** takes the most probable letter at each sign token, under the table and the order-4 letter model. So one label can take other letters in context.
- **The key and the decode.** `key.tsv` gives each label with its key letter, its token count, the letter that the fitted table gives it most (`table_letter`), its shown tokens (`shown`) and the share of those that take the key letter (`shown_as_key`). The key letter equals the shown letter on 1,079 of the 1,110 shown letters: **.972 (real)**. So `key.tsv` alone does not give `decryption.txt`.
- **The display rule.** A token shows its letter only when all three tests pass:
  - its label is firm;
  - the decodes from the distinct keys of the best hill agree on it (here the hill has one key, so this test removes nothing);
  - the decode's probability for that letter is at least .7.
- The table's form and the value .7 were chosen before any real result, on twins.
- The decode takes 1 token as a null (real). It shows as `·`, like every token with no shown letter.
- **An exact rebuild** of `decryption.txt` needs the letter model and our code. We do not publish them here. We reran our own read stage from the saved starts, and it gave the same decode on every token.

## 5. Twins of this size

Each twin is real Italian, enciphered and then read by a simulated sign reader.

- **The text:** a printed Milanese dispatch, from a volume that the letter model of the twins leaves out (the twins' letter model uses the other four volumes).
- **The key:** its shape (the number of signs for each letter, signs for words, doubled letters and nulls) comes from one key sheet of the same box, cartella 1597 no. 14. That choice dates from 7 November 2026, before we adopted the rule of reading from the ciphertext alone. We read no key sheet for this read.
- **The reader:** it clusters the signs of each page and joins them across pages, with errors. Three reader settings each give about the same disagreement as the hidden test of section 2. We declared five twins at one setting, and one twin at each of the two others.
- **The size:** the real page's token count and row lengths.
- **Right:** a shown letter counts as right only when the true sign is that single letter. A word sign, a null or a damaged sign counts as wrong.

| Twin | Reader setting | Starts on the best hill (twin) | Share shown (twin) | Shown letters right (twin) |
| --- | --- | ---: | ---: | ---: |
| 1 | declared | 99 of 100 | .807 | .866 |
| 2 | declared | 95 of 100 | .808 | .900 |
| 3 | declared | 78 of 100 | .789 | .884 |
| 4 | declared | 70 of 100 | .734 | .843 |
| 5 | declared | 20 of 100 | .828 | .866 |
| 6 | cleaner | 99 of 100 | .872 | .903 |
| 7 | noisier | 31 of 100 | .632 | .847 |
| Record 5463 | unknown | 94 of 100 (real) | .976 (real) | not measured |

- The label ".87" is the mean of the five declared twins.
- **Two more twins failed.** They have the size of the ledger maintainer's transcription (1,372 tokens) and a noisier simulated reader. Each had 1 of 100 starts on its best hill (twin). They showed .582 and .254 of their tokens, and .845 and .879 of those letters were right (twin).
- The real record shows a larger share than any twin of the table (.976 real, against .632 to .872 twin). We do not know why. One possible cause: the real transcription has fewer and cleaner labels than the twins' simulated reader. A larger shown share does not mean more right letters.
- The real record has 94 of 100 starts on its best hill. The twins of the table have 20 to 99 (twin).
- **Limits of the twins.** Every twin has one writer. Its key shape comes from one key sheet of the same box. On tests of sameness, the halves of the real pages look more alike than the halves of the twins, so the twins may not copy our transcription well.
- We do not know which reader setting fits the real transcription.

## 6. Controls

- **The pair-keeping shuffle.** This control shuffles the tokens of the record. It keeps the pair counts of the joined text: all runs of the page joined into one stream. Run ends are .0026 of those pairs (real), so at most that share of pairs moves across a run end. The shuffle goes through the same steps. 25 of 100 starts end on its best hill, and .581 of its tokens show a letter (real tokens, shuffled).
- **No held-out page.** The record has one page, so no page can be held out.
- **The text check.** After the read, we looked for the longest stretch of the best-letter decode that occurs in the letter model's text. For this record it is 19 letters, `perintenderepiucose` (real). The seven twins of the table give 14 to 21 letters (twin). The two failed twins give 16 and 20 letters (twin). The shuffle gives 12 letters (real tokens, shuffled). So the check agrees with the read but does not confirm it.
- **Names.** The decode shows "Zohane Antonio da Pavia" (row L33). "zohaneantonio" and "antoniodapauia" occur 0 times in the letter model's text (real). So the letter model did not copy this name.

## 7. The earlier read and the second read, side by side

The two reads use two transcriptions of the same DECODE images. We never merge them.

| | Earlier read (`../`) | Cross-check | Second read (this folder) |
| --- | --- | --- | --- |
| Transcription | the ledger maintainer's | the ledger maintainer's | ours |
| Method | 50 fresh starts and 50 starts from the best fresh key | the method of this page: 100 fresh starts | the method of this page: 100 fresh starts |
| Sign tokens (real) | 1,372 | 1,372 | 1,137 |
| Share shown (real) | .780 | .777 | .976 |
| Starts on the best hill (real) | 16 of 50 fresh starts; a rival hill held 17 | 20 of 100 | 94 of 100 |
| Twins: shown letters right (twin) | .86 to .90 in four of five; one wrong key | the two failed twins of section 5, at this size | .843 to .900, mean .87 |

- **The cross-check** is a separate run of this page's method on the ledger maintainer's transcription. It is not the earlier read.
- **Agreement.** We aligned the cross-check and the second read letter by letter (an edit-distance alignment of the two best-letter decodes, nulls left out). Where both show a letter, they agree on .920 of 984 places (real).
- **Against the earlier read's decode.** We also aligned the second read with the earlier read's `../decryption.txt`. A global alignment pairs the two shown decodes letter by letter, and a `·` there matches any letter. Where both show a letter, they agree on .949 of 976 places (real).
- **Two controls** use the same alignment (real). The second read with its letters shuffled gives .391. Four pairs of different pages of records 5463 to 5465 give .487 to .689. So this alignment gives about .4 to .7 for text that is not the same.
- **By eye.** The earlier read's reading page shows "Antonio da Pa·ia", "che spero receuere", "solum per long·· exercitatione et perientia" and "honesto modo per intendere piu". The second read shows the same stretches, with small differences.
- The second read has far more starts on its best hill (94 of 100 against 16 of 50 and 20 of 100, real).

## 8. Two blind readers

- **The readers:** two large language models, GPT-6.1 Sol (max effort) and Grok 4.7 (xhigh effort). Each read once, on 12 November 2026, in a fresh session.
- **What they saw:** three texts in a random order, with no spaces, and no name, date, archive, key or note:
  - our decode, with the agreed null left out and each break shown as `…`;
  - control W: the words of our decode, shuffled over the whole text, then cut into lines of the same lengths;
  - control L: our decode with the letters shuffled inside each word; the gaps keep their places.
- **The words** for the controls come from one unigram split over the vocabulary of the Milanese dispatches.
- **A calibration case:** the same test on a twin of records 5464 and 5465, in the layout of record 5465. Its shown letters are .942 right (twin). The readers did not know that it was a twin.
- **Declared in advance.** We fixed the cases, the seeds, the prompt and the rule for a word before any reader ran.
- **The share** is each reader's own estimate of the letters that make sense. It is an estimate, not a count. Where a reader counted the gaps (`·`) too, we divide its share by the shown fraction of the text: 1,110 shown letters of 1,136 letters and gaps (real), and 4,771 of 5,305 for the twin (twin). So every converted share below is a share of the shown letters. The reader's own figure follows in brackets. "As given" marks a share whose basis the reader did not state.

| Text | Reader 1 (Sol): share | Reader 2 (Grok): share | Rank by both |
| --- | ---: | ---: | --- |
| Our decode (real) | about 87% (85% of letters and gaps) | about 72% (70% of letters and gaps) | first |
| Control W (real, words shuffled) | about 46% (45%) | about 31% (30%) | second |
| Control L (real, letters shuffled) | about 2% (2%) | about 5% (5%) | third |
| The twin's decode, in its own case (twin) | about 67% (60% of letters and gaps) | about 60% (as given) | first |

- Both readers name Italian. Reader 1: "It reads substantially as connected sentences in a letter concerning instruction and writing in cipher." Reader 2: "It reads as sentences for most of its length."
- **The word, by the declared rule: reads as sentences.** Both readers rank our decode first, name one language and say that it reads as sentences. The twin case gets the same word, so the rule is not too strict for these texts.
- **Against the twin.** Both readers give our decode a larger share (real) than the twin's decode (twin). The twin's shown letters are .942 right (twin). We do not turn a reader's share into a share of right letters.
- **Control W keeps real words.** So the gap between our decode and control W is the evidence for sentences. It is about 41 points for each reader (real). For the twin it is about 56 points (reader 1) and 35 points (reader 2, from shares as given) (twin).
- **The quotes.** A script checked each quoted stretch against the text that the reader saw. All 13 quotes of reader 1 stand. Of the 19 quotes of reader 2, 17 stand. In the other two, the reader changed a letter: "amicitia" for `amicicia`, and "tanti" for `tenti` (across rows L11 to L12).
- **The twin's quotes.** All 14 quotes of reader 1 on the twin's decode stand. Of the 13 quotes of reader 2, 6 stand as quoted, 1 stands when the gap marks are ignored, 3 stand only when split at the reader's own ellipses or brackets, and 3 do not stand.
- Reader 1 quotes "zohane antonio da pauia" (rows L32 to L35). Reader 2 names "Messer Zohane Antonio" from row L01. Both quote the stretch on long practice and experience (L27 to L28).
- **The earlier read of this record**, on the other transcription, got about 70% to 75% and about 65% from the same two models (`../check.md`, section 8).

## 9. What does not support the read

- No key sheet and no clear text. Nobody has checked a decoded word against the ink.
- The transcription is a machine reading, not verified. A hidden test gave the same sign to only .62 of the labels that the two halves of this page share (real).
- The twins have one writer, and they take their key shape from one key sheet of the same box. The real pages look more alike than the twins do.
- Two noisier twins failed: 1 of 100 starts on the best hill (twin).
- The real page shows a larger share than any twin, and we do not know why.
- The shown share proves nothing by itself: the shuffle still shows .581 of its tokens (real tokens, shuffled).
- The text check does not confirm the read: failed twins also gave stretches of 16 and 20 letters (twin).
- The display rule alone does not catch a wrong key. In the tests of the earlier read, one twin at that read's size (1,372 tokens) ended on a wrong key and still showed 66% of its signs (twin).
- The blind readers give estimates, not counts. They are language models, not historians.
- The letter model can write a word or a phrase that is common in the dispatches. So a single word proves little. Repeated words, names and long stretches are stronger.
- The readings in `reading.md` are ours. They supply letters and mark doubts.

## 10. The files

- `reading.md`: the stretches that read, with an English translation.
- `decryption.txt`: our decode, row by row, one character for each token of our transcription.
- `key.tsv`: our key, one row for each label.
- `channel.tsv`: the fitted table.
- `check.md`: this page.
- `decryption.txt` has a short header with its source. `key.tsv` and `channel.tsv` have no header of their own. This page gives their source and credits.

## 11. Credits

- **DECODE**, the database of historical ciphers of the DECRYPT project: record 5463. The document is in the Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597. DECODE's images are for research use only. No DECODE image is in this repository.
- **The cipher ledger's maintainer** (https://github.com/dbourdeau/cyphersolver) made the transcription that the earlier read and the cross-check of section 7 use. His notes give fragments of this record: "desideroso", "sperare" and "perche".
