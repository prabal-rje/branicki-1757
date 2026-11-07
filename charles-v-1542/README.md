# Charles V to Ferrante Gonzaga, Monzón, 11 August 1542

Emperor Charles V writes to Ferrante Gonzaga, Prince of Molfetta, his viceroy of Sicily. The letter is signed "Yo el Rey" and countersigned "Idiáquez". The back gives the address, and it marks this copy as the duplicate.

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

The labels below name the shapes in `transcription.txt`. A label is a description, not a value.

| With a digit | Consonant |
| --- | --- |
| x | d |
| z | r |
| d | p |
| n | m |
| a | t |
| w | tr |
| q | n |
| t | l |
| g | c |
| b | s |
| S, I, F | b |
| P | f |
| Q | pr |
| c | g with digits 1 to 5, qu with digits 6 to 0 |

| With no digit | Letter |
| --- | --- |
| h | e |
| v | o |
| y | a |
| t | y |
| n | u |
| D | i |
| x, z | n |
| f, T | s |
| o, r, Q | r |
| c | l |
| C | c |
| E | p |
| M | m |
| G, F | f |
| s | a doubled or palatal consonant: ss, ll, rr or ñ |
| X | a null |

The rare shapes:

- D is a delta, and S is a sigma.
- P is a hooked stem, and Q is a looped angle.
- I is a short stroke, and C is an arch.
- E is a slant with a dot, G is a triangle, and X is a crossed loop.

## How it was solved

The plan came from the sign statistics of the letter itself, with no key, sibling letter or crib. A solver on a Spanish letter model then gave the letters, and the text was read from that.

- **Transcription:** two passes agree on 94.4% of signs. Each difference is settled on the scan, which gives 705 signs.
- **Score, on the first pass:** the key scores -2.21 per letter under the Spanish model. Shuffled signs score -3.33.
- **Repeat runs, on the first pass:** all six starts reach the same key.
- **Held-out half, on the first pass:** a key fitted on the first half agrees with the full key on 89.7% of tokens in the second half. Each half has only about 350 tokens.
- **Blind read:** a reader with no context named this text as Spanish, and it named two shuffled controls as noise.

## What stays open

I compared the raw key stream with the reading, letter by letter, and counted b, u and v as one letter. `decryption.txt` shows the raw stream.

- **Straight from the key:** about 97% of the cipher's letters.
- **Fixed by sense:** about 3%. These are writer's slips, and rare signs with too few uses to fix by counts.
- **Unread:** nothing now.

These readings stay doubtful, and the reading marks most of them with `[?word]`:

- "screbir", from "screbil".
- "della", from "de=a". The sign s also gives ll.
- "amenaçavan", from "amenaban".
- "cediesse", which could also be "se diesse".
- "Anguillara", from "lannuilara". I have not identified this count.
- "haver", from "caber", which comes three times. This one is not marked in the reading.

I found no printed copy. But the chancery's clear draft may survive in Spanish archives, and I could not check those.

No historian has checked this reading yet.

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
