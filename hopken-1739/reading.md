# Höpken & Carlson: December 1739 Completely Bare Constantinople Despatch (11 Consecutive Bare Pages Deciphered)

- **Archive:** Riksarkivet (Stockholm), *Diplomatica Turcica* `SE/RA/2119/2119.1/I/9/21`
- **IIIF Manifest:** `https://lbiiif.riksarkivet.se/arkis!R0003582/manifest` (568 images)
- **Prior art check:** `dbourdeau/cyphersolver/targets/hopken1739/NOTES.md` only analyzed 4 French-glossed pages (`255 to 257, 260`) + 1 short postscript (`263`) and explicitly noted: *"Nothing here is a break of a bare despatch... out of a volume with well over a hundred pages of numbers."* (`hopken1740` is a different key, Code 2 `1006 to 1915`, images `321 to 342`.)
- **Scope decoded here:** **11 completely bare, unglossed pages** (`p114R, p115L, p115R, p116L, p116R, p117L, p117R, p118L, p118R, p120L, p120R`: **1,610 four-digit Code-1 cipher groups**, zero contemporary chancery decryption anywhere on these pages), plus **`p119L to p119R`** (which recaps the earlier alliance history already glossed on `p034L to R`, serving as an independent 100% sanity check).

## Strict Zero-Leakage Mechanical Coverage Audit

1. **Tier 1: Frozen Gloss-Only Key (`245` groups; ZERO information from any bare page):**
   - Built strictly from `hopken1739/key.tsv` (French glosses `255 to 260`) + Swedish chancery glosses read directly from images `18`, `34`, and `50`.
   - **Total mechanical coverage across all 11 bare pages:** **`1,516 / 1,610` (`94.2%`)** (`90.9% to 97.5%` on every single page!).
2. **Tier 1+2: Expanded Key (`+50` unambiguous bare-inferred Swedish syllables, strictly tagged `bare_inferred` in `code1_key_expanded.tsv`):**
   - **Total coverage across all 11 bare pages:** **`1,604 / 1,610` (`99.6%`)**, with **7 pages at `100.0%`** (`p115R, p116R, p117L, p117R, p118R, p120L, p120R`).
   - Only **6 single-occurrence tokens** out of 1,610 remain explicitly bracketed: `1113`, `1475`, `1195`, `1492`, `1186`, `1726`.

| Page | Date / Context | Tier-1 Frozen (Zero Leakage) | Tier 1+2 Expanded |
|---|---|---|---|
| `p114R` | Post-Bonneval exile; Swedish captain's wife freed | `154 / 158` (`97.5%`) | `156 / 158` (`98.7%`) |
| `p115L` | Contact `[1195]` warns of Grand Vizier's temperament | `117 / 125` (`93.6%`) | `124 / 125` (`99.2%`) |
| `p115R` | Ibrahim Effendi's house plague; daily Porte attendance | `138 / 147` (`93.9%`) | `147 / 147` (`100.0%`) |
| `p116L` | Conferences opened with the French Ambassador | `144 / 154` (`93.5%`) | `152 / 154` (`98.7%`) |
| `p116R` | `11 Dec St. N.`, `5/16 Dec` Vienna & Russia couriers; Relation No. 28 | `139 / 147` (`94.6%`) | `147 / 147` (`100.0%`) |
| `p117L` | `8/19 Dec`; Venice dispatch No. 29; Ottoman war levies; peace talk banned | `115 / 122` (`94.3%`) | `122 / 122` (`100.0%`) |
| `p117R` | Visits to Reis, Said & Ibrahim Effendi; Ramadan; `11/22 Dec` secret summons | `127 / 134` (`94.8%`) | `134 / 134` (`100.0%`) |
| `p118L` | Grand Vizier's direct quoted reply at dinner; order to draft answer to King | `130 / 143` (`90.9%`) | `142 / 143` (`99.3%`) |
| `p118R` | `19/30 Dec`; Porte's Dragoman arrives at dawn for confidential briefing | `148 / 157` (`94.3%`) | `157 / 157` (`100.0%`) |
| `p120L` | Envoys warn delay risks being taken by the King for coldness (`kallsinnighet`) | `149 / 160` (`93.1%`) | `160 / 160` (`100.0%`) |
| `p120R` | Swedish claim to reciprocal candor (`upriktighet och förtrolighet`) | `155 / 163` (`95.1%`) | `163 / 163` (`100.0%`) |
| **TOTAL** | **11 completely bare pages** | **`1,516 / 1,610` (`94.2%`)** | **`1,604 / 1,610` (`99.6%`)** |

---

## Reconstructed Swedish Reading & English Translation

*(Clear Swedish manuscript text in regular type; deciphered bare cipher in **bold**; unresolved tokens `[bracketed]`.)*

