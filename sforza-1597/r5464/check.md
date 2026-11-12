# DECODE record 5464: what supports the read, and what does not

Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597, DECODE record 5464. Two pages. Italian, in cipher.

**This is a partial read from the ciphertext alone.** No key sheet and no clear text checks it. The signs are a machine transcription of the images.

A sign is one written sign of the cipher text. A sign class is one label of the transcription, from `s00` to `s59`. Several sign classes can stand for one letter.

## 1. In short

| Measure | Value |
| --- | --- |
| Signs decoded | 3,249, in 83 lines on two pages; 60 sign classes |
| Signs that show a letter | 86.4% (2,808 of 3,249) |
| Shown letters that make sense, by two blind readers | about 65% and about 70% |
| The same, as a share of all signs | 56% to 61% |
| Fresh starts that end on the main key | 36 of 50 |
| Artificial letters of this size: shown letters right | 92% to 95% in three tests; 90% and 0% in two tests at twice the noise |
| Our key and the ledger's key give the same letter | 86.6% of the signs (2,815 of 3,249) |

## 2. The signs

- The cipher ledger's sign reader made the transcription from the DECODE images. We cannot see the images.
- The file is `targets/sforza1597/ctts/r5464_best/tokens.txt` in https://github.com/dbourdeau/cyphersolver. We do not copy it.
- We decode 3,249 signs. We leave out line 50 of that file (30 signs). A hand review marks it as the archive stamp.
- The ledger estimates about 10% errors in the transcription of this record: signs merged, split or missed.

## 3. How we found the key

- **The letter model:** the printed dispatches of the Milanese ambassadors of the 1460s and 1470s (Mandrot; Gingins-La Sarra), five volumes, 1.32 million letters.
- **The starts:** 100 starts, each annealed for 600,000 moves on the letter model.
  - 50 fresh starts: 5 keys from the sign counts and 45 random keys.
  - 50 starts from the best fresh key, with 15% of the sign classes given random letters.
- **The result:** 36 of the 50 fresh starts end on one key, and all 36 give exactly the same key. In all, 86 of the 100 starts end on it. This is the main key.
- **No key from outside.** No start used the ledger's key or a key sheet.
- **Firm signs:** the 20 best keys give every sign class the same letter. So all 60 classes are firm.

`key.tsv` gives the key. Its columns:

- `sign`: the sign class;
- `letter`: the letter of the main key;
- `firm`: whether the 20 best keys agree on that letter;
- `tokens`: the number of signs of that class;
- `decoded_as` and `share`: the value that the decode gives the class most often, and the share of its signs with that value. `null` means a sign with no letter.

## 4. The decode and the display rule

- A table of P(sign | letter), with nulls and missed letters, is fitted by EM from the main key. The decode takes the most probable letter at each sign, under a letter model of order 4.
- So the decode can give one sign class different letters in different places. The fitted table changes the main letter of 9 classes. `key.tsv` alone does not give `decryption.txt`.
- **The display rule.** A sign shows its letter only when all three tests pass:
  - its sign class is firm;
  - the decodes from the distinct keys of the main hill agree on it (here the main hill has one key, so this test removes nothing);
  - the decode's probability for that letter is at least 0.7.
- We chose the table's form and the value 0.7 on two artificial letters of the size of records 5425 to 5430. We chose them before any result on a real letter.
- The decode takes 88 signs as nulls. They show as `·`, like every sign with no shown letter.

## 5. Artificial letters of this size

Each artificial letter is real Italian, enciphered and then read by a simulated sign reader.

- **The text:** a printed Milanese dispatch, from a volume that the letter model of these tests leaves out.
- **The key:** shaped like a key of 1446 in the same box: several signs for common letters, signs for words and names, and nulls.
- **The reader:** it misses, adds, splits and joins signs. At the lower noise, it misses about 3% of the signs and adds about 3% false signs. At twice the noise, it misses and adds about 6%.
- **The size:** two pages of 2,001 and 1,248 signs, 60 sign classes, as in this record.
- **Right:** a shown letter counts as right only when the true sign is that single letter. A word sign, a null or a damaged sign counts as wrong.

| Test | Noise | Fresh starts on the main key | Signs that show a letter | Shown letters right |
| --- | --- | ---: | ---: | ---: |
| 1 | lower | 27 of 50 | 78.9% | 94.7% |
| 2 | lower | 38 of 50 | 82.2% | 92.3% |
| 3 | lower | 33 of 50 | 78.6% | 92.8% |
| 4 | twice | 33 of 50 | 71.0% | 89.9% |
| 5 | twice | 2 of 50 | 37.8% | 0.3% (a wrong key) |
| Record 5464 | unknown | 36 of 50 | 86.4% | not measured |

