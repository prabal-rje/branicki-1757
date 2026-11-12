# Sforza chancery letters in cipher (Milan): partial reads

This folder holds our partial reads of eight cipher letters of the Sforza chancery. The letters are DECODE records 5425 to 5430, 5464 and 5465 (Archivio di Stato di Milano, Carteggio Sforzesco, cartella 1597).

- The reads of records 5464 and 5465 are open.
- The read of records 5425 to 5430 is in one encrypted file.

A sign is one written sign of the cipher text, as the machine transcription gives it.

## What we claim

We found keys and partial reads from the ciphertext alone. We used no key from outside. Records 5425 to 5430 share one key. Records 5464 and 5465 each have their own key.

- **Record 5464** reads in stretches of sentences.
  - Our decode shows a letter on 86% of the signs.
  - Two blind readers found sense in 65% to 70% of the shown letters. That is 56% to 61% of all signs.
- **Record 5465** reads in patches only.
  - Our decode shows a letter on 68% of the signs.
  - The two blind readers found sense in about 55% of the shown letters. That is 37% of all signs.
- **Records 5425 to 5430** (six letters): our decode shows a letter on 62% of the signs. No sentence reads yet.

A shown letter is not a letter read. "86% of the signs show a letter" does not mean "86% read".

The blind readers are two large language models. Each saw only our decode and two shuffled copies of it, with no name, date or source. `r5464/check.md` gives the test.

## What we do not claim

- **A checked decipherment.** No key sheet and no clear text checks these reads.
- **A checked transcription.** The signs are a machine transcription of the images. Nobody has checked a decoded word against the ink.
- **A measured accuracy for every read.**
  - On artificial letters of the size of record 5464, 90% to 95% of the shown letters were right in four tests of five. In the fifth test, the method found a wrong key, and almost no shown letter was right.
  - Record 5465 has no artificial test letters of its own.
  - On artificial letters of the size of records 5425 to 5430, 87% to 93% of the shown letters were right.
  - Each `check.md` gives the tests and their limits.

## The files

- `r5464/`:
  - `reading.md`: the stretches that read, with an English translation;
  - `decryption.txt`: our decode, line by line;
  - `key.tsv`: our key;
  - `check.md`: what supports the read, and what does not.
- `r5465/`: `decryption.txt`, `key.tsv` and `check.md`. It has no reading page, because it reads in patches only.
- `sforza-1597-a-sealed-2026-11-12.tar.gpg`: our read of records 5425 to 5430, sealed on 12 November 2026.
  - GnuPG encrypted it (symmetric, AES-256).
  - We will publish its passphrase here when we have a better version.
  - Then anyone can decrypt it with `gpg --decrypt sforza-1597-a-sealed-2026-11-12.tar.gpg` and see what we held on this date.

## Credits

- **The signs** are the sign transcription of the cipher ledger (https://github.com/dbourdeau/cyphersolver, target `sforza1597`). Its maintainer made it from the DECODE images with his sign reader.
  - Our files do not copy his token files. A reader needs them to follow our decode sign by sign.
  - Record 5464: `targets/sforza1597/ctts/r5464_best/tokens.txt`.
  - Record 5465: `targets/sforza1597/ctts/r5465_best/tokens.txt`.
  - Records 5425 to 5430: `targets/sforza1597/ctts/a_best/tokens.txt`.
- **The ledger's maintainer read part of record 5464 first.**
  - His partial reading of 7 November 2026: by his count, 27% of the letters fall in words of four letters or more.
  - His key found the main letters first.
  - Our key gives the same letter as his on 87% of the signs.

## Source and terms

DECODE, the database of historical ciphers of the DECRYPT project: records 5425 to 5430, 5464 and 5465. The documents are in the Archivio di Stato di Milano.

DECODE's images are for research use only. None is in this repository.
