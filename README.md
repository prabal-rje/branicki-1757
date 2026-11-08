# Cipher letters read: Charles V, 1542, the Duke of Guastalla, 1717, a Polish letter of 1736, four French letters, 1756-1757, and Carranza's telegrams, 1915

Letters that the archives and the historical cipher ledger at https://github.com/dbourdeau/cyphersolver listed as unread when I read them. All were read from the ciphertext, with no key from outside.

| Letter | Date | What it says | Read it |
| --- | --- | --- | --- |
| [Charles V to Ferrante Gonzaga](https://lodovico.medialibrary.it/media/schedadl.aspx?id=c710a32c-42a7-4159-8abc-472aed58f7c9) | Monzón, 11 August 1542 | The Emperor tells his viceroy of Sicily that no help can come for the infantry, the galleys and La Goleta. Spies report that the main French effort is heading for Perpignan. | [Notes](charles-v-1542/README.md), [Spanish](charles-v-1542/reading.md), [English](charles-v-1542/translation.md) |
| [Antonio Ferdinando Gonzaga, Duke of Guastalla](https://lodovico.medialibrary.it/media/schedadl.aspx?id=848189d6-1008-497b-bcde-0e3a3ad9757f) | Guastalla, 24 September 1717 | The duke will not sign a "lettera reversale" that gives up old claims in return for imperial land. | [Notes](guastalla-1717/README.md), [Italian](guastalla-1717/reading.md), [English](guastalla-1717/translation.md) |
| [AGAD 1401](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225114) | 4 February [?1736] | Polish exiles in Prussia learn that France will not keep Stanisław Leszczyński on the Polish throne. They set conditions for his abdication. | [Notes](agad-1401/README.md), [Polish](agad-1401/reading.md), [English](agad-1401/translation.md) |
| [AGAD 446](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28224155) | Białystok, 22 March 1757 | Hetman Jan Klemens Branicki to Antoni Potocki, palatine of Bełz. Branicki plans a manifesto against an envoy's abuse of his mission. The envoy is probably Stanisław Poniatowski, later King of Poland. | [French](reading_446.md), [English](translation_446.md) |
| [AGAD 1398](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225111) | Jaswojnie, 24 July 1757 | Signed Matusevic. A field report on the Russian army under Apraxin at the frontier of Prussia: requisitions, Cossacks, and town deputies who come to submit. | [French](letters/1398/reading.md), [English](letters/1398/translation.md) |
| [AGAD 1399](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225112) | 1756, before August | An insider's report on Hetman Radziwiłł's party in Lithuania. A congress at Iwie agrees a fund of 146,000 francs to buy the coming dietines, and lists five lords' shares. | [French](letters/1399/reading.md), [English](letters/1399/translation.md) |
| [AGAD 1400](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225113) | Nieśwież, 11 September 1756 | Signed Boeven. A bloody election assembly at Brest, and a rival party spreading two hundred thousand francs across Lithuania. | [French](letters/1400/reading.md), [English](letters/1400/translation.md) |
| [Carranza's telegrams](https://www.cehm.org.mx/Buscador/FichaBasica/38647?Tipo=A) | Veracruz, May and June 1915 | Ten telegrams in the war against Villa: ammunition for Obregón, a million pesos for Pablo González, rifles to buy in New York. | [Notes](carranza-1915/README.md), [Spanish](carranza-1915/reading.md), [English](carranza-1915/translation.md) |

The ledger's catalogue numbers:

- Charles V: 1560
- Guastalla: part of 1569
- 446: 1578
- 1398 to 1401: 1579
- Carranza's telegrams: 1464

## What opened them

My bespoke count matching algorithm did the work on most of these. Each number is the share of tokens that it gets right on that text alone, with no key, crib or other letter.

| Text | Tokens right |
| --- | ---: |
| AGAD 1399 | 99.4% |
| AGAD 446 | 98.9% |
| AGAD 1400 | 98.9% |
| AGAD 1401 | 98.2% |
| AGAD 1398 | 93.1% |
| Carranza, largest set (758 tokens) | 65% to 77%, over six runs |

Charles V's letter and the Guastalla letter are the exceptions. Count matching does not read Charles V's sign-and-digit plan, so that letter needed a different bespoke fit. The Guastalla letter also came from a bespoke fit, on an Italian letter model.

## Charles V, 1542

Each base sign is a consonant, and a small digit above it adds the vowel. `charles-v-1542/README.md` gives the table, the checks and what stays open.

A bespoke fit took the plan from the letter's own sign statistics, then solved it on a Spanish letter model.

A 1906 history of Gonzaga's rule in Sicily supports the content. The letter repeats the order to pay the Count of Anguillara, and that same month the Count went over to the French with his galleys.

## Guastalla, 1717

Most letters are two-digit numbers, and a single digit can end a word with its vowel. A few numbers stand for whole words, such as 18 for "non".

A bespoke fit took the key from this letter alone, on an Italian letter model. `guastalla-1717/README.md` gives the checks and what stays open.

## AGAD 1401, 1736

One number stands for one letter, and about 14 code groups stand for names. Two groups written without dots are not code: they spell "ham" and "han", the Khan.

Bespoke count matching based on Polish next-letter counts deciphered 98.2% of letter tokens, on this letter alone. Reading the numbers against the Polish gives the same values, and settles the rare signs. `agad-1401/README.md` gives the checks and what stays open.

## The French letters, AGAD Warsaw, fonds 338

Each reference code is AGAD 1/338/0/1/ plus the letter number. One key reads all four.

Almost entirely read. Every cipher letter reads as French. A few number codes stay open, mostly names and titles.

Bespoke count matching algorithm based on the French next-letter counts (deciphered 98.9% of tokens on 446 and 1400, and 99.4% on 1399, in one shot).

### What stands out

- **An informer.** Boeven signs 1400. A 1909 history makes him Hetman Radziwiłł's secretary, in touch with the French minister in 1756 and on the French payment list. 1399 looks like his hand, and it reports on "mon maître". This is my reading.
- **The same congress in a memoir.** Matuszewicz's memoirs describe the Iwie congress of 1399, with two of the same shares and the same depositary. Their hetman's share and total differ, so the letter is a separate source.
- **Names in print.** The memoirs and the 1909 history name most people in these letters with the same titles. `letters/README.md` gives each match and its page.

### How I date them

**1400.** The date line ends with the code groups 824 811 823 818 810. Numbers 805 to 824 are number words, so this reads "mil sept cent cinquante six". The second-last group is less sure, because of a blot.

**1399.** It has no date line. It plans for the Tribunal of 1757, and for shares due next August. Matuszewicz's memoirs place the collection at Iwie in 1756.

**1398.** It gives 24 July with no year. The memoirs put Matuszewicz at Jaswojnie in July 1757, as Apraxin marched on Prussia.

### Key

A reciprocal alphabet of 12 pairs. Each pair swaps: a stands for h, and h stands for a.

a-h, b-q, c-r, d-s, e-l, f-t, g-z, i-m, k-x, n-o, p-u, w-y

## Carranza's telegrams, 1915

In the number telegrams, four runs of numbers each go through the alphabet from their own start. The letter telegrams swap thirteen pairs of letters.

Bespoke count matching based on Spanish next-letter counts opened the number telegrams. It gets 65% to 77% of tokens right on the largest set, and those readable fragments gave the plan of the key.

The key family may already be in print. I have not reached Narváez's 2019 book or 2025 article. `carranza-1915/README.md` gives the checks and what stays open.

## Files

**Charles V:** `charles-v-1542/` has the notes, the reading, the translation, the transcription and the line-by-line decryption.

**Guastalla:** `guastalla-1717/` has the notes, the reading, the translation, the transcription, the line-by-line decryption and the key.

**AGAD 1401:** `agad-1401/` has the notes, the reading, the translation, the transcription, the line-by-line decryption and the key.

**Carranza's telegrams:** `carranza-1915/` has the same files.

**The French letters:**

- `letters/numbers.md`: the number code, with the evidence for each value
- `letters/README.md`: short summaries, the outside checks and the corrections
- `letters/1398/`, `letters/1399/`, `letters/1400/`: the reading, the translation, the transcription and the line-by-line decryption of each letter
- `reading_446.md`: letter 446 in French
- `translation_446.md`: letter 446 in English
- `transcription_446.txt`: the cipher text of 446, line by line
- `decryption_446.txt`: the decryption of 446, line by line
- `clear_446.txt`: the clear parts of 446, as written
- `key.tsv`: the key

## Status

- Charles V: 240 of 246 cipher words read, 97.6%. Six stay marked, where the writer left out a letter or wrote a wrong sign.
- Guastalla: the cipher part reads as sense, apart from about ten code groups and a few doubtful passages.
- 446, 1399 and 1400 come from reconciled transcriptions. Cipher words read: 446 376 of 389, 1399 744 of 750, 1400 490 of 493.
- Pages 2 to 4 of 1398 come from a hand reread, checked against three blind passes and settled on the enlarged scan. Cipher words read: 590 of 613.
- AGAD 1401: 518 of 530 cipher words read, 97.7%. Nine code groups stay open.
- Carranza's telegrams: 96.5% of the number tokens give the reading's letter as typed. The others are mostly the clerk's slips, repaired by sense.

In the readings, `[195]` is a number group that stays unread, and `[?word]` is a doubtful reading.

No historian has checked these readings yet.

© 2026 Prabal Gupta. First published here, 7 November 2026. Released under CC BY 4.0: reuse it, and credit me.