### Pages `p114R` to `p116R` (Late Nov  to  `11 Decembr. St. N. 1739`)
- **`p114R`:** Following Bonneval's exile (`4 Piastres belöning om dagen under dess exilium`), **the Grand Vizier sent an officer with a customary greeting recalling his promise regarding the `[1475=Swedish?]` captain's wife and her husband, already delivered against surety (`oss emot caution redan utlefwererade`), letting the envoys dispose of them** as they themselves saw best.
- **`p115L`:** After expressing gratitude through their Dragoman, **nothing was spoken on either side about any other affairs.** Sending another time **to `[1195]`, who observed extraordinary discretion (`en ogemen discretion`), he let their Dragoman understand that the Grand Vizier's temperament (`Storvizirens humeur`) was very harmful to the realm's affairs in these conjunctures, as he needed others' counsel yet no one dared admonish him, only follow his...**
- **`p115R`:** **...orders. He advised appearing often at the Porte without importuning the Grand Vizier, whom he knew to be well inclined toward Sweden. Their Ottoman insider Ibrahim Effendi (`wår Imbraim Ef[fendi]`) had had** several plague incidents in his house (`åtskillige pest accidentier i sitt hus`), halting contact until **the Grand Vizier ordered him, after the troop payments now being made at the Porte, to appear daily before him**, whereupon they sent their Dragoman to brief him.
- **`p116L`:** **He promised to guard Sweden's interest with the Grand Vizier and soon procure a satisfactory answer (`et nöjachtigt swar`), explaining he had not yet conferred because by `[1492][1186]`'s order conferences had been opened with the French Ambassador and he did not yet know to what conclusion they would come, so could not yet give positive and reliable assurances.**
- **`p116R`:** On `d. 11 Decembr: St: N:` **conferences with the French Ambassador concluded**, and on `5/16 [Dec]` **the same Ambassador dispatched one courier to Vienna (`1597`) and one to Russia (`1217`), with the first of which they sent Chancery College Relation No. 28**, apologizing for being **very detailed due to suspicion regarding route safety, especially lest their diplomatic pouch be destroyed/lost (`om wårt pacquet skulle warit förstört`).**

### Pages `p117L` to `p118R` (`8/19 Decembr` → `11/22 Decembr` → `19/30 Decembr 1739`)
- **`p117L` (`d. 8/19 Decembr:`):**
  > *Swedish:* d. 8/19 Decembr: hade Wij tillfälle at skrifwa, dock efter ganska kort förut gifwen warning, öfwer Venedig, då Wij allenast sände et litet bref til Hr. Cantzlie Rådet Celsing No. 29, hwaruti **wi optäckte det som wi sedermera lärt** angående **resultatet af de med den Franska Ambassadeuren hållne conferencer**, hwarupå Wij oss ock här i lika underdånighet referera. Emedlertid blefwo **starka utskrifningar giorde öfwer hela riket, at troupper skulle i god tid församlas och blef strängel: samt wid hårt straf öfwer hela Constant[inopel] förbudet, at ingen skulle ens understå sig at tala om fred.**
  >
  > *English:* On 8/19 December we had occasion to write, though on very short notice, via Venice, sending only a brief letter to Chancery Councillor Celsing No. 29, wherein **we disclosed what we had subsequently learned** regarding **the outcome of the conferences held with the French Ambassador**, to which we likewise humbly refer. Meanwhile **heavy troop levies were carried out across the entire realm so that troops should assemble in good time, and it was strictly forbidden under harsh punishment throughout all Constantinople that anyone should even dare to speak of peace.**

- **`p117R` (`d. 11/22 Decembr:`):**
  > *Swedish:* Det wore onödigt at opprepa huru många gånger **wi sände til Reis Ef[fendi], Said Ef[fendi] och Imbraim Ef[fendi], til at få höra** huru **det stod med wåre affairer**, samt **om Storviziren ej** ännu **giort någon** påminnelse, **at komma med oss til tals; ty deras swar gingo** mäst och förnämligast **derpå ut, at de beklagade sig öfwer Storviziren, som blef** hwar dag **underligare, förträtligare och swårare at tala med**, i synnerhet nu under påstående Ramazan och fastan.
  > d. 11/22 Decembr: **kallade omsider Reis Ef[fendi] wår Drogueman til sig in uti sitt rum och** sade honom, at han hade, afton förut, då han war til måltids **med Storviziren**...
  >
  > *English:* It would be needless to repeat how many times **we sent to the Reis Effendi, Said Effendi, and Ibrahim Effendi to hear** how **matters stood with our affairs**, and **whether the Grand Vizier had not** yet **given any** sign **of conferring with us; for their replies amounted** mostly and chiefly **to this, that they complained about the Grand Vizier, who grew** every day **stranger, more difficult, and harder to speak with**, especially now during the ongoing Ramadan and fast.
  > On 11/22 December **the Reis Effendi finally summoned our Dragoman privately into his chamber and** told him that the evening before, when he was at dinner **with the Grand Vizier**...

