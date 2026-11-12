# DECODE record 5463: what supports the read, and what does not

Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597, DECODE record 5463. One page. Italian, in cipher.

**This is a partial read from the ciphertext alone, not checked against a key.** No key sheet and no clear text checks it. The signs are a machine transcription of the images.

A sign is one written sign of the cipher text. A sign class is one label of the transcription, from `s00` to `s49`. Several sign classes can stand for one letter. A shown letter is not a letter read.

## 1. In short

| Measure | Value |
| --- | --- |
| Signs decoded | 1,372, in 39 lines on one page; 50 sign classes |
| Signs that show a letter | 78.0% (1,070 of 1,372) |
| Shown letters that make sense, by two blind readers | about 70% to 75%, and about 65% |
| The same, as a share of all signs | 51% to 59% |
| Signs inside vocabulary words of 4 letters or more | 36.4% |
| Fresh starts that end on the main hill | 16 of 50; a rival hill holds 17 of 50 |
| Artificial letters of this size: shown letters right | 86% to 90% in four tests; 49% in one test with a wrong key |
| The same steps on a shuffle of this record | 54.9% of its signs show a letter; 8.6% inside vocabulary words |

**The shown share is no evidence by itself.** The shuffle of this record still shows a letter on 55% of its signs. The evidence is the fresh-start count, the words and the blind readers.

## 2. The signs

- The cipher ledger's sign reader made the transcription from the DECODE images. This read did not use the images.
- The file is `targets/sforza1597/ctts/r5463_best/tokens.txt` in https://github.com/dbourdeau/cyphersolver. We do not copy it.
- We decode all 39 lines and all 1,372 signs. No hand review marks a stamp line in this record.
- The ledger's notes estimate about 10% sign errors for this family of records: signs merged, split or missed.

## 3. How we found the key

The method is the one of record 5464, unchanged. We declared every setting and seed before any fit.

- **The letter model:** the printed dispatches of the Milanese ambassadors of the 1460s and 1470s (Mandrot; Gingins-La Sarra), five volumes, 1.32 million letters.
- **The starts:** 100 starts, each annealed for 600,000 moves on the letter model.
  - 50 fresh starts: 5 keys from the sign counts and 45 random keys.
  - 50 starts from the best fresh key, with 15% of the sign classes given random letters.
- **No key from outside.** No start used the ledger's key or a key sheet.

| Starts | Number | Hills | On the main hill | On the rival hill |
| --- | ---: | ---: | ---: | ---: |
| Fresh | 50 | 11 | 16 | 17 |
| From the best fresh key | 50 | 3 | 17 | 32 |
| All | 100 | 12 | 33 | 49 |

- A start is on a hill when its key gives the same letter as the hill's best key on at least 90% of the signs.
- **The main hill** has the best score. 22 starts give exactly its best key. It holds 4 distinct keys.
- **The rival hill** scores 5.2 lower (−5,738.2 against −5,733.0). More starts end on it. Its best key gives the same letter as the main key on 81.3% of the signs, and on 35 of the 50 classes.
- **Firm signs:** the 20 best keys all give the main key. So all 50 classes are firm, and this test removes no sign.

`key.tsv` gives the best key of the main hill. Its columns are the same as for record 5464:

- `sign`, `letter`, `firm` and `tokens`;
- `decoded_as` and `share`: the value that the decode gives the class most often, and the share of its signs with that value. `null` means a sign with no letter.

## 4. The decode and the display rule

- A table of P(sign | letter), with nulls and missed letters, is fitted by EM from each distinct key of the main hill. The decode uses the key whose table fits best. That key differs from the best key on 4 classes (4.7% of the signs).
- The decode takes the most probable letter at each sign, under a letter model of order 4. So it can give one sign class different letters in different places. The fitted table changes the main letter of 9 classes. `key.tsv` alone does not give `decryption.txt`.
- **The display rule.** A sign shows its letter only when all three tests pass:
  - its sign class is firm;
  - the decodes from the 4 distinct keys of the main hill agree on it (they agree on 92.9% of the signs);
  - the decode's probability for that letter is at least 0.7.
- The table's form and the value 0.7 were chosen before any real result, on two artificial letters of the size of records 5425 to 5430.
- The decode takes 79 signs as nulls. They show as `·`, like every sign with no shown letter.

## 5. Artificial letters of this size

Each artificial letter is real Italian, enciphered and then read by a simulated sign reader.

- **The text:** a printed Milanese dispatch, from a volume that the letter model of these tests leaves out.
- **The key:** shaped like a key of 1446 in the same box. It has 2 to 5 signs for common letters, signs for words, names and doubled letters, and nulls.
- **The reader:** it misses, adds, splits and joins signs, then puts them in 50 classes. At the lower noise, it misses about 3% of the signs and adds about 3%. At twice the noise, about 6% each.
- **The size:** one run of 1,372 signs, 50 classes, as in this record.
- **Right:** a shown letter counts as right only when the true sign is that single letter. A word sign, a null or a damaged sign counts as wrong.

| Test | Noise | Fresh starts on the main hill | Signs that show a letter | Shown letters right | Signs inside vocabulary words of 4+ |
| --- | --- | ---: | ---: | ---: | ---: |
| 1 | lower | 50 of 50 | 83.6% | 86.5% | 37.1% |
| 2 | lower | 48 of 50 | 81.3% | 90.0% | 42.1% |
| 3 | lower | 11 of 50 | 78.1% | 85.6% | 33.5% |
| 4 | twice | 22 of 50 | 70.0% | 88.2% | 25.7% |
| 5 | twice | 1 of 50 | 66.2% | 48.9% (a wrong key) | 16.7% |
| Record 5463 | unknown | 16 of 50 | 78.0% | not measured | 36.4% |

