# ![ROBIN_logo_small.png](https://github.com/LooseLab/ROBIN/blob/30b443ee8f2635c36d946aadaf1447aa9016831d/src/robin/images/ROBIN_logo_small.png) ROBIN
-----
## Test Data Set A

This data set is provided for users to test the ROBIN tool for rapid diagnostics from Nanopore data. ROBIN is available from https://github.com/LooseLab/ROBIN and is required for analysis of these data.

The bam files contained within the test_data_set folder are derived from a barcoded sample set with reads from three cell lines, NA12878, NB4 and 22Rv1. The reads were base called with dorado version 0.8 using the HAC model with 5mC 5hmC calling. The reads are mapped to hg38 with no alts and no unplaced sequences. 

These reads are provided solely for the purpose of testing a ROBIN installation on a small data set. They will not result in a "valid" or meaningful classification with respect to CNS tumours.

<strong>These are not patient derived reads.</strong>

## Usage

Please download this repo:

```commandline
git clone https://github.com/LooseLab/ROBIN_test_set_A
```

Then configure and run ROBIN as in the ROBIN repository, but for the watch directory (-w) point ROBIN to the ROBIN_test_set_A/test_data_set folder.

## Expected Results

Below are typical screenshots that you should see if using this data set.

### Summary Classification

![summary_classification.png](resources/summary_classification.png)

### Methylation Results

![img.png](resources/img.png)

![img_1.png](resources/img_1.png)

![img_2.png](resources/img_2.png)

![img_3.png](resources/img_3.png)

### CNV Results

![img_4.png](resources/img_4.png)

Specific chromosome 9 example:

![img_5.png](resources/img_5.png)


### Target Coverage

![img_6.png](resources/img_6.png)

![img_7.png](resources/img_7.png)

*** Please note - no SNP calls should be generated from this data set as no individual targets cross the threshold for calling.

### MGMT and Fusions

No reads cover the MGMT promoter in this test data set, nor are any fusions present. So these reports should be negative.

### Example sample report.

An example sample report is available here:

[NA12878_05_NB4_06_22Rv1_07_run_report.pdf](resources/NA12878_05_NB4_06_22Rv1_07_run_report.pdf)





