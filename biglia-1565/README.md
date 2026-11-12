# Melchiorre Biglia to Rome, December 1565: a cipher letter from Vienna

**Read with my own algorithm, from the ciphertext alone, without the key.**

**The letter has been read before.** Brice Dudout transcribed it, rebuilt its key from the ciphertext and read it (L'Europe chiffrée, 29 October 2026; his site is https://bdudout.github.io/europe-chiffree/en/documents.html). No key of the time is known. I used only his transcription of the digits. His key and his reading stayed out of my read. I compared my read with his reading only after my read was fixed.

**The check, in short.** Within words, 82.2% of the aligned letter pairs agree with his reading, with gaps left out (957 of 1,164). Words paired in a random order give 29.0% on average. But my cut of the digits is wrong. The cipher has two-digit codes for syllables, and my read takes each digit as a code by itself.

- **Where:** Milan, Veneranda Biblioteca Ambrosiana, Trotti 22, the register of Melchiorre Biglia's letters. Letter 2: fol. 7r, lines 33 to 45, and fol. 7v, lines 1 to 23. Vienna to Rome, December 1565.
- **The images** are in the digital library of the Università Cattolica. I copy no image.
- **The transcription** of the digits is Brice Dudout's (L'Europe chiffrée). I took it from the copy in the cipher ledger at https://github.com/dbourdeau/cyphersolver (folder `targets/biglia1565`). I do not copy it. Each line of `decryption.txt` gives the folio and line, so that a reader can follow it on the manuscript.
- **DECODE:** no DECODE record is known to me for this letter.

## What the read says

These are my readings of the decoded text. `reading.md` gives each one with its line and an English translation. The check compared letters, not these readings one by one. So this list describes my read, not the letter.

- **The writer speaks in the first person:** "me", "trouarmi", "certifico". He uses words of devotion and affection: "afezione e deuotione" (affection and devotion), "tante amoreuoli nimostratione" (so many loving demonstrations).
- **Troops.** "milia fanti" (a thousand foot soldiers) and "[d]ue mila cauali" (two thousand horse). Also "li capi di ss[e] fanti" (the captains of these foot soldiers).
- **The king.** "uerso el re" (toward the king).
- **A person of rank.** Someone "wished to send a person of his own blood" ("persona di su[o] sangue").
- **The date.** "di ·ecembre del" (of December, of [the year]).

## The check, in short

`check.md` gives every number with its count.

| Measure | Value |
| --- | --- |
| Letters equal, word by word, of aligned letters (gaps left out) | 82.2% (957 of 1,164) |
| The same, with gaps counted as misses | 67.7% (953 of 1,407) |
| Control: each word against a word 1 to 5 places later | 27.7% to 32.4% |
| Control: words in a random order (20 seeds) | 29.0% on average |
| Words spelled exactly (gaps left out) | 42.1% (151 of 359) |
| Codes of the reading that my cut matches (same place and length) | 55.1% (702 of 1,275) |
| The same, word spaces left out | 35.8% (318 of 888) |
| Word spaces where my read and the reading agree | 376 of 379 |

## What the read gets wrong

- **The cut.** The reading has 521 two-digit syllable codes. My read takes each digit alone, so it matches none of them. When I join the letters of the two digits, they give the right syllable at 307 of the 521.
- **Words with one digit.** Three single digits also stand for whole words: 9 for "e" (and), 4 for "quel" (that) and 3 for "questo" (this). My read gives them one letter. That is right only for "e".
- **Runs of three zeros (32).** In the reading, 21 of them are a word space and then a code that starts with 0. My read takes each as a word space and then a code 0.
- **Gaps.** My read shows a letter at 81.0% of its letter codes (1,246 of 1,539). The rest are gaps.
- **The twins were too sure.** Across the artificial test letters ("twins") of the same size, 88.2% to 91.8% of the shown letters are right. The real figure is 82.2% (957 of 1,164). The twins used my own cut, so they could not show its cost.

## How it was read

From the ciphertext alone, with no key, no crib and no other cipher.

- **The input:** Dudout's transcription of the digits, 36 lines and 2,303 digits. No key, image or reading was used.
- **The form, from the digits:** `00` ends a word. Each other digit is one code. `000` is a word space and then a code 0.
- **The key:** a table in which each digit can write several letters (a soft table). Ten digits stand for 21 letters, so some digits must stand for two or more. The fitted table gives each of the 10 digits two to five letters with a share of .1 or more (`key.tsv`).
- **The letter model:** Milanese dispatches of the 1460s and 1470s, 1.3 million letters, with word spaces. Letters such as u and v are merged, which leaves 21 letters.
- **The fit:** a model in which a chain of unseen letters writes the digits. Each letter writes a digit through a table learned by EM. 100 starts; the best 40 were refined with a longer letter context.
- **The display:** a letter shows when the 5 best starts give it and the best start gives it a probability of .7 or more.
- **A control:** I ran the first stage of the fit (20 starts) on shuffled digits. It scores far lower: a log likelihood of −3,965.4, against −3,668.5 for the real digits.

## Caveats

- **The reading that I compare with is a modern reconstruction.** Dudout rebuilt the key from the ciphertext alone. His reading is 95.0% complete by sense: 313 words certain, 42 probable, 7 restored and 19 unresolved. I count the probable and restored words as true.
- **The cut of his reading into codes** is mine, by the fewest-codes rule. Some words allow two cuts.
- **Doubtful digits** in the transcription touch my read and his reading in the same way.
- **The letter model** is a century older than the letter.
- **Short words** are the least sure. A word that reads "lo" or "la" (the) stands 25 times. It may be wrong, or it may stand for a title.
- **u and v** count as one letter, and **i and j** count as one letter.
- **One count seen early.** Before the check, I saw the counts of the reference codes by class. My method and display rule were already fixed then. I saw no key value and no text of the reading.

## Words used here

- **Code:** a group of one or two digits that stands for a letter, a syllable or a word.
- **Cut:** the division of the digit stream into codes.
- **EM:** a standard method that changes a table step by step to make the text more likely.
- **Folio:** a leaf of the manuscript; 7r is the front of leaf 7, and 7v its back.
- **Log likelihood:** a score of how well a model explains the text. A larger value is a better fit.
- **Crib:** a piece of the plain text that the solver knows in advance.
- **Start:** one run of the search, from its own random key.
- **Twin:** an artificial test letter, made with a known key and read by the same method.
- **Gap:** a code with no shown letter, written `·`.

## Files

- `reading.md`: the stretches that read, with English translations
- `check.md`: the comparison with Dudout's reading
- `decryption.txt`: the full decode, line by line, with gap marks
- `key.tsv`: my key: for each digit, the letters that write it
- `key_check.tsv`: each digit beside its values in Dudout's reading
