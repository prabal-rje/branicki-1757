# Jean Bazin to Henri de Valois, king elect of Poland: Cracow, September 1573

**Read from the ciphertext alone, with my own algorithm. I had no key, no crib and no other cipher letter.**

**Checked afterwards against a clear text printed in 1867.** Of my decoded letters that line up with a printed letter, 84.1% are equal (12,254 of 14,570). A wrong passage of the same print gives 47%.

Jean Bazin was sent to Poland by the French court. This long letter, mostly in cipher, reports to the newly elected king on the state of Poland in September 1573.

- **Where:** Bibliothèque nationale de France, Cinq cents de Colbert 338, pp. 191 to 198.
- **Scans:** Gallica, ark btv1b10033937d (https://gallica.bnf.fr/ark:/12148/btv1b10033937d).
- **Ledger:** catalogue 1571 at https://github.com/dbourdeau/cyphersolver. On 11 November 2026 it listed the letter as open.
- **The print:** the marquis de Noailles, *Henri de Valois et la Pologne en 1572*, vol. 3 (Paris, 1867), pp. 475 to 484 (https://archive.org/details/henridevaloisetl03noaiuoft). It gives the letter in clear, with gaps, and with no key. Bazin's instruction is on its p. 474.

I found the print after the key and the decoded letters were fixed. `check.md` gives the times.

## What this read adds to the print of 1867

- **A key.** The print does not say how the cipher works. `key.tsv` gives a value for each sign label, as the algorithm found it. `key_check.tsv` sets each value beside the print.
- **Text that the print leaves out.** My decode has three passages of 75 to 300 letters that the edition does not print, and four shorter ones.
- **The order of the pages.** The letter reads in the page order 191, 192, 195, 196, 193, 194, 197, 198. So the two middle leaves are out of order in the volume as it is numbered.
- **A measured blind read.** The print measures what the algorithm does on a real cipher of 15,409 signs.

`check.md` gives the evidence and the limits of each point.

## What the letter says

Each point gives its pages. `reading.md` and `translation.md` give the text.

- **A diet of Great Poland (p. 192).** Only three articles were treated. One asks a lord to choose between two offices. By the print, he is the palatine of Cracow, who is also marshal of the realm. One is a rendering of accounts for some monies. One concerns the liberty of religions.
- **Money and Danzig (p. 195).** Sums are owed: "three or four hundred thousand florins" and "fifty thousand florins each year". Danzig settles for "two hundred thousand florins", half now and half within a certain time. The trade of Muscovy, Denmark and a port are named.
- **The coronation and the burial (p. 196, in clear).** The coronation was fixed for 3 October at the election, and the day is now disputed. The burial of the late king must come first.
- **Little Poland and Lithuania (p. 193).** The assemblies are never certain. The chancellor and the archbishop are named. Rich garments are made "to show the contentment and the hope". By the print, the Infanta has them made.
- **The Muscovite and the Tartars (p. 197).** The Muscovite grants a truce of one year. It was asked only until the coronation. If the king does not come by Saint Martin's day (11 November), another election reads as threatened. A battle with the Tartars two years earlier has weakened the Muscovite, so Lithuania is at peace.
- **The Ottomans (pp. 197 and 198).** Letters of "Mahomet Bascha" congratulate the Poles on the election and warn them to pay the Tartars their pension. Polish frontier soldiers, called Cossacks, raided the Tartars and took eight pieces of artillery. That angered "the Grand Seigneur". A despatch goes to calm him and to do justice.
- **Requests (p. 198).** The writer asks whether it is good to write to "Monsieur d'Acqs". He asks for orders about the cost of a castellan's horses and soldiers.

Read it: [French](reading.md), [English](translation.md). Both are as I made them before the check. `check.md` lists what the print contradicts.

## The check, in short

| Measure | Value |
| --- | --- |
| Decoded letters equal to the print, of those that line up with a printed letter | 84.1% (12,254 of 14,570) |
| The same, page by page | 78.3% (p. 191) to 89.4% (p. 198) |
| The same measure for a wrong passage of the print | 47.0% |
| Every decoded letter counted, with extra letters as errors | 80.1% |
| Names and facts that I marked firm | 18 of 18 confirmed |
| Names that I marked as guesses: Danzig, Muscovy, liberty of religion | 3 of 3 confirmed |
| Places where my reading contradicts the print | 4 found so far |

- A search of the letter model's training texts found no sign of this letter. The longest shared run is 27 letters, a courtesy formula.
- The print leaves out some passages, and it modernizes some spelling. Both count against my read in these numbers.

## The cipher and the key

- The transcription uses 53 sign labels. My key gives each label one letter. Frequent letters have several labels.
- No frequent label shows evidence of being a null.
- On the alignment with the print, the key is right for 83.8% of the sign tokens.
- Twelve labels each cover two printed letters, for example e and i. They are the largest cause of error that I can name.
- The counts suggest that seven labels stand for two letters, such as ss and ll. A key with one letter for each label cannot read them.
- My key gives no label the value `g`. So the decryption never writes g: "arande" stands for grande.

`check.md` gives the details.

## How it was read

From the ciphertext alone, with no other cipher letter, key or crib.

- **Transcription.** Two independent passes labelled the sign shapes. They agree on 94% of 15,409 cipher signs. Where they disagree, the fit picks one side for each kind of disagreement. Where one pass has a sign that the other lacks, the place is left out (`transcription.txt`).
- **Letter model.** French letter counts from texts of 1441 to 1666 that I hold: chronicles, letters, memoirs and pamphlets.
- **Fit.** The search tries a key and scores how likely the decoded stream is as French. It ran 120 times from different starting keys. 89 runs end close to the best score. A letter shows when 90% of those runs agree. 99.3% of signs show a letter.

## Caveats

- `reading.md` follows the page numbers of the volume. Read its passages in this order: 1 to 5, 9 to 11, 15, 6 to 8, 12 to 14, 16. No firm passage comes from p. 194.
- Single words are weak evidence. The long stretches are strong.
- The clear passages are not part of the decipherment. A pass read them from the scan.
- **The addressee.** My first files named Charles IX, by mistake. The print's heading and the letter itself give Henri.
- **The date.** The print gives 15 September 1573. My reading of the clear subscription gave "XX[e?]", marked as uncertain.
- The comparison rests on one alignment of my letters with the print. `check.md` gives its limits.

## Words used here

- **Crib:** a piece of the plain text that the solver knows in advance.
- **Null:** a sign that stands for nothing.
- **Sign label:** the name that the transcription gives to one sign shape.
- **Sign token:** one sign at one place in the text.
- **Diet:** an assembly of the nobles of a region or of the realm.
- **Castellan:** the governor of a castle and its district.

## Files

- `reading.md`: the French, in normal spelling where the read is firm
- `translation.md`: the English
- `check.md`: the check against the print, the passages that the print leaves out, the cover names and the order of the pages
- `transcription.txt`: the merged sign labels and the clear words, line by line
- `decryption.txt`: the decryption, line by line, with gap marks
- `key.tsv`: the key
- `key_check.tsv`: each label's value beside the letters that the print has at its places
