# Cardinal Alessandro Farnese to Giovanni Poggio, 1542

**Read in part from the ciphertext alone, without any published key or corrected transcription.**

- **DECODE:** record R92 (ff. 70r to 73v), https://de-crypt.org/decrypt-web/RecordsView/92.
- **Source transcription:** DECODE's public transcription of 2016 (made before the solution). The cipher part holds 6,532 digits across 113 cipher lines on ff. 70r to 73r; f. 73v is in clear.
- **Use:** research only. I copy no DECODE image and no DECODE transcription file. Each line of [decryption.txt](decryption.txt) gives the folio and cipher-line number of DECODE record R92, so that a reader with access to DECODE can follow it. When you use this material, cite DECODE and record R92.
- **State:** from ciphertext; partial read. Simon Klee published a solution and key for DECODE R92 on 16 September 2026 (https://simonklee.dk/farnese-letter; reviewed in `cyphersolver` as `targets/vatican5`). Neither his key nor any corrected transcription was opened or used before this key and read were fixed on 22 November 2026.

## The cipher

Single digits stand for the frequent letters (`8=e`, `5=a`, `4=o`, `6=i`, `2=r`, `7=n`, `0=s`, `1=u`, `3=m`), `9` is a null, and two-digit groups stand for the other consonants (`80=t`, `03=l`, `27=c`, `57=p`, `73=d`, `75=g`, `37=f`) and letter-plus-null pairs (`49=o`, `89=e`, `29=r`, `69=i`, `79=n`, `90=s`). The transcription also marks raised dots and commas over digits; this read uses the undotted digits alone.

Checked afterwards against `targets/vatican5/key.md`, all nine single-digit letters, the null `9`, and seven of the nine undotted two-digit letter codes (`03=l`, `73=d`, `80=t`, `57=p`, `27=c`, `37=f`, `75=g`) agree exactly. Because this read uses the undotted digits only, the rare undotted codes that collide with dotted pairs (`72=b`, `07=z`, `81=et`) and the nine dotted syllable and title codes stay open. [key.tsv](key.tsv) and [decryption.txt](decryption.txt) are unchanged from the blind run.

[key.tsv](key.tsv) gives each recovered code, its value, its count and its grade.

## What the read says

Read the firm stretches in [Italian](reading.md) and [English](translation.md).

- **Preparations against the Turk.** After a departure, the writer reports conferences involving a marquis and a prince on arming and preparing against the Turk ("del Turco", "modo di preparazione", "per tera o per mare", "armata composta di galere").
- **Defense of the Papal States and Lombardy.** Troops in the Papal States ("nel Stato Ecclesiastico di molti soldati"), defense against the Turk ("per la difesa dal Turco"), the Apostolic See ("a la Sede Apostolica"), and the guard of the lands of Lombardy ("per la guardia de le terre di Lombardia").
- **Ridolfo Gonzaga in the Mantuan territory (ff. 72v–73r).** Signor Ridolfo Gonzaga, son of Signor Giovan Francesco, has seized a fortress/castle in the Mantuan territory belonging to his brother, with infantry, and has begun to fortify it ("il Signor [Ri]dolfo Gonzaga fiolo del Signor Giovan Francesco ... ha preso ... la forte[zza] di ... castelo nel Mantovano ... ha cominciato a fortificar ... la fortification de li castelo").

## Files

- [key.tsv](key.tsv): the recovered one- and two-digit key table from ciphertext alone.
- [decryption.txt](decryption.txt): all 113 cipher lines decoded, indexed by folio (`70r` to `73r`) and line number.
- [reading.md](reading.md): readable Italian stretches from `decryption.txt`.
- [translation.md](translation.md): English translation of the readable stretches.
