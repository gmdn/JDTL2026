# Exploratory Pilot Replication Materials

This repository contains the materials used for the exploratory pilot on LLM-assisted terminological definition generation.

## Contents

- `prompts/`
  - `template_JDTL_.txt`: common definition-generation prompt.
  - One folder for each target concept:
    - `track switch`
    - `straight track section`
    - `suspension rod`
    - `travel wheel`
  - Each concept folder contains the four experimental conditions:
    - `test_P.txt`: prompt-only (`P`)
    - `test_D.txt`: documentary-grounded (`D`)
    - `test_T.txt`: concept-system-grounded (`T`)
    - `test_DT.txt`: combined documentary + concept-system grounding (`D+T`)

- `TEST_GPT_JDTL.xlsx`
  - Generated definitions for the four concepts and four conditions.
  - Human evaluation scores for each target concept.

## Experimental setup

All definitions were generated with **GPT-5.6 Sol High** in fresh, unpersonalized temporary ChatGPT sessions. The same generation instruction was used in all conditions; only the evidence supplied to the model varied.

The pilot includes four target concepts from the Demag KBK light lifting system and four generation conditions, for a total of **16 generated definitions**.

The evaluation uses five criteria scored from 0 to 2:

- `C1`: conceptual accuracy
- `C2`: concept-system positioning
- `C3`: delimiting characteristics
- `C4`: evidential support
- `C5`: linguistic and definitional adequacy

The workbook also reports:

- `G`: appropriate genus identified
- `S`: supported distinguishing characteristic present
- `CA`: condition adherence (`D`, `T`, and `D+T` only)

The pilot is exploratory and descriptive; it is not intended as a large-scale statistical validation.
