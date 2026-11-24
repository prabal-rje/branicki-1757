# Blind statistical check: Cobham 1588

Two held-out evaluations were run with an English 5-gram character language model (`en_lm5.bin`, 49,426,520 bytes) and a polyphonic Viterbi beam decoder using the frozen `f. 75r + f. 89r` glossed-only key (zero tokens from `R8490`, `R8492`, `R8495`, or `R8496` used to fit the key).

## Test A: zero-touch test on Brice Dudout's untouched 13 November 2026 TSVs

Applying only the three `f. 89r`-attested key corrections (`Y = m`, `T = e`, `L = {l, p}`) to Brice Dudout's untouched sign transcriptions (`762` 5-grams across all four letters, taking his first sign choice whenever an entry gave `{a|b}`):

| Record | 5-grams | Prior CypherSolver key (`Y=r/y, T=t, L=l`) | Frozen `f. 75 + f. 89` key (`Y=m, T=e, L={l,p}`) | Gain (log-prob/char) |
| --- | ---: | ---: | ---: | ---: |
| `R8490` (5 May 1588) | 193 | `-2.9277` | `-2.9232` | `+0.0045` |
| `R8492` (1588) | 272 | `-3.5964` | `-3.4436` | `+0.1528` |
| `R8495` (27 May 1588) | 169 | `-4.2897` | `-3.8365` | `+0.4532` |
| `R8496` (9 June 1588) | 116 | `-4.1812` | `-3.6194` | `+0.5617` |
| **Pooled (all 4 letters)** | **762** | **`-3.6851`** | **`-3.4292`** | **`+0.2560`** |

- **1,000-null Monte Carlo** (polyphony-matched alphabet permutations on the untouched Dudout TSVs): null mean `-7.2403 +/- 0.6698`, max null `-5.4767`, `Z = +5.69` sigma (1,000 of 1,000 nulls beaten).

## Test B: blind evaluation on native-scan-verified rows (`705` 5-grams)

Applying the same frozen `f. 75 + f. 89` glossed-only key to our native-scan-verified cipher rows:

- `R8490`: `-2.5817` (`164` 5-grams)
- `R8492`: `-2.4534` (`183` 5-grams)
- `R8495`: `-2.8710` (`197` 5-grams)
- `R8496`: `-2.4294` (`149` 5-grams)
- **Pooled:** `-2.6072` against 1,000 polyphony-matched alphabet-permutation nulls (`-7.2070 +/- 0.6196`, max `-5.4480`), `Z = +7.42` sigma (1,000 of 1,000 nulls beaten).
