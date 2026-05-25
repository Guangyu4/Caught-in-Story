# CiS Normalized Dataset Manifest

Output root: `/home/bd2/Pushshift/CiS`

## Dataset JSON Naming

- Every dataset JSON file is named `data_en.json` or `data_zh.json`.
- All dataset JSON files are top-level arrays of records with the same schema.
- This manifest is Markdown so that every `.json` under `CiS/` is a dataset file.

## Record Schema

- `data_id`
- `dimension_id`
- `dimension`
- `sub_dimension_id`
- `sub_dimension`
- `language`
- `c0_baseline`
- `c1_control`
- `c2_multi_turn`

## Normalization

- `extra_fields_policy`: deleted
- `c1_control_policy`: full_text only; fixed_opening + narrative_paragraph merged when needed
- `text_content_policy`: preserve source text and record order
- `language_policy`: language is normalized to match data_en/data_zh filename; text content is not translated or moved
- `dimension` and `sub_dimension` are normalized to match the containing directory.

## Sources

### 1 Emotion & Obligation

- `1.1` / `EIRP`
  - `en`: `1_Emotion_Obligation/1.1_EIRP/data_en.json` (235 records), source `/home/bd2/Pushshift/cxy/v2/src/result_datasets/EIRP/data_en.json`
  - `zh`: `1_Emotion_Obligation/1.1_EIRP/data_zh.json` (150 records), source `/home/bd2/Pushshift/cxy/v2/src/result_datasets/EIRP/data_zh.json`
- `1.2` / `ERA`
  - `en`: `1_Emotion_Obligation/1.2_ERA/data_en.json` (227 records), source `/home/bd2/Pushshift/cxy/v2/src/result_datasets/ERA/data_en.json`
  - `zh`: `1_Emotion_Obligation/1.2_ERA/data_zh.json` (148 records), source `/home/bd2/Pushshift/cxy/v2/src/result_datasets/ERA/data_zh.json`
- `1.3` / `ARS`
  - `en`: `1_Emotion_Obligation/1.3_ARS/data_en.json` (230 records), source `/home/bd2/Pushshift/cxy/v2/src/result_datasets/ARS/data_en.json`
  - `zh`: `1_Emotion_Obligation/1.3_ARS/data_zh.json` (150 records), source `/home/bd2/Pushshift/cxy/v2/src/result_datasets/ARS/data_zh.json`
- `1.4` / `ARN`
  - `en`: `1_Emotion_Obligation/1.4_ARN/data_en.json` (223 records), source `/home/bd2/Pushshift/cxy/v2/src/result_datasets/ARN/data_en.json`
  - `zh`: `1_Emotion_Obligation/1.4_ARN/data_zh.json` (148 records), source `/home/bd2/Pushshift/cxy/v2/src/result_datasets/ARN/data_zh.json`

### 2 Fairness & Reciprocity

- `2.1` / `2.1`
  - `en`: `2_Fairness_Reciprocity/2.1/data_en.json` (128 records), source `/home/bd2/Pushshift/cwp/v2/result_datasets/1/data_en.json`
  - `zh`: `2_Fairness_Reciprocity/2.1/data_zh.json` (73 records), source `/home/bd2/Pushshift/cwp/v2/result_datasets/1/data_zh.json`
- `2.2` / `2.2`
  - `en`: `2_Fairness_Reciprocity/2.2/data_en.json` (128 records), source `/home/bd2/Pushshift/cwp/v2/result_datasets/2/data_en.json`
  - `zh`: `2_Fairness_Reciprocity/2.2/data_zh.json` (72 records), source `/home/bd2/Pushshift/cwp/v2/result_datasets/2/data_zh.json`
- `2.3` / `2.3`
  - `en`: `2_Fairness_Reciprocity/2.3/data_en.json` (130 records), source `/home/bd2/Pushshift/cwp/v2/result_datasets/3/data_en.json`
  - `zh`: `2_Fairness_Reciprocity/2.3/data_zh.json` (70 records), source `/home/bd2/Pushshift/cwp/v2/result_datasets/3/data_zh.json`
- `2.4` / `2.4`
  - `en`: `2_Fairness_Reciprocity/2.4/data_en.json` (115 records), source `/home/bd2/Pushshift/cwp/v2/result_datasets/4/data_en.json`
  - `zh`: `2_Fairness_Reciprocity/2.4/data_zh.json` (79 records), source `/home/bd2/Pushshift/cwp/v2/result_datasets/4/data_zh.json`

### 3 Trust & Loyalty

