# Cipher letters read: Charles V, 1542, and four French letters, 1756-1757

Letters that the archives and the historical cipher ledger at https://github.com/dbourdeau/cyphersolver list as unread. All five were read from the ciphertext, with no key from outside.

| Letter | Date | What it says | Read it |
| --- | --- | --- | --- |
| [Charles V to Ferrante Gonzaga](https://lodovico.medialibrary.it/media/schedadl.aspx?id=c710a32c-42a7-4159-8abc-472aed58f7c9) | Monzón, 11 August 1542 | The Emperor tells his viceroy of Sicily that no help can come for the infantry, the galleys and La Goleta. Spies report that the main French effort is heading for Perpignan. | [Notes](charles-v-1542/README.md), [Spanish](charles-v-1542/reading.md), [English](charles-v-1542/translation.md) |
| [AGAD 446](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28224155) | Białystok, 22 March 1757 | Hetman Jan Klemens Branicki to Antoni Potocki, palatine of Bełz. Branicki plans a manifesto against an envoy's abuse of his mission. The envoy is probably Stanisław Poniatowski, later King of Poland. | [French](reading_446.md), [English](translation_446.md) |
| [AGAD 1398](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225111) | 24 July, probably 1757 | Signed Matusewic. A field report on the Russian army under Apraxin at the frontier of Prussia: requisitions, Cossacks, and town deputies who come to submit. | [French](letters/1398/reading.md), [English](letters/1398/translation.md). Page 2 is still rough. |
| [AGAD 1399](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225112) | Probably June or July 1756 | An insider's report on Hetman Radziwiłł's party in Lithuania. A congress at Iwie agrees a fund of 146,000 francs to buy the coming dietines, and lists five lords' shares. | [French](letters/1399/reading.md), [English](letters/1399/translation.md) |
| [AGAD 1400](https://www.szukajwarchiwach.gov.pl/jednostka/-/jednostka/28225113) | Nieśwież, 11 September 1756 | Signed Boeven. A bloody election assembly at Brest, and a rival party spreading two hundred thousand francs across Lithuania. | [French](letters/1400/reading.md), [English](letters/1400/translation.md) |

The ledger lists the Charles V letter as catalogue 1560, 446 as catalogue 1578, and 1398 to 1400 as catalogue 1579.

## Charles V, 1542

Each base sign is a consonant, and a small digit above it adds the vowel. `charles-v-1542/README.md` gives the table, the checks and what stays open.

The plan came from the letter's own sign statistics. A solver on a Spanish letter model then gave the letters.

## The French letters, AGAD Warsaw, fonds 338

Each reference code is AGAD 1/338/0/1/ plus the letter number. One key reads all four.

Almost entirely read. Every cipher letter reads as French. A few number codes stay open, mostly names and titles.

Bespoke count matching algorithm based on the French next-letter counts (deciphered 98.9% of tokens on 446 and 1400, and 99.4% on 1399, in one shot).

### What stands out

- **An informer.** Boeven signs 1400. A 1909 history makes him Hetman Radziwiłł's secretary, in touch with the French minister in 1756 and on the French payment list. 1399 looks like his hand, and it reports on "mon maître". This is my reading.
- **Names in print.** The same history names most people in 1399 and 1400 with the same titles. `letters/README.md` gives each match and its page.

### How I date them

**1400.** The date line ends with the code groups 824 811 823 818 810. Numbers 805 to 824 are number words, so this reads "mil sept cent cinquante six". The second-last group is less sure, because of a blot.

**1399.** It has no date line. It plans for the Tribunal of 1757, and for shares due next August, so it comes before that Tribunal's dietines.

**1398.** It gives 24 July with no year. Apraxin's army stood at the frontier of Prussia in the summer of 1757.

### Key

A reciprocal alphabet of 12 pairs. Each pair swaps: a stands for h, and h stands for a.

a-h, b-q, c-r, d-s, e-l, f-t, g-z, i-m, k-x, n-o, p-u, w-y

## Files

**Charles V:** `charles-v-1542/` has the notes, the reading, the translation, the transcription and the line-by-line decryption.

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

- Charles V: about 97% of the cipher's letters come straight from the key, about 3% are fixed by sense, and a few words stay doubtful.
- 446, 1399 and 1400 come from reconciled transcriptions.
- Page 2 of 1398 is still rough.

In the readings, `[195]` is a number group that stays unread, and `[?word]` is a doubtful reading.

No historian has checked these readings yet.

© 2026 Prabal Gupta. First published here, 7 November 2026. Released under CC BY 4.0: reuse it, and credit me.
