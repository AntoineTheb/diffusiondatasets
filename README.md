# diffusiondatasets

Personal collection of public diffusion MRI datasets.

> Notes:
> - This is a working list. APA references are best-effort and should be verified against each dataset's official citation guidance.
> - For entries where a paper or direct download URL is still unclear, the item is marked **TBD**.

## Datasets with annotated bundles

### TractoInferno
- **APA paper reference (best-effort):** Théaud, G., Houde, J.-C., Boré, A., Rheault, F., & Descoteaux, M. (2023). *TractoInferno: A large-scale diffusion MRI tractography dataset with bundle annotations*. arXiv.
- **Download:** https://openneuro.org/datasets/ds003900/versions/1.1.1
- **Acquisition / generation (brief):** Multi-subject in-vivo diffusion MRI dataset curated for tractography and bundle-level analyses.
- **Annotation procedure (brief):** White-matter bundles annotated as tractography labels for supervised/benchmark use.

### HCP105
- **APA paper reference (best-effort):** Van Essen, D. C., Smith, S. M., Barch, D. M., Behrens, T. E. J., Yacoub, E., & Ugurbil, K. (2013). The WU-Minn Human Connectome Project: An overview. *NeuroImage, 80*, 62-79. https://doi.org/10.1016/j.neuroimage.2013.05.041
- **Download:** https://zenodo.org/records/1477956
- **Acquisition / generation (brief):** Subset derived from high-quality Human Connectome Project diffusion acquisitions.
- **Annotation procedure (brief):** Bundle annotations provided for tractography benchmarking workflows.

### CamCAN benchmark
- **APA paper reference (best-effort):** Shafto, M. A., Tyler, L. K., Dixon, M., Taylor, J. R., Rowe, J. B., Cusack, R., ... Cam-CAN. (2014). The Cambridge Centre for Ageing and Neuroscience (Cam-CAN) study protocol. *BMC Neurology, 14*, 204. https://doi.org/10.1186/s12883-014-0204-1
- **Download:** https://brainlife.io/pub/6a014fb3ea4d9f77d878b3cf
- **Acquisition / generation (brief):** Adult lifespan diffusion MRI cohort adapted into a tractography benchmark format.
- **Annotation procedure (brief):** Bundle labels/segmentations distributed through the benchmark package.

### HCP-YA updated benchmark
- **APA paper reference (best-effort):** Van Essen, D. C., Smith, S. M., Barch, D. M., Behrens, T. E. J., Yacoub, E., & Ugurbil, K. (2013). The WU-Minn Human Connectome Project: An overview. *NeuroImage, 80*, 62-79. https://doi.org/10.1016/j.neuroimage.2013.05.041
- **Download:** https://brainlife.io/pub/69d5696404be87075a466ef4
- **Acquisition / generation (brief):** Updated benchmark based on HCP Young Adult diffusion MRI.
- **Annotation procedure (brief):** Harmonized bundle annotations for updated tractography evaluation.

## Test-retest

### Penthera 3T
- **APA paper reference (best-effort):** Tax, C. M. W., Grussu, F., Kaden, E., Ning, L., Rudrapatna, U., John Evans, C., ... Jones, D. K. (2019). Cross-scanner and cross-protocol diffusion MRI data harmonisation: A benchmark database and evaluation of algorithms. *NeuroImage, 195*, 285-299. https://doi.org/10.1016/j.neuroimage.2019.01.077
- **Download:** https://zenodo.org/records/2602049
- **Acquisition / generation (brief):** Repeated diffusion MRI sessions at 3T for repeatability analysis.
- **Annotation procedure (brief):** Primarily test-retest diffusion measurements; no bundle annotations expected by default.

### Penthera 1.5T
- **APA paper reference (best-effort):** Tax, C. M. W., Grussu, F., Kaden, E., Ning, L., Rudrapatna, U., John Evans, C., ... Jones, D. K. (2019). Cross-scanner and cross-protocol diffusion MRI data harmonisation: A benchmark database and evaluation of algorithms. *NeuroImage, 195*, 285-299. https://doi.org/10.1016/j.neuroimage.2019.01.077
- **Download:** https://zenodo.org/records/2602022
- **Acquisition / generation (brief):** Repeated diffusion MRI sessions at 1.5T for repeatability/scanner-comparison studies.
- **Annotation procedure (brief):** Primarily raw/reconstructed diffusion data for reliability benchmarking.

## Phantoms

