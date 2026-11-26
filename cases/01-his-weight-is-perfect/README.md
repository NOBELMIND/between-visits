> **Invented patient. Not medical advice.**
> This case is fiction written for teaching. Please do not post real patient information in replies, issues or discussions.

# Between Visits — Case 1: "His weight is perfect"

*Draft for cardiologist review. Not yet published.*

## The patient

Mr. A is a 76-year-old retired bus driver with ischemic cardiomyopathy (left ventricular ejection fraction 30%), hypertension and stage 3a chronic kidney disease. He lives with his wife, who helps with his log.

He was just discharged after five days in hospital for acute decompensated heart failure. He lost about 6 kg with intravenous diuretics and went home breathing comfortably, with mild ankle swelling. His team estimated his dry weight at about 81 kg.

**Discharge medicines**

- Furosemide 40 mg twice daily (before admission: 40 mg once daily)
- Sacubitril/valsartan 49/51 mg twice daily
- Spironolactone 25 mg once daily
- Dapagliflozin 10 mg once daily
- Metoprolol succinate 50 mg once daily
- Aspirin 81 mg and atorvastatin 40 mg once daily

He was told to weigh himself every morning, keep to a fluid limit of about 1.5 litres a day, and call if his weight went up. His home program sends an automatic alert when weight rises.

## The 14 days at home

Day 1 is his first morning home. Home readings are in [`timeline.csv`](timeline.csv); clinic blood tests are in [`labs.csv`](labs.csv) (day 0 = discharge).

| Day | Weight (kg) | BP sitting | Pulse | Breathless (0–4) | Ankles | Dizzy standing | Urine | Notes |
|---|---|---|---|---|---|---|---|---|
| 1 | 83.8 | 128/76 | 70 | 2 | mild | no | plenty | First day home |
| 2 | 83.1 | 126/74 | 68 | 2 | mild | no | plenty | |
| 3 | 82.5 | 124/74 | 70 | 1 | trace | no | plenty | |
| 4 | 82.0 | 122/72 | 70 | 1 | trace | no | plenty | Clinic visit, bloods |
| 5 | 81.6 | 120/70 | 72 | 1 | none | no | plenty | |
| 6 | 81.3 | 118/70 | 72 | 1 | none | no | normal | |
| 7 | 81.2 | 116/68 | 74 | 1 | none | no | normal | Hot day, ate less |
| 8 | 81.4 | 114/66 | 74 | 1 | none | no | normal | Gardening; knee sore, "took the pain pills from the cabinet" |
| 9 | 81.2 | 110/64 | 76 | 0 | none | slightly | normal | Loose stools x3; missed evening metoprolol |
| 10 | 81.0 | 108/62 | 78 | 0 | none | slightly | less | Loose stools x2; "keeping to my fluid limit" |
| 11 | — | 104/60 | 80 | 0 | none | yes | less | Forgot to weigh |
| 12 | 81.1 | 102/60 | 80 | 0 | none | yes | less, dark | Night leg cramps; still taking knee pills |
| 13 | 81.2 | 98/58 | 82 | 0 | none | yes | less, dark | Clinic bloods; "wife says I look pale" |
| 14 | 81.0 | 96/58 | 84 | 0 | none | yes | less, dark | Thirsty; greyed out standing from the toilet; "breathing fine" |

**Clinic blood tests**

| Test | Day 0 (discharge) | Day 4 | Day 13 (resulted this morning) |
|---|---|---|---|
| Sodium (mmol/L) | 137 | 136 | 131 |
| Potassium (mmol/L) | 4.4 | 4.7 | 5.9 (not hemolyzed) |
| Creatinine (mg/dL) | 1.15 | 1.24 | 2.05 |
| Urea nitrogen (mg/dL) | 24 | 28 | 61 |
| eGFR (mL/min/1.73 m²) | 64 | 58 | 32 |
| Bicarbonate (mmol/L) | — | — | 19 |
| Magnesium (mg/dL) | — | — | 2.3 |
| NT-proBNP (pg/mL) | 2850 | — | 1310 |

No weight-gain alert fired at any point in the 14 days.

## The question

It is the morning of Day 14. The day-13 blood results have just come back, and Mr. A's log for today is in.

**Would you call this patient today, and what would you change?**

Write your answer before you open the discussion. The answer will be released later.

## About the sealed answer

The answer was written before this case was published and sealed with a SHA-256 hash, also saved in [`seal.txt`](seal.txt):

```
a1d88898bc2cf25c8358917c5c938511b790dd94959e66f8ab5eca2b7156c7a8
```

When the answer is released, we will also publish the answer file (`answer-01.md`) and its salt file (`salt-01.txt`). To verify the seal, run

```
cat salt-01.txt answer-01.md | shasum -a 256
```

(or `sha256sum` on Linux) and check that the result matches the hash in `seal.txt`. If they match, the answer has not changed since the case went up.