- `3.1` / `RLB`
  - `en`: `3_Trust_Loyalty/3.1_RLB/data_en.json` (238 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Trust & Loyalty/RLB/data_en.json`
  - `zh`: `3_Trust_Loyalty/3.1_RLB/data_zh.json` (158 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Trust & Loyalty/RLB/data_zh.json`
- `3.2` / `FLB`
  - `en`: `3_Trust_Loyalty/3.2_FLB/data_en.json` (235 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Trust & Loyalty/FLB/data_en.json`
  - `zh`: `3_Trust_Loyalty/3.2_FLB/data_zh.json` (156 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Trust & Loyalty/FLB/data_zh.json`
- `3.3` / `GLB`
  - `en`: `3_Trust_Loyalty/3.3_GLB/data_en.json` (232 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Trust & Loyalty/GLB/data_en.json`
  - `zh`: `3_Trust_Loyalty/3.3_GLB/data_zh.json` (159 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Trust & Loyalty/GLB/data_zh.json`
- `3.4` / `BFLB`
  - `en`: `3_Trust_Loyalty/3.4_BFLB/data_en.json` (238 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Trust & Loyalty/BFLB/data_en.json`
  - `zh`: `3_Trust_Loyalty/3.4_BFLB/data_zh.json` (159 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Trust & Loyalty/BFLB/data_zh.json`

### 4 RDB

- `4.1` / `ARB`
  - `en`: `4_RDB/4.1_ARB/data_en.json` (134 records), source `/home/bd2/Pushshift/zyt/RDB/4.1ARB/eng/RDB_ARB_eng_trial.json`
  - `zh`: `4_RDB/4.1_ARB/data_zh.json` (84 records), source `/home/bd2/Pushshift/zyt/RDB/4.1ARB/chi/RDB_ARB_chi_trial.json`
- `4.2` / `CSB`
  - `en`: `4_RDB/4.2_CSB/data_en.json` (129 records), source `/home/bd2/Pushshift/zyt/RDB/4.2CSB/eng/RDB_CSB_eng_trial.json`
  - `zh`: `4_RDB/4.2_CSB/data_zh.json` (87 records), source `/home/bd2/Pushshift/zyt/RDB/4.2CSB/chi/RDB_CSB_chi_trial.json`
- `4.3` / `EMB`
  - `en`: `4_RDB/4.3_EMB/data_en.json` (120 records), source `/home/bd2/Pushshift/zyt/RDB/4.3EMB/eng/RDB_EMB_eng_trial.json`
  - `zh`: `4_RDB/4.3_EMB/data_zh.json` (76 records), source `/home/bd2/Pushshift/zyt/RDB/4.3EMB/chi/RDB_EMB_chi_trial.json`
- `4.4` / `MPB`
  - `en`: `4_RDB/4.4_MPB/data_en.json` (121 records), source `/home/bd2/Pushshift/zyt/RDB/4.4MPB/eng/RDB_MPB_eng_trial.json`
  - `zh`: `4_RDB/4.4_MPB/data_zh.json` (82 records), source `/home/bd2/Pushshift/zyt/RDB/4.4MPB/chi/RDB_MPB_chi_trial.json`

### 5 Norm & Propriety

- `5.1` / `PCOB`
  - `en`: `5_Norm_Propriety/5.1_PCOB/data_en.json` (169 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Norm & Propriety/PCOB/data_en.json`
  - `zh`: `5_Norm_Propriety/5.1_PCOB/data_zh.json` (160 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Norm & Propriety/PCOB/data_zh.json`
- `5.2` / `FDB`
  - `en`: `5_Norm_Propriety/5.2_FDB/data_en.json` (188 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Norm & Propriety/FDB/data_en.json`
  - `zh`: `5_Norm_Propriety/5.2_FDB/data_zh.json` (146 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Norm & Propriety/FDB/data_zh.json`
- `5.3` / `IRCB`
  - `en`: `5_Norm_Propriety/5.3_IRCB/data_en.json` (171 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Norm & Propriety/IRCB/data_en.json`
  - `zh`: `5_Norm_Propriety/5.3_IRCB/data_zh.json` (147 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Norm & Propriety/IRCB/data_zh.json`
- `5.4` / `STB`
  - `en`: `5_Norm_Propriety/5.4_STB/data_en.json` (191 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Norm & Propriety/STB/data_en.json`
  - `zh`: `5_Norm_Propriety/5.4_STB/data_zh.json` (139 records), source `/home/bd2/Pushshift/cyr/FINAL_DATASET/Norm & Propriety/STB/data_zh.json`

### 6 Autonomy & Boundary

- `6.1` / `BPB`
  - `en`: `6_Autonomy_Boundary/6.1_BPB/data_en.json` (122 records), source `/home/bd2/Pushshift/zjt/data/03_final_benchmark/by_lang/6.1_BPB_EN_final.json`
  - `zh`: `6_Autonomy_Boundary/6.1_BPB/data_zh.json` (78 records), source `/home/bd2/Pushshift/zjt/data/03_final_benchmark/by_lang/6.1_BPB_ZH_final.json`
- `6.2` / `VDB`
  - `en`: `6_Autonomy_Boundary/6.2_VDB/data_en.json` (117 records), source `/home/bd2/Pushshift/zjt/data/03_final_benchmark/by_lang/6.2_VDB_EN_final.json`
  - `zh`: `6_Autonomy_Boundary/6.2_VDB/data_zh.json` (78 records), source `/home/bd2/Pushshift/zjt/data/03_final_benchmark/by_lang/6.2_VDB_ZH_final.json`
- `6.3` / `IPB`
  - `en`: `6_Autonomy_Boundary/6.3_IPB/data_en.json` (126 records), source `/home/bd2/Pushshift/zjt/data/03_final_benchmark/by_lang/6.3_IPB_EN_final.json`
  - `zh`: `6_Autonomy_Boundary/6.3_IPB/data_zh.json` (75 records), source `/home/bd2/Pushshift/zjt/data/03_final_benchmark/by_lang/6.3_IPB_ZH_final.json`
- `6.4` / `PRB`
  - `en`: `6_Autonomy_Boundary/6.4_PRB/data_en.json` (120 records), source `/home/bd2/Pushshift/zjt/data/03_final_benchmark/by_lang/6.4_PRB_EN_final.json`
  - `zh`: `6_Autonomy_Boundary/6.4_PRB/data_zh.json` (81 records), source `/home/bd2/Pushshift/zjt/data/03_final_benchmark/by_lang/6.4_PRB_ZH_final.json`

## Sampling Update

- Date: 2026-05-17
- Random seed: `20260517`
- Operation: dimensions 2, 4, and 6 were randomly downsampled per `data_en.json` / `data_zh.json` file.
- Rule: keep `ceil(n / 2)` records per file; selected indices are sorted back into original order.

| File | Before | After | Removed |
| --- | ---: | ---: | ---: |
| `2_Fairness_Reciprocity/2.1/data_en.json` | 255 | 128 | 127 |
| `2_Fairness_Reciprocity/2.1/data_zh.json` | 145 | 73 | 72 |
| `2_Fairness_Reciprocity/2.2/data_en.json` | 255 | 128 | 127 |
| `2_Fairness_Reciprocity/2.2/data_zh.json` | 144 | 72 | 72 |
| `2_Fairness_Reciprocity/2.3/data_en.json` | 260 | 130 | 130 |
| `2_Fairness_Reciprocity/2.3/data_zh.json` | 140 | 70 | 70 |
| `2_Fairness_Reciprocity/2.4/data_en.json` | 230 | 115 | 115 |
| `2_Fairness_Reciprocity/2.4/data_zh.json` | 158 | 79 | 79 |
| `4_RDB/4.1_ARB/data_en.json` | 268 | 134 | 134 |
| `4_RDB/4.1_ARB/data_zh.json` | 167 | 84 | 83 |
| `4_RDB/4.2_CSB/data_en.json` | 257 | 129 | 128 |
| `4_RDB/4.2_CSB/data_zh.json` | 174 | 87 | 87 |
| `4_RDB/4.3_EMB/data_en.json` | 240 | 120 | 120 |
| `4_RDB/4.3_EMB/data_zh.json` | 152 | 76 | 76 |
| `4_RDB/4.4_MPB/data_en.json` | 242 | 121 | 121 |
| `4_RDB/4.4_MPB/data_zh.json` | 164 | 82 | 82 |
| `6_Autonomy_Boundary/6.1_BPB/data_en.json` | 244 | 122 | 122 |
| `6_Autonomy_Boundary/6.1_BPB/data_zh.json` | 156 | 78 | 78 |
| `6_Autonomy_Boundary/6.2_VDB/data_en.json` | 234 | 117 | 117 |
| `6_Autonomy_Boundary/6.2_VDB/data_zh.json` | 155 | 78 | 77 |
| `6_Autonomy_Boundary/6.3_IPB/data_en.json` | 251 | 126 | 125 |
| `6_Autonomy_Boundary/6.3_IPB/data_zh.json` | 150 | 75 | 75 |
| `6_Autonomy_Boundary/6.4_PRB/data_en.json` | 239 | 120 | 119 |
| `6_Autonomy_Boundary/6.4_PRB/data_zh.json` | 161 | 81 | 80 |
