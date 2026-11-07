# AGAD 1401: a Polish letter on Stanisław's abdication, 4 February [?1736]

An unsigned letter in Polish and Latin, written among the Polish exiles in Prussia. France has told them that it can no longer keep King Stanisław Leszczyński on the Polish throne.

- **Where:** AGAD Warsaw, fonds 338, reference code 1/338/0/1/1401.
- **Scans:** https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225114
- **Ledger:** catalogue 1579 at https://github.com/dbourdeau/cyphersolver leaves this letter open. Its 1398, 1399 and 1400 are the French letters in this repo. This letter uses a different cipher.

## What it says

- France has agreed preliminary articles with Vienna, and an armistice. It says that it cannot keep [125] on the Polish throne.
- A courier, Orlik, brings this as happy news. The exiles receive it in despair.
- The exiles answer with two conditions. Europe must first recognize [125] as lawful King of Poland for life. Then [125] must call a Diet, use the royal rights there, and only then abdicate.
- A second courier leaves Versailles on 11 January. The reply says that Du Theil has gone to Vienna with these articles, and that [125] must abdicate at once.
- [125] presses for the abdication. The confederated estates refuse, and they ask for some weeks to deliberate.
- Two lords leave for Warsaw, with passports from Keyserling, the Russian envoy.
- The writer asks the addressee what the Turkish power plans.

Read it: [Polish and Latin](reading.md), [English](translation.md).

## The cipher

One number stands for one letter, with a dash between words. `key.tsv` gives all 30 letter signs. About 16 code groups stand for names and titles.

| Code group | My reading | Strength |
| --- | --- | --- |
| 125 | Stanisław Leszczyński | Strong. France cannot keep 125 on the Polish throne, and asks for an abdication. |
| 455 | Augustus III | Good. The reign of 455 is to begin after the abdication. |
| 136, 142 | Warsaw | Good, from the clear text beside them. |
| 675 | the marquis de Monti | Weak. The text calls 675 the minister named to the Confederated Estates. I have not checked this name in print. |
| 435 | the Turks | Weak. |

These stay unread: 175, 195, 613, 145, 715, 505, 4345, 156, 5455 and 289.

## How it was read

From the ciphertext alone, with no other letter, key or crib. The letter values came by hand from the numbers and the Polish.

Bespoke count matching based on Polish next-letter counts, run on this letter alone, then agrees with those values on 98.2% of letter tokens.

- **Transcription:** two passes agree on 99.1% of 2,844 tokens. Each of the 23 differences was settled on the scan.
- **Score:** the key scores -3.52 per letter under a Polish model. Three shuffled controls score -4.70 to -4.86.
- **Solver:** a solver on that model agrees with the key on 93.1% of tokens.
- **Blind read:** a reader with no context named this text as Polish with Latin, and it named three controls as noise. It translated about 85% of the clauses.

Limits of these checks:

- The Polish model comes from 19th-century and 20th-century text, and the letter has long Latin stretches. So a wrong key can outscore the true one: the solver's key scores -3.07.
- I changed the model once after a first look, because runs of one letter were winning. The margin over the controls was 1.11 before that change and 1.19 after.
- I ran no held-out half. A short solve on half the text fell into a degenerate key, which says nothing about the split.

## The date

The date line reads "D. 4. Feb:", and the year's third digit looks like 2. The contents fix 1736: the preliminaries of Vienna, and a courier sent on 11 January. That year is my inference.

## The addressee

The catalogue card says that the letter is perhaps to Branicka. The text addresses a man, and it asks what the Turkish power plans. So the card looks wrong to me. The signature is a flourish that I cannot read.

## Earlier work

As far as I checked, nobody has read this letter. That is not proof that nobody has.

**Checked:**

- The ledger's catalogue, target folders and issues, live on 7 November 2026.
- The card and scans of this letter, and the cards of 1397, 1402 and 1403. No clear copy or decipherment of this text turned up.
- A text comparison with letters 446, 1398, 1399 and 1400. They share only stray phrases.
- A keyword scan of Konopczyński 1909, and one web search on the names.

**Not checked:**

- The rest of the Branicka fonds, unit by unit.
- Other archives that hold the exiles' papers of 1736.
- Printed editions of the 1733-1736 correspondence.

## Status

The cipher parts hold 472 words. Ten code tokens stay wholly open, and about 20 more are conjectures. So more than 95% of the cipher words read as sense.

The clear parts are a working reading, not an edition. No historian has checked this reading yet.

## Files

- `reading.md`: the letter in Polish and Latin
- `translation.md`: the letter in English
- `transcription.txt`: the numbers and the clear parts, line by line
- `decryption.txt`: the decryption, line by line
- `key.tsv`: the letter key

© 2026 Prabal Gupta. First published here, 7 November 2026. Released under CC BY 4.0: reuse it, and credit me.
