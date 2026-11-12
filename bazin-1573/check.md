# Bazin 1573: the check against the print of 1867

## 1. What was compared

- **My side:** the key, the decryption and the reading in this folder.
- **The print:** the marquis de Noailles, *Henri de Valois et la Pologne en 1572*, vol. 3 (Paris, 1867), pp. 475 to 484 (https://archive.org/details/henridevaloisetl03noaiuoft). I read its pages from the scan, because its OCR text is poor.
- **The method:** each manuscript page is paired with the print, letter by letter, with the fewest changes (an edit-distance alignment). A decoded letter is right when the printed letter at its place is the same.
- **The control:** the same pairing of each page with a wrong passage of the print, and with its own passage with the words shuffled.

Before the pairing, both texts are made plain:

- accents are dropped, and ç counts as c;
- v counts as u, and j counts as i;
- œ and æ are written as two letters;
- marks that are not letters, and the editor's own insertions, are left out;
- y and i stay two letters.

**The times.** The key and the decoded letters were fixed at 22:57 on 11 November 2026. The search that found the print began at 23:08. I wrote the reading and the translation the same evening, without the print.

**The same letter.** The editor's source line names Colbert 338 and gives no page. So the alignment itself shows that this is the same letter. Every page of my decode finds one place in the print and follows its sentences in order.

## 2. The numbers

| Measure | Value |
| --- | --- |
| Decoded letters equal to the print, of those aligned to a printed letter | 84.1% (12,254 of 14,570) |
| Control: each page against a wrong passage | 47.0% (43.3% to 59.9% by page) |
| Control: each page against its own passage with shuffled words | 47.2% |
| Every decoded letter counted; a letter with no printed letter is an error | 80.1% |
| The same, without the 15 lines where the print leaves out text | 82.1% |
| Aligned gap marks counted as errors | 82.4% |
| Sign tokens for which the key gives the printed letter | 83.8% (12,304 of 14,675) |

The print has four dotted gaps. The 22 decoded letters at those gaps are not scored.

| Page | 191 | 192 | 193 | 194 | 195 | 196 | 197 | 198 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Equal letters | 78.3% | 83.1% | 86.7% | 88.2% | 82.5% | 81.4% | 86.4% | 89.4% |
| Wrong-passage control | 44.8% | 47.2% | 46.2% | 50.6% | 43.3% | 59.9% | 45.7% | 44.9% |

The control of page 196 is high, because about a third of that page is in clear. So few cipher letters are aligned there.

How much of the print the cipher covers:

| Share of the print's letters | Value |
| --- | --- |
| Covered by a cipher sign of my decode | 76.2% |
| Covered by words that are in clear in the manuscript | 11.7% |
| No counterpart in my transcription | 12.1% |

The last share holds three things:

- the opening of the letter, which is not on pp. 191 to 198 (604 letters);
- the first line of pp. 193, 195 and 197, which my transcription lacks (about 184 letters);
- printed letters inside the pages that have no decoded letter. This is the largest part.

## 3. Names and facts

Before the check, I marked each name as firm or as a guess. The print confirms all of them.

| My reading | I marked it | The print |
| --- | --- | --- |
| Monsieur de Valence | firm | confirmed |
| Lansac | firm | confirmed |
| Monsieur d'Acqs | firm | confirmed |
| Mahomet Bascha | firm | confirmed |
| the Grand Seigneur | firm | confirmed |
| the Muscovite, the Tartars, Cossacks | firm | confirmed |
| the marshal of the court | firm | confirmed |
| the chancellor of the realm; the archbishop | firm | confirmed |
| a castellan | firm | confirmed |
| the senate, the deputies, the diet, the estates, the palatinate | firm | confirmed |
| Poland, Great and Little Poland | firm | confirmed |
| Lithuania | firm | confirmed |
| Cracow | firm | confirmed |
| Russia and Podolia | firm | confirmed |
| Denmark | firm | confirmed |
| the four sums in florins | firm | confirmed |
| Saint Martin's day | firm | confirmed |
| a truce for one year | firm | confirmed |
| Danzig | guess | confirmed |
| Muscovy | guess | confirmed |
| liberty of religion | guess | confirmed |

## 4. What the print contradicts

The check covered the names above and my summary of each passage. It did not compare every sentence of `reading.md` with the print. So this list can be incomplete.

Four places of `reading.md` contradict the print:

- **Passage 11 (p. 195).** My fragment reads as if a secret understanding exists between the parties. In the print, the writer says that the understanding that he feared most does not exist.
- **Passage 14 (p. 198), the horses.** My reading has a castellan "who keeps two horses". The print has two hundred horses. My decode has no letters for the hundred at that place. So the difference is in the cipher as transcribed, or in the edition.
- **Passage 14 (p. 198), the expense.** My reading calls the expense "very necessary". The print has "non grandement nécessaire", not very necessary. My decode has the "non" too. I dropped it in the reading.
- **Passage 15 (p. 196, in clear).** My reading has the body brought to Warsaw. The print has "en ceste ville", to this town, which is Cracow.

Five smaller points differ:

- p. 192: my "sent" is "give" in the print;
- p. 192: my "by the writings of" is "the Emperor's artifices and letters";
- p. 195: my "those of Poland" is "the king of Poland";
- p. 198: my "during the coming" is "before your coming";
- p. 193: my passage 6 joins two sentences. In the print, the Infanta has the garments made, and the next sentence is about the lords.

## 5. What my read adds to the print

The print leaves out text in these places. My decode reads French there. The text is in the spelling of the decode. `·` is a gap mark, and «…» is a word in clear.

| Page and lines | Letters | The decode | In English | How sure |
| --- | --- | --- | --- | --- |
| p. 193, lines 35 to 41 | about 300 | "…unerandmalaesetaploor teyeaucouideruine… «may Januier» neustdespuschededeca maislecor·eetcustearosemasequiatousioursetedediia «may» seruice demeureentiere utnonsuulementceyelamaisdeaucoupdaultntresquiuoientestedaduiscontraire" | Great harm and ruin could have come to this realm, if Your Majesty had not sent here. But the body and "this great mass", always devoted to your service, remain whole, with many who were of the contrary opinion. | high |
| p. 195, lines 45 to 47 | about 100 | "le «Doctur» sestserue·ecesteo·aseondepuislamortdqueu «fortitudo» ·dempescherlecouercudedanscic" | The «Doctur» has used this occasion, since the death of the late «fortitudo», to hinder the trade of Danzig. | high |
| p. 196, lines 24 to 26 | about 75 | "…deuata·roistrecequilspatparchacunandinemoetiepourlemoinsaupaurauant" | …and to raise what they pay each year by at least half over what they paid before. | high |
| p. 198, line 8 | 19 | "depuisdeuxsutroistoe·" | for two or three (days?) | medium |
| p. 193, lines 5 to 6 | 13 | "…ut plrtant iusques ac·uue…" | for all that, until | low |
| p. 194, line 13 | 8 | "apresque" | after | low |
| p. 195, line 36 | 9 | "…ntpourceuaer" | for that purpose | low |

The print has four dotted gaps. My decode has letters at three of them:

- p. 192, lines 26 to 27: "nonseuurdeuale…", which reads as "monsieur de Vale[nce]";
- p. 192, lines 34 to 35: "un chee part";
- p. 194, line 11: "rusuur".

The fourth gap holds a word in clear, «Coram». The print gives it no sense.

One more place is in clear text, not in the decode. At p. 193, lines 46 to 47, my transcription reads "pour accroistre voz maiesté grandeur et puissance", and the last word is doubtful. The print stops at "vostre majesté et grandeure".

## 6. The key against the print

`key_check.tsv` gives every sign label with my value and the letters that the print has at its places. In that file, "y=i" means that y and i count as one letter. That holds for this section too.

| Verdict for a sign label | Labels | Share of the sign tokens |
| --- | --- | --- |
| "pure": right, and one letter has 85% or more | 22 | 64.9% |
| "diffuse": right, with no clear second letter | 9 | 6.6% |
| "mixed": right, but a second letter has 15% or more | 12 | 27.2% |
| wrong | 2 | 1.0% |
| rare (fewer than 20 tokens) | 8 | 0.3% |

**The key and the search.** On this alignment, the key is right on 83.8% of the sign tokens. The best single value for each label gives 84.0%. The alignment was built on my decode, so this comparison favours my key.

**Mixed labels.** Twelve labels each cover two printed letters. They hold 27.2% of the tokens. They give 959 of the 2,316 wrong letters (41%), which is the largest cause that I can name. The largest six:

| Label | My value | The print has |
| --- | --- | --- |
| `s` | e | e 65%, i 28% |
| `a` | u | u 64%, e 30% |
| `dag` | n | n 53%, l 30% |
| `t` | u | u 64%, f 30% |
| `8` | a | a 63%, g 32% |
| `y` | u | u 58%, m 32% |

- Some labels change their use from leaf to leaf. `dag` is n on pp. 193 and 194, and mostly l on pp. 195 to 198. The transcription worked one leaf at a time.
- For `a`, two signs under one label are likely. For `s`, the question is not decided: two similar signs under one label, or one sign with two values. Only the page images can decide.

**Labels for two letters.** The counts suggest that seven labels stand where the print has two letters:

- `at` for ss;
- `the` and `inf` for ll;
- `6` for rr;
- `2` for ee;
- `lam` for es;
- `tri`, probably, for mm.

A key with one letter for each label cannot read them. So my decode has "queyes" where the print has "quelles". I did not look at the page images for this point. Another cause is possible, such as a sign with a doubling stroke.

**The letter g.** The print has 127 g's at sign places. The transcription puts them under the labels `8`, `sig` and `r`, and g is the smaller part of each. So my key gives no label the value g.

**A ceiling.** Suppose that each of the fourteen mixed and wrong labels were split in two, and each half took its own letter. That key would be right on 91.5% of the sign tokens on this alignment. This is a calculation. I have not tested a corrected transcription.

**Other causes.** Wrong letters also come from places where the two transcription passes disagree, from the print's spelling and left-out text, and from the alignment itself.

### My estimate before the check

Before the check, I made artificial letters with the same size and sign counts, and misread a share of their signs at random. They read 89% to 94% of their letters right. The real number is 80% to 84%.

- About 3 points of the gap come from the print: its left-out text and its spelling.
- The rest comes from my noise model. The real wrong letters are not random: 43% are vowel for vowel, and 53% fall in five labels.

## 7. The cover names

Some words in clear stand for persons, titles and pronouns. My reading leaves them as they are. The print gives their sense:

| Word in clear | Places | The print has |
| --- | --- | --- |
| may Januier (also may Janvier, mau Januier) | 32 or more | "Vostre Majesté" |
| may | 18 | "vostre"; once "la coronation de" |
| Juno | 23 | "vous" |
| Januier | 7 | "Majesté" or "Majestés" |
| Doctur | 10 | "le Docteur": the king of Denmark, by the editor's note |
| stature | 4 | "le Protée": the duke of Prussia, by the editor's note |
| fortitudo | 5 | "Fortitudo", "le roy" or "feu roy": probably King Sigismund Augustus, by the editor's note |
| cur | 2 | "l'Empereur" |
| atque | 2 | "le palatin de Cracovie" |

## 8. The order of the pages

- Each page of my decode finds one place in the print.
- The order of those places in the print is 191, 192, 195, 196, 193, 194, 197, 198.
- The text reads across the joins. Page 192 ends at the castellan of Danzig, and page 195 begins with the reasons from Monsieur de Valence. Page 196 ends with the burial, and page 193 begins with Little Poland.
- So the leaf with pp. 195 and 196 belongs before the leaf with pp. 193 and 194.
- Two causes are possible: the leaves were bound in the wrong order, or the page numbers were written after such a binding.

## 9. The date and the addressee

- **The date.** The print ends "De Cracovie, ce 15 septembre 1573". My reading of the clear subscription gave "XX[e?]" for the day, marked as uncertain.
- **The addressee.** The print's heading names the king elect, Henri de Valois, and the letter speaks to him. My first files named Charles IX, by mistake.

## 10. Limits of this check

- Every count uses one alignment, and the alignment was built on my decode. So it favours my key a little. The controls show what an alignment gives by chance.
- The print is the truth here, but it is not complete. It leaves out passages, it has four dotted gaps, and it modernizes some spelling. These places count against my read.
- The two-letter labels and the merged labels come from counts. I did not look at the page images for them.
- Section 4 is not a full comparison of my reading with the print.
- The check changed no value of the key and no line of the reading.
