# Blind statistical check: Salvius 1633 (DECODE R4339)

Evaluated with an independent classical Latin character 4-gram language model trained on 526,617 characters (Caesar, Tacitus, Cicero; zero overlap with 17th-century diplomatic Swedish) against 1,000 exact letter-permutation nulls preserving homophone-group and null-block structure.

- **Direct blind coverage from `R4338 + R4340` glosses alone (zero `R4339` input):** `93` of `137` two-digit tokens (`67.9%`).
- **Auto-blind rule (`+/-2` contiguous-block completion from `R4338 + R4340` glosses only, zero tuning on `R4339`):** real Latin LM `-2.1539` (`64` 4-grams) vs. 1,000 nulls `-4.4871 +/- 0.4188` (max `-2.8897`), `Z = +5.57` sigma (1,000 of 1,000 nulls beaten).
- **Full 1633 key (all 15 two-digit runs in `R4339`):** real Latin LM `-2.1322` (`73` 4-grams) vs. 1,000 nulls `-4.4783 +/- 0.3944` (max `-2.9123`), `Z = +5.95` sigma (1,000 of 1,000 nulls beaten).
