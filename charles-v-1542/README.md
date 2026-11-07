# Charles V to Ferrante Gonzaga, Monzón, 11 August 1542

Emperor Charles V writes to Ferrante Gonzaga, his viceroy of Sicily. The letter is signed "Yo el Rey" and countersigned "Idiáquez".

- **Where:** Biblioteca Estense Universitaria, Modena, Autografoteca Campori, Lettera K, Karl V, sfasc. IV, cc. 109-110.
- **Scans:** https://lodovico.medialibrary.it/media/schedadl.aspx?id=c710a32c-42a7-4159-8abc-472aed58f7c9
- **Ledger:** catalogue 1560 at https://github.com/dbourdeau/cyphersolver lists this letter as still unread. The undated letter in the same entry (cc. 131-132) is not covered here.

## What it says

- Sicily cannot pay for its infantry, its galleys and the fort of La Goleta without outside help.
- The Emperor's other kingdoms are as short or worse, so no help can come now.
- La Goleta must be provided for, because of the Turkish fleet.
- Spies report that the main French effort is coming to the frontier of Perpignan, and that the French threaten Navarre.
- The Viscount Cicala must be paid for his galleys, because someone is soliciting him to take another contract.

Read it: [Spanish](reading.md), [English](translation.md).

## The cipher

A base sign is a consonant, and a small digit above it adds the vowel. The digits 1 to 5 and the digits 6 to 9 and 0 both run a, e, i, o, u. A sign with no digit is a single letter.

| Sign | With digit 1-5 | With digit 6-0 | No digit |
| --- | --- | --- | --- |
| x | d | | n |
| z | r | b | i |
| q | | n | e |
| t | f | l | y |
| d | p | | |
| n | m | | u |
| g | h, rarely c | c | |
| b | | s | |
| a | t | | m |
| w | tr | | |
| c | g | qu | l |

These signs have no digit: f is s, h is e, v is o, y is a, o is r.

The sign s marks a doubled or palatal consonant: "de-s-e" is "desse", "se-s-aladamente" is "señaladamente", and "Perpi-s-an" is "Perpiñan".

Letters in the table name the shapes in `transcription.txt`. A shape label is a description, not a value. A few rare signs are in `decryption.txt` only. I fixed those by sense, so they are less sure.

## How it was solved

The plan came from the sign statistics of the letter itself, with no key, sibling letter or crib. A solver on a Spanish letter model then gave the letters, and I read the text from that.

- **Transcription:** two passes agree on 96.3% of 702 signs. I checked the clear lines and the doubtful signs against enlarged scans.
- **Score:** the key scores -2.21 per letter under the Spanish model. Shuffled signs score -3.33.
- **Repeat runs:** all six starts reach the same key.
- **Held-out half:** a key fitted on the first half agrees with the full key on 89.7% of tokens in the second half. Each half has only about 350 tokens.
- **Blind read:** a reader with no context named this text as Spanish, and it named two shuffled controls as noise.

## What stays open

I compared the raw key stream with the reading, letter by letter. `decryption.txt` shows the raw stream.

- **Straight from the key:** about 94% of the cipher's letters.
- **Fixed by sense:** about 5%. These are spelling (b for v), a dropped letter, or a rare sign with too few uses to fix by counts.
- **Unread:** about 1%, one short phrase. After "pudiéredes ayudar", the string "nosurebil" makes no sense to me.

Four readings are doubtful:

- "y a sus rentas", from the string "yasurintas".
- "haver", from the string "caber", which comes three times.
- "como", a blotted clear word before "que huviere lugar".
- "Novellara", from the string "niuilara". The Counts of Novellara were a Gonzaga branch, but I found no count of that house in Sicily in 1542.

I found no printed copy. But the chancery's clear draft may survive in Spanish archives, and I could not check those.

## Context, from memory and not checked here

- France declared war on Charles V in July 1542. That autumn a French army under the Dauphin besieged Perpignan and failed to take it.
- La Goleta was the Spanish fort at Tunis.
- Alonso de Idiáquez was a secretary of Charles V.

## Files

- `reading.md`: the letter in Spanish
- `translation.md`: the letter in English
- `transcription.txt`: the cipher and the clear text, line by line, with shape labels
- `decryption.txt`: the decryption, line by line

The page images stay with the Biblioteca Estense under their own licence (CC BY-NC-SA). They are not copied here.

© 2026 Prabal Gupta. First published here, 7 November 2026. Released under CC BY 4.0: reuse it, and credit me.
