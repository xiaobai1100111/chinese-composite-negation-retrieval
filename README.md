# Chinese composite negation retrieval

Data, saved scores, and verification scripts for **Supervision tradeoffs in Chinese text-to-image retrieval with composite negation**.

Runze Zhang, College of Information Science and Engineering, Huaqiao University. Contact: roude@stu.hqu.edu.cn.

## Download

- [Version 1.1 — Excel-compatible CSVs](PRL_Data_and_Score_Recheck_RELEASE_v1.1.zip)
- [Version 1.0 — original release](PRL_Data_and_Score_Recheck_RELEASE_v1.0.zip)

Version 1.1 adds UTF-8 encoding signatures to CSVs that lacked them and updates the inventories and documentation. Table text and numerical values are not edited. If Excel still needs an import setting, select UTF-8 and a comma delimiter. Version 1.0 remains available for traceability.

## Contents

- Evaluation labels and image identifiers; current Study II has 157 families and 471 images.
- Saved model scores, current and historical result tables, and training-budget results.
- Joint human review records and the correction/exclusion manifest.
- Four saved-score/integrity verification scripts and one figure-generation script.

Source images, model weights, and the full training or embedding-inference environment are not included. See README.txt inside the archive for file-level descriptions. Two non-author reviewers jointly completed the review and follow-up; these are consensus records, not independently collected ratings.

## Use

Extract one archive and run the following commands from its extracted root using Python 3 and NumPy:

```text
python verify_file_integrity.py
python verify_revised_scores.py
python verify_budget_scores.py
python verify_prl_tables.py
```

These scripts check stored files and aggregation of saved scores. They require no GPU or model/image downloads. Figure generation additionally requires Matplotlib:

```text
python plot_figure_1.py
```

Current main tables are in `prl_tables/`. Supplementary tables S1-S28 and retained full-report main tables are in `tables/`; 33 CSV versions are in `tables/csv/`.

## Licenses

Data and documentation are licensed under **CC BY 4.0**, within the author's rights. The five original Python scripts are licensed under **MIT**. Third-party rights are retained. Read [LICENSING.txt](LICENSING.txt), the full texts in [LICENSES](LICENSES/), and [THIRD_PARTY_NOTICES.txt](THIRD_PARTY_NOTICES.txt).

## Citation

Runze Zhang. *Data, saved scores, and verification scripts for Supervision tradeoffs in Chinese text-to-image retrieval with composite negation*. Version 1.1. 2026. https://github.com/xiaobai1100111/chinese-composite-negation-retrieval

No DOI has been assigned. Cite the archive version and, where possible, a fixed commit or release link.

## Archive checksum

SHA-256 for `PRL_Data_and_Score_Recheck_RELEASE_v1.1.zip`:

```text
68de862a97278213230e05b589bc13170ddc78e25fb8461fb98a525c3ea9e300
```
