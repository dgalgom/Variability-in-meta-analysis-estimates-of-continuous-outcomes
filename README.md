# Variability-in-meta-analysis-estimates-of-continuous-outcomes
This repository is part of the methodological work in evidence synthesis developed in the **Centre for Reviews and Dissemination** (CRD; University of York) and the **Bristol Medical School** (University of Bristol). It investigates the variability in meta-analysis estimates of continuous outcomes using different standardization and re-expression methods.

## Study analysing different standardization methods and how to re-express those estimates using scale-specific re-expression methods
Our work entitled "*Variability in meta-analysis estimates of continouous outcomes using different standardization and scale-specific re-expression methods*" tried to clarify (1) the impact of using different data standardization and scale-specific re-expression methods in meta-analyses using standardized mean differences (*SMDs*), and (2) to give some recommendations to promote methodological guide and transparency in meta-analyses.

### When you import the dataset in your environment... 
You may need some clarification on the meaning of the variables. Let's crumble our dataset:

  + `studyID` refers to each of the included studies in the meta-analysis.
  + `class` is the first level of specificity referring to the intervention. In this level we can find `Physical activity` or `Usual care`.
  + `agent` is the second level of specificity referring to the intervention. In this level we can find the specific intervention that a study performed (e.g., `Ambulation` consisted on movements oriented to real life and/or walkings across the wards).
  + `component` is the third level of specificity. It is a dismantling of each intervention.
  + `pre_n` is the study sample at baseline.
  + `pre_mean`is the mean value of physical performance measured by the Short Physical Performance Battery (SPPB) or the Barthel Index (BI) at baseline.
  + `pre_sd` is the standard deviation (SD) of the mean value at baseline.
  + `post_n` is the study sample at post-intervention time point.
  + `post_mean`is the mean value of physical performance measured by the Short Physical Performance Battery (SPPB) or the Barthel Index (BI) at post-intervention time point.
  + `post_sd` is the standard deviation of the mean value at post-intervention time point.
  + `ward` referes to the type of hospital ward where the intervention was conducted.
  + `measure` corresponds to the scale used to measure the physical performance of the patients.
  + `lower_better` refers if a lower mean value means a greater improvement in the outcome. This is not the case.
  + `outcome` is the type of analysed outcome.
  + `y` is the mean change from baseline.
  + `sd` is the standard deviation of `y`.
  + `se` is the standard error of `y`.
  + `post_sd_pooled` corresponds to the pooled standard deviation of a specific scale and study at post-intervention time point.
  + `pre_sd_pooled` corresponds to the pooled standard deviation of a specific scale and study at baseline.
  +  `y_int` is the rescaled mean change from baseline using an internal SD reference by scale.
  +  `sd_int` is the rescaled standard deviation of `y_int`.
  +  `y_ext` is the rescaled mean change from baseline using an external SD reference by scale.
  +  `sd_ext` is the rescaled standard deviation of `y_ext`.
  +  `diff` refers to the mean difference between intervention and control arms of the same study.
  +  `se_diff` is the corresponding standard error of `diff` values.
  +  `diff_ext` is the rescaled mean difference using an external sD reference by scale.
  +  `se_diff_ext` is the rescaled variance of `diff_ext`.
  +  `diff_int` is the rescaled mean difference using an internal sD reference by scale.
  +  `se_diff_int` is the rescaled variance of `diff_int`.
  +  `diff_pre` is the rescaled mean difference using the pooled SD of each study at baseline.
  +  `se_diff_pre` is the rescaled variance of `diff_pre`.
  +  `diff_post` is the rescaled mean difference using the pooled SD of each study at post-intervention time point.
  +  `se_diff_post` is the rescaled variance of `diff_post`.