- The display rule alone does not catch a wrong key. Test 5 still shows 38% of its signs.
- In these tests, the fresh starts separate test 5 from the others: 2 on the main key, against 27 to 38. Record 5464 has 36. This is one failure only, so it is not a proven test.
- We do not know which noise fits the real transcription.

## 6. The pair-keeping shuffle

We ran this control on records 5425 to 5430, not on this record. It shuffles the signs and keeps the count of each pair of neighbouring signs.

- No fresh start of 50 ended on a main key.
- The display rule still showed a letter on 28% of the signs.
- So a high share of shown letters does not show by itself that there is a text.

## 7. Two blind readers

- **The readers:** two large language models, GPT-6.1 Sol (max effort) and Grok 4.7 (xhigh effort). Each read once, on 12 November 2026.
- **What they saw:** three texts in a random order, with no spaces, and no name, date, archive, key or note.
  - Our decode, with the 88 nulls left out.
  - Control W: the words of our decode, shuffled over the whole text, then cut into lines of the same lengths.
  - Control L: our decode with the letters shuffled inside each word. The gaps keep their places.
- **The words** for the controls come from one unigram split over the vocabulary of the Milanese dispatches.
- **The share** is each reader's own estimate of the shown letters that make sense. It is an estimate, not a count.

| Text | Reader 1 (Sol): share | Reader 2 (Grok): share | Rank by both |
| --- | ---: | ---: | --- |
| Our decode | about 65% | about 70% | first |
| Control W | about 10% | about 15% | second |
| Control L | 1% or less | about 3% | third |

- As a share of all 3,249 signs, the first line is 56% to 61%.
- Control W keeps real words. So the gap between our decode and control W, about 55 points, is the evidence for sentences.
- Reader 1: "Substantial stretches read as connected prose, although some words and transitions remain damaged." Reader 2: "It reads as clauses of one diplomatic letter, with gaps."

## 8. A comparison with the ledger's decode

The ledger's maintainer read this record in part first. We compared his refined decode with ours by one measure. **The measure is ours, not his.**

- **His decode:** `targets/sforza1597/ctts/r5464_best/text_refined.txt`, from our copy of his repository of 7 November 2026. It gives a letter on every sign. We fold it to our 21 letters and leave out line 50.
- **The words:** one unigram split, line by line, over the vocabulary of the Milanese dispatches. A gap ends a word.
- **The share:** letters inside vocabulary words of 4 letters or more, and of 5 letters or more, as a share of all 3,249 signs.

| Decode | Signs with a letter | In words of 4 letters or more | In words of 5 letters or more |
| --- | ---: | ---: | ---: |
| His refined decode | 100% | 44.8% | 28.7% |
| His decode, letters shuffled over the text (mean of 20) | 100% | 10.5% | 2.1% |
| Our decode, a letter on every sign (before the display rule) | 95.2% | 49.7% | 36.5% |
| Our decode as in `decryption.txt` | 86.4% | 43.9% | 32.0% |
| The same, words shuffled over the text (mean of 20) | 86.4% | 42.6% | 29.7% |
| The same, letters shuffled over the text (mean of 20) | 86.4% | 5.5% | 0.9% |

- **The floor** is the letter shuffle. A word shuffle keeps the words, so it stays near the real decode. This measure counts words. It does not see sentences.
- **The measure favours our decode.** Our letter model and this vocabulary come from the same dispatches. His decode used his own period Italian text.
- **His own count**, by his own method, is 27% of the letters in words of four letters or more.
- **The keys.** His decode gives one letter to each sign class. Our main key gives the same letter as his on 2,815 of the 3,249 signs (86.6%), and on 46 of the 60 sign classes.

## 9. What does not support the read

- No key sheet and no clear text. Nobody has checked a decoded word against the ink.
- The transcription is a machine reading, with about 10% errors by the ledger's estimate.
- One artificial letter of this size ended on a wrong key, and the display rule did not catch it.
- No shuffle control ran on this record itself.
- The blind readers give estimates, not counts. They are language models, not historians.
- The letter model can write a word that is common in the dispatches. So a single word proves little. Repeated words and long stretches are stronger.
- The readings in `reading.md` are ours. They supply letters and mark doubts.

## 10. Credits

- **DECODE**, the database of historical ciphers of the DECRYPT project: record 5464. The document is in the Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597.
- **The sign transcription** is the work of the cipher ledger's maintainer (https://github.com/dbourdeau/cyphersolver, `targets/sforza1597/ctts/r5464_best/tokens.txt`). A reader needs that file to follow our decode sign by sign.
- **His earlier partial reading** of 7 November 2026: by his count, 27% of the letters fall in words of four letters or more. His key found the main letters first. Our key gives the same letter as his on 87% of the signs.
