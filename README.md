# Urinary Metabolite Discrimination Model of Violent Behavior

This repository contains the analysis notebooks and a synthetic example sociodemographic input dataset associated with an exploratory study of urinary metabolic signatures related to violent behavior in incarcerated adult males. The computational workflow covers feature selection, classifier construction and evaluation, and SHAP-based model interpretation.

## Repository contents

| File | Description |
| --- | --- |
| [`Feature selection_RFE_RFECV_LASSO_EN.ipynb`](./Feature%20selection_RFE_RFECV_LASSO_EN.ipynb) | Feature-selection workflow using RFE/RFECV together with LASSO and Elastic Net procedures. |
| [`Model construction and SHAP.ipynb`](./Model%20construction%20and%20SHAP.ipynb) | Construction and evaluation of RF, XGB, LGBM, SVM, and Ridge classifiers, followed by SHAP-based interpretation of fitted models. |
| [`Synthetic_Violence_Input_Dataset.xlsx`](./Synthetic_Violence_Input_Dataset.xlsx) | Structurally matched synthetic example of the sociodemographic input format. The workbook contains a `Synthetic_Input` sheet and a `README` sheet describing the variable coding. |

## Suggested workflow

1. Download or clone the repository.
2. Review the `README` sheet in `Synthetic_Violence_Input_Dataset.xlsx` for the input structure and coding definitions.
3. Update the input paths and column names in the notebooks if required by the local directory structure.
4. Run `Feature selection_RFE_RFECV_LASSO_EN.ipynb` first.
5. Use the selected features in `Model construction and SHAP.ipynb` for model fitting, evaluation, and SHAP analysis.

The notebooks are intended to be run in a Python/Jupyter environment. Required packages should be installed according to the import statements at the beginning of each notebook.

## Synthetic sociodemographic input data

`Synthetic_Violence_Input_Dataset.xlsx` contains 246 entirely synthetic records: 115 records coded as non-violent and 131 records coded as violent behavior. The dataset was generated from the aggregate distributions reported in Table 1 of the associated study. It does not contain information from, represent, or permit reconstruction of any participant.

The workbook illustrates the expected sociodemographic input structure. It does not contain measured metabolomic data and therefore cannot reproduce the numerical results reported in the article.

## Data availability

The preprocessed feature-level metabolomic data are available in the Supplementary File (`Supplemental_Metabolomic_Data.xlsx`) accompanying the associated article. These data are not raw LC-MS/MS instrument output and do not permit reproduction of the upstream metabolomic processing procedures.

Participant-level sociodemographic, personality, and violence-phenotype data are not publicly available because of the risk of indirect identification in this incarcerated population and the applicable ethical and judicial privacy requirements. These restricted data may be requested from the corresponding author ([minlanyuan@outlook.com](mailto:minlanyuan@outlook.com)) for verification or reproduction of the reported analyses, subject to relevant institutional approval and an appropriate data-use agreement. Requests for other research purposes require separate ethical and institutional approval.

The archived analysis code and structurally matched synthetic example input dataset are available at [https://doi.org/10.5281/zenodo.21534920](https://doi.org/10.5281/zenodo.21534920).

## Scope and interpretation

This repository supports verification and demonstration of an exploratory research workflow. The synthetic dataset is not suitable for substantive inference. SHAP values describe model-based feature contributions and should not be interpreted as causal effects or direct evidence of biological mechanisms. The classifiers have not undergone independent external validation and should not be used for individual-level forensic, judicial, or clinical decision-making.

## Contact

For questions concerning restricted data access or reproduction of the reported analyses, contact the corresponding author at [minlanyuan@outlook.com](mailto:minlanyuan@outlook.com).

## Citation

When using this repository, please cite the associated article and the archived code and synthetic data record: [https://doi.org/10.5281/zenodo.21534920](https://doi.org/10.5281/zenodo.21534920).
