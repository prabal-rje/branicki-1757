# Cipher letters read: a letter to Lorenzo de' Medici, 1479, Charles V, 1542, Jean Bazin, 1573, the Duke of Guastalla, 1717, a Polish letter of 1736, five French letters, 1756-1757, and Mexican telegrams, 1911 and 1915

Letters that the archives and the historical cipher ledger at https://github.com/dbourdeau/cyphersolver listed as unread when I read them. All but one were read from the ciphertext, with no key from outside. The 1911 telegram was read with the archive's own key card.

One letter is a special case. Jean Bazin's letter of 1573 has been in print in clear since 1867. I found that print after my read, and it now checks the read.

Three more ciphers have a known key. They are the Morosini despatches of 1587 to 1589, the Francia 346 letters of 1632 to 1634 and a letter of Melchiorre Biglia of 1565. I read them without the key, as a check of my algorithm. They have their own section below.

| Letter | Date | What it says | Read it |
| --- | --- | --- | --- |
| [A letter to Lorenzo de' Medici](https://archiviodistatofirenze.cultura.gov.it/map/riproduzione/?id=79510) | Toledo, 1479; endorsed 31 August | An unnamed writer at the court of Castile reports on a league "for the defence of the states", an agreement with the queen, a marriage or betrothal, a papal legate and a tithe on the clergy. Read in part. | [Notes](medici-1479/README.md), [Italian](medici-1479/reading.md), [English](medici-1479/translation.md) |
| [Charles V to Ferrante Gonzaga](https://lodovico.medialibrary.it/media/schedadl.aspx?id=c710a32c-42a7-4159-8abc-472aed58f7c9) | Monzón, 11 August 1542 | The Emperor tells his viceroy of Sicily that no help can come for the infantry, the galleys and La Goleta. Spies report that the main French effort is heading for Perpignan. | [Notes](charles-v-1542/README.md), [Spanish](charles-v-1542/reading.md), [English](charles-v-1542/translation.md) |
| [Jean Bazin to Henri de Valois](https://gallica.bnf.fr/ark:/12148/btv1b10033937d) | Cracow, September 1573 | A French envoy reports to the king elect of Poland: a diet, money and Danzig, a truce with Muscovy, the Tartars and letters of Mahomet Bascha. 84% of the aligned letters agree with a print of 1867. | [Notes](bazin-1573/README.md), [French](bazin-1573/reading.md), [English](bazin-1573/translation.md), [Check](bazin-1573/check.md) |
| [Antonio Ferdinando Gonzaga, Duke of Guastalla](https://lodovico.medialibrary.it/media/schedadl.aspx?id=848189d6-1008-497b-bcde-0e3a3ad9757f) | Guastalla, 24 September 1717 | The duke will not sign a "lettera reversale" that gives up old claims in return for imperial land. | [Notes](guastalla-1717/README.md), [Italian](guastalla-1717/reading.md), [English](guastalla-1717/translation.md) |
| [AGAD 1401](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225114) | 4 February [?1736] | Polish exiles in Prussia learn that France will not keep Stanisław Leszczyński on the Polish throne. They set conditions for his abdication. | [Notes](agad-1401/README.md), [Polish](agad-1401/reading.md), [English](agad-1401/translation.md) |
| [AGAD 446](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28224155) | Białystok, 22 March 1757 | Hetman Jan Klemens Branicki to Antoni Potocki, palatine of Bełz. Branicki plans a manifesto against an envoy's abuse of his mission. The envoy is probably Stanisław Poniatowski, later King of Poland. | [French](reading_446.md), [English](translation_446.md) |
| [AGAD 1398](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225111) | Jaswojnie, 24 July 1757 | Signed Matusewic. A field report on the Russian army under Apraxin at the frontier of Prussia: requisitions, Cossacks, and town deputies who come to submit. | [French](letters/1398/reading.md), [English](letters/1398/translation.md) |
| [AGAD 1399](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225112) | 1756, before August | An insider's report on Hetman Radziwiłł's party in Lithuania. A congress at Iwie agrees a fund of 146,000 francs to buy the coming dietines, and lists five lords' shares. | [French](letters/1399/reading.md), [English](letters/1399/translation.md) |
| [AGAD 1400](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225113) | Nieśwież, 11 September 1756 | Signed Boeven. A bloody election assembly at Brest, and a rival party spreading two hundred thousand francs across Lithuania. | [French](letters/1400/reading.md), [English](letters/1400/translation.md) |
| [AGAD 131](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28223838) | Wilno, 11 July 1757 | Probably Matuszewicz. Requests for French subsidies for the Tribunal, and the Strutyński affair: a killing at the Brasław dietine, shielded by Apraksin. Read in part. | [Notes](agad-131/README.md), [Polish and French](agad-131/reading.md), [English](agad-131/translation.md) |
| [A telegram to González Garza](https://www.cehm.org.mx/) | Mexico City, 19 May 1911 | Two Maderistas pass on General Huerta's warning: a military mutiny against the addressee is feared in the capital. Read with the archive's key card. | [Notes](mexico-1911/README.md), [Spanish](mexico-1911/reading.md), [English](mexico-1911/translation.md) |
| [Carranza's telegrams](https://www.cehm.org.mx/Buscador/FichaBasica/38647?Tipo=A) | Veracruz, May and June 1915 | Ten telegrams in the war against Villa: ammunition for Obregón, a million pesos for Pablo González, rifles to buy in New York. | [Notes](carranza-1915/README.md), [Spanish](carranza-1915/reading.md), [English](carranza-1915/translation.md) |

The ledger's catalogue numbers:

- The Medici letter: 2322
- Charles V: 1560
- Bazin: 1571
- Guastalla: part of 1569
- 446: 1578
- 1398 to 1401: 1579
- AGAD 131: part of 1580
- The 1911 telegram: part of 1462
- Carranza's telegrams: 1464

## What opened them

My bespoke count matching algorithm did the work on most of these. Each number is the share of tokens that it gets right on that text alone, with no key, crib or other letter.

| Text | Tokens right |
| --- | ---: |
| AGAD 1399 | 99.4% |
| AGAD 446 | 98.9% |
| AGAD 1400 | 98.9% |
| AGAD 1401 | 98.2% |
| AGAD 131 | 97.7% |
| AGAD 1398 | 93.1% |
| Carranza, largest set (758 tokens) | 65% to 77%, over six runs |

Charles V's letter and the Guastalla letter are the exceptions. Count matching does not read Charles V's sign-and-digit plan, so that letter needed a different bespoke fit. The Guastalla letter also came from a bespoke fit, on an Italian letter model. The 1911 telegram needed no fit, because the archive keeps its key card.

Bazin's letter came from a bespoke fit on a French letter model, for a cipher with several signs for each frequent letter. It is the one text here with an outside check: 84.1% of its decoded letters that line up with the print of 1867 are equal.

## A letter to Lorenzo de' Medici, 1479

One sign stands for each letter, and code numbers and symbols stand for persons. The key came from the cipher alone, with the clear words between the cipher runs as cribs.

It is read in part, because the archive's images are small. `medici-1479/README.md` gives the checks and what stays open.

## Charles V, 1542

Each base sign is a consonant, and a small digit above it adds the vowel. `charles-v-1542/README.md` gives the table, the checks and what stays open.

A bespoke fit took the plan from the letter's own sign statistics, then solved it on a Spanish letter model.

A 1906 history of Gonzaga's rule in Sicily supports the content. The letter repeats the order to pay the Count of Anguillara, and that same month the Count went over to the French with his galleys.

## Jean Bazin, 1573

The transcription has 53 sign labels, with several for each frequent letter. The key came from this letter alone, from a fit on a French letter model.

A clear text of the letter was printed in 1867. I found it after the key was fixed. `bazin-1573/check.md` compares the two:

- of my decoded letters that line up with a printed letter, 84.1% are equal, against 47% for a wrong passage;
- my decode has three passages that the print leaves out;
- the letter reads in the page order 191, 192, 195, 196, 193, 194, 197, 198.

## Guastalla, 1717

Most letters are two-digit numbers, and a single digit can end a word with its vowel. A few numbers stand for whole words, such as 18 for "non".

A bespoke fit took the key from this letter alone, on an Italian letter model. `guastalla-1717/README.md` gives the checks and what stays open.

## AGAD 1401, 1736

One number stands for one letter, and about 14 code groups stand for names. Two groups written without dots are not code: they spell "ham" and "han", the Khan.

Bespoke count matching based on Polish next-letter counts deciphered 98.2% of letter tokens, on this letter alone. Reading the numbers against the Polish gives the same values, and settles the rare signs. `agad-1401/README.md` gives the checks and what stays open.

## The French letters, AGAD Warsaw, fonds 338

Each reference code is AGAD 1/338/0/1/ plus the letter number. One key reads all five.

446, 1398, 1399 and 1400 are almost entirely read, and 131 is read in part. Every cipher letter reads as French. A few number codes stay open, mostly names and titles.

Bespoke count matching algorithm based on the French next-letter counts (deciphered 98.9% of tokens on 446 and 1400, and 99.4% on 1399, in one shot).

### What stands out

- **An informer.** Boeven signs 1400. A 1909 history makes him Hetman Radziwiłł's secretary, in touch with the French minister in 1756 and on the French payment list. 1399 looks like his hand, and it reports on "mon maître". This is my reading.
- **The same congress in a memoir.** Matuszewicz's memoirs describe the Iwie congress of 1399, with two of the same shares and the same depositary. Their hetman's share and total differ, so the letter is a separate source.
- **Names in print.** The memoirs and the 1909 history name most people in these letters with the same titles. `letters/README.md` gives each match and its page.
- **A killing and its protector.** 131 tells the Strutyński affair, which the memoirs and the 1909 history also tell. It probably comes from Matuszewicz, like 1398. `agad-131/README.md` gives the limits of its reading.

### How I date them

**1400.** The date line ends with the code groups 824 811 823 818 810. Numbers 805 to 824 are number words, so this reads "mil sept cent cinquante six". The second-last group is less sure, because of a blot.

**1399.** It has no date line. It plans for the Tribunal of 1757, and for shares due next August. Matuszewicz's memoirs place the collection at Iwie in 1756.

**1398.** It gives 24 July with no year. The memoirs put Matuszewicz at Jaswojnie in July 1757, as Apraxin marched on Prussia.

### Key

A reciprocal alphabet of 12 pairs. Each pair swaps: a stands for h, and h stands for a.

a-h, b-q, c-r, d-s, e-l, f-t, g-z, i-m, k-x, n-o, p-u, w-y

## A telegram of 19 May 1911

The archive's own key card reads it: a shifted alphabet that counts ch, ll and ñ as letters. The same card reads a telegram of the next day. A hand of the time glossed that telegram in pencil, and all ten coded words agree. `mexico-1911/README.md` gives the checks and what stays open.

## Carranza's telegrams, 1915

In the number telegrams, four runs of numbers each go through the alphabet from their own start. The letter telegrams swap thirteen pairs of letters.

Bespoke count matching based on Spanish next-letter counts opened the number telegrams. It gets 65% to 77% of tokens right on the largest set, and those readable fragments gave the plan of the key.

The key family may already be in print. I have not reached Narváez's 2019 book or 2025 article. `carranza-1915/README.md` gives the checks and what stays open.

## Three ciphers with a known key, read as a check of my algorithm

I read these three from the ciphertext alone, without the key. Their keys are in print or online. So I checked each read afterwards against a published key or a modern reading. Each folder explains the reference and its limits. The checks show what my algorithm gets right, and where it fails.

| Cipher | Date | What it says | Read it |
| --- | --- | --- | --- |
| Morosini, 35 DECODE records between R17 and R58 (Vatican, Francia 22 and 18/3) | 1587 to 1589 | My read shows the Council of Trent, the nuncio, Guise, Navarre, Paris, Angers and Brissac, a castle and a river bridge. Where my cut matches a single-letter code, 95.1% of my letters are right (80,553 of 84,667). But my read recovers only 72.7% of all single-letter codes (80,553 of 110,821). Read in part. | [Notes](morosini-1587/README.md), [Italian and English](morosini-1587/reading.md), [Check](morosini-1587/check.md) |
| Francia 346, DECODE records R74 to R78, R5626, R5635, R5636, R5637, R5640, R5643, R5647 and R5648, with R5642, R5645, R5646, R5649, R5650 and R5651 in an appendix (Vatican) | 1632 to 1634 | My read shows Benavides, the Imperial court, Nuremberg and Regensburg, the Swedes, a universal peace, and pensions. Of the true letters that my read shows, 99.2% are right (6,953 of 7,012). But about a third of the graded shown tokens are not letter codes (3,579 of 10,591). | [Notes](francia-346-leaves/README.md), [Italian and English](francia-346-leaves/reading.md), [Check](francia-346-leaves/check.md) |
| Melchiorre Biglia to Rome (Milan, Ambrosiana, Trotti 22) | Vienna, December 1565 | My read shows words of devotion, foot soldiers and horse, and the king. Within words, 82.2% of the aligned letter pairs agree with Brice Dudout's reading, with gaps left out (957 of 1,164). | [Notes](biglia-1565/README.md), [Italian and English](biglia-1565/reading.md), [Check](biglia-1565/check.md) |

### Morosini, 1587 to 1589

Codes of one, two or three digits stand for letters, syllables and words, and some codes are nulls. A. Meister printed the key in 1906. George Lasry rebuilt it in part on DECODE in 2020.

My algorithm read all 35 records as one text, without the key. The read is partial. Where my cut matches a single-letter code of the key, 95.1% of my letters are right (80,553 of 84,667). In all, it recovers 72.7% of the single-letter codes (80,553 of 110,821).

My cut misses the three-digit letter codes, and my key reads the digit 2 as i, not a. Three of my 18 smaller test windows ended on a wrong key, and nothing flagged them. Over the window sizes, the mean recovery on the real text is 49.7% to 72.7%. On artificial test letters of the same sizes, it is 81.1% to 96.6%. `morosini-1587/check.md` gives the details.

### Francia 346, 1632 to 1634

A lone 6 is a word space, pairs 2x are nulls, and the other pairs stand for letters and syllables. Three-digit codes stand for words and names. George Lasry published the key on DECODE in 2020.

My key reads 39 of the 40 letter codes right. But it also gives letters to codes that are syllables, nulls or no code at all. It does not read the three-digit codes. `francia-346-leaves/check.md` gives the details.

### Biglia, 1565

A single digit mostly stands for a letter, and some digits have both a vowel and a consonant value. Two digits together mostly make a syllable. `00` is a word space. Brice Dudout read the letter and rebuilt its key from the ciphertext (L'Europe chiffrée, 29 October 2026).

My algorithm took each digit as a code by itself, so it misses the syllables. Even so, within words, 82.2% of the aligned letter pairs agree with Dudout's reading, with gaps left out (957 of 1,164). Words in a random order give 29.0% on average. `biglia-1565/check.md` gives the details.

DECODE's images are for research only. Biglia's images carry no reuse licence. I copy no image and no transcription. Each decryption gives the place of each line: the DECODE record, page and row or line, or for Biglia the folio and line.

## Files

**The Medici letter:** `medici-1479/` has the notes, the reading, the translation, the transcription, the line-by-line decryption, the key and the open code groups.

**Charles V:** `charles-v-1542/` has the notes, the reading, the translation, the transcription and the line-by-line decryption.

**Bazin:** `bazin-1573/` has the notes, the check against the print, the reading, the translation, the transcription, the line-by-line decryption, the key and the key check.

**Guastalla:** `guastalla-1717/` has the notes, the reading, the translation, the transcription, the line-by-line decryption and the key.

**AGAD 1401:** `agad-1401/` has the notes, the reading, the translation, the transcription, the line-by-line decryption and the key.

**AGAD 131:** `agad-131/` has the notes, the reading, the translation, the transcription, the line-by-line decryption and the key.

**The 1911 telegram:** `mexico-1911/` has the notes, the reading, the translation, the transcription, the reading of each coded word and the key card's alphabet.

**Carranza's telegrams:** `carranza-1915/` has the notes, the reading, the translation, the transcription, the line-by-line decryption and the key.

**Morosini:** `morosini-1587/` has the notes, the check against the published key, the reading, the line-by-line decryption, the key and the key check.

**Francia 346:** `francia-346-leaves/` has the notes, the check against the published key, the reading, the line-by-line decryption, the key and the key check.

**Biglia:** `biglia-1565/` has the notes, the check against Dudout's reading, the reading, the line-by-line decryption, the key and the key check.

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

- The Medici letter: read in part. 88 of 113 cipher words are read in full, 77.9%, and 663 of 730 letter positions, 90.8%. About 60 code groups and symbols stay unread.
- Charles V: 240 of 246 cipher words read, 97.6%. Six stay marked, where the writer left out a letter or wrote a wrong sign.
- Bazin: 84.1% of the decoded letters that line up with the print of 1867 are equal (12,254 of 14,570). The reading gives the firm stretches only.
- Guastalla: the cipher part reads as sense, apart from about ten code groups and a few doubtful passages.
- 446, 1399 and 1400 come from reconciled transcriptions. Cipher words read: 446 376 of 389, 1399 744 of 750, 1400 490 of 493.
- Pages 2 to 4 of 1398 come from a reread made with the key in view, checked against three blind passes and settled on the enlarged scan. Cipher words read: 590 of 613.
- AGAD 1401: 518 of 530 cipher words read, 97.7%. Nine code groups stay open.
- AGAD 131: read in part. Two transcription passes agree on 88%, and about 300 differences are not yet settled on the scan. About 25 of some 460 cipher words stay doubtful.
- The 1911 telegram: read in full with the archive's key card. Three words keep a doubt.
- Carranza's telegrams: 96.5% of the number tokens give the reading's letter as typed. The others are mostly the clerk's slips, repaired by sense.
- Morosini: read in part, with no key; 95.1% of the matched single-letter codes right (80,553 of 84,667). 72.7% of all single-letter codes recovered (80,553 of 110,821). The cut is wrong for the three-digit letter codes. A second search for the missing code forms failed its test on artificial letters, so it did not run on the real text. The read is the first one.
- Francia 346: read with no key; 99.2% of the shown true letters right (6,953 of 7,012). 65.7% of the graded shown tokens show the true letter (6,953 of 10,591).
- Biglia: read with no key; within words, 82.2% of the aligned letter pairs equal to Dudout's reading, with gaps left out (957 of 1,164). The cut misses the syllable codes.

In the readings, `[195]` is a number group that stays unread, and `[?word]` is a doubtful reading.

The cipher ledger at https://github.com/dbourdeau/cyphersolver checks contributed readings against the contributor's files and a word list, not against the scans.

- It marks the Branicki letters (446, 1398 to 1400), Charles V and AGAD 1401 as complete, and credits their keys to me.
- It confirmed that the Carranza key decodes the telegrams. It holds that page until someone checks printed sources for the same tables.
- Guastalla, the 1911 telegram and AGAD 131 are with the ledger as issues #329, #330 and #331.

© 2026 Prabal Gupta. First published here, 7 November 2026. Released under CC BY 4.0: reuse it, and credit me.