### FiberCup (MICCAI 2015 / Neher formulations)
- **APA paper reference (best-effort):** Fillard, P., Poupon, C., Mangin, J.-F., Frouin, V., Clark, C. A., Le Bihan, D., ... Poupon, F. (2011). Quantitative evaluation of 10 tractography algorithms on a realistic diffusion MR phantom. *NeuroImage, 56*(1), 220-234. https://doi.org/10.1016/j.neuroimage.2011.01.032
- **Download:** **TBD** (current target is to publish a cleaned-up personal version)
- **Acquisition / generation (brief):** Synthetic/phantom diffusion data with known fiber geometry and controlled crossings.
- **Annotation procedure (brief):** Ground-truth pathways are defined by phantom design.

### ISMRM 2015 tractography challenge phantom
- **APA paper reference (best-effort):** Maier-Hein, K. H., Neher, P. F., Houde, J.-C., Côté, M.-A., Garyfallidis, E., Zhong, J., ... Descoteaux, M. (2017). The challenge of mapping the human connectome based on diffusion tractography. *Nature Communications, 8*, 1349. https://doi.org/10.1038/s41467-017-01285-x
- **Download:** http://tractometer.org/ismrm2015/
- **Acquisition / generation (brief):** Simulated phantom with known fiber tracts for controlled tractography evaluation.
- **Annotation procedure (brief):** Ground-truth streamlines/tract definitions provided by simulation framework.

### 99 synthetic subjects
- **APA paper reference:** **TBD**
- **Download:** **TBD**
- **Acquisition / generation (brief):** Synthetic multi-subject diffusion cohort.
- **Annotation procedure (brief):** Expected simulation-derived labels; exact release details still to be confirmed.

## Tumors / lesions

### OpenNeuro ds004910
- **APA paper reference:** **TBD** (dataset-specific citation to be added)
- **Download:** https://openneuro.org/datasets/ds004910/versions/1.0.1
- **Acquisition / generation (brief):** In-vivo diffusion MRI with tumor/lesion relevance.
- **Annotation procedure (brief):** Check OpenNeuro metadata for lesion/tumor labeling details.

### BTC post-op (OpenNeuro ds002080)
- **APA paper reference:** **TBD** (dataset-specific citation to be added)
- **Download:** https://openneuro.org/datasets/ds002080/versions/4.0.1
- **Acquisition / generation (brief):** Post-operative brain tumor case cohort including diffusion MRI.
- **Annotation procedure (brief):** Labels/clinical annotations distributed through the OpenNeuro release.

### BTC pre-op (OpenNeuro ds001226)
- **APA paper reference:** **TBD** (dataset-specific citation to be added)
- **Download:** https://openneuro.org/datasets/ds001226/versions/5.0.1
- **Acquisition / generation (brief):** Pre-operative brain tumor diffusion MRI cohort.
- **Annotation procedure (brief):** Labels/metadata available in dataset documentation.

## b-tensor encoding

### Cardiff dataset
- **APA paper reference:** **TBD**
- **Download:** **TBD**
- **Acquisition / generation (brief):** b-tensor encoded diffusion MRI acquisition (linear/planar/spherical encoding expected).
- **Annotation procedure (brief):** Primarily acquisition-focused dataset; annotation details to confirm.

### Kerkelä dataset
- **APA paper reference:** Kerkelä, L., Henriques, R. N., Hall, M. G., & others. (2020). *Constrained and rotationally invariant mapping of microscopic diffusion anisotropy with diffusion-relaxation MRI*. (Best-effort placeholder; verify exact publication metadata.)
- **Download:** **TBD**
- **Acquisition / generation (brief):** Tensor-valued diffusion encoding dataset for microstructure modeling.
- **Annotation procedure (brief):** Not typically bundle-annotated; mainly quantitative model fitting use-cases.

## Multi-TE

### SciDB dataset
- **APA paper reference:** **TBD**
- **Download:** https://www.scidb.cn/en/detail?dataSetId=411f844eb7974da68d08569a1cb27693#p2
- **Acquisition / generation (brief):** Multi-echo diffusion MRI dataset.
- **Annotation procedure (brief):** Annotation details should be checked in the dataset release metadata.

## Time-varying gradients

### 300 mT/m gradient comprehensive dataset
- **APA paper reference (best-effort):** Jones, D. K., Alexander, D. C., Cercignani, M., et al. (2021). Comprehensive diffusion MRI dataset for in vivo human brain microstructure mapping using 300 mT/m gradients. *Figshare collection*.
- **Download:** https://springernature.figshare.com/collections/Comprehensive_diffusion_MRI_dataset_for_in_vivo_human_brain_microstructure_mapping_using_300_mT_m_gradients/5315474
- **Acquisition / generation (brief):** High-gradient diffusion MRI with broad protocol coverage for microstructure mapping.
- **Annotation procedure (brief):** Typically quantitative acquisition release; verify any segmentation/ROI annotations per sub-study.