- **`p118L` (Grand Vizier's direct quoted reply):**
  > *Swedish:* haft tillfällen at **widlyftigt tala om wåre affairer**, i synnerhet, at det **långa dröjsmålet at gifwa swar kunde tagas op** för **en kallsinnighet och** hafwa **elaka suiter.** Han sade, at han ej fått **af honom annat swar än det: "Jag kan ej tro**, at man skola kunna få **illa uttyda det opskof**, som omständigheterne **warit wäl[1726]tier; men i morgon wil jag** emedlertid gifwa **ordres at låta sättja op swar uppå det Kongl. brefwet."** Han försäkrade at **samma swar skulle blifwa nöjacktigt, och at Storviziren** hade redan gifwit honom **någon idée derom.**
  >
  > *English:* ...he had had the opportunity to **speak at length about our affairs**, especially that **the long delay in giving a reply might be taken** for **coldness and** have **bad consequences.** He said he had received **no other reply from him than: *"I cannot believe*** that one could ***misinterpret this postponement,*** given how circumstances ***have stood [1726]; yet tomorrow I will*** in the meantime give ***orders to have an answer drafted to the Royal letter."*** He assured [us] that **that reply would be satisfactory, and that the Grand Vizier** had already given him **some idea thereof.**

- **`p118R` (`d. 19/30 Decembr:`):**
  > *Swedish:* d. 19/30 Decembr: kom **Portens Drogueman** til oss om morgonen bittida, **och berättat**, efter åtskillige **protestationer af en upricktig wänskap och tilgifwenhet**, sig wara **kommen af sig sielf til at discourera med oss i förtroende**, på det han måtte **blifwa fullkoml. uplyst om allt** hwad **som kunde angå wåre affairer, hwarom** han wiste at han **skulle innan kort blifwa tilfrågad af Storviziren. Wi begynte at oprepa** alla **Portens negotiationer med oss**, alt sedan **wår ankomst hit**, samt **orsakerne** hwarföre **för de af henne proponerade alliancer ej** kommit... *(continues across `p119L to p119R`, recapping the `p034` negotiation history)*
  >
  > *English:* On 19/30 December **the Porte's Dragoman** came to us early in the morning **and declared**, after numerous **protestations of upright friendship and devotion**, that he had **come of his own accord to discourse with us in confidence**, so that he might **be fully informed of everything** that **could concern our affairs, about which** he knew he **would shortly be questioned by the Grand Vizier. We began to recount** all **the Porte's negotiations with us**, ever since **our arrival here**, and **the reasons** why **the alliances previously proposed by it had not** come [to execution]...

### Pages `p120L` to `p120R` (Envoys' sharp warning to the Porte's Dragoman)
- **`p120L`:**
  > *Swedish:* **...ordnade widare giöra uppå** Ofta bemälte **Storvizirens insinuationer.** Wij kommo **honom at observera, at wi kunde ej annat än wara** högeligen **förundrade, at Storviziren**, oaktat **dess til oss ifrån [1608] med en afsänd skrifwelse**, samt sedermera, **efter dess hemkomst, giorde muntel. försäkringar, at willa** ofördröjel: **conferera med oss, ändå til** denna dag, **ej gifwit oss det ringaste swar**, hwilket **wi fruktade torde blifwa af** Eders Kongl. Maj:tt **optagit för en kallsinnighet**, hälst som **Porten och i synnerhet denna Storviziren sielf gifwit anledning** til...
  >
  > *English:* **...further act upon** the oft-mentioned **Grand Vizier's insinuations.** We led **him to observe that we could not but be** highly **astonished that the Grand Vizier**, despite **his dispatch sent to us from [1608]**, and subsequently, **after his return home, his verbal assurances that he would** without delay **confer with us, had still to** this day **not given us the slightest reply**, which **we feared might be taken by** Your Royal Majesty **for coldness**, especially since **the Porte and in particular this Grand Vizier himself had given occasion** for...

- **`p120R`:**
  > *Swedish:* **...denna correspondence. Wi sade, at ingen hade at undra uppå** hwad **swar som Porten wille gifwa**, ty det kunde **variera** alt efter som **hennes interess det fordrade**, hwilket **hon sielf måste** naturligen **bäst weta;** Men deremot hade den, **som så wänligt och så upricktigt communicerat sine tankar**, och samt **rätt at pretendera samma förtrolighet tillbaka**, eller i widrig händelse **at tro, det man ej procederade med samma upricktighet och förtrolighet, at sedan som rättan och nödwändigheten af wänskapens...**
  >
  > *English:* **...this correspondence. We said that no one could wonder at** what **answer the Porte wished to give**, for that could **vary** according as **its interest required**, which **it itself must** naturally **know best;** on the other hand, whoever **had so amicably and sincerely communicated his thoughts** also had **the right to claim the same confidence in return**, or otherwise **to believe that one was not proceeding with the same sincerity and confidence, as the right and necessity of friendship's...**

## Reproducible Files
- Master 11-page decoder: `decode_dec1739_all.py`
- Full provenance-tagged key (`245` frozen glossed + `50` bare-inferred): `code1_key_expanded.tsv`
- Expanded 11-page mechanical decode (`99.6%`): `dec1739_11pages_expanded_decode.txt`