- **The declared rule:** the method reads at this size when 3 or more of the 5 tests get 85% of their shown letters right. Four tests do.
- With 50 classes, the simulated reader could not reach the purity of the lower noise. Its classes are a little less pure than declared.
- **The display rule alone does not catch a wrong key.** Test 5 still shows 66% of its signs, with fewer than half of them right.
- The fresh starts separate test 5 from the others: 1 on the main hill, against 11 to 50. Record 5463 has 16. This is one failure only, so it is not a proven test.
- **Rival hills in the tests.** Tests 3 and 4 also had a rival hill within 2 of the best score. In test 3, the rival hill had the better key. Both tests still read.
- We do not know which noise fits the real transcription.

## 6. The pair-keeping shuffle of this record

This control shuffles the signs of record 5463 and keeps the count of each pair of neighbouring signs. It goes through the same steps.

- 1 fresh start of 50 ended on its best hill.
- The display rule still showed a letter on 54.9% of the signs.
- Only 8.6% of its signs fall inside vocabulary words of 4 letters or more. The real decode has 36.4%.
- So a high share of shown letters does not show by itself that there is a text. The words do.

## 7. Words

- **The measure:** one unigram split of each line over the vocabulary of the Milanese dispatches. A gap ends a word. We count the signs inside vocabulary words of 4 letters or more, and of 5 letters or more, as a share of all 1,372 signs.
- **The measure favours our decodes.** The letter model and this vocabulary come from the same dispatches.

| Decode | Signs with a letter | In words of 4+ | In words of 5+ |
| --- | ---: | ---: | ---: |
| Record 5463 | 78.0% | 36.4% | 25.0% |
| The same, words shuffled over the text (mean of 20) | 78.0% | 34.7% | 23.2% |
| The same, letters shuffled over the text (mean of 20) | 78.0% | 4.8% | 0.7% |
| The pair-keeping shuffle of the record, decoded | 54.9% | 8.6% | 3.9% |
| Artificial letters that read | 70.0% to 83.6% | 25.7% to 42.1% | 18.7% to 29.2% |
| The artificial letter with a wrong key | 66.2% | 16.7% | 10.6% |

- A word shuffle keeps the words, so it stays near the real decode. This measure counts words. It does not see sentences. The blind readers judge sentences.
- The artificial letters are cut into lines of 35 signs. Line ends split words, so their shares and the real share are close in kind, not exact matches.

## 8. Two blind readers

- **The readers:** two large language models, GPT-6.1 Sol (max effort) and Grok 4.7 (xhigh effort). Each read once, on 12 November 2026.
- **What they saw:** three texts in a random order, with no spaces, and no name, date, archive, key or note.
  - Our decode, with the 79 nulls left out.
  - Control W: the words of our decode, shuffled over the whole text, then cut into lines of the same lengths.
  - Control L: our decode with the letters shuffled inside each word. The gaps keep their places.
- **The share** is each reader's own estimate of the shown letters that make sense. It is an estimate, not a count.

| Text | Reader 1 (Sol): share | Reader 2 (Grok): share | Rank by both |
| --- | ---: | ---: | --- |
| Our decode | about 70% to 75% | about 65% | first |
| Control W | about 36% | about 30% in phrases | second |
| Control L | about 6% | about 5% | third |

- As a share of all 1,372 signs, the first line is 51% (Grok) to 59% (Sol).
- Reader 1 gave its shares over the letters and the gaps. We convert them to the 1,070 shown letters.
- **Control W keeps real words.** Reader 2 finds 60% of its letters in words that it knows, but only 30% in phrases. So the difference is in the sentences, not in the words.
- Reader 1 on our decode: "It reads as damaged prose, probably correspondence." Reader 2: "It does read as sentences, with damaged patches."
- Both readers quote the same stretches, on lines 5, 14, 20, 27 to 28 and 36 to 37.

## 9. What does not support the read

- No key sheet and no clear text. Nobody has checked a decoded word against the ink.
- The transcription is a machine reading. The ledger's notes estimate about 10% sign errors for this family.
- **The main hill is not alone.** A rival hill with 17 fresh starts scores only 5.2 lower. The two hills differ on 15 sign classes, with 256 signs. 125 of the 1,070 shown letters fall on these classes. The display rule does not test the rival hill. In one artificial letter, the rival hill held the better key.
- One artificial letter of this size ended on a wrong key, and the display rule did not catch it.
- The shuffle of this record shows a letter on 55% of its signs. So the shown share is no evidence.
- The blind readers give estimates, not counts. They are language models, not historians.
- The letter model can write a word that is common in the dispatches. So a single word proves little. Repeated words and long stretches are stronger.
- The readings in `reading.md` are ours. They supply letters and mark doubts.

## 10. Credits

- **DECODE**, the database of historical ciphers of the DECRYPT project: record 5463. The document is in the Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597.
- **The sign transcription** is the work of the cipher ledger's maintainer (https://github.com/dbourdeau/cyphersolver, `targets/sforza1597/ctts/r5463_best/tokens.txt`). A reader needs that file to follow our decode sign by sign.
- **He saw fragments of this record first.** His notes give "desideroso", "sperare" and "perche". Our read shows "desidero·o" (line 7), "spero" (line 14) and "perche" (lines 5 and 20).
